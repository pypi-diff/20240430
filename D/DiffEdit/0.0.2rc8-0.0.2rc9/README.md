# Comparing `tmp/diffedit-0.0.2rc8.tar.gz` & `tmp/diffedit-0.0.2rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffedit-0.0.2rc8.tar", max compression
+gzip compressed data, was "diffedit-0.0.2rc9.tar", max compression
```

## Comparing `diffedit-0.0.2rc8.tar` & `diffedit-0.0.2rc9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/LICENSE
--rw-r--r--   0        0        0     5062 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/README.md
--rw-r--r--   0        0        0     4983 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/__init__.py
--rw-r--r--   0        0        0       57 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/constants.py
--rw-r--r--   0        0        0    10994 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/diff_edit_model.py
--rw-r--r--   0        0        0     2243 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/image_processing.py
--rw-r--r--   0        0        0     8789 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/mask_generation.py
--rw-r--r--   0        0        0      852 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/mask_inpainting.py
--rw-r--r--   0        0        0     3833 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/model_composer.py
--rw-r--r--   0        0        0     7551 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/scripts/image_edit.py
--rw-r--r--   0        0        0   434756 2024-04-25 10:07:43.365490 diffedit-0.0.2rc8/src/diff_edit/scripts/mask.png
--rw-r--r--   0        0        0   491401 2024-04-25 10:07:43.365490 diffedit-0.0.2rc8/src/diff_edit/scripts/result.png
--rw-r--r--   0        0        0     6581 1970-01-01 00:00:00.000000 diffedit-0.0.2rc8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 15:30:04.367664 diffedit-0.0.2rc9/LICENSE
+-rw-r--r--   0        0        0     6308 2024-04-25 15:30:04.367664 diffedit-0.0.2rc9/README.md
+-rw-r--r--   0        0        0     4983 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/constants.py
+-rw-r--r--   0        0        0    10994 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/diff_edit_model.py
+-rw-r--r--   0        0        0     2243 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/image_processing.py
+-rw-r--r--   0        0        0     8789 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/mask_generation.py
+-rw-r--r--   0        0        0      852 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/mask_inpainting.py
+-rw-r--r--   0        0        0     3833 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/model/model_composer.py
+-rw-r--r--   0        0        0     7609 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/scripts/image_edit.py
+-rw-r--r--   0        0        0   434756 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/scripts/mask.png
+-rw-r--r--   0        0        0   491401 2024-04-25 15:30:04.371664 diffedit-0.0.2rc9/src/diff_edit/scripts/result.png
+-rw-r--r--   0        0        0     7827 1970-01-01 00:00:00.000000 diffedit-0.0.2rc9/PKG-INFO
```

### Comparing `diffedit-0.0.2rc8/LICENSE` & `diffedit-0.0.2rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/README.md` & `diffedit-0.0.2rc9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,40 +13,89 @@
 <table>
 <head>
 <th> Prompt: <i>remove</i> ⟶ <i>add</i>)</th><th>Original image</th> <th>Mask</th> <th>Edited</th>
 </head>
 <body>
 <tr>
 <td>"lion" ⟶ "dog"</td>
-<td><img src="static/ai_gen_lion.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_lion_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_lion_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_lion.jpeg" width="256" height="256" alt="An AI generated lion"></td>
+<td><img src="static/ai_gen_lion_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the 'lion'"></td>
+<td><img src="static/ai_gen_lion_result.png" width="256" height="256"
+         alt="The edited image with the 'dog' instead of the 'lion'"></td>
 </tr>
 <tr>
 <td>"house" ⟶ "3-floor hotel"</td>
-<td><img src="static/ai_gen_house.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_house_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_house_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_house.jpeg" width="256" height="256" alt="An AI generated house"></td>
+<td><img src="static/ai_gen_house_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the 'house'"></td>
+<td><img src="static/ai_gen_house_result.png" width="256" height="256"
+         alt="The edited image with the '3-floor hotel' instead of the 'house'"></td>
 </tr>
 <tr>
 <td>"an F1 race" ⟶ "a motogp race"</td>
