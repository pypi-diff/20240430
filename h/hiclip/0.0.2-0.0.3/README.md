# Comparing `tmp/hiclip-0.0.2.tar.gz` & `tmp/hiclip-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiclip-0.0.2.tar", max compression
+gzip compressed data, was "hiclip-0.0.3.tar", max compression
```

## Comparing `hiclip-0.0.2.tar` & `hiclip-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,145 @@
--rw-r--r--   0        0        0     1068 2024-04-28 07:45:53.376206 hiclip-0.0.2/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-28 07:45:53.376206 hiclip-0.0.2/README.md
--rw-r--r--   0        0        0      175 2024-04-28 07:45:53.376206 hiclip-0.0.2/hiclip/__init__.py
--rw-r--r--   0        0        0      135 2024-04-28 07:45:53.376206 hiclip-0.0.2/hiclip/_constants.py
--rw-r--r--   0        0        0     4394 2024-04-28 07:45:53.376206 hiclip-0.0.2/hiclip/_data.py
--rw-r--r--   0        0        0    15869 2024-04-28 07:45:53.376206 hiclip-0.0.2/hiclip/_model.py
--rw-r--r--   0        0        0     7721 2024-04-28 07:45:53.380206 hiclip-0.0.2/hiclip/_module.py
--rw-r--r--   0        0        0     6244 2024-04-28 07:45:53.380206 hiclip-0.0.2/hiclip/_train.py
--rw-r--r--   0        0        0     2342 2024-04-28 07:45:53.380206 hiclip-0.0.2/hiclip/_utils.py
--rw-r--r--   0        0        0     1633 2024-04-28 07:45:53.380206 hiclip-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 hiclip-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-30 02:53:29.112737 hiclip-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1522 2024-04-30 02:53:29.112737 hiclip-0.0.3/README.md
+-rw-r--r--   0        0        0      614 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/.flake8
+-rw-r--r--   0        0        0       44 2024-04-30 02:53:29.716738 hiclip-0.0.3/hiclip/Torchelie/.git
+-rw-r--r--   0        0        0      650 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1081 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       24 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/.gitignore
+-rw-r--r--   0        0        0      575 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/.readthedocs.yml
+-rw-r--r--   0        0        0     1086 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/LICENSE
+-rw-r--r--   0        0        0    15574 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/README.md
+-rw-r--r--   0        0        0      634 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/docs/Makefile
+-rw-r--r--   0        0        0      480 2024-04-30 02:53:30.424740 hiclip-0.0.3/hiclip/Torchelie/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   127534 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/_static/dream_example.jpg
+-rw-r--r--   0        0        0   221189 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/_static/style_example.png
+-rw-r--r--   0        0        0    47282 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/_static/vis_example.jpg
+-rw-r--r--   0        0        0      161 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/_templates/klass.rst
+-rw-r--r--   0        0        0     1201 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/callbacks.rst
+-rw-r--r--   0        0        0     2475 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/conf.py
+-rw-r--r--   0        0        0      103 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/data_learning.rst
+-rw-r--r--   0        0        0      787 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/datasets.rst
+-rw-r--r--   0        0        0      121 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/distributions.rst
+-rw-r--r--   0        0        0       78 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/hyper.rst
+-rw-r--r--   0        0        0     1111 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/index.rst
+-rw-r--r--   0        0        0     1273 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/loss.rst
+-rw-r--r--   0        0        0      795 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/make.bat
+-rw-r--r--   0        0        0     2421 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/models.rst
+-rw-r--r--   0        0        0     2340 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/nn.rst
+-rw-r--r--   0        0        0      391 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/optimizers.rst
+-rw-r--r--   0        0        0    15074 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/recipe_tuto.rst
+-rw-r--r--   0        0        0     1394 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/recipes.rst
+-rw-r--r--   0        0        0      483 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/transforms.rst
+-rw-r--r--   0        0        0       79 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/docs/utils.rst
+-rw-r--r--   0        0        0     2478 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/examples/conditional.py
+-rw-r--r--   0        0        0     2639 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/examples/gan.py
+-rw-r--r--   0        0        0     2916 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/examples/mnist.py
+-rw-r--r--   0        0        0     1869 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/examples/pixelcnn.py
+-rw-r--r--   0        0        0   157873 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/logo.png
+-rw-r--r--   0        0        0      108 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/requirements-docs.txt
+-rw-r--r--   0        0        0       77 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/requirements.txt
+-rwxr-xr-x   0        0        0      673 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/run_tests.sh
+-rw-r--r--   0        0        0      405 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/setup.py
+-rw-r--r--   0        0        0   114686 2024-04-30 02:53:30.428740 hiclip-0.0.3/hiclip/Torchelie/tests/dream_me.jpg
+-rw-r--r--   0        0        0   125190 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/style.jpg
+-rw-r--r--   0        0        0     2113 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_datalearning.py
+-rw-r--r--   0        0        0     1226 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_datasets.py
+-rw-r--r--   0        0        0     2342 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_loss.py
+-rw-r--r--   0        0        0     1537 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_models.py
+-rw-r--r--   0        0        0     2753 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_nn.py
+-rw-r--r--   0        0        0      559 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_optims.py
+-rw-r--r--   0        0        0     2814 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_recipes.py
+-rw-r--r--   0        0        0      426 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_sched.py
+-rw-r--r--   0        0        0     2377 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_tensorboard_callback.py
+-rw-r--r--   0        0        0     1282 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_tranforms.py
+-rw-r--r--   0        0        0      735 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/tests/test_utils.py
+-rw-r--r--   0        0        0      356 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/callbacks/__init__.py
+-rw-r--r--   0        0        0     2341 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/callbacks/avg.py
+-rw-r--r--   0        0        0    30088 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/callbacks/callbacks.py
+-rw-r--r--   0        0        0     6501 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/callbacks/inspector.py
+-rw-r--r--   0        0        0     7665 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/data_learning.py
+-rw-r--r--   0        0        0    11045 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/datasets/__init__.py
+-rw-r--r--   0        0        0     3909 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/datasets/concat.py
+-rw-r--r--   0        0        0     1599 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/datasets/debug.py
+-rw-r--r--   0        0        0     2581 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/datasets/ms1m.py
+-rw-r--r--   0        0        0     4081 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/datasets/pix2pix.py
+-rw-r--r--   0        0        0     2982 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/distributions.py
+-rw-r--r--   0        0        0    11705 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/hyper.py
+-rw-r--r--   0        0        0     1287 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/__init__.py
+-rw-r--r--   0        0        0     4899 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/bitempered.py
+-rw-r--r--   0        0        0     1473 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/deepdreamloss.py
+-rw-r--r--   0        0        0     3956 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/face_rec.py
+-rw-r--r--   0        0        0      492 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/focal.py
+-rw-r--r--   0        0        0     2174 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/functional/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/gan/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/gan/hinge.py
+-rw-r--r--   0        0        0     3828 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/gan/penalty.py
+-rw-r--r--   0        0        0     1212 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/gan/standard.py
+-rw-r--r--   0        0        0     8672 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/neuralstyleloss.py
+-rw-r--r--   0        0        0     2097 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/loss/perceptualloss.py
+-rw-r--r--   0        0        0     3662 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/lr_scheduler.py
+-rw-r--r--   0        0        0      524 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/attention.py
+-rw-r--r--   0        0        0     3405 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/autogan.py
+-rw-r--r--   0        0        0     5608 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/classifier.py
+-rw-r--r--   0        0        0     3640 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/efficient.py
+-rw-r--r--   0        0        0     3334 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/hourglass.py
+-rw-r--r--   0        0        0     3878 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/patchgan.py
+-rw-r--r--   0        0        0     1966 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/perceptualnet.py
+-rw-r--r--   0        0        0     2673 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/pix2pix.py
+-rw-r--r--   0        0        0     4831 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/pix2pixhd.py
+-rw-r--r--   0        0        0     7728 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/pixcnn.py
+-rw-r--r--   0        0        0     8469 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/resnet.py
+-rw-r--r--   0        0        0     5577 2024-04-30 02:53:30.432740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/snres_discr.py
+-rw-r--r--   0        0        0     7151 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/stylegan2.py
+-rw-r--r--   0        0        0     3029 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/unet.py
+-rw-r--r--   0        0        0     2581 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/models/vgg.py
+-rw-r--r--   0        0        0      594 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/adain.py
+-rw-r--r--   0        0        0     8074 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/batchnorm.py
+-rw-r--r--   0        0        0    10828 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/blocks.py
+-rw-r--r--   0        0        0      931 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/condseq.py
+-rw-r--r--   0        0        0     6867 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/conv.py
+-rw-r--r--   0        0        0     1159 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/debug.py
+-rw-r--r--   0        0        0     4979 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/encdec.py
+-rw-r--r--   0        0        0     2291 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/functional/__init__.py
+-rw-r--r--   0        0        0     2093 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/functional/vq.py
+-rw-r--r--   0        0        0     2889 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/graph.py
+-rw-r--r--   0        0        0      581 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/imagenetinputnorm.py
+-rw-r--r--   0        0        0     1742 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/interpolate.py
+-rw-r--r--   0        0        0     8511 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/layers.py
+-rw-r--r--   0        0        0     3424 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/maskedconv.py
+-rw-r--r--   0        0        0     1053 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/noise.py
+-rw-r--r--   0        0        0      188 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/pixelnorm.py
+-rw-r--r--   0        0        0    14512 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/resblock.py
+-rw-r--r--   0        0        0      681 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/reshape.py
+-rw-r--r--   0        0        0    11854 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/utils.py
+-rw-r--r--   0        0        0     4937 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/vq.py
+-rw-r--r--   0        0        0     1993 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/nn/withsavedactivations.py
+-rw-r--r--   0        0        0    10363 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/optim.py
+-rw-r--r--   0        0        0      954 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/__init__.py
+-rw-r--r--   0        0        0    14734 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/classification.py
+-rw-r--r--   0        0        0     4101 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/deepdream.py
+-rw-r--r--   0        0        0     4759 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/feature_vis.py
+-rw-r--r--   0        0        0     3148 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/gan.py
+-rw-r--r--   0        0        0     9380 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/image_prior.py
+-rw-r--r--   0        0        0     6238 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/neural_style.py
+-rw-r--r--   0        0        0     8891 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/pix2pix.py
+-rw-r--r--   0        0        0     7922 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/recipebase.py
+-rw-r--r--   0        0        0    13099 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/stylegan2.py
+-rw-r--r--   0        0        0     2299 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/trainandcall.py
+-rw-r--r--   0        0        0     3299 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/trainandtest.py
+-rw-r--r--   0        0        0    10022 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/recipes/unpaired.py
+-rw-r--r--   0        0        0      809 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/serving_utils.py
+-rw-r--r--   0        0        0     6974 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/transforms/__init__.py
+-rw-r--r--   0        0        0    10468 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/transforms/differentiable.py
+-rw-r--r--   0        0        0    17689 2024-04-30 02:53:30.436740 hiclip-0.0.3/hiclip/Torchelie/torchelie/utils.py
+-rw-r--r--   0        0        0      175 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_constants.py
+-rw-r--r--   0        0        0     4394 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_data.py
+-rw-r--r--   0        0        0    15869 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_model.py
+-rw-r--r--   0        0        0     7721 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_module.py
+-rw-r--r--   0        0        0     6244 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_train.py
+-rw-r--r--   0        0        0     2342 2024-04-30 02:53:29.112737 hiclip-0.0.3/hiclip/_utils.py
+-rw-r--r--   0        0        0     1633 2024-04-30 02:53:29.116737 hiclip-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 hiclip-0.0.3/PKG-INFO
```

### Comparing `hiclip-0.0.2/LICENSE` & `hiclip-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/README.md` & `hiclip-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 Then, install the appropriate version of PyTorch. After experimental verification, hiclip works well in the environment of pytorch 2.0.1 + CUDA 11.7.
 ``` bash
 # This is just an example, you can find the appropriate version in https://pytorch.org/get-started/previous-versions/
 pip install torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2
 ```
 
 ## Tutorial
