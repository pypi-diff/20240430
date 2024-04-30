# Comparing `tmp/audioseal-0.1.2.tar.gz` & `tmp/audioseal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioseal-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "audioseal-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `audioseal-0.1.2.tar` & `audioseal-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      295 2024-02-04 13:47:46.756335 audioseal-0.1.2/.github/pull_request_template.md
--rw-r--r--   0        0        0     2882 2024-02-29 12:27:08.569572 audioseal-0.1.2/.github/workflows/lint_and_test.yaml
--rw-r--r--   0        0        0     2511 2024-02-04 13:47:46.763895 audioseal-0.1.2/.gitignore
--rw-r--r--   0        0        0      811 2024-02-04 13:47:46.766289 audioseal-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      854 2024-02-29 13:09:05.303532 audioseal-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     3536 2024-02-04 13:47:46.771104 audioseal-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2275 2024-02-04 13:47:46.773177 audioseal-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1088 2024-02-04 13:47:46.775534 audioseal-0.1.2/LICENSE
--rw-r--r--   0        0        0    19333 2024-02-04 13:47:46.779190 audioseal-0.1.2/LICENSE_weights
--rw-r--r--   0        0        0     6932 2024-02-29 13:09:05.307150 audioseal-0.1.2/README.md
--rw-r--r--   0        0        0  2490680 2024-02-29 13:09:05.332059 audioseal-0.1.2/examples/Getting_started.ipynb
--rw-r--r--   0        0        0     9659 2024-02-29 13:09:05.334899 audioseal-0.1.2/examples/attacks.py
--rw-r--r--   0        0        0    14199 2024-02-29 13:09:05.338620 audioseal-0.1.2/examples/colab.ipynb
--rwxr-xr-x   0        0        0     1299 2024-02-04 13:47:46.814892 audioseal-0.1.2/examples/notebook.py
--rw-r--r--   0        0        0     1896 2024-02-29 12:27:08.608306 audioseal-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      129 2024-02-04 13:47:46.818914 audioseal-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0       45 2024-02-29 12:31:21.305987 audioseal-0.1.2/requirements.txt
--rw-r--r--   0        0        0      552 2024-02-29 13:09:05.341966 audioseal-0.1.2/src/audioseal/__init__.py
--rw-r--r--   0        0        0     2765 2024-02-04 13:52:00.851132 audioseal-0.1.2/src/audioseal/builder.py
--rw-r--r--   0        0        0      594 2024-02-04 13:52:00.854274 audioseal-0.1.2/src/audioseal/cards/audioseal_detector_16bits.yaml
--rw-r--r--   0        0        0      838 2024-02-04 13:52:00.856484 audioseal-0.1.2/src/audioseal/cards/audioseal_wm_16bits.yaml
--rw-r--r--   0        0        0      198 2024-02-04 13:52:00.860114 audioseal-0.1.2/src/audioseal/libs/__init__.py
--rw-r--r--   0        0        0      198 2024-02-04 13:52:00.864083 audioseal-0.1.2/src/audioseal/libs/audiocraft/__init__.py
--rw-r--r--   0        0        0      277 2024-02-04 13:52:00.868040 audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/__init__.py
--rw-r--r--   0        0        0    11184 2024-02-04 13:52:00.871481 audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/conv.py
--rw-r--r--   0        0        0      823 2024-02-04 13:52:00.873863 audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/lstm.py
--rw-r--r--   0        0        0    16316 2024-02-29 12:27:08.612084 audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/seanet.py
--rw-r--r--   0        0        0     6261 2024-02-04 13:52:00.879766 audioseal-0.1.2/src/audioseal/loader.py
--rw-r--r--   0        0        0     8457 2024-02-29 13:09:05.345471 audioseal-0.1.2/src/audioseal/models.py
--rw-r--r--   0        0        0        0 2024-02-29 12:27:08.617043 audioseal-0.1.2/src/audioseal/py.typed
--rw-r--r--   0        0        0     1618 2024-02-29 13:09:05.349715 audioseal-0.1.2/tests/test_models.py
--rw-r--r--   0        0        0     7858 1970-01-01 00:00:00.000000 audioseal-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      295 2024-03-16 13:42:50.529051 audioseal-0.1.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2926 2024-04-30 17:24:39.171504 audioseal-0.1.3/.github/workflows/lint_and_test.yaml
+-rw-r--r--   0        0        0     2542 2024-04-30 17:24:39.172104 audioseal-0.1.3/.gitignore
+-rw-r--r--   0        0        0      775 2024-04-30 17:24:39.172853 audioseal-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1182 2024-04-30 17:24:39.173716 audioseal-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3536 2024-03-16 13:42:50.531180 audioseal-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2275 2024-03-16 13:42:50.531610 audioseal-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1088 2024-03-16 13:42:50.532054 audioseal-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7247 2024-04-30 15:32:08.956067 audioseal-0.1.3/README.md
+-rw-r--r--   0        0        0  2490680 2024-03-16 13:42:50.558414 audioseal-0.1.3/examples/Getting_started.ipynb
+-rw-r--r--   0        0        0    20909 2024-04-30 15:27:59.632127 audioseal-0.1.3/examples/attack_benchmarking_example.ipynb
+-rw-r--r--   0        0        0    10612 2024-04-30 17:24:39.174960 audioseal-0.1.3/examples/attacks.py
+-rw-r--r--   0        0        0    14199 2024-03-16 13:42:50.559658 audioseal-0.1.3/examples/colab.ipynb
+-rwxr-xr-x   0        0        0     1299 2024-03-16 13:42:50.559873 audioseal-0.1.3/examples/notebook.py
+-rw-r--r--   0        0        0     1896 2024-03-16 13:42:50.560091 audioseal-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-30 17:24:39.175652 audioseal-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0       45 2024-04-30 16:26:58.776133 audioseal-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      552 2024-04-30 17:24:39.176516 audioseal-0.1.3/src/audioseal/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-30 17:24:39.177682 audioseal-0.1.3/src/audioseal/builder.py
+-rw-r--r--   0        0        0      604 2024-04-30 17:24:39.178971 audioseal-0.1.3/src/audioseal/cards/audioseal_detector_16bits.yaml
+-rw-r--r--   0        0        0      848 2024-04-30 17:24:39.179965 audioseal-0.1.3/src/audioseal/cards/audioseal_wm_16bits.yaml
+-rw-r--r--   0        0        0      198 2024-03-16 13:42:50.562260 audioseal-0.1.3/src/audioseal/libs/__init__.py
+-rw-r--r--   0        0        0      198 2024-03-16 13:42:50.562610 audioseal-0.1.3/src/audioseal/libs/audiocraft/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-16 13:42:50.562987 audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/__init__.py
+-rw-r--r--   0        0        0    11183 2024-04-30 17:24:39.181086 audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/conv.py
+-rw-r--r--   0        0        0      823 2024-03-16 13:42:50.563489 audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/lstm.py
+-rw-r--r--   0        0        0    16317 2024-04-30 17:24:39.182559 audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/seanet.py
+-rw-r--r--   0        0        0     7201 2024-04-30 17:24:39.183404 audioseal-0.1.3/src/audioseal/loader.py
+-rw-r--r--   0        0        0     8517 2024-04-30 17:24:39.184303 audioseal-0.1.3/src/audioseal/models.py
+-rw-r--r--   0        0        0        0 2024-03-16 13:42:50.564406 audioseal-0.1.3/src/audioseal/py.typed
+-rw-r--r--   0        0        0     2023 2024-04-30 17:24:39.185144 audioseal-0.1.3/tests/test_models.py
+-rw-r--r--   0        0        0     8173 1970-01-01 00:00:00.000000 audioseal-0.1.3/PKG-INFO
```

### Comparing `audioseal-0.1.2/.github/workflows/lint_and_test.yaml` & `audioseal-0.1.3/.github/workflows/lint_and_test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         run: |
           sudo apt-get install libsndfile1
           python -m pip install --upgrade pip
           # We also test that pyproject.toml and requirements*.txt are synced
           pip install -r requirements-dev.txt
           pip install -e .
       - name: pytest_unit