-<td><img src="static/ai_gen_f1.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_f1_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_f1_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_f1.jpeg" width="256" height="256" alt="An AI generated image of an F1 competition"></td>
+<td><img src="static/ai_gen_f1_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the F1 cars"></td>
+<td><img src="static/ai_gen_f1_result.png" width="256" height="256"
+         alt="The edited image with the 'motogp' instead of the 'F1'"></td>
 </tr>
 </body>
 </table>
 
 All the previous masks was generated with: `num-samples = 10`
 
 ## Installation
 
+You can install the package in different ways, depending on your needs.
+
+
+
+<details>
+  <summary> Optional step (recommended)</summary>
+  
+Create a virtual environment, to avoid conflicts with other packages. Here are some alternatives:
+
+- with `venv`:
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+
+- with `poetry`:
+```bash
+poetry shell
+```
+
+- with `conda`:
+```bash
+conda create -n diff-edit python=3.10
+conda activate diff-edit
+```
+
+</details>
+
+
+Install the package from PyPi:
+```bash
+pip install diff-edit
+```
+<details>
+    <summary> Alternative ways</summary>
+
+Install the package from source:
+```bash
+poetry install
+```
+
+Install the package in editable mode, suggested for further development:
 ```bash
 pip install -e .
 ```
+</details>
 
 ## Usage
 
 For a fast evaluation use the script <a href="https://github.com/Gennaro-Farina/DiffEdit/blob/main/src/diff_edit/examples/image_edit.py">image_edit.py</a>:
 
 ```bash
 python image_edit.py --input_image <path_to_image> --output_image <path_to_output_image> --prompt <prompt>
```

#### html2text {}