+### generate train dataset
 ```python
 import hiclip
 
 
 # uri also support .cool file
 dataset = hiclip.setup_data(
     main_cooler_uri="main/K562.mcool::/resolutions/5000",
     sub_cooler_uri="sub/K562.mcool::/resolutions/5000",
     target_cooler_uri="target/K562.mcool::/resolutions/5000",
 )
 dataset.write(filename="dataset", compression="gzip")
 ```
-
+### train
 ```python
 import anndata
 import hiclip
 
 
 dataset = anndata.read_h5ad("dataset")
 hiclip.HiClip.setup_anndata(dataset)
@@ -38,21 +39,26 @@
     max_epochs=200,
     save_ckpt_every_n_epoch=2,
     plan_kwargs={"lr": 1e-3, "weight_decay": 0},
     batch_size=4,
     num_workers=16,
 )
 ```
-
+### predict or observe
 ```python
 import anndata
 import hiclip
 
 
 dataset = anndata.read_h5ad("dataset")
-
 model = hiclip.HiClip.load(
-    ".hiclip/2024-02-26_16-59-10_val_hiclip_metric/epoch=...",
+    ".hiclip/202X-XX-XX_XX-XX-XX_val_hiclip_metric/epoch=...",
     dataset
 )
+
+# if predict
 pred: anndata.AnnData = model.predict(dataset)
-```
+# if observe
+pred = model.observe(main_cooler_uri, sub_cooler_uri, chrom, start, end)
+```
+
+**The specific case is in the examples folder.**
```