-        run: pytest -s -v tests/
+        run: pytest -s -v tests/test_models.py
 
   unit_test_old_torch:
     runs-on: ubuntu-latest
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix:
@@ -78,11 +78,11 @@
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Install dependencies
         run: |
           sudo apt-get install libsndfile1
           python -m pip install --upgrade pip
-          pip install torch==1.13.0 torchaudio==0.13.0 func_argparse soundfile pytest omegaconf numpy julius
+          pip install torch==1.13.0 torchaudio==0.13.0 func_argparse soundfile pytest omegaconf numpy julius huggingface_hub
           pip install --no-deps -e .
       - name: pytest_unit
-        run: pytest -s -v tests/
+        run: pytest -s -v tests/test_models.py
```

### Comparing `audioseal-0.1.2/.gitignore` & `audioseal-0.1.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -98,9 +98,12 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
+# Visual Studio Code
+.vscode/
+
 # local training outputs
 outputs/*
```

### Comparing `audioseal-0.1.2/.pre-commit-config.yaml` & `audioseal-0.1.3/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,17 @@
       - id: check-ast
       - id: check-merge-conflict
       - id: check-added-large-files
         args: ["--maxkb=2000"]
       - id: end-of-file-fixer
 
   - repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.4.2
     hooks:
       - id: black
-        language_version: python3.8
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         exclude: README.md
```

### Comparing `audioseal-0.1.2/CODE_OF_CONDUCT.md` & `audioseal-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/CONTRIBUTING.md` & `audioseal-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/LICENSE` & `audioseal-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/README.md` & `audioseal-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray"></a>
 
 Inference code for AudioSeal, a method for speech localized watermarking, with state-of-the-art robustness and detector speed (training code coming soon).
 More details can be found in the [paper](https://arxiv.org/abs/2401.17264).
 
 [[`arXiv`](https://arxiv.org/abs/2401.17264)]
-[[`Colab notebook`](https://colab.research.google.com/github/facebookresearch/audioseal/blob/master/examples/colab.ipynb)]
+[[`Colab notebook`](https://colab.research.google.com/github/facebookresearch/audioseal/blob/master/examples/colab.ipynb)][[🤗`Hugging Face`](https://huggingface.co/facebook/audioseal)]
 
 ![fig](https://github.com/facebookresearch/audioseal/assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2)
 
+# Updates:
+
+- 2024-04-02: We have updated our license to full MIT license (including the license for the model weights) ! Now you can use AudioSeal in commercial application too !
+- 2024-02-29: AudioSeal 0.1.2 is out, with more bug fixes for resampled audios and updated notebooks
+
 # Abtract
 
 We introduce AudioSeal, a method for speech localized watermarking, with state-of-the-art robustness and detector speed. It jointly trains a generator that embeds a watermark in the audio, and a detector that detects the watermarked fragments in longer audios, even in the presence of editing.
 Audioseal achieves state-of-the-art detection performance of both natural and synthetic speech at the sample level (1/16k second resolution), it generates limited alteration of signal quality and is robust to many types of audio editing. 
 Audioseal is designed with a fast, single-pass detector, that significantly surpasses existing models in speed — achieving detection up to two orders of magnitude faster, making it ideal for large-scale and real-time applications.
 
 # :mate: Installation
@@ -31,15 +36,15 @@
 git clone https://github.com/facebookresearch/audioseal
 cd audioseal
 pip install -e .
 ```
 
 # :gear: Models
 
-We provide the checkpoints for the following models:
+You can find all the model checkpoints on the [Hugging Face Hub](https://huggingface.co/facebook/audioseal). We provide the checkpoints for the following models:
 
 - [AudioSeal Generator](src/audioseal/cards/audioseal_wm_16bits.yaml).
   It takes as input an audio signal (as a waveform), and outputs a watermark of the same size as the input, that can be added to the input to watermark it.
   Optionally, it can also take as input a secret message of 16-bits that will be encoded in the watermark.
 - [AudioSeal Detector](src/audioseal/cards/audioseal_detector_16bits.yaml).
   It takes as input an audio signal (as a waveform), and outputs a probability that the input contains a watermark at each sample of the audio (every 1/16k s).
   Optionally, it may also output the secret message encoded in the watermark.
@@ -112,15 +117,14 @@
 
 - If you use torchaudio to handle your audios and encounter the error `Couldn't find appropriate backend to handle uri ...`, this is due to newer version of 
 torchaudio does not handle the default backend well. Either downgrade your torchaudio to `2.0.1` or earlier, or install `soundfile` as your audio backend.
 
 # License
 
 - The code in this repository is released under the MIT license as found in the [LICENSE file](LICENSE).
-- The models weights in this repository are released under the CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights).
 
 # Maintainers:
 - [Tuan Tran](https://github.com/antoine-tran)
 - [Hady Elsahar](https://github.com/hadyelsahar)
 - [Pierre Fernandez](https://github.com/pierrefdz)
 - [Robin San Roman](https://github.com/robinsrm)
```

#### html2text {}

```diff
@@ -1,54 +1,59 @@
 # :loud_sound: AudioSeal: Proactive Localized Watermarking _[_P_y_t_h_o_n_]_[_C_o_d_e_ _s_t_y_l_e_:
 _b_l_a_c_k_]Inference code for AudioSeal, a method for speech localized watermarking,
 with state-of-the-art robustness and detector speed (training code coming
 soon). More details can be found in the [paper](https://arxiv.org/abs/
 2401.17264). [[`arXiv`](https://arxiv.org/abs/2401.17264)] [[`Colab notebook`]
 (https://colab.research.google.com/github/facebookresearch/audioseal/blob/
-master/examples/colab.ipynb)] ![fig](https://github.com/facebookresearch/
-audioseal/assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2) # Abtract We
-introduce AudioSeal, a method for speech localized watermarking, with state-of-
-the-art robustness and detector speed. It jointly trains a generator that
-embeds a watermark in the audio, and a detector that detects the watermarked
-fragments in longer audios, even in the presence of editing. Audioseal achieves
-state-of-the-art detection performance of both natural and synthetic speech at
-the sample level (1/16k second resolution), it generates limited alteration of
-signal quality and is robust to many types of audio editing. Audioseal is
-designed with a fast, single-pass detector, that significantly surpasses
-existing models in speed â achieving detection up to two orders of magnitude
-faster, making it ideal for large-scale and real-time applications. # :mate:
-Installation AudioSeal requires Python >=3.8, Pytorch >= 1.13.0, [omegaconf]
-(https://omegaconf.readthedocs.io/), [julius](https://pypi.org/project/julius/
-), and numpy. To install from PyPI: ``` pip install audioseal ``` To install
-from source: Clone this repo and install in editable mode: ``` git clone https:
-//github.com/facebookresearch/audioseal cd audioseal pip install -e . ``` # :
-gear: Models We provide the checkpoints for the following models: - [AudioSeal
-Generator](src/audioseal/cards/audioseal_wm_16bits.yaml). It takes as input an
-audio signal (as a waveform), and outputs a watermark of the same size as the
-input, that can be added to the input to watermark it. Optionally, it can also
-take as input a secret message of 16-bits that will be encoded in the
-watermark. - [AudioSeal Detector](src/audioseal/cards/
-audioseal_detector_16bits.yaml). It takes as input an audio signal (as a
-waveform), and outputs a probability that the input contains a watermark at
-each sample of the audio (every 1/16k s). Optionally, it may also output the
-secret message encoded in the watermark. Note that the message is optional and
-has no influence on the detection output. It may be used to identify a model
-version for instance (up to $2**16=65536$ possible choices). **Note**: We are
-working to release the training code for anyone wants to build their own
-watermarker. Stay tuned ! # :abacus: Usage Audioseal provides a simple API to
-watermark and detect the watermarks from an audio sample. Example usage:
-```python from audioseal import AudioSeal # model name corresponds to the YAML
-card file name found in audioseal/cards model = AudioSeal.load_generator
-("audioseal_wm_16bits") # Other way is to load directly from the checkpoint #
-model = Watermarker.from_pretrained(checkpoint_path, device = wav.device) # a
-torch tensor of shape (batch, channels, samples) and a sample rate # It is
-important to process the audio to the same sample rate as the model # expectes.
-In our case, we support 16khz audio wav, sr = ..., 16000 watermark =
-model.get_watermark(wav, sr) # Optional: you can add a 16-bit message to embed
-in the watermark # msg = torch.randint(0, 2, (wav.shape(0),
+master/examples/colab.ipynb)][[ð¤`Hugging Face`](https://huggingface.co/
+facebook/audioseal)] ![fig](https://github.com/facebookresearch/audioseal/
+assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2) # Updates: - 2024-04-02:
+We have updated our license to full MIT license (including the license for the
+model weights) ! Now you can use AudioSeal in commercial application too ! -
+2024-02-29: AudioSeal 0.1.2 is out, with more bug fixes for resampled audios
+and updated notebooks # Abtract We introduce AudioSeal, a method for speech
+localized watermarking, with state-of-the-art robustness and detector speed. It
+jointly trains a generator that embeds a watermark in the audio, and a detector
+that detects the watermarked fragments in longer audios, even in the presence
+of editing. Audioseal achieves state-of-the-art detection performance of both
+natural and synthetic speech at the sample level (1/16k second resolution), it
+generates limited alteration of signal quality and is robust to many types of
+audio editing. Audioseal is designed with a fast, single-pass detector, that
+significantly surpasses existing models in speed â achieving detection up to
+two orders of magnitude faster, making it ideal for large-scale and real-time
+applications. # :mate: Installation AudioSeal requires Python >=3.8, Pytorch >=
+1.13.0, [omegaconf](https://omegaconf.readthedocs.io/), [julius](https://
+pypi.org/project/julius/), and numpy. To install from PyPI: ``` pip install
+audioseal ``` To install from source: Clone this repo and install in editable
+mode: ``` git clone https://github.com/facebookresearch/audioseal cd audioseal
+pip install -e . ``` # :gear: Models You can find all the model checkpoints on
+the [Hugging Face Hub](https://huggingface.co/facebook/audioseal). We provide
+the checkpoints for the following models: - [AudioSeal Generator](src/
+audioseal/cards/audioseal_wm_16bits.yaml). It takes as input an audio signal
+(as a waveform), and outputs a watermark of the same size as the input, that
+can be added to the input to watermark it. Optionally, it can also take as
+input a secret message of 16-bits that will be encoded in the watermark. -
+[AudioSeal Detector](src/audioseal/cards/audioseal_detector_16bits.yaml). It
+takes as input an audio signal (as a waveform), and outputs a probability that
+the input contains a watermark at each sample of the audio (every 1/16k s).
+Optionally, it may also output the secret message encoded in the watermark.
+Note that the message is optional and has no influence on the detection output.
+It may be used to identify a model version for instance (up to $2**16=65536$
+possible choices). **Note**: We are working to release the training code for
+anyone wants to build their own watermarker. Stay tuned ! # :abacus: Usage
+Audioseal provides a simple API to watermark and detect the watermarks from an
+audio sample. Example usage: ```python from audioseal import AudioSeal # model
+name corresponds to the YAML card file name found in audioseal/cards model =
+AudioSeal.load_generator("audioseal_wm_16bits") # Other way is to load directly
+from the checkpoint # model = Watermarker.from_pretrained(checkpoint_path,
+device = wav.device) # a torch tensor of shape (batch, channels, samples) and a
+sample rate # It is important to process the audio to the same sample rate as
+the model # expectes. In our case, we support 16khz audio wav, sr = ..., 16000
+watermark = model.get_watermark(wav, sr) # Optional: you can add a 16-bit
+message to embed in the watermark # msg = torch.randint(0, 2, (wav.shape(0),
 model.msg_processor.nbits), device=wav.device) # watermark =
 model.get_watermark(wav, message = msg) watermarked_audio = wav + watermark
 detector = AudioSeal.load_detector("audioseal_detector_16bits") # To detect the
 messages in the high-level. result, message = detector.detect_watermark
 (watermarked_audio, sr) print(result) # result is a float number indicating the
 probability of the audio being watermarked, print(message) # message is a
 binary vector of 16 bits # To detect the messages in the low-level. result,
@@ -70,17 +75,15 @@
 which is not compatible in Windows. Try to invalidate the cache by removing the
 files in `C:\Users\\.cache\audioseal` and re-run again. - If you use torchaudio
 to handle your audios and encounter the error `Couldn't find appropriate
 backend to handle uri ...`, this is due to newer version of torchaudio does not
 handle the default backend well. Either downgrade your torchaudio to `2.0.1` or
 earlier, or install `soundfile` as your audio backend. # License - The code in
 this repository is released under the MIT license as found in the [LICENSE
-file](LICENSE). - The models weights in this repository are released under the
-CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights). #
-Maintainers: - [Tuan Tran](https://github.com/antoine-tran) - [Hady Elsahar]
-(https://github.com/hadyelsahar) - [Pierre Fernandez](https://github.com/
-pierrefdz) - [Robin San Roman](https://github.com/robinsrm) # Citation If you
-find this repository useful, please consider giving a star :star: and please
-cite as: ``` @article{sanroman2024proactive, title={Proactive Detection of
-Voice Cloning with Localized Watermarking}, author={San Roman, Robin and
-Fernandez, Pierre and Elsahar, Hady and DÂ´efossez, Alexandre and Furon, Teddy
-and Tran, Tuan}, journal={arXiv preprint}, year={2024} } ```
+file](LICENSE). # Maintainers: - [Tuan Tran](https://github.com/antoine-tran) -
+[Hady Elsahar](https://github.com/hadyelsahar) - [Pierre Fernandez](https://
+github.com/pierrefdz) - [Robin San Roman](https://github.com/robinsrm) #
+Citation If you find this repository useful, please consider giving a star :
+star: and please cite as: ``` @article{sanroman2024proactive, title={Proactive
+Detection of Voice Cloning with Localized Watermarking}, author={San Roman,
+Robin and Fernandez, Pierre and Elsahar, Hady and DÂ´efossez, Alexandre and
+Furon, Teddy and Tran, Tuan}, journal={arXiv preprint}, year={2024} } ```
```

### Comparing `audioseal-0.1.2/examples/Getting_started.ipynb` & `audioseal-0.1.3/examples/Getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/examples/attacks.py` & `audioseal-0.1.3/examples/attacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 
         n_samples = int(sample_rate * duration)
         impulse_response = torch.zeros(n_samples).type(tensor.type()).to(tensor.device)
 
         # Define a few reflections with decreasing amplitude
         impulse_response[0] = 1.0  # Direct sound
 
-        impulse_response[
-            int(sample_rate * duration) - 1
-        ] = volume  # First reflection after 100ms
+        impulse_response[int(sample_rate * duration) - 1] = (
+            volume  # First reflection after 100ms
+        )
 
         # Add batch and channel dimensions to the impulse response
         impulse_response = impulse_response.unsqueeze(0).unsqueeze(0)
 
         # Convolve the audio signal with the impulse response
         reverbed_signal = julius.fft_conv1d(tensor, impulse_response)
 
@@ -261,7 +261,31 @@
         return audio_effect_return(tensor=tensor * (1 - amount / 100), mask=mask)
 
     @staticmethod
     def identity(
         tensor: torch.Tensor, mask: tp.Optional[torch.Tensor] = None
     ) -> tp.Union[tp.Tuple[torch.Tensor, torch.Tensor], torch.Tensor]:
         return audio_effect_return(tensor=tensor, mask=mask)
+
+    @staticmethod
+    def shush(
+        tensor: torch.Tensor,
+        fraction: float = 0.001,
+        mask: tp.Optional[torch.Tensor] = None
+    ) -> tp.Union[tp.Tuple[torch.Tensor, torch.Tensor], torch.Tensor]:
+        """
+        Sets a specified chronological fraction of indices of the input tensor (audio signal) to 0.
+
+        Parameters:
+        - tensor (torch.Tensor): Input audio tensor. Assumes tensor shape is (batch_size, channels, time).
+        - fraction (float): Fraction of indices to be set to 0 (from the start of the tensor) (default: 0.001, i.e, 0.1%)
+
+        Returns:
+        - torch.Tensor: Transformed audio tensor.
+        """
+        time = tensor.size(-1)
+        shush_tensor = tensor.detach().clone()
+        
+        # Set the first `fraction*time` indices of the waveform to 0
+        shush_tensor[:, :, :int(fraction*time)] = 0.0
+                
+        return audio_effect_return(tensor=shush_tensor, mask=mask)
```

### Comparing `audioseal-0.1.2/examples/colab.ipynb` & `audioseal-0.1.3/examples/colab.ipynb`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/examples/notebook.py` & `audioseal-0.1.3/examples/notebook.py`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/pyproject.toml` & `audioseal-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/src/audioseal/__init__.py` & `audioseal-0.1.3/src/audioseal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 
 A Pytorch-based localized algorithm for proactive detection
 of the watermarkings in AI-generated audios, with very fast
 detector.
 
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 from audioseal import builder
 from audioseal.loader import AudioSeal
 from audioseal.models import AudioSealDetector, AudioSealWM, MsgProcessor
```

### Comparing `audioseal-0.1.2/src/audioseal/builder.py` & `audioseal-0.1.3/src/audioseal/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from dataclasses import asdict, dataclass, is_dataclass
+from typing import Any, Dict, List, Mapping, Optional
 
+from omegaconf import DictConfig, OmegaConf
 from torch import device, dtype
 from typing_extensions import TypeAlias
 
 from audioseal.libs import audiocraft
 from audioseal.models import AudioSealDetector, AudioSealWM, MsgProcessor
 
 Device: TypeAlias = device
@@ -67,40 +68,51 @@
 @dataclass
 class AudioSealDetectorConfig:
     nbits: int
     seanet: SEANetConfig
     detector: DetectorConfig
 
 
+def as_dict(obj: Any) -> Dict[str, Any]:
+    if isinstance(obj, dict):
+        return obj
+    if is_dataclass(obj):
+        return asdict(obj)
+    elif isinstance(obj, DictConfig):
+        return OmegaConf.to_container(obj)  # type: ignore
+    else:
+        raise NotImplementedError(f"Unsupported type for config: {type(obj)}")
+
+
 def create_generator(
     config: AudioSealWMConfig,
     *,
     device: Optional[Device] = None,
     dtype: Optional[DataType] = None,
 ) -> AudioSealWM:
     """Create a generator from hparams"""
 
     #  Currently the encoder hparams are the same as
     # SEANet, but this can be changed in the future.
-    encoder = audiocraft.modules.SEANetEncoder(**config.seanet)  # type: ignore[arg-type]
+    encoder = audiocraft.modules.SEANetEncoder(**as_dict(config.seanet))
     encoder = encoder.to(device=device, dtype=dtype)
 
-    decoder_config = {**config.seanet, **config.decoder}  # type: ignore
-    decoder = audiocraft.modules.SEANetDecoder(**decoder_config)  # type: ignore[arg-type]
+    decoder_config = {**as_dict(config.seanet), **as_dict(config.decoder)}
+    decoder = audiocraft.modules.SEANetDecoder(**as_dict(decoder_config))
     decoder = decoder.to(device=device, dtype=dtype)
 
     msgprocessor = MsgProcessor(nbits=config.nbits, hidden_size=config.seanet.dimension)
     msgprocessor = msgprocessor.to(device=device, dtype=dtype)
 
     return AudioSealWM(encoder=encoder, decoder=decoder, msg_processor=msgprocessor)
 
 
 def create_detector(
     config: AudioSealDetectorConfig,
     *,
     device: Optional[Device] = None,
     dtype: Optional[DataType] = None,
 ) -> AudioSealDetector:
-    detector_config = {**config.seanet, **config.detector}  # type: ignore
+    detector_config = {**as_dict(config.seanet), **as_dict(config.detector)}
     detector = AudioSealDetector(nbits=config.nbits, **detector_config)
     detector = detector.to(device=device, dtype=dtype)
     return detector
```

### Comparing `audioseal-0.1.2/src/audioseal/cards/audioseal_detector_16bits.yaml` & `audioseal-0.1.3/src/audioseal/cards/audioseal_detector_16bits.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @package __global__
 
 name: audioseal_detector_16bits
 model_type: seanet
-checkpoint: "https://dl.fbaipublicfiles.com/audioseal/6edcf62f/detector.pth"
+checkpoint: "https://huggingface.co/facebook/audioseal/resolve/main/detector_base.pth"
 nbits: 16
 seanet:
   activation: ELU
   activation_params:
     alpha: 1.0
   causal: false
   channels: 1
```

### Comparing `audioseal-0.1.2/src/audioseal/cards/audioseal_wm_16bits.yaml` & `audioseal-0.1.3/src/audioseal/cards/audioseal_wm_16bits.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 name: audioseal_wm_16bits
 model_type: seanet
-checkpoint: "https://dl.fbaipublicfiles.com/audioseal/6edcf62f/generator.pth"
+checkpoint: "https://huggingface.co/facebook/audioseal/resolve/main/generator_base.pth"
 nbits: 16
 seanet:
   activation: ELU
   activation_params:
     alpha: 1.0
   causal: false
   channels: 1
```

### Comparing `audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/conv.py` & `audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
-# 
+#
 # Vendor from https://github.com/facebookresearch/audiocraft
 
 import math
 import typing as tp
 import warnings
 
 import torch
```

### Comparing `audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/lstm.py` & `audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `audioseal-0.1.2/src/audioseal/libs/audiocraft/modules/seanet.py` & `audioseal-0.1.3/src/audioseal/libs/audiocraft/modules/seanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     def forward(self, x):
         orig_nframes = x.shape[-1]
         x = self.model(x)
         x = self.reverse_convolution(x)
         # make sure dim didn't change
         return x[:, :, :orig_nframes]
 
+
 class SEANetDecoder(nn.Module):
     """SEANet decoder.
 
     Args:
         channels (int): Audio channels.
         dimension (int): Intermediate representation dimension.
         n_filters (int): Base width for the model.
```

### Comparing `audioseal-0.1.2/src/audioseal/loader.py` & `audioseal-0.1.3/src/audioseal/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     cast,
 )
 from urllib.parse import urlparse  # noqa: F401
 
 import torch
 from omegaconf import DictConfig, OmegaConf
 
+import audioseal
 from audioseal.builder import (
     AudioSealDetectorConfig,
     AudioSealWMConfig,
     create_detector,
     create_generator,
 )
 from audioseal.models import AudioSealDetector, AudioSealWM
@@ -76,19 +77,37 @@
 
     cache_dir = _get_cache_dir(
         ["AUDIOSEAL_CACHE_DIR", "AUDIOCRAFT_CACHE_DIR", "XDG_CACHE_HOME"]
     )
     parts = urlparse(str(model_path))
     if parts.scheme == "https":
 
-        # TODO: Add HF Hub
         hash_ = sha1(parts.path.encode()).hexdigest()[:24]
         return torch.hub.load_state_dict_from_url(
             str(model_path), model_dir=cache_dir, map_location=device, file_name=hash_
         )
+    elif str(model_path).startswith("facebook/audioseal/"):
+        hf_filename = str(model_path)[len("facebook/audioseal/") :]
+
+        try:
+            from huggingface_hub import hf_hub_download
+        except ModuleNotFoundError:
+            print(
+                f"The model path {model_path} seems to be a direct HF path, "
+                "but you do not install Huggingface_hub. Install with for example "
+                "`pip install huggingface_hub` to use this feature."
+            )
+        file = hf_hub_download(
+            repo_id="facebook/audioseal",
+            filename=hf_filename,
+            cache_dir=cache_dir,
+            library_name="audioseal",
+            library_version=audioseal.__version__,
+        )
+        return torch.load(file, map_location=device)
     else:
         raise ModelLoadError(f"Path or uri {model_path} is unknown or does not exist")
 
 
 def load_local_model_config(model_card: str) -> Optional[DictConfig]:
     config_file = Path(__file__).parent / "cards" / (model_card + ".yaml")
     if Path(config_file).is_file():
@@ -96,16 +115,18 @@
     else:
         return None
 
 
 class AudioSeal:
 
     @staticmethod
-    def _parse_model(
-        model_card_or_path: str, model_type: Type[AudioSealT]
+    def parse_model(
+        model_card_or_path: str,
+        model_type: Type[AudioSealT],
+        nbits: Optional[int] = None,
     ) -> Tuple[Dict[str, Any], AudioSealT]:
         """
         Parse the information from the model card or checkpoint path using
         the schema `model_type` that defines the model type
         """
         # Get the raw checkpoint and config from the local model cards
         config = load_local_model_config(model_card_or_path)
@@ -120,72 +141,87 @@
             checkpoint = load_model_checkpoint(checkpoint)
 
         # Get the raw checkpoint and config from the checkpoint path
         else:
             config_dict = {}
             checkpoint = load_model_checkpoint(model_card_or_path)
 
-        # If the checkpoint has config in its, take this but uses the info
-        # in the mode as precedence
-        assert isinstance(
-            checkpoint, dict
-        ), f"Expect loaded checkpoint to be a dictionary, get {type(checkpoint)}"
-        assert isinstance(
-            config_dict, dict
-        ), f"Except loaded config to be a dictionary, get {type(config_dict)}"
         if "xp.cfg" in checkpoint:
-            config = {**checkpoint["xp.cfg"], **config_dict}  # type: ignore
-            assert config is not None
-            assert (
-                "seanet" in config
-            ), f"missing seanet backbone config in {model_card_or_path}"
-
-            # Patch 1: Resolve the variables in the checkpoint
-            config = OmegaConf.create(config)
-            OmegaConf.resolve(config)
-            config = OmegaConf.to_container(config)  # type: ignore
-
-            # Patch 2: Put decoder, encoder and detector outside seanet
-            seanet_config = config["seanet"]
-            for key_to_patch in ["encoder", "decoder", "detector"]:
-                if key_to_patch in seanet_config:
-                    config_to_patch = config.get(key_to_patch) or {}
-                    config[key_to_patch] = {
-                        **config_to_patch,
-                        **seanet_config.pop(key_to_patch),
-                    }
+            config_dict = {**checkpoint["xp.cfg"], **config_dict}  # type: ignore
 
-            config["seanet"] = seanet_config
+        model_config = AudioSeal.parse_config(config_dict, config_type=model_type, nbits=nbits)  # type: ignore
 
         if "model" in checkpoint:
             checkpoint = checkpoint["model"]
 
+        return checkpoint, model_config
+
+    @staticmethod
+    def parse_config(
+        config: Dict[str, Any],
+        config_type: Type[AudioSealT],
+        nbits: Optional[int] = None,
+    ) -> AudioSealT:
+
+        assert "seanet" in config, f"missing seanet backbone config in {config}"
+
+        # Patch 1: Resolve the variables in the checkpoint
+        config = OmegaConf.create(config)  # type: ignore
+        OmegaConf.resolve(config)  # type: ignore
+        config = OmegaConf.to_container(config)  # type: ignore
+
+        # Patch 2: Put decoder, encoder and detector outside seanet
+        seanet_config = config["seanet"]
+        for key_to_patch in ["encoder", "decoder", "detector"]:
+            if key_to_patch in seanet_config:
+                config_to_patch = config.get(key_to_patch) or {}
+                config[key_to_patch] = {
+                    **config_to_patch,
+                    **seanet_config.pop(key_to_patch),
+                }
+
+        config["seanet"] = seanet_config
+
+        # Patch 3: Put nbits into config if specified
+        if nbits and "nbits" not in config:
+            config["nbits"] = nbits
+
         # remove attributes not related to the model_type
         result_config = {}
-        assert config, f"Empty config in {model_card_or_path}"
-        for field in fields(model_type):
+        assert config, f"Empty config"
+        for field in fields(config_type):
             if field.name in config:
                 result_config[field.name] = config[field.name]
 
-        schema = OmegaConf.structured(model_type)
+        schema = OmegaConf.structured(config_type)
         schema.merge_with(result_config)
-        return checkpoint, schema
+        return schema
 
     @staticmethod
-    def load_generator(model_card_or_path: str) -> AudioSealWM:
+    def load_generator(
+        model_card_or_path: str,
+        nbits: Optional[int] = None,
+    ) -> AudioSealWM:
         """Load the AudioSeal generator from the model card"""
-        checkpoint, config = AudioSeal._parse_model(
-            model_card_or_path, AudioSealWMConfig
+        checkpoint, config = AudioSeal.parse_model(
+            model_card_or_path,
+            AudioSealWMConfig,
+            nbits=nbits,
         )
 
         model = create_generator(config)
         model.load_state_dict(checkpoint)
         return model
 
     @staticmethod
-    def load_detector(model_card_or_path: str) -> AudioSealDetector:
-        checkpoint, config = AudioSeal._parse_model(
-            model_card_or_path, AudioSealDetectorConfig
+    def load_detector(
+        model_card_or_path: str,
+        nbits: Optional[int] = None,
+    ) -> AudioSealDetector:
+        checkpoint, config = AudioSeal.parse_model(
+            model_card_or_path,
+            AudioSealDetectorConfig,
+            nbits=nbits,
         )
         model = create_detector(config)
         model.load_state_dict(checkpoint)
         return model
```

### Comparing `audioseal-0.1.2/src/audioseal/models.py` & `audioseal-0.1.3/src/audioseal/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,30 +105,32 @@
             sample_rate = 16_000
         assert sample_rate
         if sample_rate != 16000:
             x = julius.resample_frac(x, old_sr=sample_rate, new_sr=16000)
         hidden = self.encoder(x)
 
         if self.msg_processor is not None:
-            if message is None:
-                self.message = self.message or torch.randint(
-                    0, 2, (x.shape[0], self.msg_processor.nbits), device=x.device
-                )
-                message = self.message
+            if self.message is None:
+                self.message = torch.randint(0, 2, (x.shape[0], self.msg_processor.nbits), device=x.device)
+            else:
+                self.message = self.message.to(device=x.device)
+
+            
+            message = self.message
 
             hidden = self.msg_processor(hidden, message)
 
         watermark = self.decoder(hidden)
 
         if sample_rate != 16000:
-            watermark = julius.resample_frac(watermark, old_sr=16000, new_sr=sample_rate)
+            watermark = julius.resample_frac(
+                watermark, old_sr=16000, new_sr=sample_rate
+            )
 
-        return watermark[
-            ..., : length
-        ]  # trim output cf encodec codebase
+        return watermark[..., :length]  # trim output cf encodec codebase
 
     def forward(
         self,
         x: torch.Tensor,
         sample_rate: Optional[int] = None,
         message: Optional[torch.Tensor] = None,
         alpha: float = 1.0,
@@ -160,46 +162,47 @@
         self.detector = torch.nn.Sequential(encoder, last_layer)
         self.nbits = nbits
 
     def detect_watermark(
         self,
         x: torch.Tensor,
         sample_rate: Optional[int] = None,
-        message_threshold: float = 0.5
+        message_threshold: float = 0.5,
     ) -> Tuple[float, torch.Tensor]:
         """
         A convenience function that returns a probability of an audio being watermarked,
         together with its message in n-bits (binary) format. If the audio is not watermarked,
         the message will be random.
         Args:
             x: Audio signal, size: batch x frames
             sample_rate: The sample rate of the input audio
             message_threshold: threshold used to convert the watermark output (probability
-                of each bits being 0 or 1) into the binary n-bit message. 
+                of each bits being 0 or 1) into the binary n-bit message.
         """
         if sample_rate is None:
             logger.warning(COMPATIBLE_WARNING)
             sample_rate = 16_000
         result, message = self.forward(x, sample_rate=sample_rate)  # b x 2+nbits
-        detected = torch.count_nonzero(torch.gt(result[:, 1, :], 0.5)) / result.shape[-1]
+        detected = (
+            torch.count_nonzero(torch.gt(result[:, 1, :], 0.5)) / result.shape[-1]
+        )
         detect_prob = detected.cpu().item()  # type: ignore
         message = torch.gt(message, message_threshold).int()
         return detect_prob, message
 
     def decode_message(self, result: torch.Tensor) -> torch.Tensor:
         """
         Decode the message from the watermark result (batch x nbits x frames)
         Args:
             result: watermark result (batch x nbits x frames)
         Returns:
             The message of size batch x nbits, indicating probability of 1 for each bit
         """
-        assert (
-            (result.dim() > 2 and result.shape[1] == self.nbits) or
-            (self.dim() == 2 and result.shape[0] == self.nbits)
+        assert (result.dim() > 2 and result.shape[1] == self.nbits) or (
+            self.dim() == 2 and result.shape[0] == self.nbits
         ), f"Expect message of size [,{self.nbits}, frames] (get {result.size()})"
         decoded_message = result.mean(dim=-1)
         return torch.sigmoid(decoded_message)
 
     def forward(
         self,
         x: torch.Tensor,
```

### Comparing `audioseal-0.1.2/tests/test_models.py` & `audioseal-0.1.3/tests/test_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import urllib
 
 import pytest
 import torch
 import torchaudio
 
 from audioseal import AudioSeal
+from audioseal.models import AudioSealDetector, AudioSealWM
 
 
 @pytest.fixture
 def example_audio(tmp_path):
     url = "https://keithito.com/LJ-Speech-Dataset/LJ037-0171.wav"
     with open(tmp_path / "test.wav", "wb") as f:
         resp = urllib.request.urlopen(url)
@@ -33,21 +34,30 @@
 
     secret_message = torch.randint(0, 2, (1, 16), dtype=torch.int32)
     watermark = model(audio, sample_rate=sr, message=secret_message, alpha=0.8)
 
     watermarked_audio = audio + watermark
 
     detector = AudioSeal.load_detector(("audioseal_detector_16bits"))
-    result, message = detector.detect_watermark(watermarked_audio, sample_rate=sr)   # noqa
+    result, message = detector.detect_watermark(watermarked_audio, sample_rate=sr)  # noqa
 
     # Due to non-deterministic decoding, messages are not always the same as message
     print(f"\nOriginal message: {secret_message}")
     print(f"Decoded message: {message}")
     print(
         "Matching bits in decoded and original messages: "
         f"{torch.count_nonzero(torch.eq(message, secret_message)).item()}\n"
     )
-    assert result > 0.6
+    assert result > 0.5
 
     # Try to detect the unwatermarked audio
     result, _ = detector.detect_watermark(audio, sample_rate=sr)  # noqa
     assert result < 0.5
+
+
+def test_loading_from_hf(example_audio):
+    audio, sr = example_audio
+
+    generator = AudioSeal.load_generator("facebook/audioseal/generator_base.pth", nbits=16)
+    detector = AudioSeal.load_detector("facebook/audioseal/detector_base.pth", nbits=16)
+
+    assert isinstance(generator, AudioSealWM) and isinstance(detector, AudioSealDetector)
```

### Comparing `audioseal-0.1.2/PKG-INFO` & `audioseal-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioseal
-Version: 0.1.2
+Version: 0.1.3
 Summary: Watermarking and detection for speech audios
 Author: Facebook AI Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
@@ -29,18 +29,23 @@
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray"></a>
 
 Inference code for AudioSeal, a method for speech localized watermarking, with state-of-the-art robustness and detector speed (training code coming soon).
 More details can be found in the [paper](https://arxiv.org/abs/2401.17264).
 
 [[`arXiv`](https://arxiv.org/abs/2401.17264)]
-[[`Colab notebook`](https://colab.research.google.com/github/facebookresearch/audioseal/blob/master/examples/colab.ipynb)]
+[[`Colab notebook`](https://colab.research.google.com/github/facebookresearch/audioseal/blob/master/examples/colab.ipynb)][[🤗`Hugging Face`](https://huggingface.co/facebook/audioseal)]
 
 ![fig](https://github.com/facebookresearch/audioseal/assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2)
 
+# Updates:
+
+- 2024-04-02: We have updated our license to full MIT license (including the license for the model weights) ! Now you can use AudioSeal in commercial application too !
+- 2024-02-29: AudioSeal 0.1.2 is out, with more bug fixes for resampled audios and updated notebooks
+
 # Abtract
 
 We introduce AudioSeal, a method for speech localized watermarking, with state-of-the-art robustness and detector speed. It jointly trains a generator that embeds a watermark in the audio, and a detector that detects the watermarked fragments in longer audios, even in the presence of editing.
 Audioseal achieves state-of-the-art detection performance of both natural and synthetic speech at the sample level (1/16k second resolution), it generates limited alteration of signal quality and is robust to many types of audio editing. 
 Audioseal is designed with a fast, single-pass detector, that significantly surpasses existing models in speed — achieving detection up to two orders of magnitude faster, making it ideal for large-scale and real-time applications.
 
 # :mate: Installation
@@ -57,15 +62,15 @@
 git clone https://github.com/facebookresearch/audioseal
 cd audioseal
 pip install -e .
 ```
 
 # :gear: Models
 
-We provide the checkpoints for the following models:
+You can find all the model checkpoints on the [Hugging Face Hub](https://huggingface.co/facebook/audioseal). We provide the checkpoints for the following models:
 
 - [AudioSeal Generator](src/audioseal/cards/audioseal_wm_16bits.yaml).
   It takes as input an audio signal (as a waveform), and outputs a watermark of the same size as the input, that can be added to the input to watermark it.
   Optionally, it can also take as input a secret message of 16-bits that will be encoded in the watermark.
 - [AudioSeal Detector](src/audioseal/cards/audioseal_detector_16bits.yaml).
   It takes as input an audio signal (as a waveform), and outputs a probability that the input contains a watermark at each sample of the audio (every 1/16k s).
   Optionally, it may also output the secret message encoded in the watermark.
@@ -138,15 +143,14 @@
 
 - If you use torchaudio to handle your audios and encounter the error `Couldn't find appropriate backend to handle uri ...`, this is due to newer version of 
 torchaudio does not handle the default backend well. Either downgrade your torchaudio to `2.0.1` or earlier, or install `soundfile` as your audio backend.
 
 # License
 
 - The code in this repository is released under the MIT license as found in the [LICENSE file](LICENSE).
-- The models weights in this repository are released under the CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights).
 
 # Maintainers:
 - [Tuan Tran](https://github.com/antoine-tran)
 - [Hady Elsahar](https://github.com/hadyelsahar)
 - [Pierre Fernandez](https://github.com/pierrefdz)
 - [Robin San Roman](https://github.com/robinsrm)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audioseal Version: 0.1.2 Summary: Watermarking and
+Metadata-Version: 2.1 Name: audioseal Version: 0.1.3 Summary: Watermarking and
 detection for speech audios Author: Facebook AI Research Requires-Python: >=3.8
 Description-Content-Type: text/markdown Classifier: License :: OSI Approved ::
 MIT License Classifier: Topic :: Scientific/Engineering Classifier: Development
 Status :: 4 - Beta Requires-Dist: numpy Requires-Dist: omegaconf Requires-Dist:
 julius Requires-Dist: torch>=1.13.0 Requires-Dist: func_argparse ; extra ==
 "dev" Requires-Dist: torchaudio ; extra == "dev" Requires-Dist: soundfile ;
 extra == "dev" Requires-Dist: pytest ; extra == "dev" Requires-Dist: black ;
@@ -12,55 +12,60 @@
 github.com/facebookresearch/audioseal/issues Provides-Extra: dev # :loud_sound:
 AudioSeal: Proactive Localized Watermarking _[_P_y_t_h_o_n_]_[_C_o_d_e_ _s_t_y_l_e_:
 _b_l_a_c_k_]Inference code for AudioSeal, a method for speech localized watermarking,
 with state-of-the-art robustness and detector speed (training code coming
 soon). More details can be found in the [paper](https://arxiv.org/abs/
 2401.17264). [[`arXiv`](https://arxiv.org/abs/2401.17264)] [[`Colab notebook`]
 (https://colab.research.google.com/github/facebookresearch/audioseal/blob/
-master/examples/colab.ipynb)] ![fig](https://github.com/facebookresearch/
-audioseal/assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2) # Abtract We
-introduce AudioSeal, a method for speech localized watermarking, with state-of-
-the-art robustness and detector speed. It jointly trains a generator that
-embeds a watermark in the audio, and a detector that detects the watermarked
-fragments in longer audios, even in the presence of editing. Audioseal achieves
-state-of-the-art detection performance of both natural and synthetic speech at
-the sample level (1/16k second resolution), it generates limited alteration of
-signal quality and is robust to many types of audio editing. Audioseal is
-designed with a fast, single-pass detector, that significantly surpasses
-existing models in speed â achieving detection up to two orders of magnitude
-faster, making it ideal for large-scale and real-time applications. # :mate:
-Installation AudioSeal requires Python >=3.8, Pytorch >= 1.13.0, [omegaconf]
-(https://omegaconf.readthedocs.io/), [julius](https://pypi.org/project/julius/
-), and numpy. To install from PyPI: ``` pip install audioseal ``` To install
-from source: Clone this repo and install in editable mode: ``` git clone https:
-//github.com/facebookresearch/audioseal cd audioseal pip install -e . ``` # :
-gear: Models We provide the checkpoints for the following models: - [AudioSeal
-Generator](src/audioseal/cards/audioseal_wm_16bits.yaml). It takes as input an
-audio signal (as a waveform), and outputs a watermark of the same size as the
-input, that can be added to the input to watermark it. Optionally, it can also
-take as input a secret message of 16-bits that will be encoded in the
-watermark. - [AudioSeal Detector](src/audioseal/cards/
-audioseal_detector_16bits.yaml). It takes as input an audio signal (as a
-waveform), and outputs a probability that the input contains a watermark at
-each sample of the audio (every 1/16k s). Optionally, it may also output the
-secret message encoded in the watermark. Note that the message is optional and
-has no influence on the detection output. It may be used to identify a model
-version for instance (up to $2**16=65536$ possible choices). **Note**: We are
-working to release the training code for anyone wants to build their own
-watermarker. Stay tuned ! # :abacus: Usage Audioseal provides a simple API to
-watermark and detect the watermarks from an audio sample. Example usage:
-```python from audioseal import AudioSeal # model name corresponds to the YAML
-card file name found in audioseal/cards model = AudioSeal.load_generator
-("audioseal_wm_16bits") # Other way is to load directly from the checkpoint #
-model = Watermarker.from_pretrained(checkpoint_path, device = wav.device) # a
-torch tensor of shape (batch, channels, samples) and a sample rate # It is
-important to process the audio to the same sample rate as the model # expectes.
-In our case, we support 16khz audio wav, sr = ..., 16000 watermark =
-model.get_watermark(wav, sr) # Optional: you can add a 16-bit message to embed
-in the watermark # msg = torch.randint(0, 2, (wav.shape(0),
+master/examples/colab.ipynb)][[ð¤`Hugging Face`](https://huggingface.co/
+facebook/audioseal)] ![fig](https://github.com/facebookresearch/audioseal/
+assets/1453243/5d8cd96f-47b5-4c34-a3fa-7af386ed59f2) # Updates: - 2024-04-02:
+We have updated our license to full MIT license (including the license for the
+model weights) ! Now you can use AudioSeal in commercial application too ! -
+2024-02-29: AudioSeal 0.1.2 is out, with more bug fixes for resampled audios
+and updated notebooks # Abtract We introduce AudioSeal, a method for speech
+localized watermarking, with state-of-the-art robustness and detector speed. It
+jointly trains a generator that embeds a watermark in the audio, and a detector
+that detects the watermarked fragments in longer audios, even in the presence
+of editing. Audioseal achieves state-of-the-art detection performance of both
+natural and synthetic speech at the sample level (1/16k second resolution), it
+generates limited alteration of signal quality and is robust to many types of
+audio editing. Audioseal is designed with a fast, single-pass detector, that
+significantly surpasses existing models in speed â achieving detection up to
+two orders of magnitude faster, making it ideal for large-scale and real-time
+applications. # :mate: Installation AudioSeal requires Python >=3.8, Pytorch >=
+1.13.0, [omegaconf](https://omegaconf.readthedocs.io/), [julius](https://
+pypi.org/project/julius/), and numpy. To install from PyPI: ``` pip install
+audioseal ``` To install from source: Clone this repo and install in editable
+mode: ``` git clone https://github.com/facebookresearch/audioseal cd audioseal
+pip install -e . ``` # :gear: Models You can find all the model checkpoints on
+the [Hugging Face Hub](https://huggingface.co/facebook/audioseal). We provide
+the checkpoints for the following models: - [AudioSeal Generator](src/
+audioseal/cards/audioseal_wm_16bits.yaml). It takes as input an audio signal
+(as a waveform), and outputs a watermark of the same size as the input, that
+can be added to the input to watermark it. Optionally, it can also take as
+input a secret message of 16-bits that will be encoded in the watermark. -
+[AudioSeal Detector](src/audioseal/cards/audioseal_detector_16bits.yaml). It
+takes as input an audio signal (as a waveform), and outputs a probability that
+the input contains a watermark at each sample of the audio (every 1/16k s).
+Optionally, it may also output the secret message encoded in the watermark.
+Note that the message is optional and has no influence on the detection output.
+It may be used to identify a model version for instance (up to $2**16=65536$
+possible choices). **Note**: We are working to release the training code for
+anyone wants to build their own watermarker. Stay tuned ! # :abacus: Usage
+Audioseal provides a simple API to watermark and detect the watermarks from an
+audio sample. Example usage: ```python from audioseal import AudioSeal # model
+name corresponds to the YAML card file name found in audioseal/cards model =
+AudioSeal.load_generator("audioseal_wm_16bits") # Other way is to load directly
+from the checkpoint # model = Watermarker.from_pretrained(checkpoint_path,
+device = wav.device) # a torch tensor of shape (batch, channels, samples) and a
+sample rate # It is important to process the audio to the same sample rate as
+the model # expectes. In our case, we support 16khz audio wav, sr = ..., 16000
+watermark = model.get_watermark(wav, sr) # Optional: you can add a 16-bit
+message to embed in the watermark # msg = torch.randint(0, 2, (wav.shape(0),
 model.msg_processor.nbits), device=wav.device) # watermark =
 model.get_watermark(wav, message = msg) watermarked_audio = wav + watermark
 detector = AudioSeal.load_detector("audioseal_detector_16bits") # To detect the
 messages in the high-level. result, message = detector.detect_watermark
 (watermarked_audio, sr) print(result) # result is a float number indicating the
 probability of the audio being watermarked, print(message) # message is a
 binary vector of 16 bits # To detect the messages in the low-level. result,
@@ -82,17 +87,15 @@
 which is not compatible in Windows. Try to invalidate the cache by removing the
 files in `C:\Users\\.cache\audioseal` and re-run again. - If you use torchaudio
 to handle your audios and encounter the error `Couldn't find appropriate
 backend to handle uri ...`, this is due to newer version of torchaudio does not
 handle the default backend well. Either downgrade your torchaudio to `2.0.1` or
 earlier, or install `soundfile` as your audio backend. # License - The code in
 this repository is released under the MIT license as found in the [LICENSE
-file](LICENSE). - The models weights in this repository are released under the
-CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights). #
-Maintainers: - [Tuan Tran](https://github.com/antoine-tran) - [Hady Elsahar]
-(https://github.com/hadyelsahar) - [Pierre Fernandez](https://github.com/
-pierrefdz) - [Robin San Roman](https://github.com/robinsrm) # Citation If you
-find this repository useful, please consider giving a star :star: and please
-cite as: ``` @article{sanroman2024proactive, title={Proactive Detection of
-Voice Cloning with Localized Watermarking}, author={San Roman, Robin and
-Fernandez, Pierre and Elsahar, Hady and DÂ´efossez, Alexandre and Furon, Teddy
-and Tran, Tuan}, journal={arXiv preprint}, year={2024} } ```
+file](LICENSE). # Maintainers: - [Tuan Tran](https://github.com/antoine-tran) -
+[Hady Elsahar](https://github.com/hadyelsahar) - [Pierre Fernandez](https://
+github.com/pierrefdz) - [Robin San Roman](https://github.com/robinsrm) #
+Citation If you find this repository useful, please consider giving a star :
+star: and please cite as: ``` @article{sanroman2024proactive, title={Proactive
+Detection of Voice Cloning with Localized Watermarking}, author={San Roman,
+Robin and Fernandez, Pierre and Elsahar, Hady and DÂ´efossez, Alexandre and
+Furon, Teddy and Tran, Tuan}, journal={arXiv preprint}, year={2024} } ```
```

