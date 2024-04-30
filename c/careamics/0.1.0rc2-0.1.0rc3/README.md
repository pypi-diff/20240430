# Comparing `tmp/careamics-0.1.0rc2.tar.gz` & `tmp/careamics-0.1.0rc3.tar.gz`

## Comparing `careamics-0.1.0rc2.tar` & `careamics-0.1.0rc3.tar`

### file list

```diff
@@ -1,91 +1,170 @@
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/dependabot.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/pull_request_template.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/n2v_full_reference.yml
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/2D/example_BSD68.ipynb
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/2D/example_SEM.ipynb
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/2D/n2v_2D_BSD.yml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/2D/n2v_2D_SEM.yml
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/3D/example_flywing_3D.ipynb
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/3D/n2v_3D.yml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/examples/3D/n2v_flywing_3D.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/__init__.py
--rw-r--r--   0        0        0    34132 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/engine.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/bioimage/__init__.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/bioimage/io.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/bioimage/rdf.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/bioimage/docs/Noise2Void.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/bioimage/docs/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/__init__.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/algorithm.py
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/config.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/config_filter.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/data.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/torch_optim.py
--rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/config/training.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/__init__.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/dataset_utils.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/extraction_strategy.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/in_memory_dataset.py
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/patching.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/prepare_dataset.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/dataset/tiff_dataset.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/losses/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/losses/loss_factory.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/losses/losses.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/manipulation/__init__.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/manipulation/pixel_manipulation.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/models/__init__.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/models/layers.py
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/models/model_factory.py
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/models/unet.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/prediction/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/prediction/prediction_utils.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/ascii_logo.txt
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/augment.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/context.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/logging.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/metrics.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/normalization.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/torch_utils.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/validators.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/src/careamics/utils/wandb.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/conftest.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/smoke_test.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/test_augment.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/test_conftest.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/test_engine.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/test_metrics.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/test_prediction_utils.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/bioimage/test_engine_bmz.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/bioimage/test_io.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/bioimage/test_rdf.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_algorithm.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_config.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_config_filters.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_data.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_torch_optimizer.py
--rw-r--r--   0        0        0    14960 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/config/test_training.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/dataset/test_dataset_utils.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/dataset/test_patching.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/dataset/test_tiff_dataset.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/manipulation/test_pixel_manipulation.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/model/test_model.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/model/test_model_factory.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/utils/test_context.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/utils/test_logging.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/utils/test_torch_utils.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/utils/test_validators.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/tests/utils/test_wandb.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/README.md
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 careamics-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/PR_TEMPLATE/pull_request.md
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2n/example_SEM_careamist.ipynb
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2n/n2n_2D_SEM.yml
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_careamist.ipynb
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_lightning.ipynb
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_SEM_lightning.ipynb
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/n2v_2D_BSD.yml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/pn2v/pN2V_Convallaria.yml
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/3D/example_flywing_3D.ipynb
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/3D/n2v_flywing_3D.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/__init__.py
+-rw-r--r--   0        0        0    28336 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/careamist.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/conftest.py
+-rw-r--r--   0        0        0    28552 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_datamodule.py
+-rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_module.py
+-rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_prediction_datamodule.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_prediction_loop.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/py.typed
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/hyperparameters_callback.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/progress_bar_callback.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/__init__.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/algorithm_model.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/callback_model.py
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/configuration_factory.py
+-rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/configuration_model.py
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/data_model.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/inference_model.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/noise_models.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/optimizer_models.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/tile_information.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/training_model.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/architecture_model.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/custom_model.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/register_model.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/unet_model.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/vae_model.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/__init__.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/algorithm_descriptions.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/references.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_activations.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_algorithms.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_architectures.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_data.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_extraction_strategies.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_loggers.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_losses.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_optimizers.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_pixel_manipulations.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_struct_axis.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_transforms.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/__init__.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/n2v_manipulate_model.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/nd_flip_model.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/normalize_model.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/transform_model.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/xy_random_rotate90_model.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/validators/__init__.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/validators/validator_utils.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/__init__.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/in_memory_dataset.py
+-rw-r--r--   0        0        0    15030 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/iterable_dataset.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/zarr_dataset.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/__init__.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/dataset_utils.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/file_utils.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_tiff.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_zarr.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/patch_transform.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/patching.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/random_patching.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/sequential_patching.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/tiled_patching.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/validate_patch_dimension.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/__init__.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/loss_factory.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/losses.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/noise_model_factory.py
+-rw-r--r--   0        0        0    17801 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/noise_models.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/__init__.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bmz_io.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/model_io_utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/__init__.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/_readme_factory.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/bioimage_utils.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/model_description.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/activation.py
+-rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/layers.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/model_factory.py
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/unet.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/prediction/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/prediction/stitch_prediction.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/__init__.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/n2v_manipulate.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/nd_flip.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/normalize.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/pixel_manipulation.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/struct_mask_parameters.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/tta.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/xy_random_rotate90.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/base_enum.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/context.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/logging.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/metrics.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/path_utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/ram.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/receptive_field.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/running_stats.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/torch_utils.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/conftest.py
+-rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_careamist.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_conftest.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_lightning_datamodule.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_lightning_module.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_algorithm_model.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_configuration_factory.py
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_configuration_model.py
+-rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_data_model.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_inference_model.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_optimizers_model.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_tile_information.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_training_model.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_architecture_model.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_custom_model.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_register_model.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_unet_model.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/support/test_supported_data.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/support/test_supported_optimizers.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/transformations/test_n2v_manipulate_model.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/transformations/test_normalize_model.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/validators/test_validator_utils.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/test_in_memory_dataset.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/test_iterable_dataset.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/dataset_utils/test_list_files.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/dataset_utils/test_read_tiff.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_patching_utils.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_random_patching.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_sequential_patching.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_tiled_patching.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/model_io/test_bmz_io.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/models/test_model_factory.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/models/test_unet.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/prediction/test_stitch_prediction.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_manipulate_n2v.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_nd_flip.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_normalize.py
+-rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_pixel_manipulation.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_supported_transforms.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_xy_random_rotate90.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_base_enum.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_context.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_logging.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_metrics.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_torch_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_wandb.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/README.md
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/PKG-INFO
```

### Comparing `careamics-0.1.0rc2/.pre-commit-config.yaml` & `careamics-0.1.0rc3/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,56 @@
----
 # enable pre-commit.ci at https://pre-commit.ci/
 # it adds:
 # 1. auto fixing pull requests
 # 2. auto updating the pre-commit configuration
 ci:
-    autoupdate_schedule: monthly
-    autofix_commit_msg: 'style(pre-commit.ci): auto fixes [...]'
-    autoupdate_commit_msg: 'ci(pre-commit.ci): autoupdate'
+  autoupdate_schedule: monthly
+  autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
+  autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 repos:
-    - repo: https://github.com/abravalheri/validate-pyproject
-      rev: v0.15
-      hooks:
-          - id: validate-pyproject
-
-    - repo: https://github.com/astral-sh/ruff-pre-commit
-      rev: v0.1.6
-      hooks:
-          - id: ruff
-            args: [--fix, --target-version, py38]
-
-    - repo: https://github.com/psf/black
-      rev: 23.11.0
-      hooks:
-          - id: black
-
-    - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.7.1
-      hooks:
-          - id: mypy
-            files: ^src/
-            additional_dependencies:
-                - numpy
-                - types-PyYAML
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.14
+    hooks:
+      - id: validate-pyproject
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.292
+    hooks:
+      - id: ruff
+        args: [--fix, --target-version, py38]
+
+  - repo: https://github.com/psf/black
+    rev: 23.9.1
+    hooks:
+      - id: black
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.5.1
+    hooks:
+      - id: mypy
+        files: "^src/"
+        additional_dependencies:
+          - numpy
+          - types-PyYAML
+          - types-setuptools
 
   # check docstrings
-    - repo: https://github.com/numpy/numpydoc
-      rev: v1.6.0
-      hooks:
-          - id: numpydoc-validation
+  - repo: https://github.com/numpy/numpydoc
+    rev: v1.6.0
+    hooks:
+      - id: numpydoc-validation
 
   # jupyter linting and formatting
-    - repo: https://github.com/nbQA-dev/nbQA
-      rev: 1.7.1
-      hooks:
-          - id: nbqa-ruff
-            args: [--fix]
-          - id: nbqa-black
-  #- id: nbqa-mypy
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
+    hooks:
+      - id: nbqa-ruff
+        args: [--fix]
+      - id: nbqa-black
+      #- id: nbqa-mypy
 
   # strip out jupyter notebooks
-    - repo: https://github.com/kynan/nbstripout
-      rev: 0.6.1
-      hooks:
-          - id: nbstripout
-
-  # yaml formatter
-    - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.3
-      hooks:
-          - id: yamlfmt
+  - repo: https://github.com/kynan/nbstripout
+    rev: 0.6.1
+    hooks:
+      - id: nbstripout
```

### Comparing `careamics-0.1.0rc2/.github/pull_request_template.md` & `careamics-0.1.0rc3/.github/PR_TEMPLATE/pull_request.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,13 +21,14 @@
 
 **Screenshots**
 If applicable, add screenshots to help explain your problem.
 
 **Desktop (please complete the following information):**
  - OS: [e.g. iOS]
  - Version [e.g. 22]
+- microscopy-portfolio version [e.g. 0.0.5]
 
 **Environment:**
 Please add here the content of your conda environment with versions.
 
 **Additional context**
 Add any other context about the problem here.
```

### Comparing `careamics-0.1.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/.github/workflows/ci.yml` & `careamics-0.1.0rc3/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,108 @@
----
 name: CI
 
 on:
-    push:
-        branches:
-            - main
-        tags:
-            - v*.*.*
-    pull_request:
-    workflow_dispatch:
-    schedule:
+  push:
+    branches:
+      - main
+    tags:
+      - "v*"
+  pull_request:
+  workflow_dispatch:
+  schedule:
     # run every week (for --pre release tests)
-        - cron: 0 0 * * 0
+    - cron: "0 0 * * 0"
 
 jobs:
-    check-manifest:
+  check-manifest:
     # check-manifest is a tool that checks that all files in version control are
     # included in the sdist (unless explicitly excluded)