### Comparing `hiclip-0.0.2/hiclip/_data.py` & `hiclip-0.0.3/hiclip/_data.py`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/hiclip/_model.py` & `hiclip-0.0.3/hiclip/_model.py`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/hiclip/_module.py` & `hiclip-0.0.3/hiclip/_module.py`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/hiclip/_train.py` & `hiclip-0.0.3/hiclip/_train.py`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/hiclip/_utils.py` & `hiclip-0.0.3/hiclip/_utils.py`

 * *Files identical despite different names*

### Comparing `hiclip-0.0.2/pyproject.toml` & `hiclip-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hiclip"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["liminghong.dev <lmh0066@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `hiclip-0.0.2/PKG-INFO` & `hiclip-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclip
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: liminghong.dev
 Author-email: lmh0066@outlook.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,27 +33,28 @@
 Then, install the appropriate version of PyTorch. After experimental verification, hiclip works well in the environment of pytorch 2.0.1 + CUDA 11.7.
 ``` bash
 # This is just an example, you can find the appropriate version in https://pytorch.org/get-started/previous-versions/
 pip install torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2
 ```
 
 ## Tutorial
+### generate train dataset
 ```python
 import hiclip
 
 
 # uri also support .cool file
 dataset = hiclip.setup_data(
     main_cooler_uri="main/K562.mcool::/resolutions/5000",
     sub_cooler_uri="sub/K562.mcool::/resolutions/5000",
     target_cooler_uri="target/K562.mcool::/resolutions/5000",
 )
 dataset.write(filename="dataset", compression="gzip")
 ```
-
+### train
 ```python
 import anndata
 import hiclip
 
 
 dataset = anndata.read_h5ad("dataset")
 hiclip.HiClip.setup_anndata(dataset)
@@ -63,21 +64,26 @@
     max_epochs=200,
     save_ckpt_every_n_epoch=2,
     plan_kwargs={"lr": 1e-3, "weight_decay": 0},
     batch_size=4,
     num_workers=16,
 )
 ```
-
+### predict or observe
 ```python
 import anndata
 import hiclip
 
 
 dataset = anndata.read_h5ad("dataset")
-
 model = hiclip.HiClip.load(
-    ".hiclip/2024-02-26_16-59-10_val_hiclip_metric/epoch=...",
+    ".hiclip/202X-XX-XX_XX-XX-XX_val_hiclip_metric/epoch=...",
     dataset
 )
+
+# if predict
 pred: anndata.AnnData = model.predict(dataset)
+# if observe
+pred = model.observe(main_cooler_uri, sub_cooler_uri, chrom, start, end)
 ```
+
+**The specific case is in the examples folder.**
```

