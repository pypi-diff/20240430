# Comparing `tmp/scimba-0.4.1.tar.gz` & `tmp/scimba-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimba-0.4.1.tar", last modified: Wed Apr 17 13:19:24 2024, max compression
+gzip compressed data, was "scimba-0.4.2.tar", last modified: Tue Apr 30 13:05:44 2024, max compression
```

## Comparing `scimba-0.4.1.tar` & `scimba-0.4.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.778298 scimba-0.4.1/
--rw-r--r--   0 boileau    (502) staff       (20)     1072 2023-09-04 07:10:54.000000 scimba-0.4.1/LICENSE
--rw-r--r--   0 boileau    (502) staff       (20)     4767 2024-04-17 13:19:24.778080 scimba-0.4.1/PKG-INFO
--rw-r--r--   0 boileau    (502) staff       (20)     3741 2024-04-17 13:19:16.000000 scimba-0.4.1/README.md
--rw-r--r--   0 boileau    (502) staff       (20)     1086 2024-04-16 11:54:20.000000 scimba-0.4.1/pyproject.toml
--rw-r--r--   0 boileau    (502) staff       (20)       38 2024-04-17 13:19:24.778344 scimba-0.4.1/setup.cfg
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.758201 scimba-0.4.1/src/
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.759433 scimba-0.4.1/src/applications/
--rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.1/src/applications/__init__.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.759557 scimba-0.4.1/src/scimba/
--rw-r--r--   0 boileau    (502) staff       (20)      435 2024-04-17 13:19:16.000000 scimba-0.4.1/src/scimba/__init__.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.762298 scimba-0.4.1/src/scimba/equations/
--rw-r--r--   0 boileau    (502) staff       (20)      119 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    23566 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/domain.py
--rw-r--r--   0 boileau    (502) staff       (20)     2525 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/genericSL_advection_diffusion_equation.py
--rw-r--r--   0 boileau    (502) staff       (20)     8548 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/nonlinear_ode_basic.py
--rw-r--r--   0 boileau    (502) staff       (20)     9299 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/ode_basic.py
--rw-r--r--   0 boileau    (502) staff       (20)     1130 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_antiderivative.py
--rw-r--r--   0 boileau    (502) staff       (20)     1260 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_elliptic.py
--rw-r--r--   0 boileau    (502) staff       (20)     2039 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_heat.py
--rw-r--r--   0 boileau    (502) staff       (20)     2896 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_laplacian.py
--rw-r--r--   0 boileau    (502) staff       (20)     1575 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_laplacian_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)     2409 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1x1v_transport.py
--rw-r--r--   0 boileau    (502) staff       (20)     1261 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_2d_laplacian.py
--rw-r--r--   0 boileau    (502) staff       (20)    35904 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pdes.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.763092 scimba-0.4.1/src/scimba/generativenets/
--rw-r--r--   0 boileau    (502) staff       (20)      147 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/generativenets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)        5 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/generativenets/energy_models.py
--rw-r--r--   0 boileau    (502) staff       (20)     6689 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/gaussian_mixtures.py
--rw-r--r--   0 boileau    (502) staff       (20)     4980 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/normalizingflows.py
--rw-r--r--   0 boileau    (502) staff       (20)     7503 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/simpleflows.py
--rw-r--r--   0 boileau    (502) staff       (20)     7607 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/trainer_likelihood.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.763485 scimba-0.4.1/src/scimba/largenets/
--rw-r--r--   0 boileau    (502) staff       (20)       77 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2173 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/continuous_autoencoder.py
--rw-r--r--   0 boileau    (502) staff       (20)     8941 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/pointnet.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.764978 scimba-0.4.1/src/scimba/nets/
--rw-r--r--   0 boileau    (502) staff       (20)      119 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/nets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    12262 2024-04-16 11:55:31.000000 scimba-0.4.1/src/scimba/nets/activation.py
--rw-r--r--   0 boileau    (502) staff       (20)     1603 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/convexnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     2044 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/nets/henonnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     8945 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/mlp.py
--rw-r--r--   0 boileau    (502) staff       (20)     4788 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/rbfnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     3973 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/siren.py
--rw-r--r--   0 boileau    (502) staff       (20)     8062 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/training.py
--rw-r--r--   0 boileau    (502) staff       (20)     5448 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/training_tools.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.766932 scimba-0.4.1/src/scimba/neural_operators/
--rw-r--r--   0 boileau    (502) staff       (20)      118 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     1984 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     2471 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     2185 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     4950 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     9037 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     6666 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      848 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     1057 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     1002 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      356 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_t.py
--rw-r--r--   0 boileau    (502) staff       (20)      708 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      783 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_xt.py
--rw-r--r--   0 boileau    (502) staff       (20)     3399 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/local_sublayer.py
--rw-r--r--   0 boileau    (502) staff       (20)     3235 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/pre_post_processinglayer.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.767912 scimba-0.4.1/src/scimba/neuralgalerkin/
--rw-r--r--   0 boileau    (502) staff       (20)      121 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/neuralgalerkin/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)      885 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/neuralgalerkin/elliptic_reduced_ng.py
--rw-r--r--   0 boileau    (502) staff       (20)    13037 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    11820 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)     4225 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/projector_training.py
--rw-r--r--   0 boileau    (502) staff       (20)     9728 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/reduced_ng.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.768523 scimba-0.4.1/src/scimba/numericalmethods/
--rw-r--r--   0 boileau    (502) staff       (20)       76 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     3610 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/mesh.py
--rw-r--r--   0 boileau    (502) staff       (20)     3905 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/neural_finite_element.py
--rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/neural_spectral.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.769259 scimba-0.4.1/src/scimba/odelearning/
--rw-r--r--   0 boileau    (502) staff       (20)      333 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2703 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/abstract_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)     2425 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/generation_ode_data.py
--rw-r--r--   0 boileau    (502) staff       (20)     1505 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/odelearning/generic_flux.py
--rw-r--r--   0 boileau    (502) staff       (20)     1574 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/loss_odelearning.py
--rw-r--r--   0 boileau    (502) staff       (20)     4194 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/odelearning/training_diffphy_ode.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.771061 scimba-0.4.1/src/scimba/pinns/
--rw-r--r--   0 boileau    (502) staff       (20)      333 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/pinns/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    11935 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_losses.py
--rw-r--r--   0 boileau    (502) staff       (20)    15699 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    15132 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    13666 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    18397 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     7900 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)    15285 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    20632 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    17740 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    46911 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    15301 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_xv.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.772061 scimba-0.4.1/src/scimba/pinos/
--rw-r--r--   0 boileau    (502) staff       (20)       33 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/pinos/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2829 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     5818 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     6463 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    11518 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    16685 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    14060 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_x.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.773831 scimba-0.4.1/src/scimba/sampling/
--rw-r--r--   0 boileau    (502) staff       (20)       65 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/sampling/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)      890 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/abstract_sampling.py
--rw-r--r--   0 boileau    (502) staff       (20)     8344 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)    20795 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_pde_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    12841 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_pde_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     1698 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/grid_sampling.py
--rw-r--r--   0 boileau    (502) staff       (20)      671 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/quad.py
--rw-r--r--   0 boileau    (502) staff       (20)    16527 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_functions.py
--rw-r--r--   0 boileau    (502) staff       (20)     7620 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)     1651 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_parameters.py
--rw-r--r--   0 boileau    (502) staff       (20)    16895 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_pde.py
--rw-r--r--   0 boileau    (502) staff       (20)    12729 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_pde_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    11087 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/uniform_sampling.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.777498 scimba-0.4.1/src/scimba.egg-info/
--rw-r--r--   0 boileau    (502) staff       (20)     4767 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/PKG-INFO
--rw-r--r--   0 boileau    (502) staff       (20)     4670 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/SOURCES.txt
--rw-r--r--   0 boileau    (502) staff       (20)        1 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/dependency_links.txt
--rw-r--r--   0 boileau    (502) staff       (20)      153 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/requires.txt
--rw-r--r--   0 boileau    (502) staff       (20)       20 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/top_level.txt
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.777321 scimba-0.4.1/tests/
--rw-r--r--   0 boileau    (502) staff       (20)     4941 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_DeepOnet_space.py
--rw-r--r--   0 boileau    (502) staff       (20)     3320 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_DeepOnet_time.py
--rw-r--r--   0 boileau    (502) staff       (20)     3659 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_Laplacian2D.py
--rw-r--r--   0 boileau    (502) staff       (20)     2607 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_advection_xv1d_nn.py
--rw-r--r--   0 boileau    (502) staff       (20)     3313 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_cond.py
--rw-r--r--   0 boileau    (502) staff       (20)      997 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_gaussianmixture.py
--rw-r--r--   0 boileau    (502) staff       (20)     3439 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_grad_div_2D_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)     3153 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_heat_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)       75 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_import.py
--rw-r--r--   0 boileau    (502) staff       (20)     1215 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_kinetic_constant_transport_1X1V.py
--rw-r--r--   0 boileau    (502) staff       (20)     8254 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_bean.py
--rw-r--r--   0 boileau    (502) staff       (20)     5353 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_domainhole.py
--rw-r--r--   0 boileau    (502) staff       (20)     2787 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_rbfnet_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)     2997 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_signeddistance.py
--rw-r--r--   0 boileau    (502) staff       (20)     1275 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian_1d.py
--rw-r--r--   0 boileau    (502) staff       (20)     3690 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_linearized_Euler.py
--rw-r--r--   0 boileau    (502) staff       (20)     1156 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_mlp.py
--rw-r--r--   0 boileau    (502) staff       (20)     4038 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_multiscale_fourier.py
--rw-r--r--   0 boileau    (502) staff       (20)     2792 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_neural_galerkin.py
--rw-r--r--   0 boileau    (502) staff       (20)    14390 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_Laplacian_2D.py
--rw-r--r--   0 boileau    (502) staff       (20)     6926 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_odes.py
--rw-r--r--   0 boileau    (502) staff       (20)     7130 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_spacetime_system.py
--rw-r--r--   0 boileau    (502) staff       (20)     1546 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_normalizingflow.py
--rw-r--r--   0 boileau    (502) staff       (20)     2465 2024-01-08 14:56:39.000000 scimba-0.4.1/tests/test_odelearning_sir.py
--rw-r--r--   0 boileau    (502) staff       (20)     5821 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_pendulum.py
--rw-r--r--   0 boileau    (502) staff       (20)     1822 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_poisson_xv1D.py
--rw-r--r--   0 boileau    (502) staff       (20)     1482 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_simple_ode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.188684 scimba-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-09-27 09:34:10.000000 scimba-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4999 2024-04-30 13:05:44.188684 scimba-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3873 2024-04-30 12:56:53.000000 scimba-0.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2024-04-30 12:56:53.000000 scimba-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 13:05:44.188684 scimba-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.132684 scimba-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.148684 scimba-0.4.2/src/applications/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 13:05:22.000000 scimba-0.4.2/src/applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.148684 scimba-0.4.2/src/scimba/
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.152684 scimba-0.4.2/src/scimba/equations/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-03 09:48:10.000000 scimba-0.4.2/src/scimba/equations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23566 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/equations/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/genericSL_advection_diffusion_equation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8548 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/nonlinear_ode_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9299 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/equations/ode_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1d_antiderivative.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1d_elliptic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1d_heat.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1d_laplacian.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1d_laplacian_xv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_1x1v_transport.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/equations/pde_2d_laplacian.py
+-rw-rw-rw-   0 root         (0) root         (0)    35904 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/equations/pdes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.152684 scimba-0.4.2/src/scimba/generativenets/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-09-28 13:15:22.000000 scimba-0.4.2/src/scimba/generativenets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-09-27 09:34:10.000000 scimba-0.4.2/src/scimba/generativenets/energy_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6689 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/generativenets/gaussian_mixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     4980 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/generativenets/normalizingflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     7503 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/generativenets/simpleflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     7607 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/generativenets/trainer_likelihood.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.156684 scimba-0.4.2/src/scimba/largenets/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-03 09:48:10.000000 scimba-0.4.2/src/scimba/largenets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2024-03-04 10:49:23.000000 scimba-0.4.2/src/scimba/largenets/continuous_autoencoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8941 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/largenets/pointnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.156684 scimba-0.4.2/src/scimba/nets/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-09-28 13:15:22.000000 scimba-0.4.2/src/scimba/nets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12262 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/nets/activation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2024-03-04 10:49:23.000000 scimba-0.4.2/src/scimba/nets/convexnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-12-14 13:00:52.000000 scimba-0.4.2/src/scimba/nets/henonnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     8945 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/nets/mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4788 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/nets/rbfnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3973 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/nets/siren.py
+-rw-rw-rw-   0 root         (0) root         (0)     8062 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/nets/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     5448 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/nets/training_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.160684 scimba-0.4.2/src/scimba/neural_operators/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-03 09:48:10.000000 scimba-0.4.2/src/scimba/neural_operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/neural_operators/deep_operator_t.py
+-rw-rw-rw-   0 root         (0) root         (0)     2471 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/neural_operators/deep_operator_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/deep_operator_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2024-04-19 11:01:46.000000 scimba-0.4.2/src/scimba/neural_operators/deeponet_t.py
+-rw-rw-rw-   0 root         (0) root         (0)     9037 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/deeponet_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/deeponet_x.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/neural_operators/greenkernel_t.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/neural_operators/greenkernel_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/greenkernel_x.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-02-23 23:18:58.000000 scimba-0.4.2/src/scimba/neural_operators/kernel_layer_t.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/kernel_layer_x.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-02-23 23:18:58.000000 scimba-0.4.2/src/scimba/neural_operators/kernel_layer_xt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neural_operators/local_sublayer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3235 2024-02-23 23:18:58.000000 scimba-0.4.2/src/scimba/neural_operators/pre_post_processinglayer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.160684 scimba-0.4.2/src/scimba/neuralgalerkin/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-09-28 13:15:22.000000 scimba-0.4.2/src/scimba/neuralgalerkin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2023-12-14 13:00:52.000000 scimba-0.4.2/src/scimba/neuralgalerkin/elliptic_reduced_ng.py
+-rw-rw-rw-   0 root         (0) root         (0)    13037 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neuralgalerkin/neural_galerkin_x.py
+-rw-rw-rw-   0 root         (0) root         (0)    11820 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/neuralgalerkin/neural_galerkin_xv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4225 2024-04-23 21:44:29.000000 scimba-0.4.2/src/scimba/neuralgalerkin/projector_training.py
+-rw-rw-rw-   0 root         (0) root         (0)     9728 2024-04-19 11:01:46.000000 scimba-0.4.2/src/scimba/neuralgalerkin/reduced_ng.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.160684 scimba-0.4.2/src/scimba/numericalmethods/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-03 09:48:10.000000 scimba-0.4.2/src/scimba/numericalmethods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/numericalmethods/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/numericalmethods/neural_finite_element.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 13:05:22.000000 scimba-0.4.2/src/scimba/numericalmethods/neural_spectral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.160684 scimba-0.4.2/src/scimba/odelearning/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-14 13:00:52.000000 scimba-0.4.2/src/scimba/odelearning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2024-02-08 11:20:56.000000 scimba-0.4.2/src/scimba/odelearning/abstract_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2023-12-18 14:21:59.000000 scimba-0.4.2/src/scimba/odelearning/generation_ode_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/odelearning/generic_flux.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-12-18 14:21:59.000000 scimba-0.4.2/src/scimba/odelearning/loss_odelearning.py
+-rw-rw-rw-   0 root         (0) root         (0)     4194 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/odelearning/training_diffphy_ode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.164684 scimba-0.4.2/src/scimba/pinns/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-09-28 13:15:22.000000 scimba-0.4.2/src/scimba/pinns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11935 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/pinn_losses.py
+-rw-rw-rw-   0 root         (0) root         (0)    15699 2024-04-03 09:48:10.000000 scimba-0.4.2/src/scimba/pinns/pinn_t.py
+-rw-rw-rw-   0 root         (0) root         (0)    15132 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/pinns/pinn_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)    13666 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/pinns/pinn_txv.py
+-rw-rw-rw-   0 root         (0) root         (0)    18397 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/pinn_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     7900 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/pinns/pinn_xv.py
+-rw-rw-rw-   0 root         (0) root         (0)    15285 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/training_t.py
+-rw-rw-rw-   0 root         (0) root         (0)    20632 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/training_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)    17740 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/training_txv.py
+-rw-rw-rw-   0 root         (0) root         (0)    46911 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/training_x.py
+-rw-rw-rw-   0 root         (0) root         (0)    15301 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinns/training_xv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.164684 scimba-0.4.2/src/scimba/pinos/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-12-14 13:00:52.000000 scimba-0.4.2/src/scimba/pinos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/pinos/pino_t.py
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/pinos/pino_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/pinos/pino_x.py
+-rw-rw-rw-   0 root         (0) root         (0)    11518 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinos/training_t.py
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinos/training_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)    14060 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/pinos/training_x.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.168684 scimba-0.4.2/src/scimba/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-09-28 13:15:22.000000 scimba-0.4.2/src/scimba/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/abstract_sampling.py
+-rw-rw-rw-   0 root         (0) root         (0)     8344 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/sampling/data_sampling_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)    20795 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/data_sampling_pde_tx.py
+-rw-rw-rw-   0 root         (0) root         (0)    12841 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/data_sampling_pde_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/sampling/grid_sampling.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-02-28 10:12:30.000000 scimba-0.4.2/src/scimba/sampling/quad.py
+-rw-rw-rw-   0 root         (0) root         (0)    16527 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/sampling_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7620 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/sampling/sampling_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/sampling_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16895 2024-04-30 12:56:53.000000 scimba-0.4.2/src/scimba/sampling/sampling_pde.py
+-rw-rw-rw-   0 root         (0) root         (0)    12729 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/sampling_pde_txv.py
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2024-04-30 11:48:24.000000 scimba-0.4.2/src/scimba/sampling/uniform_sampling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.184684 scimba-0.4.2/src/scimba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4999 2024-04-30 13:05:44.000000 scimba-0.4.2/src/scimba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4670 2024-04-30 13:05:44.000000 scimba-0.4.2/src/scimba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 13:05:44.000000 scimba-0.4.2/src/scimba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-30 13:05:44.000000 scimba-0.4.2/src/scimba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-30 13:05:44.000000 scimba-0.4.2/src/scimba.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:05:44.184684 scimba-0.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4941 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_DeepOnet_space.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_DeepOnet_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3659 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_Laplacian2D.py
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_advection_xv1d_nn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_cond.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_gaussianmixture.py
+-rw-rw-rw-   0 root         (0) root         (0)     3439 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_grad_div_2D_pinns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_heat_pinns.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_kinetic_constant_transport_1X1V.py
+-rw-rw-rw-   0 root         (0) root         (0)     8254 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_laplacian2D_bean.py
+-rw-rw-rw-   0 root         (0) root         (0)     5353 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_laplacian2D_domainhole.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_laplacian2D_rbfnet_pinns.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_laplacian2D_signeddistance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_laplacian_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_linearized_Euler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2024-04-30 12:56:53.000000 scimba-0.4.2/tests/test_mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_multiscale_fourier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_neural_galerkin.py
+-rw-rw-rw-   0 root         (0) root         (0)    14390 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_nonlinear_Laplacian_2D.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_nonlinear_odes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_nonlinear_spacetime_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2024-02-23 23:18:58.000000 scimba-0.4.2/tests/test_normalizingflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2465 2024-02-08 11:20:56.000000 scimba-0.4.2/tests/test_odelearning_sir.py
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_pendulum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_poisson_xv1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-30 11:48:24.000000 scimba-0.4.2/tests/test_simple_ode.py
```

### Comparing `scimba-0.4.1/LICENSE` & `scimba-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/PKG-INFO` & `scimba-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scimba
-Version: 0.4.1
+Version: 0.4.2
 Summary: This library implements some common tools for scientific machine learning
 Author: Emmanuel Franck
 License: MIT