-        runs-on: ubuntu-latest
-        steps:
-            - uses: actions/checkout@v4
-            - run: pipx run check-manifest
-
-    test:
-        name: ${{ matrix.platform }} (${{ matrix.python-version }})
-        runs-on: ${{ matrix.platform }}
-        strategy:
-            fail-fast: false
-            matrix:
-                python-version: ['3.8', '3.9', '3.10', '3.11']
-                platform: [ubuntu-latest, macos-latest, windows-latest]
-
-        steps:
-            - name: 🛑 Cancel Previous Runs
-              uses: styfle/cancel-workflow-action@0.12.0
-              with:
-                  access_token: ${{ github.token }}
-
-            - uses: actions/checkout@v4
-
-            - name: 🐍 Set up Python ${{ matrix.python-version }}
-              uses: actions/setup-python@v5
-              with:
-                  python-version: ${{ matrix.python-version }}
-                  cache-dependency-path: pyproject.toml
-                  cache: pip
-
-            - name: Install Dependencies
-              run: |
-                  python -m pip install -U pip
-                  # if running a cron job, we add the --pre flag to test against pre-releases
-                  python -m pip install .[test] ${{ github.event_name == 'schedule' && '--pre' || ''  }}
-
-            - name: 🧪 Run Tests
-              run: pytest --color=yes --cov --cov-report=xml --cov-report=term-missing -m "not gpu"
-
-            # If something goes wrong with --pre tests, we can open an issue in the repo
-            - name: 📝 Report --pre Failures
-              if: failure() && github.event_name == 'schedule'
-              uses: JasonEtco/create-an-issue@v2
-              env:
-                  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-                  PLATFORM: ${{ matrix.platform }}
-                  PYTHON: ${{ matrix.python-version }}
-                  RUN_ID: ${{ github.run_id }}
-                  TITLE: '[test-bot] pip install --pre is failing'
-              with:
-                  filename: .github/TEST_FAIL_TEMPLATE.md
-                  update_existing: true
-
-            - name: Coverage
-              uses: codecov/codecov-action@v3
-
-    deploy:
-        name: Deploy
-        needs: test
-        if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
-        runs-on: ubuntu-latest
-
-        permissions:
-            # IMPORTANT: this permission is mandatory for trusted publishing on PyPi
-            # see https://docs.pypi.org/trusted-publishers/
-            id-token: write
-            # This permission allows writing releases
-            contents: write
-
-        steps:
-            - uses: actions/checkout@v4
-              with:
-                  fetch-depth: 0
-
-            - name: 🐍 Set up Python
-              uses: actions/setup-python@v5
-              with:
-                  python-version: 3.x
-
-            - name: 👷 Build
-              run: |
-                  python -m pip install build
-                  python -m build
-
-            - name: 🚢 Publish to PyPI
-              uses: pypa/gh-action-pypi-publish@release/v1
-
-            - uses: softprops/action-gh-release@v1
-              with:
-                  generate_release_notes: true
-                  files: ./dist/*
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - run: pipx run check-manifest
+
+  test:
+    name: ${{ matrix.platform }} (${{ matrix.python-version }})
+    runs-on: ${{ matrix.platform }}
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners/about-github-hosted-runners#standard-github-hosted-runners-for-public-repositories
+        platform: [ubuntu-latest, macos-13, windows-latest]
+
+    steps:
+      - name: 🛑 Cancel Previous Runs
+        uses: styfle/cancel-workflow-action@0.11.0
+        with:
+          access_token: ${{ github.token }}
+
+      - uses: actions/checkout@v3
+
+      - name: 🐍 Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          cache-dependency-path: "pyproject.toml"
+          cache: "pip"
+
+      - name: Install Dependencies
+        run: |
+          python -m pip install -U pip
+          # if running a cron job, we add the --pre flag to test against pre-releases
+          python -m pip install .[dev] ${{ github.event_name == 'schedule' && '--pre' || ''  }}
+
+      - name: 🧪 Run Tests
+        run: pytest --color=yes --cov --cov-report=xml --cov-report=term-missing -m "not gpu"
+
+      # If something goes wrong with --pre tests, we can open an issue in the repo
+      - name: 📝 Report --pre Failures
+        if: failure() && github.event_name == 'schedule'
+        uses: JasonEtco/create-an-issue@v2
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          PLATFORM: ${{ matrix.platform }}
+          PYTHON: ${{ matrix.python-version }}
+          RUN_ID: ${{ github.run_id }}
+          TITLE: "[test-bot] pip install --pre is failing"
+        with:
+          filename: .github/TEST_FAIL_TEMPLATE.md
+          update_existing: true
+
+      - name: Coverage
+        uses: codecov/codecov-action@v3
+
+  deploy:
+    name: Release
+    needs: test
+    if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
+    runs-on: ubuntu-latest
+
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
+
+      # This permission allows writing releases
+      contents: write
+
+    steps:
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.9"
+
+      - name: Build
+        run: |
+          python -m pip install build
+          python -m build
+
+      - name: Publish to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+
+      - uses: softprops/action-gh-release@v2
+        with:
+          generate_release_notes: true
```

### Comparing `careamics-0.1.0rc2/examples/n2v_full_reference.yml` & `careamics-0.1.0rc3/examples/3D/n2v_flywing_3D.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,73 @@
----
 # Name, composed of letters, numbers, spaces, dashes and underscores
-experiment_name: project_name
+experiment_name: N2V_flywing_3D
 
 # Working directory (logs, models, etc), its parent folder must exist
-working_directory: path/to/working_directory
-
-# Optional
-# Absolute or relative (wrt working_directory) path to model
-trained_model: best_model.pth
+working_directory: n2v_bsd
 
 algorithm:
   # Loss, currently only n2v is supported
-    loss: n2v
+  loss: n2v
 
   # Model, currently only UNet is supported
-    model: UNet
+  model: UNet
 
   # Dimensions 2D (False) or 3D (True)
-    is_3D: false
+  is_3D: True
 
-  # Optional, masking strategy, currently only default is supported
-    masking_strategy: default
-  # Optional, percentage of masked pixel per patch (between 0.1 and 20%)
-    masked_pixel_percentage: 0.2
   # Optional, parameters of the model
-    model_parameters:
-    # Depth betwen 1 and 10
-        depth: 2
+  model_parameters:
     # Number of filters of the first level, must be divisible by 2
-        num_filter_base: 32
+    num_channels_init: 32
 
 training:
   # Number of epochs, greater or equal than 1
-    num_epochs: 100
+  num_epochs: 50
 
   # Patch size, 2D or 3D, divisible by 2
-    patch_size: [64, 64]
+  patch_size: [32, 64, 64]
 
   # Batch size, greater or equal than 1
-    batch_size: 128
+  batch_size: 4
 
   # Optimizer
-    optimizer:
+  optimizer:
     # Name, one of Adam or SGD
-        name: Adam
+    name: Adam
 
     # Optional, parameters of the optimizer
     # see https://pytorch.org/docs/stable/optim.html#algorithms
-        parameters:
-            lr: 0.0004
+    parameters:
+      lr: 0.0004
 
   # Learning rate scheduler
-    lr_scheduler:
+  lr_scheduler:
     # Name, one of ReduceLROnPlateau or StepLR
-        name: ReduceLROnPlateau
+    name: ReduceLROnPlateau
     # Optional, parameters of the learning rate scheduler
     # see https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate
-        parameters:
-            mode: min
-            patience: 10
-            factor: 0.5
+    parameters:
+      factor: 0.5
 
   # Use augmentation (True or False)
-    augmentation: true
+  augmentation: True
 
   # Optional, use WandB (True or False), must be installed in your conda environment
-    use_wandb: false
+  use_wandb: False
 
   # Optional, number of workers for data loading, greater or equal than 0
-    num_workers: 0
+  num_workers: 4
 
   # Optional, automatic mixed precision
-    amp:
+  amp:
     # Use (True or False)
-        use: true
-    # Optional, scaling parameter for mixed precision training, power of 2 recommended.
-    # minimum is 512, maximum is 65536
-        init_scale: 1024
-
-  # Torch.compile (True or False)
-    compile:
-        use: false
+    use: True
 
 data:
   # Controls the type of dataloader to use. Set to False if data won't fit into memory
-    in_memory: false
-
-  # Extension of the data, e.g. tiff or zarr
-    data_format: tiff
+  in_memory: True
+  
+  # Extension of the data, one of npy, tiff and tif
+  data_format: tif
 
   # Axes, among STCZYX with constraints on order
-    axes: SYX
+  axes: ZYX
```

### Comparing `careamics-0.1.0rc2/examples/2D/example_BSD68.ipynb` & `careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_careamist.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9683809694854953%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, 'from careamics import CAREamist\\n'), (7, 'from "*

 * *            "careamics.lightning_datamodule import (\\n'), (8, '    "*

 * *            "CAREamicsPredictDataModule,\\n'), (9, ')\\n'), (10, 'from careamics.utils.metrics "*

 * *            "import psnr')], delete: [8, 7, 0]}}, 9: {'source': {insert: [(0, '### Initialize the "*

 * *            "Model\\n'), (2, 'Create a Pytorch Lightning module\\n')], delete: [2, 0]}}, 10: "*

 * *            '{\'source\': [\'engine = CAREamist(source="n […]*

```diff
@@ -2,23 +2,25 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pprint\n",
                 "from pathlib import Path\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import tifffile\n",
                 "from careamics_portfolio import PortfolioManager\n",
                 "\n",
-                "from careamics.engine import Engine\n",
-                "from careamics.metrics import psnr"
+                "from careamics import CAREamist\n",
+                "from careamics.lightning_datamodule import (\n",
+                "    CAREamicsPredictDataModule,\n",
+                ")\n",
+                "from careamics.utils.metrics import psnr"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -105,45 +107,28 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Initialize the Engine\n",
+                "### Initialize the Model\n",
                 "\n",
-                "Engine contains the dataloading pipeline and the model training logic. We'll initialize the engine with the config file, but it can also be initialized from a pre-trained checkpoint.\n",
+                "Create a Pytorch Lightning module\n",
                 "\n",
                 "Please take as look at the [documentation](https://careamics.github.io) to see the full list of parameters and configuration options"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "engine = Engine(config_path=\"n2v_2D_BSD.yml\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Visualize training configuration"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pprint.PrettyPrinter(indent=2).pprint(engine.cfg.model_dump(exclude_optionals=False))"
+                "engine = CAREamist(source=\"n2v_2D_BSD.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -154,162 +139,143 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_stats, val_stats = engine.train(train_path=train_path, val_path=val_path)"
+                "engine.train(train_source=train_path, val_source=val_path)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize statistics"
+                "### Define a prediction datamodule"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.plot([next(iter(d.values())) for d in train_stats], label=\"Train loss\")\n",
-                "plt.plot([next(iter(d.values())) for d in val_stats], label=\"Validation loss\")\n",
-                "plt.legend(loc=\"best\")\n",
-                "plt.xlabel(\"Epoch\")"
+                "pred_data_module = CAREamicsPredictDataModule(\n",
+                "    pred_data=test_path,\n",
+                "    data_type=\"tiff\",\n",
+                "    tile_size=(256, 256),\n",
+                "    axes=\"YX\",\n",
+                "    batch_size=1,\n",
+                "    tta_transforms=True,\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize files to denoise"
+                "### Run prediction\n",
+                "\n",
+                "We need to specify the path to the data we want to denoise"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "test_img = tifffile.imread(test_path / \"bsd68_gaussian25_1.tiff\")\n",
-                "plt.imshow(test_img, cmap=\"gray\")\n",
-                "print(test_img.shape)"
+                "preds = engine.predict(source=pred_data_module)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Run prediction\n",
-                "\n",
-                "We need to specify the path to the data we want to denoise"
+                "### Visualize results and compute metrics\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "preds = engine.predict(\n",
-                "    input=test_path, tile_shape=[256, 256], overlaps=[48, 48], axes=\"YX\"\n",
-                ")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Visualize results and compute metrics\n"
+                "# Create a list of ground truth images\n",
+                "\n",
+                "gts = [tifffile.imread(f) for f in sorted(gt_path.glob(\"*.tiff\"))]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Create a list of ground truth images\n",
+                "# Plot single image\n",
                 "\n",
-                "gts = [tifffile.imread(f) for f in sorted(gt_path.glob(\"*.tiff\"))]"
+                "image_idx = 0\n",
+                "_, subplot = plt.subplots(1, 2, figsize=(10, 10))\n",
+                "\n",
+                "subplot[0].imshow(preds[image_idx].squeeze(), cmap=\"gray\")\n",
+                "subplot[0].set_title(\"Prediction\")\n",
+                "subplot[1].imshow(gts[image_idx], cmap=\"gray\")\n",
+                "subplot[1].set_title(\"Ground truth\")\n",
+                "\n",
+                "\n",
+                "# Calculate PSNR for single image\n",
+                "psnr_single = psnr(preds[image_idx].squeeze(), gts[image_idx].squeeze())\n",
+                "print(f\"PSNR for image {image_idx}: {psnr_single}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Plot single image\n",
                 "\n",
                 "image_idx = 0\n",
                 "_, subplot = plt.subplots(1, 2, figsize=(10, 10))\n",
                 "\n",
-                "subplot[0].imshow(preds[image_idx], cmap=\"gray\")\n",
+                "subplot[0].imshow(preds[image_idx].squeeze(), cmap=\"gray\")\n",
                 "subplot[0].set_title(\"Prediction\")\n",
                 "subplot[1].imshow(gts[image_idx], cmap=\"gray\")\n",
                 "subplot[1].set_title(\"Ground truth\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Calculate PSNR for single image\n",
                 "\n",
-                "psnr_single = psnr(gts[image_idx], preds[image_idx])\n",
+                "psnr_single = psnr(gts[image_idx], preds[image_idx].squeeze())\n",
                 "print(f\"PSNR for image {image_idx}: {psnr_single}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "psnr_total = 0\n",
                 "\n",
                 "for pred, gt in zip(preds, gts):\n",
-                "    psnr_total += psnr(gt, pred)\n",
+                "    psnr_total += psnr(gt, pred.squeeze())\n",
                 "\n",
                 "print(f\"PSNR total: {psnr_total / len(preds)}\")"
             ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Export to bioimage.io"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "engine.save_as_bioimage(engine.cfg.experiment_name + \"bioimage.zip\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.11.3 ('caremics')",
             "language": "python",
             "name": "python3"
@@ -320,15 +286,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.9.18"
         },
         "vscode": {
             "interpreter": {
                 "hash": "0d2a5a3ab9ff26e8b66efec3883fa5121030bb852a7a4271db665831444e4e91"
             }
         }
     },
```

### Comparing `careamics-0.1.0rc2/examples/2D/example_SEM.ipynb` & `careamics-0.1.0rc3/examples/2D/n2n/example_SEM_careamist.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9624103197150072%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'import numpy as np\\n'), (8, 'from careamics import "*

 * *            "CAREamist')], delete: [9, 7, 0]}}, 3: {'source': {insert: [(2, 'files = "*

 * *            "portfolio.denoising.N2N_SEM.download(root_path)\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(3, '\\n'), (4, '# Display images\\n'), (5, 'side = "*

 * *            "int(np.ceil(np.sqrt(train_image.shape[0])))\\n'), (6, 'fig, ax = plt.subplots(side, "*

 * *            "side, figsize=(15, 15))\\n'), (7, '\\n') […]*

```diff
@@ -2,24 +2,23 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pprint\n",
                 "import shutil\n",
                 "from pathlib import Path\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
                 "import tifffile\n",
                 "from careamics_portfolio import PortfolioManager\n",
-                "from matplotlib.pyplot import imshow\n",
                 "\n",
-                "from careamics.engine import Engine"
+                "from careamics import CAREamist"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -41,15 +40,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Download files\n",
                 "root_path = Path(\"./data\")\n",
-                "files = portfolio.denoising.N2V_SEM.download(root_path)\n",
+                "files = portfolio.denoising.N2N_SEM.download(root_path)\n",
                 "print(f\"List of downloaded files: {files}\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -62,15 +61,22 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load images\n",
                 "train_image = tifffile.imread(files[0])\n",
                 "print(f\"Train image shape: {train_image.shape}\")\n",
-                "imshow(train_image, cmap=\"gray\")"
+                "\n",
+                "# Display images\n",
+                "side = int(np.ceil(np.sqrt(train_image.shape[0])))\n",
+                "fig, ax = plt.subplots(side, side, figsize=(15, 15))\n",
+                "\n",
+                "for i in range(train_image.shape[0]):\n",
+                "    ax.flat[i].imshow(train_image[i], cmap=\"gray\")\n",
+                "    ax.flat[i].axis(\"off\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -79,130 +85,104 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "val_image = tifffile.imread(files[1])\n",
+                "val_image = tifffile.imread(files[2])\n",
                 "print(f\"Validation image shape: {val_image.shape}\")\n",
-                "imshow(val_image, cmap=\"gray\")"
+                "\n",
+                "# Display images\n",
+                "side = int(np.ceil(np.sqrt(val_image.shape[0])))\n",
+                "fig, ax = plt.subplots(side, side, figsize=(15, 15))\n",
+                "for i in range(val_image.shape[0]):\n",
+                "    ax.flat[i].imshow(val_image[i], cmap=\"gray\")\n",
+                "    ax.flat[i].axis(\"off\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_path = Path(root_path / \"n2v_sem\")\n",
+                "# Set paths\n",
+                "\n",
+                "data_path = Path(root_path / \"n2n_sem\")\n",
                 "train_path = data_path / \"train\"\n",
-                "val_path = data_path / \"val\"\n",
+                "test_path = data_path / \"val\"\n",
                 "\n",
                 "train_path.mkdir(parents=True, exist_ok=True)\n",
-                "val_path.mkdir(parents=True, exist_ok=True)\n",
+                "test_path.mkdir(parents=True, exist_ok=True)\n",
                 "\n",
                 "shutil.copy(root_path / files[0], train_path / \"train_image.tif\")\n",
-                "shutil.copy(root_path / files[1], val_path / \"val_image.tif\")"
+                "shutil.copy(root_path / files[1], test_path / \"test_image.tif\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Initialize the Engine\n",
+                "#### Initialize the Model\n",
                 "\n",
-                "Engine contains the dataloading pipeline and the model training logic. We'll initialize the engine with the config file, but it can also be initialized from a pre-trained checkpoint.\n",
+                "Create a Pytorch Lightning module\n",
                 "\n",
                 "Please take as look at the [documentation](https://careamics.github.io) to see the full list of parameters and configuration options"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "engine = Engine(config_path=\"n2v_2D_SEM.yml\")"
+                "engine = CAREamist(source=\"n2n_2D_SEM.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize training configuration"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pprint.PrettyPrinter(indent=2).pprint(engine.cfg.model_dump(exclude_optionals=False))"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Run training \n",
+                "### Part 3. Run training \n",
                 "\n",
                 "We need to specify the paths to training and validation data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_stats, val_stats = engine.train(train_path=train_path, val_path=val_path)"
+                "engine.train(\n",
+                "    train_source=train_image[0],\n",
+                "    val_source=train_image[1],\n",
+                "    train_target=train_image[2],\n",
+                "    val_target=train_image[3],\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize statistics"
+                "### Run prediction\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.plot([next(iter(d.values())) for d in train_stats], label=\"Train loss\")\n",
-                "plt.plot([next(iter(d.values())) for d in val_stats], label=\"Validation loss\")\n",
-                "plt.legend(loc=\"best\")\n",
-                "plt.xlabel(\"Epoch\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Run prediction\n",
-                "\n",
-                "We need to specify the path to the data we want to denoise"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "preds = engine.predict(input=train_path, tile_shape=[256, 256], overlaps=[48, 48])"
+                "preds = engine.predict(source=val_image[0], tile_size=(256, 256))"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -211,32 +191,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "imshow(preds.squeeze(), cmap=\"gray\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Export to bioimage.io"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "engine.save_as_bioimage(engine.cfg.experiment_name + \"bioimage.zip\")"
+                "fi, ax = plt.subplots(1, 2, figsize=(15, 15))\n",
+                "ax[0].imshow(preds[0].squeeze(), cmap=\"gray\")\n",
+                "ax[0].set_title(\"Prediction\")\n",
+                "ax[1].imshow(val_image[0].squeeze(), cmap=\"gray\")\n",
+                "ax[1].set_title(\"Ground Truth\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -255,15 +222,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.9.18"
         },
         "vscode": {
             "interpreter": {
                 "hash": "faf8b084d52efbff00ddf863c4fb0ca7a3b023f9f18590a5b65c31dc02d793e2"
             }
         }
     },
```

### Comparing `careamics-0.1.0rc2/examples/2D/n2v_2D_BSD.yml` & `careamics-0.1.0rc3/examples/2D/pn2v/pN2V_Convallaria.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,71 @@
----
 # Name, composed of letters, numbers, spaces, dashes and underscores
-experiment_name: N2V_BSD
+experiment_name: pN2V_Convallaria
 
 # Working directory (logs, models, etc), its parent folder must exist
-working_directory: n2v_bsd
+working_directory: pN2V_Convallaria
 
 algorithm:
+  algorithm_type: pn2v
   # Loss, currently only n2v is supported
-    loss: n2v
+  loss: pn2v
 
   # Model, currently only UNet is supported
-    model: UNet
+  model: UNet
 
+  # Noise model, Histogram or GMM
+  noise_model:
+    model_type: hist
+    parameters:
+      min_value: 350
+      max_value: 6500
+      bins: 256
+  
   # Dimensions 2D (False) or 3D (True)
-    is_3D: false
-
-  # Optional, parameters of the model
-    model_parameters:
-    # Number of filters of the first level, must be divisible by 2
-        num_channels_init: 32
+  is_3D: False
 
 training:
   # Number of epochs, greater or equal than 1
-    num_epochs: 100
+  num_epochs: 10
 
   # Patch size, 2D or 3D, divisible by 2
-    patch_size: [64, 64]
+  patch_size: [64, 64]
 
   # Batch size, greater or equal than 1
-    batch_size: 128
+  batch_size: 128
 
   # Optimizer
-    optimizer:
+  optimizer:
     # Name, one of Adam or SGD
-        name: Adam
+    name: Adam
     # Optional, parameters of the optimizer
     # see https://pytorch.org/docs/stable/optim.html#algorithms
-        parameters:
-            lr: 0.0004
+    parameters:
+      lr: 0.0004
 
   # Learning rate scheduler
-    lr_scheduler:
+  lr_scheduler:
     # Name, one of ReduceLROnPlateau or StepLR
-        name: ReduceLROnPlateau
+    name: ReduceLROnPlateau
     # Optional, parameters of the learning rate scheduler
     # see https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate
-        parameters:
-            factor: 0.5
+    parameters:
+      factor: 0.5
 
   # Use augmentation (True or False)
-    augmentation: true
+  augmentation: True
 
   # Optional, use WandB (True or False), must be installed in your conda environment
-    use_wandb: false
+  use_wandb: False
 
   # Optional, number of workers for data loading, greater or equal than 0
-    num_workers: 4
-
-  # Optional, automatic mixed precision
-    amp:
-    # Use (True or False)
-        use: true
-
-  # Torch.compile (True or False)
-    compile:
-        use: false
+  num_workers: 0
 
 data:
   # Controls the type of dataloader to use. Set to False if data won't fit into memory
-    in_memory: true
+  in_memory: True
 
   # Extension of the data, one of npy, tiff and tif
-    data_format: tiff
+  data_format: tiff
 
   # Axes, among STCZYX with constraints on order
-    axes: SYX
+  axes: YX
```

### Comparing `careamics-0.1.0rc2/examples/2D/n2v_2D_SEM.yml` & `careamics-0.1.0rc3/examples/2D/n2v/n2v_2D_BSD.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,60 @@
----
 # Name, composed of letters, numbers, spaces, dashes and underscores
-experiment_name: N2V_SEM
-
-# Working directory (logs, models, etc), its parent folder must exist
-working_directory: n2v_sem
+experiment_name: N2V_BSD_n2v2
 
 algorithm:
-  # Loss, currently only n2v is supported
-    loss: n2v
-
-  # Model, currently only UNet is supported
-    model: UNet
-
-  # Dimensions 2D (False) or 3D (True)
-    is_3D: false
+  algorithm: n2v
+  loss: n2v
+  model:
+    architecture: UNet
+    n2v2: False
+  optimizer_parameters:
+    lr: 1e-3
+  lr_scheduler_parameters:
+   factor: 0.5
+   patience: 10
 
 training:
   # Number of epochs, greater or equal than 1
-    num_epochs: 100
-
-  # Patch size, 2D or 3D, divisible by 2
-    patch_size: [64, 64]
+  num_epochs: 1
 
   # Batch size, greater or equal than 1
-    batch_size: 128
-
-  # Optimizer
-    optimizer:
-    # Name, one of Adam or SGD
-        name: Adam
-    # Optional, parameters of the optimizer
-    # see https://pytorch.org/docs/stable/optim.html#algorithms
-        parameters:
-            lr: 0.0004
-
-  # Learning rate scheduler
-    lr_scheduler:
-    # Name, one of ReduceLROnPlateau or StepLR
-        name: ReduceLROnPlateau
-    # Optional, parameters of the learning rate scheduler
-    # see https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate
-        parameters:
-            factor: 0.5
-
-  # Use augmentation (True or False)
-    augmentation: true
+  batch_size: 128
 
   # Optional, use WandB (True or False), must be installed in your conda environment
-    use_wandb: false
+  use_wandb: False
 
-  # Optional, number of workers for data loading, greater or equal than 0
-    num_workers: 4
+  callbacks:
+    # Optional, any parameter for Pytorch lightning callbacks
 
-data:
-  # Controls the type of dataloader to use. Set to False if data won't fit into memory
-    in_memory: true
+    # Optional, any parameter for Pytorch lightning ModelCheckpoint
+    checkpoint:
+      # Optional, monitor the validation loss (val_loss) or the validation accuracy (val_acc)
+      # parameters:
+      # dirpath: 'checkpoints'
+      # monitor : val_loss
+      save_last: True
+      save_top_k: 3
+      # TODO should it be here or in predict ?
+      # Optional, path to the checkpoint to load the model
+      # load_path: ''
+
+  # Optional, automatic mixed precision
+  amp:
+    # Use (True or False)
+    use: True
 
-  # Extension of the data, one of npy, tiff and tif
-    data_format: tif
+data:
+  # Extension of the data
+  data_type: tiff
 
+  patch_size: [64, 64]
+  
   # Axes, among STCZYX with constraints on order
-    axes: YX
+  axes: SYX
+
+  tta_transforms: True
+
+  batch_size: 128
+
+  # Optional, number of workers for data loading, greater or equal than 0
+  num_workers: 0
```

### Comparing `careamics-0.1.0rc2/examples/3D/example_flywing_3D.ipynb` & `careamics-0.1.0rc3/examples/2D/n2v/example_SEM_lightning.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9512389698203843%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'import shutil\\n'), (6, 'from pytorch_lightning import "*

 * *            "Trainer\\n'), (8, 'from careamics import CAREamicsModule\\n'), (9, 'from "*

 * *            "careamics.lightning_datamodule import (\\n'), (10, '    "*

 * *            "CAREamicsPredictDataModule,\\n'), (11, '    CAREamicsTrainDataModule,\\n'), (12, "*

 * *            "')\\n'), (13, 'from careamics.lightning_prediction import CAREamicsPredictionLoop')], "*

 * *            "delete: [10, 8, 7, 4, 0]}}, 1: {'source': [ […]*

```diff
@@ -2,298 +2,311 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pprint\n",
+                "import shutil\n",
                 "from pathlib import Path\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
                 "import tifffile\n",
                 "from careamics_portfolio import PortfolioManager\n",
-                "from itkwidgets import compare, view  # \"pip install itkwidgets \"if necessary\n",
-                "from matplotlib.pyplot import imshow\n",
+                "from pytorch_lightning import Trainer\n",
                 "\n",
-                "from careamics.engine import Engine"
+                "from careamics import CAREamicsModule\n",
+                "from careamics.lightning_datamodule import (\n",
+                "    CAREamicsPredictDataModule,\n",
+                "    CAREamicsTrainDataModule,\n",
+                ")\n",
+                "from careamics.lightning_prediction import CAREamicsPredictionLoop"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Import Dataset Portfolio\n"
+                "### Import Dataset Portfolio"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Explore portfolio\n",
                 "portfolio = PortfolioManager()\n",
                 "print(portfolio.denoising)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Read the specific dataset \n",
-                "bla "
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Download files\n",
-                "root_path = Path(\"data\")\n",
-                "files = portfolio.denoising.Flywing.download(root_path)\n",
+                "root_path = Path(\"./data\")\n",
+                "files = portfolio.denoising.N2V_SEM.download(root_path)\n",
                 "print(f\"List of downloaded files: {files}\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "data_path = Path(root_path / \"denoising-Flywing.unzip\")\n",
-                "\n",
-                "data_path.mkdir(parents=True, exist_ok=True)"
-            ]
-        },
-        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize the data"
+                "### Visualize training data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_image = tifffile.imread(next(iter(data_path.rglob(\"*.tif\"))))\n",
+                "# Load images\n",
+                "train_image = tifffile.imread(files[0])\n",
                 "print(f\"Train image shape: {train_image.shape}\")\n",
-                "imshow(np.max(train_image, axis=0), cmap=\"magma\")"
+                "plt.imshow(train_image, cmap=\"gray\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### [Optional] Visualize the data in 3D"
+                "### Visualize validation data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# View 3D image\n",
-                "view(train_image)"
+                "val_image = tifffile.imread(files[1])\n",
+                "print(f\"Validation image shape: {val_image.shape}\")\n",
+                "plt.imshow(val_image, cmap=\"gray\")"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Initialize the Engine\n",
+                "data_path = Path(root_path / \"n2v_sem\")\n",
+                "train_path = data_path / \"train\"\n",
+                "val_path = data_path / \"val\"\n",
                 "\n",
-                "Engine contains the dataloading pipeline and the model training logic. We'll initialize the engine with the config file, but it can also be initialized from a pre-trained checkpoint.\n",
+                "train_path.mkdir(parents=True, exist_ok=True)\n",
+                "val_path.mkdir(parents=True, exist_ok=True)\n",
                 "\n",
-                "Please take as look at the [documentation](https://careamics.github.io) to see the full list of parameters and configuration options"
+                "shutil.copy(root_path / files[0], train_path / \"train_image.tif\")\n",
+                "shutil.copy(root_path / files[1], val_path / \"val_image.tif\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "engine = Engine(config_path=\"n2v_flywing_3D.yml\")"
+                "### Initialize the Model\n",
+                "\n",
+                "Please take as look at the [documentation](https://careamics.github.io) to see the full list of parameters and configuration options"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Visualize training configuration"
+                "# N2V2 requires changes to the UNet model and to the Dataset (augmentations)\n",
+                "use_n2v2 = False  # change to True to use N2V2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pprint.PrettyPrinter(indent=2).pprint(engine.cfg.model_dump(exclude_optionals=False))"
+                "model = CAREamicsModule(\n",
+                "    algorithm=\"n2v\",\n",
+                "    loss=\"n2v\",\n",
+                "    architecture=\"UNet\",\n",
+                "    model_parameters={\"n2v2\": False},\n",
+                "    optimizer_parameters={\"lr\": 1e-3},\n",
+                "    lr_scheduler_parameters={\"factor\": 0.5, \"patience\": 10},\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "\n",
-                "Start training"
+                "### Initialize the datamodule"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_stats, val_stats = engine.train(train_path=data_path, val_path=data_path)"
+                "train_data_module = CAREamicsTrainDataModule(\n",
+                "    train_data=train_path,\n",
+                "    val_data=val_path,\n",
+                "    data_type=\"tiff\",\n",
+                "    patch_size=(64, 64),\n",
+                "    axes=\"YX\",\n",
+                "    batch_size=128,\n",
+                "    dataloader_params={\"num_workers\": 0},\n",
+                "    use_n2v2=use_n2v2,\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize statistics"
+                "### Run training \n",
+                "\n",
+                "We need to specify the paths to training and validation data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.plot([next(iter(d.values())) for d in train_stats], label=\"Train loss\")\n",
-                "plt.plot([next(iter(d.values())) for d in val_stats], label=\"Validation loss\")\n",
-                "plt.legend(loc=\"best\")\n",
-                "plt.xlabel(\"Epoch\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Predict"
+                "trainer = Trainer(max_epochs=1, default_root_dir=\"sem_n2v2_test_struct\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "preds = engine.predict(input=data_path, tile_shape=[32, 64, 64], overlaps=[24, 48, 48])"
+                "trainer.fit(model, datamodule=train_data_module)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualize predictions\n"
+                "### Define the prediction datamodule"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(f\"Train image shape: {preds.shape}\")\n",
-                "imshow(np.max(preds.squeeze(), axis=0), cmap=\"magma\")"
+                "pred_data_module = CAREamicsPredictDataModule(\n",
+                "    pred_data=train_path,\n",
+                "    data_type=\"tiff\",\n",
+                "    tile_size=(256, 256),\n",
+                "    axes=\"YX\",\n",
+                "    batch_size=1,\n",
+                "    tta_transforms=True,\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### [Optional] Visualize predictions in 3D"
+                "### Run prediction\n",
+                "\n",
+                "We need to specify the path to the data we want to denoise"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "compare(train_image, preds.squeeze())"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Save predictions"
+                "tiled_loop = CAREamicsPredictionLoop(trainer)\n",
+                "trainer.predict_loop = tiled_loop"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tifffile.imwrite(\"flywing_preds.tif\", preds.squeeze())"
+                "preds = trainer.predict(model, datamodule=pred_data_module)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Export to bioimage.io"
+                "### Visualize the prediction"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "engine.save_as_bioimage(engine.cfg.experiment_name + \"bioimage.zip\")"
+                "image_idx = 0\n",
+                "_, subplot = plt.subplots(1, 2, figsize=(10, 10))\n",
+                "\n",
+                "subplot[0].imshow(preds[0].squeeze(), cmap=\"gray\")\n",
+                "subplot[0].set_title(\"Prediction\")\n",
+                "subplot[1].imshow(train_image, cmap=\"gray\")\n",
+                "subplot[1].set_title(\"Initial image\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.11.3 ('caremics')",
+            "display_name": "Python 3.9.13 ('HDNn')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.9.18"
         },
         "vscode": {
             "interpreter": {
-                "hash": "0d2a5a3ab9ff26e8b66efec3883fa5121030bb852a7a4271db665831444e4e91"
+                "hash": "faf8b084d52efbff00ddf863c4fb0ca7a3b023f9f18590a5b65c31dc02d793e2"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `careamics-0.1.0rc2/src/careamics/dataset/dataset_utils.py` & `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_tiff.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,21 @@
-"""Convenience methods for datasets."""
 import logging
+from fnmatch import fnmatch
 from pathlib import Path
-from typing import List, Union
 
 import numpy as np
 import tifffile
 
+from careamics.config.support import SupportedData
+from careamics.utils.logging import get_logger
 
-def list_files(data_path: Union[str, Path], data_format: str) -> List[Path]:
-    """
-    Return a list of path to files in a directory.
-
-    Parameters
-    ----------
-    data_path : str
-        Path to the folder containing the data.
-    data_format : str
-        Extension of the files to load, without period, e.g. `tif`.
-
-    Returns
-    -------
-    List[Path]
-        List of pathlib.Path objects.
-    """
-    files = sorted(Path(data_path).rglob(f"*.{data_format}*"))
-    return files
+logger = get_logger(__name__)
 
 
-def _update_axes(array: np.ndarray, axes: str) -> np.ndarray:
-    """
-    Update axes of the sample to match the config axes.
-
-    This method concatenate the S and T axes.
-
-    Parameters
-    ----------
-    array : np.ndarray
-        Input array.
-    axes : str
-        Description of axes in format STCZYX.
-
-    Returns
-    -------
-    np.ndarray
-        Updated array.
-    """
-    # concatenate ST axes to N, return NCZYX
-    if "S" in axes or "T" in axes:
-        new_axes_len = len(axes.replace("Z", "").replace("YX", ""))
-        # TODO test reshape as it can scramble data, moveaxis is probably better
-        array = array.reshape(-1, *array.shape[new_axes_len:]).astype(np.float32)
-
-    else:
-        array = np.expand_dims(array, axis=0).astype(np.float32)
-
-    return array
-
-
-def read_tiff(file_path: Path, axes: str) -> np.ndarray:
+def read_tiff(file_path: Path, *args: list, **kwargs: dict) -> np.ndarray:
     """
     Read a tiff file and return a numpy array.
 
     Parameters
     ----------
     file_path : Path
         Path to a file.
@@ -82,30 +36,26 @@
     ValueError
         If the file is not a valid tiff.
     ValueError
         If the data dimensions are incorrect.
     ValueError
         If the axes length is incorrect.
     """
-    if file_path.suffix[:4] == ".tif":
+    if fnmatch(file_path.suffix, SupportedData.get_extension(SupportedData.TIFF)):
         try:
-            sample = tifffile.imread(file_path)
+            array = tifffile.imread(file_path)
         except (ValueError, OSError) as e:
             logging.exception(f"Exception in file {file_path}: {e}, skipping it.")
             raise e
     else:
         raise ValueError(f"File {file_path} is not a valid tiff.")
 
-    sample = sample.squeeze()
-
-    if len(sample.shape) < 2 or len(sample.shape) > 4:
+    # check dimensions
+    # TODO or should this really be done here? probably in the LightningDataModule
+    # TODO this should also be centralized somewhere else (validate_dimensions)
+    if len(array.shape) < 2 or len(array.shape) > 6:
         raise ValueError(
-            f"Incorrect data dimensions. Must be 2, 3 or 4 (got {sample.shape} for"
+            f"Incorrect data dimensions. Must be 2, 3 or 4 (got {array.shape} for"
             f"file {file_path})."
         )
 
-    # check number of axes
-    if len(axes) != len(sample.shape):
-        raise ValueError(f"Incorrect axes length (got {axes} for file {file_path}).")
-    sample = _update_axes(sample, axes)
-
-    return sample
+    return array
```

### Comparing `careamics-0.1.0rc2/src/careamics/models/unet.py` & `careamics-0.1.0rc3/src/careamics/models/unet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 UNet model.
 
 A UNet encoder, decoder and complete model.
 """
-from typing import Callable, List, Optional
+from typing import Any, List, Union
 
 import torch
 import torch.nn as nn
 
-from .layers import Conv_Block
+from ..config.support import SupportedActivation
+from .activation import get_activation
+from .layers import Conv_Block, MaxBlurPool
 
 
 class UnetEncoder(nn.Module):
     """
     Unet encoder pathway.
 
     Parameters
@@ -38,14 +40,15 @@
         conv_dim: int,
         in_channels: int = 1,
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
         pool_kernel: int = 2,
+        n2v2: bool = False,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         conv_dim : int
@@ -61,15 +64,19 @@
         dropout : float, optional
             Dropout probability, by default 0.0.
         pool_kernel : int, optional
             Kernel size for the max pooling layers, by default 2.
         """
         super().__init__()
 
-        self.pooling = getattr(nn, f"MaxPool{conv_dim}d")(kernel_size=pool_kernel)
+        self.pooling = (
+            getattr(nn, f"MaxPool{conv_dim}d")(kernel_size=pool_kernel)
+            if not n2v2
+            else MaxBlurPool(dim=conv_dim, kernel_size=3, max_pool_size=pool_kernel)
+        )
 
         encoder_blocks = []
 
         for n in range(depth):
             out_channels = num_channels_init * (2**n)
             in_channels = in_channels if n == 0 else out_channels // 2
             encoder_blocks.append(
@@ -78,15 +85,14 @@
                     in_channels=in_channels,
                     out_channels=out_channels,
                     dropout_perc=dropout,
                     use_batch_norm=use_batch_norm,
                 )
             )
             encoder_blocks.append(self.pooling)
-
         self.encoder_blocks = nn.ModuleList(encoder_blocks)
 
     def forward(self, x: torch.Tensor) -> List[torch.Tensor]:
         """
         Forward pass.
 
         Parameters
@@ -130,14 +136,15 @@
     def __init__(
         self,
         conv_dim: int,
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
+        n2v2: bool = False,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         conv_dim : int
@@ -153,32 +160,41 @@
         """
         super().__init__()
 
         upsampling = nn.Upsample(
             scale_factor=2, mode="bilinear" if conv_dim == 2 else "trilinear"
         )
         in_channels = out_channels = num_channels_init * 2 ** (depth - 1)
+
+        self.n2v2 = n2v2
+
         self.bottleneck = Conv_Block(
             conv_dim,
             in_channels=in_channels,
             out_channels=out_channels,
             intermediate_channel_multiplier=2,
             use_batch_norm=use_batch_norm,
             dropout_perc=dropout,
         )
 
         decoder_blocks = []
         for n in range(depth):
             decoder_blocks.append(upsampling)
-            in_channels = num_channels_init * 2 ** (depth - n)
-            out_channels = num_channels_init
+            in_channels = (
+                num_channels_init ** (depth - n)
+                if (self.n2v2 and n == depth - 1)
+                else num_channels_init * 2 ** (depth - n)
+            )
+            out_channels = in_channels // 2
             decoder_blocks.append(
                 Conv_Block(
                     conv_dim,
-                    in_channels=in_channels,
+                    in_channels=in_channels + in_channels // 2
+                    if n > 0
+                    else in_channels,
                     out_channels=out_channels,
                     intermediate_channel_multiplier=2,
                     dropout_perc=dropout,
                     activation="ReLU",
                     use_batch_norm=use_batch_norm,
                 )
             )
@@ -196,34 +212,40 @@
             output of the encoder.
 
         Returns
         -------
         torch.Tensor
             Output of the decoder.
         """
-        x = features[0]
-        skip_connections = features[1:][::-1]
+        x: torch.Tensor = features[0]
+        skip_connections: torch.Tensor = features[1:][::-1]
+
         x = self.bottleneck(x)
+
         for i, module in enumerate(self.decoder_blocks):
             x = module(x)
             if isinstance(module, nn.Upsample):
-                x = torch.cat([x, skip_connections[i // 2]], axis=1)
+                if self.n2v2:
+                    if x.shape != skip_connections[-1].shape:
+                        x = torch.cat([x, skip_connections[i // 2]], axis=1)
+                else:
+                    x = torch.cat([x, skip_connections[i // 2]], axis=1)
         return x
 
 
 class UNet(nn.Module):
     """
     UNet model.
 
-    Adapted for PyTorch from
+    Adapted for PyTorch from:
     https://github.com/juglab/n2v/blob/main/n2v/nets/unet_blocks.py.
 
     Parameters
     ----------
-    conv_dim : int
+    conv_dims : int
         Number of dimensions of the convolution layers (2 or 3).
     num_classes : int, optional
         Number of classes to predict, by default 1.
     in_channels : int, optional
         Number of input channels, by default 1.
     depth : int, optional
         Number of downsamplings, by default 3.
@@ -237,30 +259,32 @@
         Kernel size of the pooling layers, by default 2.
     last_activation : Optional[Callable], optional
         Activation function to use for the last layer, by default None.
     """
 
     def __init__(
         self,
-        conv_dim: int,
+        conv_dims: int,
         num_classes: int = 1,
         in_channels: int = 1,
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
         pool_kernel: int = 2,
-        last_activation: Optional[Callable] = None,
+        final_activation: Union[SupportedActivation, str] = SupportedActivation.NONE,
+        n2v2: bool = False,
+        **kwargs: Any,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
-        conv_dim : int
+        conv_dims : int
             Number of dimensions of the convolution layers (2 or 3).
         num_classes : int, optional
             Number of classes to predict, by default 1.
         in_channels : int, optional
             Number of input channels, by default 1.
         depth : int, optional
             Number of downsamplings, by default 3.
@@ -274,36 +298,38 @@
             Kernel size of the pooling layers, by default 2.
         last_activation : Optional[Callable], optional
             Activation function to use for the last layer, by default None.
         """
         super().__init__()
 
         self.encoder = UnetEncoder(
-            conv_dim,
+            conv_dims,
             in_channels=in_channels,
             depth=depth,
             num_channels_init=num_channels_init,
             use_batch_norm=use_batch_norm,
             dropout=dropout,
             pool_kernel=pool_kernel,
+            n2v2=n2v2,
         )
 
         self.decoder = UnetDecoder(
-            conv_dim,
+            conv_dims,
             depth=depth,
             num_channels_init=num_channels_init,
             use_batch_norm=use_batch_norm,
             dropout=dropout,
+            n2v2=n2v2,
         )
-        self.final_conv = getattr(nn, f"Conv{conv_dim}d")(
+        self.final_conv = getattr(nn, f"Conv{conv_dims}d")(
             in_channels=num_channels_init,
             out_channels=num_classes,
             kernel_size=1,
         )
-        self.last_activation = last_activation if last_activation else nn.Identity()
+        self.final_activation = get_activation(final_activation)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         Forward pass.
 
         Parameters
         ----------
@@ -314,9 +340,9 @@
         -------
         torch.Tensor
             Output of the model.
         """
         encoder_features = self.encoder(x)
         x = self.decoder(*encoder_features)
         x = self.final_conv(x)
-        x = self.last_activation(x)
+        x = self.final_activation(x)
         return x
```

### Comparing `careamics-0.1.0rc2/src/careamics/utils/context.py` & `careamics-0.1.0rc3/src/careamics/utils/context.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,32 @@
 """
 import os
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Iterator, Union
 
 
+def get_careamics_home() -> Path:
+    """Return the CAREamics home directory.
+
+    CAREamics home directory is a hidden folder in home.
+
+    Returns
+    -------
+    Path
+        CAREamics home directory path.
+    """
+    home = Path.home() / ".careamics"
+
+    if not home.exists():
+        home.mkdir(parents=True, exist_ok=True)
+
+    return home
+
+
 @contextmanager
 def cwd(path: Union[str, Path]) -> Iterator[None]:
     """
     Change the current working directory to the given path.
 
     This method can be used to generate files in a specific directory, once out of the
     context, the working directory is set back to the original one.
@@ -25,16 +43,18 @@
     Returns
     -------
     Iterator[None]
         None values.
 
     Examples
     --------
-    >>> with cwd(path):
-    ...     pass
+    The context is whcnaged within the block and then restored to the original one.
+
+    >>> with cwd(my_path):
+    ...     pass # do something
     """
     path = Path(path)
 
     if not path.exists():
         path.mkdir(parents=True, exist_ok=True)
 
     old_pwd = Path(".").absolute()
```

### Comparing `careamics-0.1.0rc2/src/careamics/utils/logging.py` & `careamics-0.1.0rc3/src/careamics/utils/logging.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/src/careamics/utils/metrics.py` & `careamics-0.1.0rc3/src/careamics/utils/metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -108,53 +108,7 @@
     -------
     Union[float, torch.tensor]
         Scale invariant PSNR value.
     """
     range_parameter = (np.max(gt) - np.min(gt)) / np.std(gt)
     gt_ = _zero_mean(gt) / np.std(gt)
     return psnr(_zero_mean(gt_), _fix(gt_, pred), range_parameter)
-
-
-class MetricTracker:
-    """
-    Metric tracker class.
-
-    This class is used to track values, sum, count and average of a metric over time.
-
-    Attributes
-    ----------
-    val : int
-        Last value of the metric.
-    avg : torch.Tensor.float
-        Average value of the metric.
-    sum : int
-        Sum of the metric values (times number of values).
-    count : int
-        Number of values.
-    """
-
-    def __init__(self) -> None:
-        """Constructor."""
-        self.reset()
-
-    def reset(self) -> None:
-        """Reset the metric tracker state."""
-        self.val = 0.0
-        self.avg: torch.Tensor.float = 0.0
-        self.sum = 0.0
-        self.count = 0.0
-
-    def update(self, value: int, n: int = 1) -> None:
-        """
-        Update the metric tracker state.
-
-        Parameters
-        ----------
-        value : int
-            Value to update the metric tracker with.
-        n : int
-            Number of values, equals to batch size.
-        """
-        self.val = value
-        self.sum += value * n
-        self.count += n
-        self.avg = self.sum / self.count
```

### Comparing `careamics-0.1.0rc2/tests/test_metrics.py` & `careamics-0.1.0rc3/tests/utils/test_metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pytest
 
 from careamics.utils.metrics import (
-    MetricTracker,
     _zero_mean,
     scale_invariant_psnr,
 )
 
 
 @pytest.mark.parametrize(
     "x",
@@ -25,28 +24,7 @@
     [
         (np.array([1, 2, 3, 4, 5, 6]), np.array([1, 2, 3, 4, 5, 6]), 332.22),
         (np.array([[1, 2, 3], [4, 5, 6]]), np.array([[1, 2, 3], [4, 5, 6]]), 332.22),
     ],
 )
 def test_scale_invariant_psnr(gt, pred, result):
     assert scale_invariant_psnr(gt, pred) == pytest.approx(result, rel=5e-3)
-
-
-def test_metric_tracker():
-    tracker = MetricTracker()
-
-    # check initial state
-    assert tracker.sum == 0
-    assert tracker.count == 0
-    assert tracker.avg == 0
-    assert tracker.val == 0
-
-    # run a few updates
-    n = 5
-    for i in range(n):
-        tracker.update(i, n)
-
-    # check values
-    assert tracker.sum == n * (n * (n - 1)) / 2
-    assert tracker.count == n * n
-    assert tracker.avg == (n - 1) / 2
-    assert tracker.val == n - 1
```

### Comparing `careamics-0.1.0rc2/tests/config/test_config.py` & `careamics-0.1.0rc3/tests/config/test_configuration_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,191 +3,186 @@
 import pytest
 
 from careamics.config import (
     Configuration,
     load_configuration,
     save_configuration,
 )
+from careamics.config.support import (
+    SupportedAlgorithm,
+    SupportedPixelManipulation,
+    SupportedTransform,
+)
 
 
 @pytest.mark.parametrize("name", ["Sn4K3", "C4_M e-L"])
-def test_config_valid_names(minimum_config: dict, name: str):
+def test_valid_names(minimum_configuration: dict, name: str):
     """Test valid names (letters, numbers, spaces, dashes and underscores)."""
-    minimum_config["experiment_name"] = name
-    myconf = Configuration(**minimum_config)
+    minimum_configuration["experiment_name"] = name
+    myconf = Configuration(**minimum_configuration)
     assert myconf.experiment_name == name
 
 
 @pytest.mark.parametrize("name", ["", "   ", "#", "/", "^", "%", ",", ".", "a=b"])
-def test_config_invalid_names(minimum_config: dict, name: str):
+def test_invalid_names(minimum_configuration: dict, name: str):
     """Test that invalid names raise an error."""
-    minimum_config["experiment_name"] = name
+    minimum_configuration["experiment_name"] = name
     with pytest.raises(ValueError):
-        Configuration(**minimum_config)
-
-
-@pytest.mark.parametrize("path", ["", "tmp"])
-def test_config_valid_working_directory(
-    tmp_path: Path, minimum_config: dict, path: str
-):
-    """Test valid working directory.
-
-    A valid working directory exists or its direct parent exists.
-    """
-    path = tmp_path / path
-    minimum_config["working_directory"] = str(path)
-    myconf = Configuration(**minimum_config)
-    assert myconf.working_directory == path
+        Configuration(**minimum_configuration)
 
 
-def test_config_invalid_working_directory(tmp_path: Path, minimum_config: dict):
-    """Test that invalid working directory raise an error.
-
-    Since its parent does not exist, this case is invalid.
+def test_3D_algorithm_and_data_compatibility(minimum_configuration: dict):
+    """Test that errors are raised if algorithm `is_3D` and data axes are
+    incompatible.
     """
-    path = tmp_path / "tmp" / "tmp"
-    minimum_config["working_directory"] = str(path)
-    with pytest.raises(ValueError):
-        Configuration(**minimum_config)
-
-    path = tmp_path / "tmp.txt"
-    path.touch()
-    minimum_config["working_directory"] = str(path)
-    with pytest.raises(ValueError):
-        Configuration(**minimum_config)
-
-
-def test_3D_algorithm_and_data_compatibility(minimum_config: dict):
-    """Test that errors are raised if algithm `is_3D` and data axes are incompatible."""
     # 3D but no Z in axes
-    minimum_config["algorithm"]["is_3D"] = True
-    with pytest.raises(ValueError):
-        Configuration(**minimum_config)
+    minimum_configuration["algorithm_config"]["model"]["conv_dims"] = 3
+    config = Configuration(**minimum_configuration)
+    assert config.algorithm_config.model.conv_dims == 2
 
     # 2D but Z in axes
-    minimum_config["algorithm"]["is_3D"] = False
-    minimum_config["data"]["axes"] = "ZYX"
-    with pytest.raises(ValueError):
-        Configuration(**minimum_config)
+    minimum_configuration["algorithm_config"]["model"]["conv_dims"] = 2
+    minimum_configuration["data_config"]["axes"] = "ZYX"
+    minimum_configuration["data_config"]["patch_size"] = [64, 64, 64]
+    config = Configuration(**minimum_configuration)
+    assert config.algorithm_config.model.conv_dims == 3
 
 
-def test_set_3D(minimum_config: dict):
+def test_set_3D(minimum_configuration: dict):
     """Test the set 3D method."""
-    conf = Configuration(**minimum_config)
+    conf = Configuration(**minimum_configuration)
 
     # set to 3D
-    conf.set_3D(True, "ZYX")
+    conf.set_3D(True, "ZYX", [64, 64, 64])
+    assert conf.data_config.axes == "ZYX"
+    assert conf.data_config.patch_size == [64, 64, 64]
+    assert conf.algorithm_config.model.conv_dims == 3
 
     # set to 2D
-    conf.set_3D(False, "SYX")
-
-    # fails if they are not compatible
-    with pytest.raises(ValueError):
-        conf.set_3D(True, "SYX")
-
-    with pytest.raises(ValueError):
-        conf.set_3D(False, "ZYX")
-
-
-def test_wrong_values_by_assignment(complete_config: dict):
-    """Test that wrong values raise an error when assigned."""
-    config = Configuration(**complete_config)
+    conf.set_3D(False, "SYX", [64, 64])
+    assert conf.data_config.axes == "SYX"
+    assert conf.data_config.patch_size == [64, 64]
+    assert conf.algorithm_config.model.conv_dims == 2
 
-    # experiment name
-    config.experiment_name = "My name is Inigo Montoya"
-    with pytest.raises(ValueError):
-        config.experiment_name = "¯\\_(ツ)_/¯"
-
-    # working directory
-    config.working_directory = complete_config["working_directory"]
-    with pytest.raises(ValueError):
-        config.working_directory = "o/o"
-
-    # data
-    config.data = complete_config["data"]
-    with pytest.raises(ValueError):
-        config.data = "I am not a data model"
-
-    # algorithm
-    config.algorithm = complete_config["algorithm"]
-    with pytest.raises(ValueError):
-        config.algorithm = None
-
-    # training
-    config.training = complete_config["training"]
-    with pytest.raises(ValueError):
-        config.training = "Hubert Blaine Wolfeschlegelsteinhausenbergerdorff Sr."
-
-    # TODO Because algorithm is a sub-model of Configuration, and the validation is
-    # done at the level of the Configuration, this does not cause any error, although
-    # it should.
-    config.algorithm.is_3D = True
 
-
-def test_minimum_config(minimum_config: dict):
-    """Test that we can instantiate a minimum config."""
-    dictionary = Configuration(**minimum_config).model_dump()
-    assert dictionary == minimum_config
-
-
-def test_complete_config(complete_config: dict):
-    """Test that we can instantiate a minimum config."""
-    dictionary = Configuration(**complete_config).model_dump()
-    assert dictionary == complete_config
-
-
-def test_config_to_dict_with_default_optionals(complete_config: dict):
-    """Test that the exclude optional options in model dump gives a full configuration,
-    including the default optional values.
-
-    Note that None values are always excluded.
-    """
-    # Algorithm default optional parameters
-    complete_config["algorithm"]["masking_strategy"] = "default"
-    complete_config["algorithm"]["masked_pixel_percentage"] = 0.2
-    complete_config["algorithm"]["model_parameters"] = {
-        "depth": 2,
-        "num_channels_init": 32,
+def test_algorithm_and_data_default_transforms(minimum_configuration: dict):
+    """Test that the default data transforms are compatible with n2v."""
+    minimum_configuration["algorithm_config"] = {
+        "algorithm": "n2v",
+        "loss": "n2v",
+        "model": {
+            "architecture": "UNet",
+        },
     }
+    Configuration(**minimum_configuration)
 
-    # Training default optional parameters
-    complete_config["training"]["optimizer"]["parameters"] = {}
-    complete_config["training"]["lr_scheduler"]["parameters"] = {}
-    complete_config["training"]["use_wandb"] = True
-    complete_config["training"]["num_workers"] = 0
-    complete_config["training"]["amp"] = {
-        "use": True,
-        "init_scale": 1024,
+
+@pytest.mark.parametrize(
+    "algorithm, strategy",
+    [
+        ("n2v", SupportedPixelManipulation.UNIFORM.value),
+        ("n2v", SupportedPixelManipulation.MEDIAN.value),
+        ("n2v2", SupportedPixelManipulation.UNIFORM.value),
+        ("n2v2", SupportedPixelManipulation.MEDIAN.value),
+    ],
+)
+def test_n2v2_and_transforms(minimum_configuration: dict, algorithm, strategy):
+    """Test that the manipulation strategy is corrected if the data transforms are
+    incompatible with n2v2."""
+    use_n2v2 = algorithm == "n2v2"
+    minimum_configuration["algorithm_config"] = {
+        "algorithm": "n2v",
+        "loss": "n2v",
+        "model": {
+            "architecture": "UNet",
+            "n2v2": use_n2v2,
+        },
     }
 
-    # instantiate config
-    myconf = Configuration(**complete_config)
-    assert myconf.model_dump(exclude_optionals=False) == complete_config
+    expected_strategy = (
+        SupportedPixelManipulation.MEDIAN.value
+        if use_n2v2
+        else SupportedPixelManipulation.UNIFORM.value
+    )
+
+    # missing ManipulateN2V
+    minimum_configuration["data_config"]["transforms"] = [
+        {"name": SupportedTransform.NDFLIP.value}
+    ]
+    config = Configuration(**minimum_configuration)
+    assert len(config.data_config.transforms) == 2
+    assert (
+        config.data_config.transforms[-1].name
+        == SupportedTransform.N2V_MANIPULATE.value
+    )
+    assert config.data_config.transforms[-1].strategy == expected_strategy
+
+    # passing ManipulateN2V with the wrong strategy
+    minimum_configuration["data_config"]["transforms"] = [
+        {
+            "name": SupportedTransform.N2V_MANIPULATE.value,
+            "strategy": strategy,
+        }
+    ]
+    config = Configuration(**minimum_configuration)
+    assert config.data_config.transforms[-1].strategy == expected_strategy
+
+
+def test_setting_n2v2(minimum_configuration: dict):
+    # make sure we use n2v
+    minimum_configuration["algorithm_config"][
+        "algorithm"
+    ] = SupportedAlgorithm.N2V.value
+
+    # test config
+    config = Configuration(**minimum_configuration)
+    assert config.algorithm_config.algorithm == SupportedAlgorithm.N2V.value
+    assert not config.algorithm_config.model.n2v2
+    assert (
+        config.data_config.transforms[-1].strategy
+        == SupportedPixelManipulation.UNIFORM.value
+    )
+
+    # set N2V2
+    config.set_N2V2(True)
+    assert config.algorithm_config.model.n2v2
+    assert (
+        config.data_config.transforms[-1].strategy
+        == SupportedPixelManipulation.MEDIAN.value
+    )
+
+    # set back to N2V
+    config.set_N2V2(False)
+    assert not config.algorithm_config.model.n2v2
+    assert (
+        config.data_config.transforms[-1].strategy
+        == SupportedPixelManipulation.UNIFORM.value
+    )
 
 
-def test_config_to_yaml(tmp_path: Path, minimum_config: dict):
+def test_config_to_yaml(tmp_path: Path, minimum_configuration: dict):
     """Test that we can export a config to yaml and load it back"""
 
     # test that we can instantiate a config
-    myconf = Configuration(**minimum_config)
+    myconf = Configuration(**minimum_configuration)
 
     # export to yaml
     yaml_path = save_configuration(myconf, tmp_path)
     assert yaml_path.exists()
 
     # load from yaml
     my_other_conf = load_configuration(yaml_path)
     assert my_other_conf == myconf
 
 
-def test_config_to_yaml_wrong_path(tmp_path: Path, minimum_config: dict):
+def test_config_to_yaml_wrong_path(tmp_path: Path, minimum_configuration: dict):
     """Test that an error is raised when the path is not a directory and not a .yml"""
 
     # test that we can instantiate a config
-    myconf = Configuration(**minimum_config)
+    myconf = Configuration(**minimum_configuration)
 
     # export to yaml
     yaml_path = tmp_path / "tmp.txt"
     with pytest.raises(ValueError):
         save_configuration(myconf, yaml_path)
 
     # existing file
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `careamics-0.1.0rc2/tests/dataset/test_dataset_utils.py` & `careamics-0.1.0rc3/tests/dataset/patching/test_tiled_patching.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 import numpy as np
 import pytest
 
-from careamics.dataset.patching import (
+from careamics.config.tile_information import TileInformation
+from careamics.dataset.patching.tiled_patching import (
     _compute_crop_and_stitch_coords_1d,
-    _compute_number_of_patches,
-    _compute_overlap,
-    _compute_patch_steps,
-    _compute_reshaped_view,
+    extract_tiles,
 )
 
 
+def check_extract_tiles(array: np.ndarray, tile_size, overlaps):
+    """Test extracting patches randomly."""
+    tile_data_generator = extract_tiles(array, tile_size, overlaps)
+
+    tiles = []
+    all_overlap_crop_coords = []
+    all_stitch_coords = []
+
+    # Assemble all tiles and their respective coordinates
+    for tile_data in tile_data_generator:
+        tile = tile_data[0]
+
+        tile_info: TileInformation = tile_data[1]
+        overlap_crop_coords = tile_info.overlap_crop_coords
+        stitch_coords = tile_info.stitch_coords
+
+        # add data to lists
+        tiles.append(tile)
+        all_overlap_crop_coords.append(overlap_crop_coords)
+        all_stitch_coords.append(stitch_coords)
+
+        # check tile shape, ignore sample dimension
+        assert tile.shape[1:] == tile_size
+        assert len(overlap_crop_coords) == len(stitch_coords) == len(tile_size)
+
+    # check that each tile has a unique set of coordinates
+    assert len(tiles) == len(all_overlap_crop_coords) == len(all_stitch_coords)
+
+    # check that all values are covered by the tiles
+    n_max = np.prod(array.shape)  # maximum value in the array
+    unique = np.unique(np.array(tiles))  # unique values in the patches
+    assert len(unique) >= n_max
+
+
 @pytest.mark.parametrize(
-    "shape, patch_sizes, expected",
+    "tile_size, overlaps",
     [
-        ((1, 10, 10), (10, 5), (1, 2)),
-        ((1, 9, 9), (4, 3), (3, 3)),
-        ((1, 10, 9), (3, 5), (4, 2)),
-        ((1, 5, 9, 10), (2, 3, 5), (3, 3, 2)),
+        ((4, 4), (2, 2)),
+        ((8, 8), (4, 4)),
     ],
 )
-def test_compute_number_of_patches(shape, patch_sizes, expected):
-    """Test computing number of patches"""
-    arr = np.ones(shape)
-
-    assert _compute_number_of_patches(arr, patch_sizes) == expected
+def test_extract_tiles_2d(array_2D, tile_size, overlaps):
+    """Test extracting tiles for prediction in 2D."""
+    check_extract_tiles(array_2D, tile_size, overlaps)
 
 
 @pytest.mark.parametrize(
-    "shape, patch_sizes, expected",
+    "tile_size, overlaps",
     [
-        ((1, 10, 10), (10, 5), (0, 0)),
-        ((1, 9, 9), (4, 3), (2, 0)),
-        ((1, 10, 9), (3, 5), (1, 1)),
+        ((4, 4, 4), (2, 2, 2)),
+        ((8, 8, 8), (4, 4, 4)),
     ],
 )
-def test_compute_overlap(shape, patch_sizes, expected):
-    """Test computing overlap between patches"""
-    arr = np.ones(shape)
-
-    assert _compute_overlap(arr, patch_sizes) == expected
-
-
-@pytest.mark.parametrize("dims", [2, 3])
-@pytest.mark.parametrize("patch_size", [2, 3])
-@pytest.mark.parametrize("overlap", [0, 1, 4])
-def test_compute_patch_steps(dims, patch_size, overlap):
-    """Test computing patch steps"""
-    patch_sizes = (patch_size,) * dims
-    overlaps = (overlap,) * dims
-    expected = (min(patch_size - overlap, patch_size),) * dims
+def test_extract_tiles_3d(array_3D, tile_size, overlaps):
+    """Test extracting tiles for prediction in 3D.
 
-    assert _compute_patch_steps(patch_sizes, overlaps) == expected
-
-
-def check_compute_reshaped_view(array, window_shape, steps):
-    """Check the number of patches"""
-
-    win = (1, *window_shape)
-    step = (1, *steps)
-    output_shape = (-1, *window_shape)
-
-    # compute views
-    output = _compute_reshaped_view(array, win, step, output_shape)
-
-    # check the number of patches
-    n_patches = [
-        np.ceil((array.shape[1 + i] - window_shape[i] + 1) / steps[i]).astype(int)
-        for i in range(len(window_shape))
-    ]
-    assert output.shape == (np.prod(n_patches), *window_shape)
+    The 3D array is a fixture of shape (1, 8, 16, 16)."""
+    check_extract_tiles(array_3D, tile_size, overlaps)
 
 
 @pytest.mark.parametrize("axis_size", [32, 35, 40])
 @pytest.mark.parametrize("patch_size, overlap", [(16, 4), (8, 6), (16, 8), (32, 24)])
 def test_compute_crop_and_stitch_coords_1d(axis_size, patch_size, overlap):
     (
         crop_coords,
@@ -117,33 +114,7 @@
     )
 
     # check that shape of all cropped tiles is equal
     assert np.array_equal(
         np.array(overlap_crop_coords)[:, 1] - np.array(overlap_crop_coords)[:, 0],
         np.array(stitch_coords)[:, 1] - np.array(stitch_coords)[:, 0],
     )
-
-
-@pytest.mark.parametrize(
-    "window_shape, steps",
-    [
-        ((5, 5), (1, 1)),
-        ((5, 5), (2, 3)),
-        ((5, 7), (1, 1)),
-    ],
-)
-def test_compute_reshaped_view_2d(array_2D, window_shape, steps):
-    """Test computing reshaped view of an array of shape (1, 10, 9)."""
-    check_compute_reshaped_view(array_2D, window_shape, steps)
-
-
-@pytest.mark.parametrize(
-    "window_shape, steps",
-    [
-        ((1, 5, 5), (2, 1, 2)),
-        ((2, 5, 5), (2, 3, 4)),
-        ((3, 7, 8), (1, 1, 3)),
-    ],
-)
-def test_compute_reshaped_view_3d(array_3D, window_shape, steps):
-    """Test computing reshaped view of an array of shape (1, 5, 10, 9)."""
-    check_compute_reshaped_view(array_3D, window_shape, steps)
```

### Comparing `careamics-0.1.0rc2/tests/utils/test_context.py` & `careamics-0.1.0rc3/tests/utils/test_context.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/tests/utils/test_logging.py` & `careamics-0.1.0rc3/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/LICENSE` & `careamics-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc2/pyproject.toml` & `careamics-0.1.0rc3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# https://peps.python.org/pep-0517/
+
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
+# read more about configuring hatch at:
+# https://hatch.pypa.io/latest/config/build/
 
 # https://hatch.pypa.io/latest/config/metadata/
 [tool.hatch.version]
 source = "vcs"
 
-# https://hatch.pypa.io/latest/config/build/
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "careamics"
@@ -18,158 +21,161 @@
 description = "Toolbox for running N2V and friends."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "BSD-3-Clause" }
 authors = [
     { name = 'Igor Zubarev', email = 'igor.zubarev@fht.org' },
     { name = 'Joran Deschamps', email = 'joran.deschamps@fht.org' },
-    { name = 'Vera Galinova', email = 'vera.galinova@fht.org' },
-    { name = 'Mehdi Seifi', email = 'mehdi.seifi@fht.org' },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
-    'torch',
-    'torchvision',
+    'torch>=2.0.0',
+    'albumentations',
+    'bioimageio.core>=0.6.0',
     'tifffile',
+    'psutil',
+    'pydantic>=2.5',
+    'pytorch_lightning>=2.2.0',
     'pyyaml',
-    'pydantic>=2.0',
     'scikit-image',
-    'bioimageio.core',
     'zarr',
 ]
 
 [project.optional-dependencies]
 # development dependencies and tooling
-dev = ["pre-commit", "pytest", "pytest-cov"]
-
-# for ci
-test = ["pytest", "pytest-cov", "wandb"]
-
-# notebooks
-notebooks = [
-    "jupyter",
-    "careamics-portfolio",
-    "itkwidgets",
-    "torchsummary",
-    "ipython",
-    "wandb",
-]
-
-# all
-all = [
+dev = [
     "pre-commit",
     "pytest",
     "pytest-cov",
-    "wandb",
-    "jupyter",
-    "careamics-portfolio",
-    "itkwidgets",
-    "torchsummary",
-    "ipython",
+    "sybil",      # doctesting
 ]
 
+# notebooks
+examples = ["jupyter", "careamics-portfolio", "matplotlib"]
+
+# loggers
+wandb = ["wandb"]
+tensorboard = ["tensorboard", "protobuf==3.20.3"]
+
 [project.urls]
 homepage = "https://careamics.github.io/"
 repository = "https://github.com/CAREamics/careamics"
 
-# https://docs.astral.sh/ruff/
+# https://beta.ruff.rs/docs
 [tool.ruff]
 line-length = 88
 target-version = "py38"
 src = ["src"]
 select = [
-    "E",    # style errors
-    "W",    # style warnings
-    "F",    # flakes
-    "I",    # isort
-    "UP",   # pyupgrade
+    "E",  # style errors
+    "W",  # style warnings
+    "F",  # flakes
+    "D",  # pydocstyle
+    "I",  # isort
+    "UP", # pyupgrade
+    # "S",    # bandit
     "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "RUF",  # ruff-specific rules
-    "TCH",  # flake8-type-checking
-    "TID",  # flake8-tidy-imports
 ]
 ignore = [
+    "D100", # Missing docstring in public module
+    "D107", # Missing docstring in __init__
+    "D203", # 1 blank line required before class docstring
+    "D212", # Multi-line docstring summary should start at the first line
+    "D213", # Multi-line docstring summary should start at the second line
+    "D401", # First line should be in imperative mood
+    "D413", # Missing blank line after last section
+    "D416", # Section name should end with a colon
+
+    # incompatibility with mypy
+    "RUF005", # collection-literal-concatenation, in prediction_utils.py:30
+
     # version specific
     "UP006", # Replace typing.List by list, mandatory for py3.8
     "UP007", # Replace Union by |, mandatory for py3.9
 ]
 ignore-init-module-imports = true
 show-fixes = true
 
+[tool.ruff.pydocstyle]
+convention = "numpy"
+
 [tool.ruff.per-file-ignores]
-"tests/*.py" = ["S"]
+"tests/*.py" = ["D", "S"]
+"setup.py" = ["D"]
 
 [tool.black]
 line-length = 88
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/"
 strict = false
-allow_untyped_defs = false
-allow_untyped_calls = false
-disallow_any_generics = false
-ignore_missing_imports = false
+# allow_untyped_defs = false
+# allow_untyped_calls = false
+# disallow_any_generics = false
+# ignore_missing_imports = false
+
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
-testpaths = ["tests"]
+testpaths = ["src/careamics", "tests"] # add src/careamics for doctest discovery
 filterwarnings = [
     # "error",
     # "ignore::UserWarning",
 ]
-markers = ["gpu: mark tests as requiring gpu"]
+addopts = "-p no:doctest"
 
+markers = ["gpu: marks tests as requiring gpu"]
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
+    "except ImportError",
     "\\.\\.\\.",
-    "except ImportError:",
     "raise NotImplementedError()",
-    "except PackageNotFoundError:",
-    "if torch.cuda.is_available():",
-    "except UsageError as e:",
-    "except ModuleNotFoundError:",
-    "except KeyboardInterrupt:",
 ]
 
 [tool.coverage.run]
 source = ["careamics"]
 
 # https://github.com/mgedmin/check-manifest#configuration
 # add files that you want check-manifest to explicitly ignore here
 # (files that are in the repo but shouldn't go in the package)
 [tool.check-manifest]
 ignore = [
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
     ".ruff_cache/**/*",
+    "setup.py",
     "tests/**/*",
 ]
 
-# https://numpydoc.readthedocs.io/en/latest/format.html
 [tool.numpydoc_validation]
 checks = [
-    "all",  # report on all checks, except the ones below
-    "EX01", # No examples section found
+    "all",  # report on all checks, except the below
+    "EX01", # Example section not found
     "SA01", # See Also section not found
-    "ES01", # No extended summary found
+    "ES01", # Extended Summar not found
+    "GL01", # Docstring text (summary) should start in the line immediately
+    # after the opening quotes
+    "GL02", # Closing quotes should be placed in the line after the last text 
+    # in the docstring
+    "GL03", # Double line break found
 ]
 exclude = [ # don't report on objects that match any of these regex
     "test_*",
 ]
```