```diff
@@ -5,46 +5,58 @@
 build_and_test.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/
 actions/workflows/build_and_test.yml) An unofficial implementation of _D_i_f_f_E_d_i_t
 based on _ð__¤__ _H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage
 the diffusion process to automatically extract a mask from an image given a
 prompt. The mask is then used to inpaint the image with the new content. To get
 a clearer overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b
 notebook. ## Results
-"lion" â¶   [static/           [static/               [static/
-"dog"        ai_gen_lion.jpeg]  ai_gen_lion_mask.png]  ai_gen_lion_result.png]
-"house" â¶  [static/           [static/               [static/
-"3-floor     ai_gen_house.jpeg] ai_gen_house_mask.png] ai_gen_house_result.png]
-hotel"
-"an F1 race" [static/           [static/               [static/
-â¶ "a       ai_gen_f1.jpeg]    ai_gen_f1_mask.png]    ai_gen_f1_result.png]
-motogp race"
+                                      [The mask of the  [The edited image with
+"lion" â¶ "dog"     [An AI generated image region      the 'dog' instead of
+                     lion]            containing the    the 'lion']
+                                      'lion']
+                                      [The mask of the  [The edited image with
+"house" â¶ "3-floor [An AI generated image region      the '3-floor hotel'
+hotel"               house]           containing the    instead of the
+                                      'house']          'house']
+                     [An AI generated [The mask of the  [The edited image with
+"an F1 race" â¶ "a  image of an F1   image region      the 'motogp' instead
+motogp race"         competition]     containing the F1 of the 'F1']
+                                      cars]
 All the previous masks was generated with: `num-samples = 10` ## Installation
-```bash pip install -e . ``` ## Usage For a fast evaluation use the script
-_i_m_a_g_e___e_d_i_t_._p_y: ```bash python image_edit.py --input_image --output_image --
-prompt ``` An example of usage is the following (resulting in _t_h_i_s image):
-```bash python image_edit.py --remove-prompt "lion" --add-prompt "dog" --image-
-link "https://github.com/Gennaro-Farina/DiffEdit/blob/main/static/
-ai_gen_lion.jpeg" --num-samples 10 ``` You can further customize the process by
-tuning the parameters of the script. Here is the full list of parameters that
-you can tune: ```bash python image_edit.py --help usage: image_edit.py [-h] [--
-remove-prompt REMOVE_PROMPT] [--add-prompt ADD_PROMPT] [--image IMAGE] [--
-image-link IMAGE_LINK] [--device {cpu,cuda,mps}] [--vae-model VAE_MODEL] [--
-tokenizer TOKENIZER] [--text-encoder TEXT_ENCODER] [--unet UNET] [--scheduler
-SCHEDULER] [--scheduler-start SCHEDULER_START] [--scheduler-end SCHEDULER_END]
-[--num-train-timesteps NUM_TRAIN_TIMESTEPS] [--beta-schedule BETA_SCHEDULE] [--
-inpainting INPAINTING] [--seed SEED] [--n N] [--save-path SAVE_PATH] Diffusion
-Image Editing arguments options: -h, --help show this help message and exit --
-remove-prompt REMOVE_PROMPT What you want to remove from the image --add-prompt
-ADD_PROMPT What you want to add to the image --image IMAGE Path to the image to
-edit --image-link IMAGE_LINK Link to the image to edit --device {cpu,cuda,mps}
---vae-model VAE_MODEL Model name. E.g. stabilityai/sd-vae-ft-ema --tokenizer
-TOKENIZER Tokenizer to tokenize the text. E.g. openai/clip-vit-large-patch14 --
-text-encoder TEXT_ENCODER Text encoder to encode the text. E.g. openai/clip-
-vit-large-patch14 --unet UNET UNet model for generating the latents. E.g.
-CompVis/stable-diffusion-v1-4 --scheduler SCHEDULER Noise scheduler. E.g.
-LMSDiscreteScheduler --scheduler-start SCHEDULER_START Scheduler start value --
-scheduler-end SCHEDULER_END Scheduler end value --num-train-timesteps
-NUM_TRAIN_TIMESTEPS Number of training timesteps --beta-schedule BETA_SCHEDULE
-Beta schedule --inpainting INPAINTING Inpainting model. E.g. runwayml/stable-
-diffusion-inpainting --seed SEED Random seed --num-samples N Number of
-diffusion steps to generate the mask --save-path SAVE_PATH Path to save the
-result. Default is /result.png ```
+You can install the package in different ways, depending on your needs.
+Optional step (recommended) Create a virtual environment, to avoid conflicts
+with other packages. Here are some alternatives: - with `venv`: ```bash python
+-m venv venv source venv/bin/activate ``` - with `poetry`: ```bash poetry shell
+``` - with `conda`: ```bash conda create -n diff-edit python=3.10 conda
+activate diff-edit ``` Install the package from PyPi: ```bash pip install diff-
+edit ``` Alternative ways Install the package from source: ```bash poetry
+install ``` Install the package in editable mode, suggested for further
+development: ```bash pip install -e . ``` ## Usage For a fast evaluation use
+the script _i_m_a_g_e___e_d_i_t_._p_y: ```bash python image_edit.py --input_image --
+output_image --prompt ``` An example of usage is the following (resulting in
+_t_h_i_s image): ```bash python image_edit.py --remove-prompt "lion" --add-prompt
+"dog" --image-link "https://github.com/Gennaro-Farina/DiffEdit/blob/main/
+static/ai_gen_lion.jpeg" --num-samples 10 ``` You can further customize the
+process by tuning the parameters of the script. Here is the full list of
+parameters that you can tune: ```bash python image_edit.py --help usage:
+image_edit.py [-h] [--remove-prompt REMOVE_PROMPT] [--add-prompt ADD_PROMPT] [-
+-image IMAGE] [--image-link IMAGE_LINK] [--device {cpu,cuda,mps}] [--vae-model
+VAE_MODEL] [--tokenizer TOKENIZER] [--text-encoder TEXT_ENCODER] [--unet UNET]
+[--scheduler SCHEDULER] [--scheduler-start SCHEDULER_START] [--scheduler-end
+SCHEDULER_END] [--num-train-timesteps NUM_TRAIN_TIMESTEPS] [--beta-schedule
+BETA_SCHEDULE] [--inpainting INPAINTING] [--seed SEED] [--n N] [--save-path
+SAVE_PATH] Diffusion Image Editing arguments options: -h, --help show this help
+message and exit --remove-prompt REMOVE_PROMPT What you want to remove from the
+image --add-prompt ADD_PROMPT What you want to add to the image --image IMAGE
+Path to the image to edit --image-link IMAGE_LINK Link to the image to edit --
+device {cpu,cuda,mps} --vae-model VAE_MODEL Model name. E.g. stabilityai/sd-
+vae-ft-ema --tokenizer TOKENIZER Tokenizer to tokenize the text. E.g. openai/
+clip-vit-large-patch14 --text-encoder TEXT_ENCODER Text encoder to encode the
+text. E.g. openai/clip-vit-large-patch14 --unet UNET UNet model for generating
+the latents. E.g. CompVis/stable-diffusion-v1-4 --scheduler SCHEDULER Noise
+scheduler. E.g. LMSDiscreteScheduler --scheduler-start SCHEDULER_START
+Scheduler start value --scheduler-end SCHEDULER_END Scheduler end value --num-
+train-timesteps NUM_TRAIN_TIMESTEPS Number of training timesteps --beta-
+schedule BETA_SCHEDULE Beta schedule --inpainting INPAINTING Inpainting model.
+E.g. runwayml/stable-diffusion-inpainting --seed SEED Random seed --num-samples
+N Number of diffusion steps to generate the mask --save-path SAVE_PATH Path to
+save the result. Default is /result.png ```
```

### Comparing `diffedit-0.0.2rc8/pyproject.toml` & `diffedit-0.0.2rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "DiffEdit"
 # version_pattern = "MAJOR.MINOR.PATCH"