-Project-URL: Homepage, https://gitlab.inria.fr/sciml/scimba
+Project-URL: Homepage, https://gitlab.inria.fr/scimba/scimba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
@@ -17,25 +17,30 @@
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Provides-Extra: doc
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx-autobuild; extra == "doc"
+Requires-Dist: Sphinx>=7.2.2; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: furo; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: sphinx-autobuild; extra == "doc"
 Provides-Extra: examples
 Requires-Dist: h5py; extra == "examples"
 Requires-Dist: PyYAML; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 
 # ScimBa
 
-[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
+[![pipeline status](https://gitlab.inria.fr/scimba/scimba/badges/main/pipeline.svg)](https://gitlab.inria.fr/scimba/scimba/-/commits/main)
+[![coverage report](https://gitlab.inria.fr/scimba/scimba/badges/main/coverage.svg)](https://sciml.gitlabpages.inria.fr/scimba/coverage)
+[![Latest Release](https://gitlab.inria.fr/scimba/scimba/-/badges/release.svg)](https://gitlab.inria.fr/scimba/scimba/-/releases)
+[![Doc](https://img.shields.io/badge/doc-sphinx-blue)](hhttps://sciml.gitlabpages.inria.fr/scimba/)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -99,31 +104,7 @@
 
 - https://openreview.net/forum?id=LZDiWaC9CGL
 - https://arxiv.org/abs/2205.10573
 - https://arxiv.org/abs/2205.02191
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
-
-## Install the project
-
-```bash
-pip install scimba
-```
-
-
-## Launch tests
-
-```bash
-pip install "scimba[test]"
-pytest
-```
-
-## Generate documentation
-
-```bash
-pip install "scimba[doc]"
-cd docs
-env PYTORCH_JIT=0 make html
-```
-
-html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.1/README.md` & `scimba-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # ScimBa
 
-[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
+[![pipeline status](https://gitlab.inria.fr/scimba/scimba/badges/main/pipeline.svg)](https://gitlab.inria.fr/scimba/scimba/-/commits/main)
+[![coverage report](https://gitlab.inria.fr/scimba/scimba/badges/main/coverage.svg)](https://sciml.gitlabpages.inria.fr/scimba/coverage)
+[![Latest Release](https://gitlab.inria.fr/scimba/scimba/-/badges/release.svg)](https://gitlab.inria.fr/scimba/scimba/-/releases)
+[![Doc](https://img.shields.io/badge/doc-sphinx-blue)](hhttps://sciml.gitlabpages.inria.fr/scimba/)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -68,31 +71,7 @@
 
 - https://openreview.net/forum?id=LZDiWaC9CGL
 - https://arxiv.org/abs/2205.10573
 - https://arxiv.org/abs/2205.02191
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
-
-## Install the project
-
-```bash
-pip install scimba
-```
-
-
-## Launch tests
-
-```bash
-pip install "scimba[test]"
-pytest
-```
-
-## Generate documentation
-
-```bash
-pip install "scimba[doc]"
-cd docs
-env PYTORCH_JIT=0 make html
-```
-
-html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.1/pyproject.toml` & `scimba-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,25 +19,31 @@
 file = "README.md"
 content-type = "text/markdown"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-Homepage = "https://gitlab.inria.fr/sciml/scimba"
+Homepage = "https://gitlab.inria.fr/scimba/scimba"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "scikit-learn"]
-doc = ["sphinx", "sphinx-autobuild", "furo"]
+doc = [
+    "Sphinx >= 7.2.2",
+    "myst-parser",
+    "furo",
+    "sphinx-copybutton",
+    "sphinx-autobuild",
+]
 examples = ["h5py", "PyYAML", "scikit-learn"]
 
 [tool.setuptools]
 include-package-data = true
 license-files = ["LICENSE"]
-package-dir = { "" = "src"}
+package-dir = { "" = "src" }
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
 [tool.setuptools.dynamic.version]
 attr = "scimba.__version__"
```

### Comparing `scimba-0.4.1/src/scimba/equations/domain.py` & `scimba-0.4.2/src/scimba/equations/domain.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/genericSL_advection_diffusion_equation.py` & `scimba-0.4.2/src/scimba/equations/genericSL_advection_diffusion_equation.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/nonlinear_ode_basic.py` & `scimba-0.4.2/src/scimba/equations/nonlinear_ode_basic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/ode_basic.py` & `scimba-0.4.2/src/scimba/equations/ode_basic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1d_antiderivative.py` & `scimba-0.4.2/src/scimba/equations/pde_1d_antiderivative.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1d_elliptic.py` & `scimba-0.4.2/src/scimba/equations/pde_1d_elliptic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1d_heat.py` & `scimba-0.4.2/src/scimba/equations/pde_1d_heat.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1d_laplacian.py` & `scimba-0.4.2/src/scimba/equations/pde_1d_laplacian.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1d_laplacian_xv.py` & `scimba-0.4.2/src/scimba/equations/pde_1d_laplacian_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_1x1v_transport.py` & `scimba-0.4.2/src/scimba/equations/pde_1x1v_transport.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pde_2d_laplacian.py` & `scimba-0.4.2/src/scimba/equations/pde_2d_laplacian.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/equations/pdes.py` & `scimba-0.4.2/src/scimba/equations/pdes.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/generativenets/gaussian_mixtures.py` & `scimba-0.4.2/src/scimba/generativenets/gaussian_mixtures.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/generativenets/normalizingflows.py` & `scimba-0.4.2/src/scimba/generativenets/normalizingflows.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/generativenets/simpleflows.py` & `scimba-0.4.2/src/scimba/generativenets/simpleflows.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/generativenets/trainer_likelihood.py` & `scimba-0.4.2/src/scimba/generativenets/trainer_likelihood.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/largenets/continuous_autoencoder.py` & `scimba-0.4.2/src/scimba/largenets/continuous_autoencoder.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/largenets/pointnet.py` & `scimba-0.4.2/src/scimba/largenets/pointnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/activation.py` & `scimba-0.4.2/src/scimba/nets/activation.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/convexnet.py` & `scimba-0.4.2/src/scimba/nets/convexnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/henonnet.py` & `scimba-0.4.2/src/scimba/nets/henonnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/mlp.py` & `scimba-0.4.2/src/scimba/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/rbfnet.py` & `scimba-0.4.2/src/scimba/nets/rbfnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/siren.py` & `scimba-0.4.2/src/scimba/nets/siren.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/training.py` & `scimba-0.4.2/src/scimba/nets/training.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/nets/training_tools.py` & `scimba-0.4.2/src/scimba/nets/training_tools.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deep_operator_t.py` & `scimba-0.4.2/src/scimba/neural_operators/deep_operator_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deep_operator_tx.py` & `scimba-0.4.2/src/scimba/neural_operators/deep_operator_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deep_operator_x.py` & `scimba-0.4.2/src/scimba/neural_operators/deep_operator_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deeponet_t.py` & `scimba-0.4.2/src/scimba/neural_operators/deeponet_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deeponet_tx.py` & `scimba-0.4.2/src/scimba/neural_operators/deeponet_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/deeponet_x.py` & `scimba-0.4.2/src/scimba/neural_operators/deeponet_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/greenkernel_t.py` & `scimba-0.4.2/src/scimba/neural_operators/greenkernel_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/greenkernel_tx.py` & `scimba-0.4.2/src/scimba/neural_operators/greenkernel_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/greenkernel_x.py` & `scimba-0.4.2/src/scimba/neural_operators/greenkernel_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/kernel_layer_x.py` & `scimba-0.4.2/src/scimba/neural_operators/kernel_layer_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/kernel_layer_xt.py` & `scimba-0.4.2/src/scimba/neural_operators/kernel_layer_xt.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/local_sublayer.py` & `scimba-0.4.2/src/scimba/neural_operators/local_sublayer.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neural_operators/pre_post_processinglayer.py` & `scimba-0.4.2/src/scimba/neural_operators/pre_post_processinglayer.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neuralgalerkin/elliptic_reduced_ng.py` & `scimba-0.4.2/src/scimba/neuralgalerkin/elliptic_reduced_ng.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_x.py` & `scimba-0.4.2/src/scimba/neuralgalerkin/neural_galerkin_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_xv.py` & `scimba-0.4.2/src/scimba/neuralgalerkin/neural_galerkin_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neuralgalerkin/projector_training.py` & `scimba-0.4.2/src/scimba/neuralgalerkin/projector_training.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/neuralgalerkin/reduced_ng.py` & `scimba-0.4.2/src/scimba/neuralgalerkin/reduced_ng.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/numericalmethods/mesh.py` & `scimba-0.4.2/src/scimba/numericalmethods/mesh.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/numericalmethods/neural_finite_element.py` & `scimba-0.4.2/src/scimba/numericalmethods/neural_finite_element.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/odelearning/abstract_ode.py` & `scimba-0.4.2/src/scimba/odelearning/abstract_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/odelearning/generation_ode_data.py` & `scimba-0.4.2/src/scimba/odelearning/generation_ode_data.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/odelearning/generic_flux.py` & `scimba-0.4.2/src/scimba/odelearning/generic_flux.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/odelearning/loss_odelearning.py` & `scimba-0.4.2/src/scimba/odelearning/loss_odelearning.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/odelearning/training_diffphy_ode.py` & `scimba-0.4.2/src/scimba/odelearning/training_diffphy_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_losses.py` & `scimba-0.4.2/src/scimba/pinns/pinn_losses.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_t.py` & `scimba-0.4.2/src/scimba/pinns/pinn_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_tx.py` & `scimba-0.4.2/src/scimba/pinns/pinn_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_txv.py` & `scimba-0.4.2/src/scimba/pinns/pinn_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_x.py` & `scimba-0.4.2/src/scimba/pinns/pinn_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/pinn_xv.py` & `scimba-0.4.2/src/scimba/pinns/pinn_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/training_t.py` & `scimba-0.4.2/src/scimba/pinns/training_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/training_tx.py` & `scimba-0.4.2/src/scimba/pinns/training_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/training_txv.py` & `scimba-0.4.2/src/scimba/pinns/training_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/training_x.py` & `scimba-0.4.2/src/scimba/pinns/training_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinns/training_xv.py` & `scimba-0.4.2/src/scimba/pinns/training_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/pino_t.py` & `scimba-0.4.2/src/scimba/pinos/pino_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/pino_tx.py` & `scimba-0.4.2/src/scimba/pinos/pino_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/pino_x.py` & `scimba-0.4.2/src/scimba/pinos/pino_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/training_t.py` & `scimba-0.4.2/src/scimba/pinos/training_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/training_tx.py` & `scimba-0.4.2/src/scimba/pinos/training_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/pinos/training_x.py` & `scimba-0.4.2/src/scimba/pinos/training_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/abstract_sampling.py` & `scimba-0.4.2/src/scimba/sampling/abstract_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/data_sampling_ode.py` & `scimba-0.4.2/src/scimba/sampling/data_sampling_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/data_sampling_pde_tx.py` & `scimba-0.4.2/src/scimba/sampling/data_sampling_pde_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/data_sampling_pde_x.py` & `scimba-0.4.2/src/scimba/sampling/data_sampling_pde_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/grid_sampling.py` & `scimba-0.4.2/src/scimba/sampling/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/quad.py` & `scimba-0.4.2/src/scimba/sampling/quad.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/sampling_functions.py` & `scimba-0.4.2/src/scimba/sampling/sampling_functions.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/sampling_ode.py` & `scimba-0.4.2/src/scimba/sampling/sampling_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/sampling_parameters.py` & `scimba-0.4.2/src/scimba/sampling/sampling_parameters.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/sampling_pde.py` & `scimba-0.4.2/src/scimba/sampling/sampling_pde.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/sampling_pde_txv.py` & `scimba-0.4.2/src/scimba/sampling/sampling_pde_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba/sampling/uniform_sampling.py` & `scimba-0.4.2/src/scimba/sampling/uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/src/scimba.egg-info/PKG-INFO` & `scimba-0.4.2/src/scimba.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scimba
-Version: 0.4.1
+Version: 0.4.2
 Summary: This library implements some common tools for scientific machine learning
 Author: Emmanuel Franck
 License: MIT
-Project-URL: Homepage, https://gitlab.inria.fr/sciml/scimba
+Project-URL: Homepage, https://gitlab.inria.fr/scimba/scimba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
@@ -17,25 +17,30 @@
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Provides-Extra: doc
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx-autobuild; extra == "doc"
+Requires-Dist: Sphinx>=7.2.2; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: furo; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: sphinx-autobuild; extra == "doc"
 Provides-Extra: examples
 Requires-Dist: h5py; extra == "examples"
 Requires-Dist: PyYAML; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 
 # ScimBa
 
-[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
+[![pipeline status](https://gitlab.inria.fr/scimba/scimba/badges/main/pipeline.svg)](https://gitlab.inria.fr/scimba/scimba/-/commits/main)
+[![coverage report](https://gitlab.inria.fr/scimba/scimba/badges/main/coverage.svg)](https://sciml.gitlabpages.inria.fr/scimba/coverage)
+[![Latest Release](https://gitlab.inria.fr/scimba/scimba/-/badges/release.svg)](https://gitlab.inria.fr/scimba/scimba/-/releases)
+[![Doc](https://img.shields.io/badge/doc-sphinx-blue)](hhttps://sciml.gitlabpages.inria.fr/scimba/)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -99,31 +104,7 @@
 
 - https://openreview.net/forum?id=LZDiWaC9CGL
 - https://arxiv.org/abs/2205.10573
 - https://arxiv.org/abs/2205.02191
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
-
-## Install the project
-
-```bash
-pip install scimba
-```
-
-
-## Launch tests
-
-```bash
-pip install "scimba[test]"
-pytest
-```
-
-## Generate documentation
-
-```bash
-pip install "scimba[doc]"
-cd docs
-env PYTORCH_JIT=0 make html
-```
-
-html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.1/src/scimba.egg-info/SOURCES.txt` & `scimba-0.4.2/src/scimba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_DeepOnet_space.py` & `scimba-0.4.2/tests/test_DeepOnet_space.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_DeepOnet_time.py` & `scimba-0.4.2/tests/test_DeepOnet_time.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_Laplacian2D.py` & `scimba-0.4.2/tests/test_Laplacian2D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_advection_xv1d_nn.py` & `scimba-0.4.2/tests/test_advection_xv1d_nn.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_cond.py` & `scimba-0.4.2/tests/test_cond.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_gaussianmixture.py` & `scimba-0.4.2/tests/test_gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_grad_div_2D_pinns.py` & `scimba-0.4.2/tests/test_grad_div_2D_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_heat_pinns.py` & `scimba-0.4.2/tests/test_heat_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_kinetic_constant_transport_1X1V.py` & `scimba-0.4.2/tests/test_kinetic_constant_transport_1X1V.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_laplacian2D_bean.py` & `scimba-0.4.2/tests/test_laplacian2D_bean.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_laplacian2D_domainhole.py` & `scimba-0.4.2/tests/test_laplacian2D_domainhole.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_laplacian2D_rbfnet_pinns.py` & `scimba-0.4.2/tests/test_laplacian2D_rbfnet_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_laplacian2D_signeddistance.py` & `scimba-0.4.2/tests/test_laplacian2D_signeddistance.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_laplacian_1d.py` & `scimba-0.4.2/tests/test_laplacian_1d.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_linearized_Euler.py` & `scimba-0.4.2/tests/test_linearized_Euler.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_mlp.py` & `scimba-0.4.2/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_multiscale_fourier.py` & `scimba-0.4.2/tests/test_multiscale_fourier.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_neural_galerkin.py` & `scimba-0.4.2/tests/test_neural_galerkin.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_nonlinear_Laplacian_2D.py` & `scimba-0.4.2/tests/test_nonlinear_Laplacian_2D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_nonlinear_odes.py` & `scimba-0.4.2/tests/test_nonlinear_odes.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_nonlinear_spacetime_system.py` & `scimba-0.4.2/tests/test_nonlinear_spacetime_system.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_normalizingflow.py` & `scimba-0.4.2/tests/test_normalizingflow.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_odelearning_sir.py` & `scimba-0.4.2/tests/test_odelearning_sir.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_pendulum.py` & `scimba-0.4.2/tests/test_pendulum.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_poisson_xv1D.py` & `scimba-0.4.2/tests/test_poisson_xv1D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.1/tests/test_simple_ode.py` & `scimba-0.4.2/tests/test_simple_ode.py`

 * *Files identical despite different names*