-version = "0.0.2rc8"
+version = "0.0.2rc9"
 description = "An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file."
 authors = ["Gennaro Farina"]
 readme = "README.md"
 packages = [
     { include = "diff_edit", from = "src" },
 ]
 license = "Apache-2.0"
```

### Comparing `diffedit-0.0.2rc8/src/diff_edit/model/diff_edit_model.py` & `diffedit-0.0.2rc9/src/diff_edit/model/diff_edit_model.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/model/image_processing.py` & `diffedit-0.0.2rc9/src/diff_edit/model/image_processing.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/model/mask_generation.py` & `diffedit-0.0.2rc9/src/diff_edit/model/mask_generation.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/model/mask_inpainting.py` & `diffedit-0.0.2rc9/src/diff_edit/model/mask_inpainting.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/model/model_composer.py` & `diffedit-0.0.2rc9/src/diff_edit/model/model_composer.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/scripts/image_edit.py` & `diffedit-0.0.2rc9/src/diff_edit/scripts/image_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,23 @@
  As all the diffusion processes, this also is influence by the seed. Given a mask, you'll get different results by
  changing the seed.
 """
 import argparse
 import torch
 import os
 
+from transformers.utils.hub import move_cache
 from fastdownload import FastDownload
 from diffusers import LMSDiscreteScheduler
 
 from diff_edit.model.model_composer import ModelComposer
 
 os.environ['CURL_CA_BUNDLE'] = ''
 
-
+move_cache()
 def parse_args():
     # Create the parser
     parser = argparse.ArgumentParser(description="Diffusion Image Editing arguments")
 
     parser.add_argument(
         "--remove-prompt",
         required=False,
```

### Comparing `diffedit-0.0.2rc8/src/diff_edit/scripts/mask.png` & `diffedit-0.0.2rc9/src/diff_edit/scripts/mask.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/src/diff_edit/scripts/result.png` & `diffedit-0.0.2rc9/src/diff_edit/scripts/result.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc8/PKG-INFO` & `diffedit-0.0.2rc9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiffEdit
-Version: 0.0.2rc8
+Version: 0.0.2rc9
 Summary: An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file.
 License: Apache-2.0
 Author: Gennaro Farina
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -49,40 +49,89 @@
 <table>
 <head>
 <th> Prompt: <i>remove</i> ⟶ <i>add</i>)</th><th>Original image</th> <th>Mask</th> <th>Edited</th>
 </head>
 <body>
 <tr>
 <td>"lion" ⟶ "dog"</td>
-<td><img src="static/ai_gen_lion.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_lion_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_lion_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_lion.jpeg" width="256" height="256" alt="An AI generated lion"></td>
+<td><img src="static/ai_gen_lion_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the 'lion'"></td>
+<td><img src="static/ai_gen_lion_result.png" width="256" height="256"
+         alt="The edited image with the 'dog' instead of the 'lion'"></td>
 </tr>
 <tr>
 <td>"house" ⟶ "3-floor hotel"</td>
-<td><img src="static/ai_gen_house.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_house_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_house_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_house.jpeg" width="256" height="256" alt="An AI generated house"></td>
+<td><img src="static/ai_gen_house_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the 'house'"></td>
+<td><img src="static/ai_gen_house_result.png" width="256" height="256"
+         alt="The edited image with the '3-floor hotel' instead of the 'house'"></td>
 </tr>
 <tr>
 <td>"an F1 race" ⟶ "a motogp race"</td>
-<td><img src="static/ai_gen_f1.jpeg" width="256" height="256"></td>
-<td><img src="static/ai_gen_f1_mask.png" width="256" height="256"></td>
-<td><img src="static/ai_gen_f1_result.png" width="256" height="256"></td>
+<td><img src="static/ai_gen_f1.jpeg" width="256" height="256" alt="An AI generated image of an F1 competition"></td>
+<td><img src="static/ai_gen_f1_mask.png" width="256" height="256" 
+         alt="The mask of the image region containing the F1 cars"></td>
+<td><img src="static/ai_gen_f1_result.png" width="256" height="256"
+         alt="The edited image with the 'motogp' instead of the 'F1'"></td>
 </tr>
 </body>
 </table>
 
 All the previous masks was generated with: `num-samples = 10`
 
 ## Installation
 
+You can install the package in different ways, depending on your needs.
+
+
+
+<details>
+  <summary> Optional step (recommended)</summary>
+  
+Create a virtual environment, to avoid conflicts with other packages. Here are some alternatives:
+
+- with `venv`:
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+
+- with `poetry`:
+```bash
+poetry shell
+```
+
+- with `conda`:
+```bash
+conda create -n diff-edit python=3.10
+conda activate diff-edit
+```
+
+</details>
+
+
+Install the package from PyPi:
+```bash
+pip install diff-edit
+```
+<details>
+    <summary> Alternative ways</summary>
+
+Install the package from source:
+```bash
+poetry install
+```
+
+Install the package in editable mode, suggested for further development:
 ```bash
 pip install -e .
 ```
+</details>
 
 ## Usage
 
 For a fast evaluation use the script <a href="https://github.com/Gennaro-Farina/DiffEdit/blob/main/src/diff_edit/examples/image_edit.py">image_edit.py</a>:
 
 ```bash
 python image_edit.py --input_image <path_to_image> --output_image <path_to_output_image> --prompt <prompt>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc8 Summary: An
+Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc9 Summary: An
 implementation of the DiffEdit algorithm for prompt-based mask creation and
 inpating. For more information, see the Readme file. License: Apache-2.0
 Author: Gennaro Farina Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev Provides-Extra: test Requires-Dist: accelerate (==0.26.1)
@@ -25,46 +25,58 @@
 badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/
 build_and_test.yml) An unofficial implementation of _D_i_f_f_E_d_i_t based on _ð__¤_
 _H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage the diffusion
 process to automatically extract a mask from an image given a prompt. The mask
 is then used to inpaint the image with the new content. To get a clearer
 overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b notebook. ##
 Results
-"lion" â¶   [static/           [static/               [static/
-"dog"        ai_gen_lion.jpeg]  ai_gen_lion_mask.png]  ai_gen_lion_result.png]
-"house" â¶  [static/           [static/               [static/
-"3-floor     ai_gen_house.jpeg] ai_gen_house_mask.png] ai_gen_house_result.png]
-hotel"
-"an F1 race" [static/           [static/               [static/
-â¶ "a       ai_gen_f1.jpeg]    ai_gen_f1_mask.png]    ai_gen_f1_result.png]
-motogp race"
+                                      [The mask of the  [The edited image with
+"lion" â¶ "dog"     [An AI generated image region      the 'dog' instead of
+                     lion]            containing the    the 'lion']
+                                      'lion']
+                                      [The mask of the  [The edited image with
+"house" â¶ "3-floor [An AI generated image region      the '3-floor hotel'
+hotel"               house]           containing the    instead of the
+                                      'house']          'house']
+                     [An AI generated [The mask of the  [The edited image with
+"an F1 race" â¶ "a  image of an F1   image region      the 'motogp' instead
+motogp race"         competition]     containing the F1 of the 'F1']
+                                      cars]
 All the previous masks was generated with: `num-samples = 10` ## Installation
-```bash pip install -e . ``` ## Usage For a fast evaluation use the script
-_i_m_a_g_e___e_d_i_t_._p_y: ```bash python image_edit.py --input_image --output_image --
-prompt ``` An example of usage is the following (resulting in _t_h_i_s image):
-```bash python image_edit.py --remove-prompt "lion" --add-prompt "dog" --image-
-link "https://github.com/Gennaro-Farina/DiffEdit/blob/main/static/
-ai_gen_lion.jpeg" --num-samples 10 ``` You can further customize the process by
-tuning the parameters of the script. Here is the full list of parameters that
-you can tune: ```bash python image_edit.py --help usage: image_edit.py [-h] [--
-remove-prompt REMOVE_PROMPT] [--add-prompt ADD_PROMPT] [--image IMAGE] [--
-image-link IMAGE_LINK] [--device {cpu,cuda,mps}] [--vae-model VAE_MODEL] [--
-tokenizer TOKENIZER] [--text-encoder TEXT_ENCODER] [--unet UNET] [--scheduler
-SCHEDULER] [--scheduler-start SCHEDULER_START] [--scheduler-end SCHEDULER_END]
-[--num-train-timesteps NUM_TRAIN_TIMESTEPS] [--beta-schedule BETA_SCHEDULE] [--
-inpainting INPAINTING] [--seed SEED] [--n N] [--save-path SAVE_PATH] Diffusion
-Image Editing arguments options: -h, --help show this help message and exit --
-remove-prompt REMOVE_PROMPT What you want to remove from the image --add-prompt
-ADD_PROMPT What you want to add to the image --image IMAGE Path to the image to
-edit --image-link IMAGE_LINK Link to the image to edit --device {cpu,cuda,mps}
---vae-model VAE_MODEL Model name. E.g. stabilityai/sd-vae-ft-ema --tokenizer
-TOKENIZER Tokenizer to tokenize the text. E.g. openai/clip-vit-large-patch14 --
-text-encoder TEXT_ENCODER Text encoder to encode the text. E.g. openai/clip-
-vit-large-patch14 --unet UNET UNet model for generating the latents. E.g.
-CompVis/stable-diffusion-v1-4 --scheduler SCHEDULER Noise scheduler. E.g.
-LMSDiscreteScheduler --scheduler-start SCHEDULER_START Scheduler start value --
-scheduler-end SCHEDULER_END Scheduler end value --num-train-timesteps
-NUM_TRAIN_TIMESTEPS Number of training timesteps --beta-schedule BETA_SCHEDULE
-Beta schedule --inpainting INPAINTING Inpainting model. E.g. runwayml/stable-
-diffusion-inpainting --seed SEED Random seed --num-samples N Number of
-diffusion steps to generate the mask --save-path SAVE_PATH Path to save the
-result. Default is /result.png ```
+You can install the package in different ways, depending on your needs.
+Optional step (recommended) Create a virtual environment, to avoid conflicts
+with other packages. Here are some alternatives: - with `venv`: ```bash python
+-m venv venv source venv/bin/activate ``` - with `poetry`: ```bash poetry shell
+``` - with `conda`: ```bash conda create -n diff-edit python=3.10 conda
+activate diff-edit ``` Install the package from PyPi: ```bash pip install diff-
+edit ``` Alternative ways Install the package from source: ```bash poetry
+install ``` Install the package in editable mode, suggested for further
+development: ```bash pip install -e . ``` ## Usage For a fast evaluation use
+the script _i_m_a_g_e___e_d_i_t_._p_y: ```bash python image_edit.py --input_image --
+output_image --prompt ``` An example of usage is the following (resulting in
+_t_h_i_s image): ```bash python image_edit.py --remove-prompt "lion" --add-prompt
+"dog" --image-link "https://github.com/Gennaro-Farina/DiffEdit/blob/main/
+static/ai_gen_lion.jpeg" --num-samples 10 ``` You can further customize the
+process by tuning the parameters of the script. Here is the full list of
+parameters that you can tune: ```bash python image_edit.py --help usage:
+image_edit.py [-h] [--remove-prompt REMOVE_PROMPT] [--add-prompt ADD_PROMPT] [-
+-image IMAGE] [--image-link IMAGE_LINK] [--device {cpu,cuda,mps}] [--vae-model
+VAE_MODEL] [--tokenizer TOKENIZER] [--text-encoder TEXT_ENCODER] [--unet UNET]
+[--scheduler SCHEDULER] [--scheduler-start SCHEDULER_START] [--scheduler-end
+SCHEDULER_END] [--num-train-timesteps NUM_TRAIN_TIMESTEPS] [--beta-schedule
+BETA_SCHEDULE] [--inpainting INPAINTING] [--seed SEED] [--n N] [--save-path
+SAVE_PATH] Diffusion Image Editing arguments options: -h, --help show this help
+message and exit --remove-prompt REMOVE_PROMPT What you want to remove from the
+image --add-prompt ADD_PROMPT What you want to add to the image --image IMAGE
+Path to the image to edit --image-link IMAGE_LINK Link to the image to edit --
+device {cpu,cuda,mps} --vae-model VAE_MODEL Model name. E.g. stabilityai/sd-
+vae-ft-ema --tokenizer TOKENIZER Tokenizer to tokenize the text. E.g. openai/
+clip-vit-large-patch14 --text-encoder TEXT_ENCODER Text encoder to encode the
+text. E.g. openai/clip-vit-large-patch14 --unet UNET UNet model for generating
+the latents. E.g. CompVis/stable-diffusion-v1-4 --scheduler SCHEDULER Noise
+scheduler. E.g. LMSDiscreteScheduler --scheduler-start SCHEDULER_START
+Scheduler start value --scheduler-end SCHEDULER_END Scheduler end value --num-
+train-timesteps NUM_TRAIN_TIMESTEPS Number of training timesteps --beta-
+schedule BETA_SCHEDULE Beta schedule --inpainting INPAINTING Inpainting model.
+E.g. runwayml/stable-diffusion-inpainting --seed SEED Random seed --num-samples
+N Number of diffusion steps to generate the mask --save-path SAVE_PATH Path to
+save the result. Default is /result.png ```
```

