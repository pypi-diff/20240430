# Comparing `tmp/thepipe_api-0.3.3.tar.gz` & `tmp/thepipe_api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.3.3.tar", last modified: Sun Apr 28 06:43:18 2024, max compression
+gzip compressed data, was "thepipe_api-0.3.4.tar", last modified: Tue Apr 30 01:45:30 2024, max compression
```

## Comparing `thepipe_api-0.3.3.tar` & `thepipe_api-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.445625 thepipe_api-0.3.3/
--rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    12404 2024-04-28 06:43:18.444634 thepipe_api-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    11622 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 06:43:18.445625 thepipe_api-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.410585 thepipe_api-0.3.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/tests/__init__.py
--rw-rw-rw-   0        0        0    11487 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.417632 thepipe_api-0.3.3/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-04-28 03:24:11.000000 thepipe_api-0.3.3/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2878 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/thepipe_api/core.py
--rw-rw-rw-   0        0        0    24815 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3704 2024-04-20 03:49:35.000000 thepipe_api-0.3.3/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.443627 thepipe_api-0.3.3/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0    12404 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.502604 thepipe_api-0.3.4/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    12322 2024-04-30 01:45:30.501605 thepipe_api-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11540 2024-04-30 01:44:28.000000 thepipe_api-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 01:45:30.502604 thepipe_api-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-30 01:44:41.000000 thepipe_api-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.465604 thepipe_api-0.3.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    11487 2024-04-28 06:43:08.000000 thepipe_api-0.3.4/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.470606 thepipe_api-0.3.4/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-04-28 03:24:11.000000 thepipe_api-0.3.4/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2878 2024-04-28 06:43:08.000000 thepipe_api-0.3.4/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    25023 2024-04-30 01:44:28.000000 thepipe_api-0.3.4/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3704 2024-04-29 04:19:09.000000 thepipe_api-0.3.4/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.500614 thepipe_api-0.3.4/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0    12322 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.3.3/LICENSE` & `thepipe_api-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.3/PKG-INFO` & `thepipe_api-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,19 +26,19 @@
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a> <a href="https://discord.gg/bXfKeGs5qV">![Join discord](https://img.shields.io/discord/1227806200478044274?color=4f69ef&label=Discord&logo=discord&logoColor=ffffff)</a>
 
-### Feed PDFs, web pages, word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code ⚡
+### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-Language models with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that want to support comprehensive textual and visual understanding across a wide range of data sources. The Pipe is available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally to let you run the compute.
 
 ![Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/science_assistantpy2.png)
 
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
@@ -96,17 +96,17 @@
 | Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Video                                 | `.mp4`, `.avi`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames from video files; supports frame extraction and OCR for text extraction from frames |
 | Audio                                 | `.mp3`, `.wav`          | ✔️               | ❌                | Extracts text from audio files; supports speech-to-text conversion        | 
-| Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
-| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
-| YouTube Video                         | YouTube video URLs                      | ✔️               | ✔️                | Extracts text from YouTube videos; supports subtitles extraction          |
+| Website                               | URLs (inputs starting with `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| GitHub Repository                     | GitHub repo URLs (inputs starting with `https://github.com` or `https://www.github.com`)                          | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| YouTube Video                         | YouTube video URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)                     | ✔️               | ✔️                | Extracts frames and transcript from YouTube videos in per-minute chunks          |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## How it works 🛠️
 
 The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
 ```json
 [
@@ -135,33 +135,16 @@
 It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [table, equation, and figure extraction](https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
 
 
 ## Local Installation 🛠️
 
-The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
-
-```bash
-git clone https://github.com/emcf/thepipe
-pip install -r requirements_local.txt
-```
-
-Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH.
-
-Now you can use The Pipe with Python:
-```bash
-from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf", local=True)
-```
-
-or from the command line:
-```bash
-thepipe path/to/folder --local
-```
+If you do not wish to use our API, you are welcome host The Pipe for yourself locally. 
+If you choose to do this, you must install a number of dependencies for the code to function correctly, some of which may incur compute costs and/or require a GPU for reasonable performance. Additional installed dependencies are required: pytorch, universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This installation process will depend on your system and compute capabilities. After installing them, follow these steps for a local setup:
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Substring to match files in the directory. Regex is not yet supported.
 - `ignore` (optional): Substring to ignore files in the directory. Regex is not yet supported.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.3 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.4 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -11,126 +11,126 @@
 _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, web pages,
-word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code
-â¡ The Pipe is a multimodal-first tool for feeding files and web pages into
-vision-language models such as GPT-4V. It is best for LLM and RAG applications
-that require a deep understanding of tricky data sources. The Pipe is available
-as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
-[Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/
-object/public/assets/science_assistantpy2.png) ## Features ð - Extracts text
-and visuals from files or web pages ð - Outputs chunks optimized for
-multimodal LLMs and RAG frameworks ð¼ï¸ - Interpret complex PDFs, web pages,
-docs, videos, data, and more ð§  - Auto-compress prompts exceeding your chosen
-token limit ð¦ - Works even with missing file extensions, in-memory data
-streams ð¾ - Works with codebases, git repos, and custom integrations ð -
-Multi-threaded â¡ï¸ ## Getting Started ð The Pipe handles a wide array of
-complex filetypes, and thus has many dependencies that must be installed
-separately. It also requires a strong machine for good response times. For this
-reason, we host it as an API that works out-of-the-box. First, install The
-Pipe. ``` pip install thepipe_api ``` The Pipe is available as a hosted API, or
-it can be set up locally. An API key is recommended for out-of-the-box
-functionality (alternatively, see the local installation section). Ensure the
-`THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one
-here](https://thepi.pe). Now you can extract comprehensive text and visuals
-from any file: ```python from thepipe_api import thepipe messages =
-thepipe.extract("example.pdf") ``` Or websites: ```python messages =
-thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
-```python response = client.chat.completions.create( model="gpt-4-vision-
-preview", messages = messages, ) ``` ![Just call OpenAI](https://
-rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
-You can also use The Pipe from the command line. Here's how to recursively
-extract from a directory, matching only files containing a substring (in this
-example, typescript files) and ignore files containing other substrings (in
-this example, anything in the "tests" folder): ```bash thepipe path/to/folder -
--match tsx --ignore tests ``` ## Supported File Types ð | Source Type |
-Input types | Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð
-| |---------------------------------------|------------------------------------
-------|-------------------|------------------|---------------------------------
-------------------------| | Directory | Any `/path/to/directory` | âï¸ |
-âï¸ | Extracts from all files in directory, supports match and ignore
-patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸
-(varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are compressible
-with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸
-| â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text
-and images of each page; can use AI for extraction of table data and images
-within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts
-images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
-| â | Extracts data from spreadsheets; converts to text representation. For
-very large datasets, will only extract column names and types | | Jupyter
-Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
-Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
-Extracts text and images from Word documents | | Microsoft PowerPoint
-Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
-PowerPoint presentations | | Video | `.mp4`, `.avi`, `.mov`, `.wmv` | âï¸ |
-âï¸ | Extracts frames from video files; supports frame extraction and OCR
-for text extraction from frames | | Audio | `.mp3`, `.wav` | âï¸ | â |
-Extracts text from audio files; supports speech-to-text conversion | | Website
-| URLs (inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts
-text from web page along with image (or images if scrollable); text-only
-extraction available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸
-| Extracts from GitHub repositories; supports branch specification | | YouTube
-Video | YouTube video URLs | âï¸ | âï¸ | Extracts text from YouTube
-videos; supports subtitles extraction | | ZIP File | `.zip` | âï¸ | âï¸ |
-Extracts contents of ZIP files; supports nested directory extraction | ## How
-it works ð ï¸ The input source is either a file path, a URL, or a directory.
-The pipe will extract information from the source and process it for downstream
-use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
-[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
-[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
-pipe is a sensible list of multimodal messages representing chunks of the
-extracted information, carefully crafted to fit within context windows for any
-models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4]
-(https://openai.com/gpt-4). The messages returned should look like this:
-```json [ { "role": "user", "content": [ { "type": "text", "text": "..." },
-{ "type": "image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ]
-} ] ``` If you want to feed these messages directly into the model, it is
-important to be mindful of the token limit. OpenAI does not allow too many
-images in the prompt (see discussion [here](https://community.openai.com/t/gpt-
-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted
-with `text_only=True` to avoid this issue, while long text files should either
-be compressed or embedded in a RAG framework. The text and images from these
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) _!_[_J_o_i_n_ _d_i_s_c_o_r_d_]_(_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
+_1_2_2_7_8_0_6_2_0_0_4_7_8_0_4_4_2_7_4_?_c_o_l_o_r_=_4_f_6_9_e_f_&_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_f_f_f_f_f_f_)
+### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-
+Language models with one line of code â¡ The Pipe is a multimodal-first tool
+for feeding files and web pages into vision-language models such as GPT-4V. It
+is best for LLM and RAG applications that want to support comprehensive textual
+and visual understanding across a wide range of data sources. The Pipe is
+available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be
+set up locally to let you run the compute. ![Science assistant demo](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+science_assistantpy2.png) ## Features ð - Extracts text and visuals from
+files or web pages ð - Outputs chunks optimized for multimodal LLMs and RAG
+frameworks ð¼ï¸ - Interpret complex PDFs, web pages, docs, videos, data, and
+more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
+Works even with missing file extensions, in-memory data streams ð¾ - Works
+with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
+## Getting Started ð The Pipe handles a wide array of complex filetypes, and
+thus has many dependencies that must be installed separately. It also requires
+a strong machine for good response times. For this reason, we host it as an API
+that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
+``` The Pipe is available as a hosted API, or it can be set up locally. An API
+key is recommended for out-of-the-box functionality (alternatively, see the
+local installation section). Ensure the `THEPIPE_API_KEY` environment variable
+is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
+extract comprehensive text and visuals from any file: ```python from
+thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or
+websites: ```python messages = thepipe.extract("https://example.com") ``` Then
+feed it into GPT-4-Vision: ```python response = client.chat.completions.create
+( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
+(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory, matching only files containing a
+substring (in this example, typescript files) and ignore files containing other
+substrings (in this example, anything in the "tests" folder): ```bash thepipe
+path/to/folder --match tsx --ignore tests ``` ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
+`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts to text representation. For very large datasets, will only extract
+column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
+Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
+Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
+documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
+Extracts text and images from PowerPoint presentations | | Video | `.mp4`,
+`.avi`, `.mov`, `.wmv` | âï¸ | âï¸ | Extracts frames from video files;
+supports frame extraction and OCR for text extraction from frames | | Audio |
+`.mp3`, `.wav` | âï¸ | â | Extracts text from audio files; supports
+speech-to-text conversion | | Website | URLs (inputs starting with `http`,
+`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
+image (or images if scrollable); text-only extraction available | | GitHub
+Repository | GitHub repo URLs (inputs starting with `https://github.com` or
+`https://www.github.com`) | âï¸ | âï¸ | Extracts from GitHub
+repositories; supports branch specification | | YouTube Video | YouTube video
+URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)
+| âï¸ | âï¸ | Extracts frames and transcript from YouTube videos in per-
+minute chunks | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
+ZIP files; supports nested directory extraction | ## How it works ð ï¸ The
+input source is either a file path, a URL, or a directory. The pipe will
+extract information from the source and process it for downstream use with
+[language models](https://en.wikipedia.org/wiki/Large_language_model), [vision
+transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
+language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
+a sensible list of multimodal messages representing chunks of the extracted
+information, carefully crafted to fit within context windows for any models
+from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
+openai.com/gpt-4). The messages returned should look like this: ```json [
+{ "role": "user", "content": [ { "type": "text", "text": "..." }, { "type":
+"image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ] } ] ```
+If you want to feed these messages directly into the model, it is important to
+be mindful of the token limit. OpenAI does not allow too many images in the
+prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-
+maximum-amount-of-images/573110/6)), so long files should be extracted with
+`text_only=True` to avoid this issue, while long text files should either be
+compressed or embedded in a RAG framework. The text and images from these
 messages may also be prepared for a vector database with
 `thepipe.core.create_chunks_from_messages` or for downstream use with RAG
 frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily
 integrate The Pipe with any LLM provider. It uses a variety of heuristics for
 optimal performance with vision-language models, including AI filetype
 detection with [filetype detection](https://opensource.googleblog.com/2024/02/
 magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI
 [table, equation, and figure extraction](https://thepi.pe/pricing), efficient
 [token compression](https://arxiv.org/abs/2403.12968), automatic [image
 encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/
 abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172)
 effects, and more, all pre-built to work out-of-the-box. ![Demo](https://
 rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20
-(6).png) ## Local Installation ð ï¸ The Pipe handles a wide array of complex
-filetypes, and thus requires installation of many different packages to
-function. It also requires a very capable machine for good response times. For
-this reason, we host it as an API that works out-of-the-box. To use The Pipe
-locally for free instead, you will need [playwright](https://github.com/
-microsoft/playwright), [ctags](https://github.com/universal-ctags/),
-[pytesseract](https://github.com/h/pytesseract), and the local python
-requirements, which differ from the more lightweight API requirements: ```bash
-git clone https://github.com/emcf/thepipe pip install -r requirements_local.txt
-``` Tip for windows users: Install the python-libmagic binaries with `pip
-install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags`
-binaries are in your PATH. Now you can use The Pipe with Python: ```bash from
-thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
-``` or from the command line: ```bash thepipe path/to/folder --local ```
-Arguments are: - `source` (required): can be a file path, a URL, or a directory
-path. - `local` (optional): Use the local version of The Pipe instead of the
-hosted API. - `match` (optional): Substring to match files in the directory.
-Regex is not yet supported. - `ignore` (optional): Substring to ignore files in
-the directory. Regex is not yet supported. - `limit` (optional): The token
-limit for the output prompt, defaults to 100K. Prompts exceeding the limit will
-be compressed. This may not work as expected with the API, as it is in active
+(6).png) ## Local Installation ð ï¸ If you do not wish to use our API, you
+are welcome host The Pipe for yourself locally. If you choose to do this, you
+must install a number of dependencies for the code to function correctly, some
+of which may incur compute costs and/or require a GPU for reasonable
+performance. Additional installed dependencies are required: pytorch,
+universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This
+installation process will depend on your system and compute capabilities. After
+installing them, follow these steps for a local setup: Arguments are: -
+`source` (required): can be a file path, a URL, or a directory path. - `local`
+(optional): Use the local version of The Pipe instead of the hosted API. -
+`match` (optional): Substring to match files in the directory. Regex is not yet
+supported. - `ignore` (optional): Substring to ignore files in the directory.
+Regex is not yet supported. - `limit` (optional): The token limit for the
+output prompt, defaults to 100K. Prompts exceeding the limit will be
+compressed. This may not work as expected with the API, as it is in active
 development. - `ai_extraction` (optional): Extract tables, figures, and math
 from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
 not extract images from documents or websites. Additionally, image files will
 be represented with OCR instead of as images. # Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h
 _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
 Contact emmett@thepi.pe for sponsorship information.
```

### Comparing `thepipe_api-0.3.3/README.md` & `thepipe_api-0.3.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -46,682 +46,677 @@
 000002d0: 7261 696c 7761 792e 6170 7025 3246 266c  railway.app%2F&l
 000002e0: 6162 656c 3d41 5049 2532 3073 7461 7475  abel=API%20statu
 000002f0: 7329 3c2f 613e 203c 6120 6872 6566 3d22  s)</a> <a href="
 00000300: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
 00000310: 2f22 3e21 5b67 6574 2041 5049 5d28 6874  /">![get API](ht
 00000320: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
 00000330: 732e 696f 2f62 6164 6765 2f41 5049 2d61  s.io/badge/API-a
-00000340: 6363 6573 732d 626c 7565 293c 2f61 3e0d  ccess-blue)</a>.
-00000350: 0a0d 0a23 2323 2046 6565 6420 5044 4673  ...### Feed PDFs
-00000360: 2c20 7765 6220 7061 6765 732c 2077 6f72  , web pages, wor
-00000370: 6420 646f 6373 2c20 736c 6964 6573 2c20  d docs, slides, 
-00000380: 7669 6465 6f73 2c20 4353 562c 2061 6e64  videos, CSV, and
-00000390: 206d 6f72 6520 696e 746f 2056 6973 696f   more into Visio
-000003a0: 6e2d 4c4c 4d73 2077 6974 6820 6f6e 6520  n-LLMs with one 
-000003b0: 6c69 6e65 206f 6620 636f 6465 20e2 9aa1  line of code ...
-000003c0: 0d0a 0d0a 5468 6520 5069 7065 2069 7320  ....The Pipe is 
-000003d0: 6120 6d75 6c74 696d 6f64 616c 2d66 6972  a multimodal-fir
-000003e0: 7374 2074 6f6f 6c20 666f 7220 6665 6564  st tool for feed
-000003f0: 696e 6720 6669 6c65 7320 616e 6420 7765  ing files and we
-00000400: 6220 7061 6765 7320 696e 746f 2076 6973  b pages into vis
-00000410: 696f 6e2d 6c61 6e67 7561 6765 206d 6f64  ion-language mod
-00000420: 656c 7320 7375 6368 2061 7320 4750 542d  els such as GPT-
-00000430: 3456 2e20 4974 2069 7320 6265 7374 2066  4V. It is best f
-00000440: 6f72 204c 4c4d 2061 6e64 2052 4147 2061  or LLM and RAG a
-00000450: 7070 6c69 6361 7469 6f6e 7320 7468 6174  pplications that
-00000460: 2072 6571 7569 7265 2061 2064 6565 7020   require a deep 
-00000470: 756e 6465 7273 7461 6e64 696e 6720 6f66  understanding of
-00000480: 2074 7269 636b 7920 6461 7461 2073 6f75   tricky data sou
-00000490: 7263 6573 2e20 5468 6520 5069 7065 2069  rces. The Pipe i
-000004a0: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
-000004b0: 2068 6f73 7465 6420 4150 4920 6174 205b   hosted API at [
-000004c0: 7468 6570 692e 7065 5d28 6874 7470 733a  thepi.pe](https:
-000004d0: 2f2f 7468 6570 692e 7065 292c 206f 7220  //thepi.pe), or 
-000004e0: 6974 2063 616e 2062 6520 7365 7420 7570  it can be set up
-000004f0: 206c 6f63 616c 6c79 2e20 0d0a 0d0a 215b   locally. ....![
-00000500: 5363 6965 6e63 6520 6173 7369 7374 616e  Science assistan
-00000510: 7420 6465 6d6f 5d28 6874 7470 733a 2f2f  t demo](https://
-00000520: 7270 6e75 747a 656d 7574 6272 756d 637a  rpnutzemutbrumcz
-00000530: 7776 7565 2e73 7570 6162 6173 652e 636f  wvue.supabase.co
-00000540: 2f73 746f 7261 6765 2f76 312f 6f62 6a65  /storage/v1/obje
-00000550: 6374 2f70 7562 6c69 632f 6173 7365 7473  ct/public/assets
-00000560: 2f73 6369 656e 6365 5f61 7373 6973 7461  /science_assista
-00000570: 6e74 7079 322e 706e 6729 0d0a 0d0a 0d0a  ntpy2.png)......
-00000580: 2323 2046 6561 7475 7265 7320 f09f 8c9f  ## Features ....
-00000590: 0d0a 0d0a 2d20 4578 7472 6163 7473 2074  ....- Extracts t
-000005a0: 6578 7420 616e 6420 7669 7375 616c 7320  ext and visuals 
-000005b0: 6672 6f6d 2066 696c 6573 206f 7220 7765  from files or we
-000005c0: 6220 7061 6765 7320 f09f 939a 0d0a 2d20  b pages ......- 
-000005d0: 4f75 7470 7574 7320 6368 756e 6b73 206f  Outputs chunks o
-000005e0: 7074 696d 697a 6564 2066 6f72 206d 756c  ptimized for mul
-000005f0: 7469 6d6f 6461 6c20 4c4c 4d73 2061 6e64  timodal LLMs and
-00000600: 2052 4147 2066 7261 6d65 776f 726b 7320   RAG frameworks 
-00000610: f09f 96bc efb8 8f0d 0a2d 2049 6e74 6572  .........- Inter
-00000620: 7072 6574 2063 6f6d 706c 6578 2050 4446  pret complex PDF
-00000630: 732c 2077 6562 2070 6167 6573 2c20 646f  s, web pages, do
-00000640: 6373 2c20 7669 6465 6f73 2c20 6461 7461  cs, videos, data
-00000650: 2c20 616e 6420 6d6f 7265 20f0 9fa7 a00d  , and more .....
-00000660: 0a2d 2041 7574 6f2d 636f 6d70 7265 7373  .- Auto-compress
-00000670: 2070 726f 6d70 7473 2065 7863 6565 6469   prompts exceedi
-00000680: 6e67 2079 6f75 7220 6368 6f73 656e 2074  ng your chosen t
-00000690: 6f6b 656e 206c 696d 6974 20f0 9f93 a60d  oken limit .....
-000006a0: 0a2d 2057 6f72 6b73 2065 7665 6e20 7769  .- Works even wi
-000006b0: 7468 206d 6973 7369 6e67 2066 696c 6520  th missing file 
-000006c0: 6578 7465 6e73 696f 6e73 2c20 696e 2d6d  extensions, in-m
-000006d0: 656d 6f72 7920 6461 7461 2073 7472 6561  emory data strea
-000006e0: 6d73 20f0 9f92 be0d 0a2d 2057 6f72 6b73  ms ......- Works
-000006f0: 2077 6974 6820 636f 6465 6261 7365 732c   with codebases,
-00000700: 2067 6974 2072 6570 6f73 2c20 616e 6420   git repos, and 
-00000710: 6375 7374 6f6d 2069 6e74 6567 7261 7469  custom integrati
-00000720: 6f6e 7320 f09f 8c90 0d0a 2d20 4d75 6c74  ons ......- Mult
-00000730: 692d 7468 7265 6164 6564 20e2 9aa1 efb8  i-threaded .....
-00000740: 8f0d 0a0d 0a23 2320 4765 7474 696e 6720  .....## Getting 
-00000750: 5374 6172 7465 6420 20f0 9f9a 800d 0a0d  Started  .......
-00000760: 0a54 6865 2050 6970 6520 6861 6e64 6c65  .The Pipe handle
-00000770: 7320 6120 7769 6465 2061 7272 6179 206f  s a wide array o
-00000780: 6620 636f 6d70 6c65 7820 6669 6c65 7479  f complex filety
-00000790: 7065 732c 2061 6e64 2074 6875 7320 6861  pes, and thus ha
-000007a0: 7320 6d61 6e79 2064 6570 656e 6465 6e63  s many dependenc
-000007b0: 6965 7320 7468 6174 206d 7573 7420 6265  ies that must be
-000007c0: 2069 6e73 7461 6c6c 6564 2073 6570 6172   installed separ
-000007d0: 6174 656c 792e 2049 7420 616c 736f 2072  ately. It also r
-000007e0: 6571 7569 7265 7320 6120 7374 726f 6e67  equires a strong
-000007f0: 206d 6163 6869 6e65 2066 6f72 2067 6f6f   machine for goo
-00000800: 6420 7265 7370 6f6e 7365 2074 696d 6573  d response times
-00000810: 2e20 466f 7220 7468 6973 2072 6561 736f  . For this reaso
-00000820: 6e2c 2077 6520 686f 7374 2069 7420 6173  n, we host it as
-00000830: 2061 6e20 4150 4920 7468 6174 2077 6f72   an API that wor
-00000840: 6b73 206f 7574 2d6f 662d 7468 652d 626f  ks out-of-the-bo
-00000850: 782e 200d 0a0d 0a46 6972 7374 2c20 696e  x. ....First, in
-00000860: 7374 616c 6c20 5468 6520 5069 7065 2e20  stall The Pipe. 
-00000870: 0d0a 6060 600d 0a70 6970 2069 6e73 7461  ..```..pip insta
-00000880: 6c6c 2074 6865 7069 7065 5f61 7069 0d0a  ll thepipe_api..
-00000890: 6060 600d 0a0d 0a54 6865 2050 6970 6520  ```....The Pipe 
-000008a0: 6973 2061 7661 696c 6162 6c65 2061 7320  is available as 
-000008b0: 6120 686f 7374 6564 2041 5049 2c20 6f72  a hosted API, or
-000008c0: 2069 7420 6361 6e20 6265 2073 6574 2075   it can be set u
-000008d0: 7020 6c6f 6361 6c6c 792e 2041 6e20 4150  p locally. An AP
-000008e0: 4920 6b65 7920 6973 2072 6563 6f6d 6d65  I key is recomme
-000008f0: 6e64 6564 2066 6f72 206f 7574 2d6f 662d  nded for out-of-
-00000900: 7468 652d 626f 7820 6675 6e63 7469 6f6e  the-box function
-00000910: 616c 6974 7920 2861 6c74 6572 6e61 7469  ality (alternati
-00000920: 7665 6c79 2c20 7365 6520 7468 6520 6c6f  vely, see the lo
-00000930: 6361 6c20 696e 7374 616c 6c61 7469 6f6e  cal installation
-00000940: 2073 6563 7469 6f6e 292e 2045 6e73 7572   section). Ensur
-00000950: 6520 7468 6520 6054 4845 5049 5045 5f41  e the `THEPIPE_A
-00000960: 5049 5f4b 4559 6020 656e 7669 726f 6e6d  PI_KEY` environm
-00000970: 656e 7420 7661 7269 6162 6c65 2069 7320  ent variable is 
-00000980: 7365 742e 2044 6f6e 2774 2068 6176 6520  set. Don't have 
-00000990: 6120 6b65 7920 7965 743f 205b 4765 7420  a key yet? [Get 
-000009a0: 6f6e 6520 6865 7265 5d28 6874 7470 733a  one here](https:
-000009b0: 2f2f 7468 6570 692e 7065 292e 0d0a 0d0a  //thepi.pe).....
-000009c0: 4e6f 7720 796f 7520 6361 6e20 6578 7472  Now you can extr
-000009d0: 6163 7420 636f 6d70 7265 6865 6e73 6976  act comprehensiv
-000009e0: 6520 7465 7874 2061 6e64 2076 6973 7561  e text and visua
-000009f0: 6c73 2066 726f 6d20 616e 7920 6669 6c65  ls from any file
-00000a00: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  :..```python..fr
-00000a10: 6f6d 2074 6865 7069 7065 5f61 7069 2069  om thepipe_api i
-00000a20: 6d70 6f72 7420 7468 6570 6970 650d 0a6d  mport thepipe..m
-00000a30: 6573 7361 6765 7320 3d20 7468 6570 6970  essages = thepip
-00000a40: 652e 6578 7472 6163 7428 2265 7861 6d70  e.extract("examp
-00000a50: 6c65 2e70 6466 2229 0d0a 6060 600d 0a4f  le.pdf")..```..O
-00000a60: 7220 7765 6273 6974 6573 3a0d 0a60 6060  r websites:..```
-00000a70: 7079 7468 6f6e 0d0a 6d65 7373 6167 6573  python..messages
-00000a80: 203d 2074 6865 7069 7065 2e65 7874 7261   = thepipe.extra
-00000a90: 6374 2822 6874 7470 733a 2f2f 6578 616d  ct("https://exam
-00000aa0: 706c 652e 636f 6d22 290d 0a60 6060 0d0a  ple.com")..```..
-00000ab0: 5468 656e 2066 6565 6420 6974 2069 6e74  Then feed it int
-00000ac0: 6f20 4750 542d 342d 5669 7369 6f6e 3a0d  o GPT-4-Vision:.
-00000ad0: 0a60 6060 7079 7468 6f6e 0d0a 7265 7370  .```python..resp
-00000ae0: 6f6e 7365 203d 2063 6c69 656e 742e 6368  onse = client.ch
-00000af0: 6174 2e63 6f6d 706c 6574 696f 6e73 2e63  at.completions.c
-00000b00: 7265 6174 6528 0d0a 2020 2020 6d6f 6465  reate(..    mode
-00000b10: 6c3d 2267 7074 2d34 2d76 6973 696f 6e2d  l="gpt-4-vision-
-00000b20: 7072 6576 6965 7722 2c0d 0a20 2020 206d  preview",..    m
-00000b30: 6573 7361 6765 7320 3d20 6d65 7373 6167  essages = messag
-00000b40: 6573 2c0d 0a29 0d0a 6060 600d 0a0d 0a21  es,..)..```....!
-00000b50: 5b4a 7573 7420 6361 6c6c 204f 7065 6e41  [Just call OpenA
-00000b60: 495d 2868 7474 7073 3a2f 2f72 706e 7574  I](https://rpnut
-00000b70: 7a65 6d75 7462 7275 6d63 7a77 7675 652e  zemutbrumczwvue.
-00000b80: 7375 7061 6261 7365 2e63 6f2f 7374 6f72  supabase.co/stor
-00000b90: 6167 652f 7631 2f6f 626a 6563 742f 7075  age/v1/object/pu
-00000ba0: 626c 6963 2f61 7373 6574 732f 494d 475f  blic/assets/IMG_
-00000bb0: 3031 3830 2e6a 7067 290d 0a0d 0a59 6f75  0180.jpg)....You
-00000bc0: 2063 616e 2061 6c73 6f20 7573 6520 5468   can also use Th
-00000bd0: 6520 5069 7065 2066 726f 6d20 7468 6520  e Pipe from the 
-00000be0: 636f 6d6d 616e 6420 6c69 6e65 2e20 4865  command line. He
-00000bf0: 7265 2773 2068 6f77 2074 6f20 7265 6375  re's how to recu
-00000c00: 7273 6976 656c 7920 6578 7472 6163 7420  rsively extract 
-00000c10: 6672 6f6d 2061 2064 6972 6563 746f 7279  from a directory
-00000c20: 2c20 6d61 7463 6869 6e67 206f 6e6c 7920  , matching only 
-00000c30: 6669 6c65 7320 636f 6e74 6169 6e69 6e67  files containing
-00000c40: 2061 2073 7562 7374 7269 6e67 2028 696e   a substring (in
-00000c50: 2074 6869 7320 6578 616d 706c 652c 2074   this example, t
-00000c60: 7970 6573 6372 6970 7420 6669 6c65 7329  ypescript files)
-00000c70: 2061 6e64 2069 676e 6f72 6520 6669 6c65   and ignore file
-00000c80: 7320 636f 6e74 6169 6e69 6e67 206f 7468  s containing oth
-00000c90: 6572 2073 7562 7374 7269 6e67 7320 2869  er substrings (i
-00000ca0: 6e20 7468 6973 2065 7861 6d70 6c65 2c20  n this example, 
-00000cb0: 616e 7974 6869 6e67 2069 6e20 7468 6520  anything in the 
-00000cc0: 2274 6573 7473 2220 666f 6c64 6572 293a  "tests" folder):
-00000cd0: 0d0a 6060 6062 6173 680d 0a74 6865 7069  ..```bash..thepi
-00000ce0: 7065 2070 6174 682f 746f 2f66 6f6c 6465  pe path/to/folde
-00000cf0: 7220 2d2d 6d61 7463 6820 7473 7820 2d2d  r --match tsx --
-00000d00: 6967 6e6f 7265 2074 6573 7473 0d0a 6060  ignore tests..``
-00000d10: 600d 0a0d 0a0d 0a23 2320 5375 7070 6f72  `......## Suppor
-00000d20: 7465 6420 4669 6c65 2054 7970 6573 20f0  ted File Types .
-00000d30: 9f93 9a0d 0a0d 0a7c 2053 6f75 7263 6520  .......| Source 
-00000d40: 5479 7065 2020 2020 2020 2020 2020 2020  Type            
-00000d50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00000d60: 2049 6e70 7574 2074 7970 6573 2020 2020   Input types    
-00000d70: 2020 2020 7c20 546f 6b65 6e20 436f 6d70      | Token Comp
-00000d80: 7265 7373 696f 6e20 f09f 979c efb8 8f20  ression ....... 
-00000d90: 7c20 496d 6167 6520 4578 7472 6163 7469  | Image Extracti
-00000da0: 6f6e 20f0 9f91 81ef b88f 207c 204e 6f74  on ....... | Not
-00000db0: 6573 20f0 9f93 8c20 2020 2020 2020 2020  es ....         
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 2020 2020 2020 2020 207c 0d0a 7c2d 2d2d           |..|---
-00000df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e10: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00000e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e50: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000e60: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ea0: 7c0d 0a7c 2044 6972 6563 746f 7279 2020  |..| Directory  
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 2020 2020 2020 2020 2020 207c 2041 6e79             | Any
-00000ed0: 2060 2f70 6174 682f 746f 2f64 6972 6563   `/path/to/direc
-00000ee0: 746f 7279 6020 2020 2020 2020 2020 2020  tory`           
-00000ef0: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
-00000f00: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00000f10: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
-00000f20: 2020 2020 7c20 4578 7472 6163 7473 2066      | Extracts f
-00000f30: 726f 6d20 616c 6c20 6669 6c65 7320 696e  rom all files in
-00000f40: 2064 6972 6563 746f 7279 2c20 7375 7070   directory, supp
-00000f50: 6f72 7473 206d 6174 6368 2061 6e64 2069  orts match and i
-00000f60: 676e 6f72 6520 7061 7474 6572 6e73 207c  gnore patterns |
-00000f70: 0d0a 7c20 436f 6465 2020 2020 2020 2020  ..| Code        
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 2020 2020 7c20 602e 7079            | `.py
-00000fa0: 602c 2060 2e74 7378 602c 2060 2e6a 7360  `, `.tsx`, `.js`
-00000fb0: 2c20 602e 6874 6d6c 602c 2060 2e63 7373  , `.html`, `.css
-00000fc0: 602c 2060 2e63 7070 602c 2065 7463 207c  `, `.cpp`, etc |
-00000fd0: 20e2 9c94 efb8 8f20 2876 6172 6965 7329   ...... (varies)
-00000fe0: 2020 207c 20e2 9d8c 2020 2020 2020 2020     | ...        
-00000ff0: 2020 2020 2020 207c 2043 6f6d 6269 6e65         | Combine
-00001000: 7320 616c 6c20 636f 6465 2066 696c 6573  s all code files
-00001010: 2e20 602e 6360 2c20 602e 6370 7060 2c20  . `.c`, `.cpp`, 
-00001020: 602e 7079 6020 6172 6520 636f 6d70 7265  `.py` are compre
-00001030: 7373 6962 6c65 2077 6974 6820 6374 6167  ssible with ctag
-00001040: 732c 206f 7468 6572 7320 6172 6520 6e6f  s, others are no
-00001050: 7420 7c0d 0a7c 2050 6c61 696e 7465 7874  t |..| Plaintext
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-00001080: 2e74 7874 602c 2060 2e6d 6460 2c20 602e  .txt`, `.md`, `.
-00001090: 7274 6660 2c20 6574 6320 2020 2020 2020  rtf`, etc       
-000010a0: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-000010b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000010c0: 20e2 9d8c 2020 2020 2020 2020 2020 2020   ...            
-000010d0: 2020 207c 2052 6567 756c 6172 2074 6578     | Regular tex
-000010e0: 7420 6669 6c65 7320 2020 2020 2020 2020  t files         
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-00001120: 7c20 5044 4620 2020 2020 2020 2020 2020  | PDF           
-00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001140: 2020 2020 2020 2020 7c20 602e 7064 6660          | `.pdf`
-00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 6363 6573 732d 626c 7565 293c 2f61 3e20  ccess-blue)</a> 
+00000350: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000360: 2f64 6973 636f 7264 2e67 672f 6258 664b  /discord.gg/bXfK
+00000370: 6547 7335 7156 223e 215b 4a6f 696e 2064  eGs5qV">![Join d
+00000380: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000390: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
+000003a0: 6973 636f 7264 2f31 3232 3738 3036 3230  iscord/122780620
+000003b0: 3034 3738 3034 3432 3734 3f63 6f6c 6f72  0478044274?color
+000003c0: 3d34 6636 3965 6626 6c61 6265 6c3d 4469  =4f69ef&label=Di
+000003d0: 7363 6f72 6426 6c6f 676f 3d64 6973 636f  scord&logo=disco
+000003e0: 7264 266c 6f67 6f43 6f6c 6f72 3d66 6666  rd&logoColor=fff
+000003f0: 6666 6629 3c2f 613e 0d0a 0d0a 2323 2320  fff)</a>....### 
+00000400: 4665 6564 2050 4446 732c 2055 524c 732c  Feed PDFs, URLs,
+00000410: 2053 6c69 6465 732c 2059 6f75 5475 6265   Slides, YouTube
+00000420: 2076 6964 656f 732c 2057 6f72 6420 646f   videos, Word do
+00000430: 6373 2061 6e64 206d 6f72 6520 696e 746f  cs and more into
+00000440: 2056 6973 696f 6e2d 4c61 6e67 7561 6765   Vision-Language
+00000450: 206d 6f64 656c 7320 7769 7468 206f 6e65   models with one
+00000460: 206c 696e 6520 6f66 2063 6f64 6520 e29a   line of code ..
+00000470: a10d 0a0d 0a54 6865 2050 6970 6520 6973  .....The Pipe is
+00000480: 2061 206d 756c 7469 6d6f 6461 6c2d 6669   a multimodal-fi
+00000490: 7273 7420 746f 6f6c 2066 6f72 2066 6565  rst tool for fee
+000004a0: 6469 6e67 2066 696c 6573 2061 6e64 2077  ding files and w
+000004b0: 6562 2070 6167 6573 2069 6e74 6f20 7669  eb pages into vi
+000004c0: 7369 6f6e 2d6c 616e 6775 6167 6520 6d6f  sion-language mo
+000004d0: 6465 6c73 2073 7563 6820 6173 2047 5054  dels such as GPT
+000004e0: 2d34 562e 2049 7420 6973 2062 6573 7420  -4V. It is best 
+000004f0: 666f 7220 4c4c 4d20 616e 6420 5241 4720  for LLM and RAG 
+00000500: 6170 706c 6963 6174 696f 6e73 2074 6861  applications tha
+00000510: 7420 7761 6e74 2074 6f20 7375 7070 6f72  t want to suppor
+00000520: 7420 636f 6d70 7265 6865 6e73 6976 6520  t comprehensive 
+00000530: 7465 7874 7561 6c20 616e 6420 7669 7375  textual and visu
+00000540: 616c 2075 6e64 6572 7374 616e 6469 6e67  al understanding
+00000550: 2061 6372 6f73 7320 6120 7769 6465 2072   across a wide r
+00000560: 616e 6765 206f 6620 6461 7461 2073 6f75  ange of data sou
+00000570: 7263 6573 2e20 5468 6520 5069 7065 2069  rces. The Pipe i
+00000580: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
+00000590: 2032 342f 3720 686f 7374 6564 2041 5049   24/7 hosted API
+000005a0: 2061 7420 5b74 6865 7069 2e70 655d 2868   at [thepi.pe](h
+000005b0: 7474 7073 3a2f 2f74 6865 7069 2e70 6529  ttps://thepi.pe)
+000005c0: 2c20 6f72 2069 7420 6361 6e20 6265 2073  , or it can be s
+000005d0: 6574 2075 7020 6c6f 6361 6c6c 7920 746f  et up locally to
+000005e0: 206c 6574 2079 6f75 2072 756e 2074 6865   let you run the
+000005f0: 2063 6f6d 7075 7465 2e0d 0a0d 0a21 5b53   compute.....![S
+00000600: 6369 656e 6365 2061 7373 6973 7461 6e74  cience assistant
+00000610: 2064 656d 6f5d 2868 7474 7073 3a2f 2f72   demo](https://r
+00000620: 706e 7574 7a65 6d75 7462 7275 6d63 7a77  pnutzemutbrumczw
+00000630: 7675 652e 7375 7061 6261 7365 2e63 6f2f  vue.supabase.co/
+00000640: 7374 6f72 6167 652f 7631 2f6f 626a 6563  storage/v1/objec
+00000650: 742f 7075 626c 6963 2f61 7373 6574 732f  t/public/assets/
+00000660: 7363 6965 6e63 655f 6173 7369 7374 616e  science_assistan
+00000670: 7470 7932 2e70 6e67 290d 0a0d 0a0d 0a23  tpy2.png)......#
+00000680: 2320 4665 6174 7572 6573 20f0 9f8c 9f0d  # Features .....
+00000690: 0a0d 0a2d 2045 7874 7261 6374 7320 7465  ...- Extracts te
+000006a0: 7874 2061 6e64 2076 6973 7561 6c73 2066  xt and visuals f
+000006b0: 726f 6d20 6669 6c65 7320 6f72 2077 6562  rom files or web
+000006c0: 2070 6167 6573 20f0 9f93 9a0d 0a2d 204f   pages ......- O
+000006d0: 7574 7075 7473 2063 6875 6e6b 7320 6f70  utputs chunks op
+000006e0: 7469 6d69 7a65 6420 666f 7220 6d75 6c74  timized for mult
+000006f0: 696d 6f64 616c 204c 4c4d 7320 616e 6420  imodal LLMs and 
+00000700: 5241 4720 6672 616d 6577 6f72 6b73 20f0  RAG frameworks .
+00000710: 9f96 bcef b88f 0d0a 2d20 496e 7465 7270  ........- Interp
+00000720: 7265 7420 636f 6d70 6c65 7820 5044 4673  ret complex PDFs
+00000730: 2c20 7765 6220 7061 6765 732c 2064 6f63  , web pages, doc
+00000740: 732c 2076 6964 656f 732c 2064 6174 612c  s, videos, data,
+00000750: 2061 6e64 206d 6f72 6520 f09f a7a0 0d0a   and more ......
+00000760: 2d20 4175 746f 2d63 6f6d 7072 6573 7320  - Auto-compress 
+00000770: 7072 6f6d 7074 7320 6578 6365 6564 696e  prompts exceedin
+00000780: 6720 796f 7572 2063 686f 7365 6e20 746f  g your chosen to
+00000790: 6b65 6e20 6c69 6d69 7420 f09f 93a6 0d0a  ken limit ......
+000007a0: 2d20 576f 726b 7320 6576 656e 2077 6974  - Works even wit
+000007b0: 6820 6d69 7373 696e 6720 6669 6c65 2065  h missing file e
+000007c0: 7874 656e 7369 6f6e 732c 2069 6e2d 6d65  xtensions, in-me
+000007d0: 6d6f 7279 2064 6174 6120 7374 7265 616d  mory data stream
+000007e0: 7320 f09f 92be 0d0a 2d20 576f 726b 7320  s ......- Works 
+000007f0: 7769 7468 2063 6f64 6562 6173 6573 2c20  with codebases, 
+00000800: 6769 7420 7265 706f 732c 2061 6e64 2063  git repos, and c
+00000810: 7573 746f 6d20 696e 7465 6772 6174 696f  ustom integratio
+00000820: 6e73 20f0 9f8c 900d 0a2d 204d 756c 7469  ns ......- Multi
+00000830: 2d74 6872 6561 6465 6420 e29a a1ef b88f  -threaded ......
+00000840: 0d0a 0d0a 2323 2047 6574 7469 6e67 2053  ....## Getting S
+00000850: 7461 7274 6564 2020 f09f 9a80 0d0a 0d0a  tarted  ........
+00000860: 5468 6520 5069 7065 2068 616e 646c 6573  The Pipe handles
+00000870: 2061 2077 6964 6520 6172 7261 7920 6f66   a wide array of
+00000880: 2063 6f6d 706c 6578 2066 696c 6574 7970   complex filetyp
+00000890: 6573 2c20 616e 6420 7468 7573 2068 6173  es, and thus has
+000008a0: 206d 616e 7920 6465 7065 6e64 656e 6369   many dependenci
+000008b0: 6573 2074 6861 7420 6d75 7374 2062 6520  es that must be 
+000008c0: 696e 7374 616c 6c65 6420 7365 7061 7261  installed separa
+000008d0: 7465 6c79 2e20 4974 2061 6c73 6f20 7265  tely. It also re
+000008e0: 7175 6972 6573 2061 2073 7472 6f6e 6720  quires a strong 
+000008f0: 6d61 6368 696e 6520 666f 7220 676f 6f64  machine for good
+00000900: 2072 6573 706f 6e73 6520 7469 6d65 732e   response times.
+00000910: 2046 6f72 2074 6869 7320 7265 6173 6f6e   For this reason
+00000920: 2c20 7765 2068 6f73 7420 6974 2061 7320  , we host it as 
+00000930: 616e 2041 5049 2074 6861 7420 776f 726b  an API that work
+00000940: 7320 6f75 742d 6f66 2d74 6865 2d62 6f78  s out-of-the-box
+00000950: 2e20 0d0a 0d0a 4669 7273 742c 2069 6e73  . ....First, ins
+00000960: 7461 6c6c 2054 6865 2050 6970 652e 200d  tall The Pipe. .
+00000970: 0a60 6060 0d0a 7069 7020 696e 7374 616c  .```..pip instal
+00000980: 6c20 7468 6570 6970 655f 6170 690d 0a60  l thepipe_api..`
+00000990: 6060 0d0a 0d0a 5468 6520 5069 7065 2069  ``....The Pipe i
+000009a0: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
+000009b0: 2068 6f73 7465 6420 4150 492c 206f 7220   hosted API, or 
+000009c0: 6974 2063 616e 2062 6520 7365 7420 7570  it can be set up
+000009d0: 206c 6f63 616c 6c79 2e20 416e 2041 5049   locally. An API
+000009e0: 206b 6579 2069 7320 7265 636f 6d6d 656e   key is recommen
+000009f0: 6465 6420 666f 7220 6f75 742d 6f66 2d74  ded for out-of-t
+00000a00: 6865 2d62 6f78 2066 756e 6374 696f 6e61  he-box functiona
+00000a10: 6c69 7479 2028 616c 7465 726e 6174 6976  lity (alternativ
+00000a20: 656c 792c 2073 6565 2074 6865 206c 6f63  ely, see the loc
+00000a30: 616c 2069 6e73 7461 6c6c 6174 696f 6e20  al installation 
+00000a40: 7365 6374 696f 6e29 2e20 456e 7375 7265  section). Ensure
+00000a50: 2074 6865 2060 5448 4550 4950 455f 4150   the `THEPIPE_AP
+00000a60: 495f 4b45 5960 2065 6e76 6972 6f6e 6d65  I_KEY` environme
+00000a70: 6e74 2076 6172 6961 626c 6520 6973 2073  nt variable is s
+00000a80: 6574 2e20 446f 6e27 7420 6861 7665 2061  et. Don't have a
+00000a90: 206b 6579 2079 6574 3f20 5b47 6574 206f   key yet? [Get o
+00000aa0: 6e65 2068 6572 655d 2868 7474 7073 3a2f  ne here](https:/
+00000ab0: 2f74 6865 7069 2e70 6529 2e0d 0a0d 0a4e  /thepi.pe).....N
+00000ac0: 6f77 2079 6f75 2063 616e 2065 7874 7261  ow you can extra
+00000ad0: 6374 2063 6f6d 7072 6568 656e 7369 7665  ct comprehensive
+00000ae0: 2074 6578 7420 616e 6420 7669 7375 616c   text and visual
+00000af0: 7320 6672 6f6d 2061 6e79 2066 696c 653a  s from any file:
+00000b00: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+00000b10: 6d20 7468 6570 6970 655f 6170 6920 696d  m thepipe_api im
+00000b20: 706f 7274 2074 6865 7069 7065 0d0a 6d65  port thepipe..me
+00000b30: 7373 6167 6573 203d 2074 6865 7069 7065  ssages = thepipe
+00000b40: 2e65 7874 7261 6374 2822 6578 616d 706c  .extract("exampl
+00000b50: 652e 7064 6622 290d 0a60 6060 0d0a 4f72  e.pdf")..```..Or
+00000b60: 2077 6562 7369 7465 733a 0d0a 6060 6070   websites:..```p
+00000b70: 7974 686f 6e0d 0a6d 6573 7361 6765 7320  ython..messages 
+00000b80: 3d20 7468 6570 6970 652e 6578 7472 6163  = thepipe.extrac
+00000b90: 7428 2268 7474 7073 3a2f 2f65 7861 6d70  t("https://examp
+00000ba0: 6c65 2e63 6f6d 2229 0d0a 6060 600d 0a54  le.com")..```..T
+00000bb0: 6865 6e20 6665 6564 2069 7420 696e 746f  hen feed it into
+00000bc0: 2047 5054 2d34 2d56 6973 696f 6e3a 0d0a   GPT-4-Vision:..
+00000bd0: 6060 6070 7974 686f 6e0d 0a72 6573 706f  ```python..respo
+00000be0: 6e73 6520 3d20 636c 6965 6e74 2e63 6861  nse = client.cha
+00000bf0: 742e 636f 6d70 6c65 7469 6f6e 732e 6372  t.completions.cr
+00000c00: 6561 7465 280d 0a20 2020 206d 6f64 656c  eate(..    model
+00000c10: 3d22 6770 742d 342d 7669 7369 6f6e 2d70  ="gpt-4-vision-p
+00000c20: 7265 7669 6577 222c 0d0a 2020 2020 6d65  review",..    me
+00000c30: 7373 6167 6573 203d 206d 6573 7361 6765  ssages = message
+00000c40: 732c 0d0a 290d 0a60 6060 0d0a 0d0a 215b  s,..)..```....![
+00000c50: 4a75 7374 2063 616c 6c20 4f70 656e 4149  Just call OpenAI
+00000c60: 5d28 6874 7470 733a 2f2f 7270 6e75 747a  ](https://rpnutz
+00000c70: 656d 7574 6272 756d 637a 7776 7565 2e73  emutbrumczwvue.s
+00000c80: 7570 6162 6173 652e 636f 2f73 746f 7261  upabase.co/stora
+00000c90: 6765 2f76 312f 6f62 6a65 6374 2f70 7562  ge/v1/object/pub
+00000ca0: 6c69 632f 6173 7365 7473 2f49 4d47 5f30  lic/assets/IMG_0
+00000cb0: 3138 302e 6a70 6729 0d0a 0d0a 596f 7520  180.jpg)....You 
+00000cc0: 6361 6e20 616c 736f 2075 7365 2054 6865  can also use The
+00000cd0: 2050 6970 6520 6672 6f6d 2074 6865 2063   Pipe from the c
+00000ce0: 6f6d 6d61 6e64 206c 696e 652e 2048 6572  ommand line. Her
+00000cf0: 6527 7320 686f 7720 746f 2072 6563 7572  e's how to recur
+00000d00: 7369 7665 6c79 2065 7874 7261 6374 2066  sively extract f
+00000d10: 726f 6d20 6120 6469 7265 6374 6f72 792c  rom a directory,
+00000d20: 206d 6174 6368 696e 6720 6f6e 6c79 2066   matching only f
+00000d30: 696c 6573 2063 6f6e 7461 696e 696e 6720  iles containing 
+00000d40: 6120 7375 6273 7472 696e 6720 2869 6e20  a substring (in 
+00000d50: 7468 6973 2065 7861 6d70 6c65 2c20 7479  this example, ty
+00000d60: 7065 7363 7269 7074 2066 696c 6573 2920  pescript files) 
+00000d70: 616e 6420 6967 6e6f 7265 2066 696c 6573  and ignore files
+00000d80: 2063 6f6e 7461 696e 696e 6720 6f74 6865   containing othe
+00000d90: 7220 7375 6273 7472 696e 6773 2028 696e  r substrings (in
+00000da0: 2074 6869 7320 6578 616d 706c 652c 2061   this example, a
+00000db0: 6e79 7468 696e 6720 696e 2074 6865 2022  nything in the "
+00000dc0: 7465 7374 7322 2066 6f6c 6465 7229 3a0d  tests" folder):.
+00000dd0: 0a60 6060 6261 7368 0d0a 7468 6570 6970  .```bash..thepip
+00000de0: 6520 7061 7468 2f74 6f2f 666f 6c64 6572  e path/to/folder
+00000df0: 202d 2d6d 6174 6368 2074 7378 202d 2d69   --match tsx --i
+00000e00: 676e 6f72 6520 7465 7374 730d 0a60 6060  gnore tests..```
+00000e10: 0d0a 0d0a 0d0a 2323 2053 7570 706f 7274  ......## Support
+00000e20: 6564 2046 696c 6520 5479 7065 7320 f09f  ed File Types ..
+00000e30: 939a 0d0a 0d0a 7c20 536f 7572 6365 2054  ......| Source T
+00000e40: 7970 6520 2020 2020 2020 2020 2020 2020  ype             
+00000e50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00000e60: 496e 7075 7420 7479 7065 7320 2020 2020  Input types     
+00000e70: 2020 207c 2054 6f6b 656e 2043 6f6d 7072     | Token Compr
+00000e80: 6573 7369 6f6e 20f0 9f97 9cef b88f 207c  ession ....... |
+00000e90: 2049 6d61 6765 2045 7874 7261 6374 696f   Image Extractio
+00000ea0: 6e20 f09f 9181 efb8 8f20 7c20 4e6f 7465  n ....... | Note
+00000eb0: 7320 f09f 938c 2020 2020 2020 2020 2020  s ....          
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ee0: 2020 2020 2020 2020 7c0d 0a7c 2d2d 2d2d          |..|----
+00000ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f10: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
+00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
+00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f50: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00000f60: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00000f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00000fa0: 0d0a 7c20 4469 7265 6374 6f72 7920 2020  ..| Directory   
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fc0: 2020 2020 2020 2020 2020 7c20 416e 7920            | Any 
+00000fd0: 602f 7061 7468 2f74 6f2f 6469 7265 6374  `/path/to/direct
+00000fe0: 6f72 7960 2020 2020 2020 2020 2020 2020  ory`            
+00000ff0: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
+00001000: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00001010: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+00001020: 2020 207c 2045 7874 7261 6374 7320 6672     | Extracts fr
+00001030: 6f6d 2061 6c6c 2066 696c 6573 2069 6e20  om all files in 
+00001040: 6469 7265 6374 6f72 792c 2073 7570 706f  directory, suppo
+00001050: 7274 7320 6d61 7463 6820 616e 6420 6967  rts match and ig
+00001060: 6e6f 7265 2070 6174 7465 726e 7320 7c0d  nore patterns |.
+00001070: 0a7c 2043 6f64 6520 2020 2020 2020 2020  .| Code         
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 2020 2020 2020 2020 207c 2060 2e70 7960           | `.py`
+000010a0: 2c20 602e 7473 7860 2c20 602e 6a73 602c  , `.tsx`, `.js`,
+000010b0: 2060 2e68 746d 6c60 2c20 602e 6373 7360   `.html`, `.css`
+000010c0: 2c20 602e 6370 7060 2c20 6574 6320 7c20  , `.cpp`, etc | 
+000010d0: e29c 94ef b88f 2028 7661 7269 6573 2920  ...... (varies) 
+000010e0: 2020 7c20 e29d 8c20 2020 2020 2020 2020    | ...         
+000010f0: 2020 2020 2020 7c20 436f 6d62 696e 6573        | Combines
+00001100: 2061 6c6c 2063 6f64 6520 6669 6c65 732e   all code files.
+00001110: 2060 2e63 602c 2060 2e63 7070 602c 2060   `.c`, `.cpp`, `
+00001120: 2e70 7960 2061 7265 2063 6f6d 7072 6573  .py` are compres
+00001130: 7369 626c 6520 7769 7468 2063 7461 6773  sible with ctags
+00001140: 2c20 6f74 6865 7273 2061 7265 206e 6f74  , others are not
+00001150: 207c 0d0a 7c20 506c 6169 6e74 6578 7420   |..| Plaintext 
 00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
-00001180: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
-00001190: 8f20 2020 207c 2045 7874 7261 6374 7320  .    | Extracts 
-000011a0: 7465 7874 2061 6e64 2069 6d61 6765 7320  text and images 
-000011b0: 6f66 2065 6163 6820 7061 6765 3b20 6361  of each page; ca
-000011c0: 6e20 7573 6520 4149 2066 6f72 2065 7874  n use AI for ext
-000011d0: 7261 6374 696f 6e20 6f66 2074 6162 6c65  raction of table
-000011e0: 2064 6174 6120 616e 6420 2069 6d61 6765   data and  image
-000011f0: 7320 7769 7468 696e 2070 6167 6573 207c  s within pages |
-00001200: 0d0a 7c20 496d 6167 6520 2020 2020 2020  ..| Image       
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 2020 7c20 602e 6a70            | `.jp
-00001230: 6760 2c20 602e 6a70 6567 602c 2060 2e70  g`, `.jpeg`, `.p
-00001240: 6e67 6020 7c20 e29d 8c20 2020 2020 2020  ng` | ...       
-00001250: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
-00001260: 8f20 2020 2020 2020 2020 2020 2020 207c  .              |
-00001270: 2045 7874 7261 6374 7320 696d 6167 6573   Extracts images
-00001280: 2c20 7573 6573 204f 4352 2069 6620 7465  , uses OCR if te
-00001290: 7874 5f6f 6e6c 7920 2020 2020 2020 2020  xt_only         
-000012a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000012b0: 0d0a 7c20 4461 7461 2054 6162 6c65 2020  ..| Data Table  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 207c 2060 2e63 7376           | `.csv
-000012e0: 602c 2060 2e78 6c73 602c 2060 2e78 6c73  `, `.xls`, `.xls
-000012f0: 7860 2020 2020 2020 2020 2020 2020 207c  x`             |
-00001300: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
-00001310: 2020 2020 2020 207c 20e2 9d8c 2020 2020         | ...    
-00001320: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
-00001330: 7261 6374 7320 6461 7461 2066 726f 6d20  racts data from 
-00001340: 7370 7265 6164 7368 6565 7473 3b20 636f  spreadsheets; co
-00001350: 6e76 6572 7473 2074 6f20 7465 7874 2072  nverts to text r
-00001360: 6570 7265 7365 6e74 6174 696f 6e2e 2046  epresentation. F
-00001370: 6f72 2076 6572 7920 6c61 7267 6520 6461  or very large da
-00001380: 7461 7365 7473 2c20 7769 6c6c 206f 6e6c  tasets, will onl
-00001390: 7920 6578 7472 6163 7420 636f 6c75 6d6e  y extract column
-000013a0: 206e 616d 6573 2061 6e64 2074 7970 6573   names and types
-000013b0: 2020 2020 2020 2020 207c 0d0a 7c20 4a75           |..| Ju
-000013c0: 7079 7465 7220 4e6f 7465 626f 6f6b 2020  pyter Notebook  
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 2020 2020 7c20 602e 6970 796e 6260 2020      | `.ipynb`  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001410: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
-00001420: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
-00001430: 2020 2020 2020 2020 207c 2045 7874 7261           | Extra
-00001440: 6374 7320 636f 6465 2c20 6d61 726b 646f  cts code, markdo
-00001450: 776e 2c20 616e 6420 696d 6167 6573 2066  wn, and images f
-00001460: 726f 6d20 4a75 7079 7465 7220 6e6f 7465  rom Jupyter note
-00001470: 626f 6f6b 7320 2020 2020 2020 2020 2020  books           
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 207c 0d0a 7c20 4d69 6372         |..| Micr
-000014a0: 6f73 6f66 7420 576f 7264 2044 6f63 756d  osoft Word Docum
-000014b0: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
-000014c0: 2020 7c20 602e 646f 6378 6020 2020 2020    | `.docx`     
+00001170: 2020 2020 2020 2020 2020 2020 7c20 602e              | `.
+00001180: 7478 7460 2c20 602e 6d64 602c 2060 2e72  txt`, `.md`, `.r
+00001190: 7466 602c 2065 7463 2020 2020 2020 2020  tf`, etc        
+000011a0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+000011b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000011c0: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
+000011d0: 2020 7c20 5265 6775 6c61 7220 7465 7874    | Regular text
+000011e0: 2066 696c 6573 2020 2020 2020 2020 2020   files          
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
+00001220: 2050 4446 2020 2020 2020 2020 2020 2020   PDF            
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 2020 2020 207c 2060 2e70 6466 6020         | `.pdf` 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001270: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
+00001280: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
+00001290: 2020 2020 7c20 4578 7472 6163 7473 2074      | Extracts t
+000012a0: 6578 7420 616e 6420 696d 6167 6573 206f  ext and images o
+000012b0: 6620 6561 6368 2070 6167 653b 2063 616e  f each page; can
+000012c0: 2075 7365 2041 4920 666f 7220 6578 7472   use AI for extr
+000012d0: 6163 7469 6f6e 206f 6620 7461 626c 6520  action of table 
+000012e0: 6461 7461 2061 6e64 2020 696d 6167 6573  data and  images
+000012f0: 2077 6974 6869 6e20 7061 6765 7320 7c0d   within pages |.
+00001300: 0a7c 2049 6d61 6765 2020 2020 2020 2020  .| Image        
+00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2020 2020 2020 2020 207c 2060 2e6a 7067           | `.jpg
+00001330: 602c 2060 2e6a 7065 6760 2c20 602e 706e  `, `.jpeg`, `.pn
+00001340: 6760 207c 20e2 9d8c 2020 2020 2020 2020  g` | ...        
+00001350: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
+00001360: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001370: 4578 7472 6163 7473 2069 6d61 6765 732c  Extracts images,
+00001380: 2075 7365 7320 4f43 5220 6966 2074 6578   uses OCR if tex
+00001390: 745f 6f6e 6c79 2020 2020 2020 2020 2020  t_only          
+000013a0: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+000013b0: 0a7c 2044 6174 6120 5461 626c 6520 2020  .| Data Table   
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 2020 2020 2020 7c20 602e 6373 7660          | `.csv`
+000013e0: 2c20 602e 786c 7360 2c20 602e 786c 7378  , `.xls`, `.xlsx
+000013f0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
+00001400: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
+00001410: 2020 2020 2020 7c20 e29d 8c20 2020 2020        | ...     
+00001420: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+00001430: 6163 7473 2064 6174 6120 6672 6f6d 2073  acts data from s
+00001440: 7072 6561 6473 6865 6574 733b 2063 6f6e  preadsheets; con
+00001450: 7665 7274 7320 746f 2074 6578 7420 7265  verts to text re
+00001460: 7072 6573 656e 7461 7469 6f6e 2e20 466f  presentation. Fo
+00001470: 7220 7665 7279 206c 6172 6765 2064 6174  r very large dat
+00001480: 6173 6574 732c 2077 696c 6c20 6f6e 6c79  asets, will only
+00001490: 2065 7874 7261 6374 2063 6f6c 756d 6e20   extract column 
+000014a0: 6e61 6d65 7320 616e 6420 7479 7065 7320  names and types 
+000014b0: 2020 2020 2020 2020 7c0d 0a7c 204a 7570          |..| Jup
+000014c0: 7974 6572 204e 6f74 6562 6f6f 6b20 2020  yter Notebook   
 000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-000014f0: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-00001500: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-00001510: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-00001520: 6163 7473 2074 6578 7420 616e 6420 696d  acts text and im
-00001530: 6167 6573 2066 726f 6d20 576f 7264 2064  ages from Word d
-00001540: 6f63 756d 656e 7473 2020 2020 2020 2020  ocuments        
-00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 7c0d 0a7c 204d 6963 726f 736f 6674 2050  |..| Microsoft P
-00001580: 6f77 6572 506f 696e 7420 5072 6573 656e  owerPoint Presen
-00001590: 7461 7469 6f6e 2020 2020 207c 2060 2e70  tation     | `.p
-000015a0: 7074 7860 2020 2020 2020 2020 2020 2020  ptx`            
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
-000015d0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-000015e0: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-000015f0: 2020 207c 2045 7874 7261 6374 7320 7465     | Extracts te
-00001600: 7874 2061 6e64 2069 6d61 6765 7320 6672  xt and images fr
-00001610: 6f6d 2050 6f77 6572 506f 696e 7420 7072  om PowerPoint pr
-00001620: 6573 656e 7461 7469 6f6e 7320 2020 2020  esentations     
-00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 2020 2020 2020 207c 0d0a 7c20 5669           |..| Vi
-00001650: 6465 6f20 2020 2020 2020 2020 2020 2020  deo             
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 7c20 602e 6d70 3460 2c20 602e      | `.mp4`, `.
-00001680: 6176 6960 2c20 602e 6d6f 7660 2c20 602e  avi`, `.mov`, `.
-00001690: 776d 7660 2020 2020 207c 20e2 9c94 efb8  wmv`     | .....
-000016a0: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
-000016b0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-000016c0: 2020 2020 2020 2020 7c20 4578 7472 6163          | Extrac
-000016d0: 7473 2066 7261 6d65 7320 6672 6f6d 2076  ts frames from v
-000016e0: 6964 656f 2066 696c 6573 3b20 7375 7070  ideo files; supp
-000016f0: 6f72 7473 2066 7261 6d65 2065 7874 7261  orts frame extra
-00001700: 6374 696f 6e20 616e 6420 4f43 5220 666f  ction and OCR fo
-00001710: 7220 7465 7874 2065 7874 7261 6374 696f  r text extractio
-00001720: 6e20 6672 6f6d 2066 7261 6d65 7320 7c0d  n from frames |.
-00001730: 0a7c 2041 7564 696f 2020 2020 2020 2020  .| Audio        
-00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001750: 2020 2020 2020 2020 207c 2060 2e6d 7033           | `.mp3
-00001760: 602c 2060 2e77 6176 6020 2020 2020 2020  `, `.wav`       
-00001770: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-00001780: 2020 2020 2020 2020 2020 7c20 e29d 8c20            | ... 
-00001790: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000017a0: 2045 7874 7261 6374 7320 7465 7874 2066   Extracts text f
-000017b0: 726f 6d20 6175 6469 6f20 6669 6c65 733b  rom audio files;
-000017c0: 2073 7570 706f 7274 7320 7370 6565 6368   supports speech
-000017d0: 2d74 6f2d 7465 7874 2063 6f6e 7665 7273  -to-text convers
-000017e0: 696f 6e20 2020 2020 2020 207c 200d 0a7c  ion        | ..|
-000017f0: 2057 6562 7369 7465 2020 2020 2020 2020   Website        
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 207c 2055 524c 7320 2869         | URLs (i
-00001820: 6e70 7574 7320 636f 6e74 6169 6e69 6e67  nputs containing
-00001830: 2060 6874 7470 602c 2060 6874 7470 7360   `http`, `https`
-00001840: 2c20 6066 7470 6029 2020 2020 2020 2020  , `ftp`)        
-00001850: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
-00001860: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00001870: 9c94 efb8 8f20 2020 207c 2045 7874 7261  .....    | Extra
-00001880: 6374 7320 7465 7874 2066 726f 6d20 7765  cts text from we
-00001890: 6220 7061 6765 2061 6c6f 6e67 2077 6974  b page along wit
-000018a0: 6820 696d 6167 6520 286f 7220 696d 6167  h image (or imag
-000018b0: 6573 2069 6620 7363 726f 6c6c 6162 6c65  es if scrollable
-000018c0: 293b 2074 6578 742d 6f6e 6c79 2065 7874  ); text-only ext
-000018d0: 7261 6374 696f 6e20 6176 6169 6c61 626c  raction availabl
-000018e0: 6520 2020 2020 2020 2020 207c 0d0a 7c20  e          |..| 
-000018f0: 4769 7448 7562 2052 6570 6f73 6974 6f72  GitHub Repositor
-00001900: 7920 2020 2020 2020 2020 2020 2020 2020  y               
-00001910: 2020 2020 2020 7c20 4769 7448 7562 2072        | GitHub r
-00001920: 6570 6f20 5552 4c73 2020 2020 2020 2020  epo URLs        
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
-00001950: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 7c20 4578 7472 6163 7473 2066 726f 6d20  | Extracts from 
-00001980: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
-00001990: 6965 733b 2073 7570 706f 7274 7320 6272  ies; supports br
-000019a0: 616e 6368 2073 7065 6369 6669 6361 7469  anch specificati
-000019b0: 6f6e 2020 2020 2020 2020 207c 0d0a 7c20  on         |..| 
-000019c0: 596f 7554 7562 6520 5669 6465 6f20 2020  YouTube Video   
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 2020 2020 2020 7c20 596f 7554 7562 6520        | YouTube 
-000019f0: 7669 6465 6f20 5552 4c73 2020 2020 2020  video URLs      
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-00001a20: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001a30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001a40: 2045 7874 7261 6374 7320 7465 7874 2066   Extracts text f
-00001a50: 726f 6d20 596f 7554 7562 6520 7669 6465  rom YouTube vide
-00001a60: 6f73 3b20 7375 7070 6f72 7473 2073 7562  os; supports sub
-00001a70: 7469 746c 6573 2065 7874 7261 6374 696f  titles extractio
-00001a80: 6e20 2020 2020 2020 2020 207c 0d0a 7c20  n          |..| 
-00001a90: 5a49 5020 4669 6c65 2020 2020 2020 2020  ZIP File        
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 2020 2020 7c20 602e 7a69 7060 2020        | `.zip`  
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-00001af0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001b00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001b10: 2045 7874 7261 6374 7320 636f 6e74 656e   Extracts conten
-00001b20: 7473 206f 6620 5a49 5020 6669 6c65 733b  ts of ZIP files;
-00001b30: 2073 7570 706f 7274 7320 6e65 7374 6564   supports nested
-00001b40: 2064 6972 6563 746f 7279 2065 7874 7261   directory extra
-00001b50: 6374 696f 6e20 2020 2020 7c0d 0a0d 0a23  ction     |....#
-00001b60: 2320 486f 7720 6974 2077 6f72 6b73 20f0  # How it works .
-00001b70: 9f9b a0ef b88f 0d0a 0d0a 5468 6520 696e  ..........The in
-00001b80: 7075 7420 736f 7572 6365 2069 7320 6569  put source is ei
-00001b90: 7468 6572 2061 2066 696c 6520 7061 7468  ther a file path
-00001ba0: 2c20 6120 5552 4c2c 206f 7220 6120 6469  , a URL, or a di
-00001bb0: 7265 6374 6f72 792e 2054 6865 2070 6970  rectory. The pip
-00001bc0: 6520 7769 6c6c 2065 7874 7261 6374 2069  e will extract i
-00001bd0: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d20  nformation from 
-00001be0: 7468 6520 736f 7572 6365 2061 6e64 2070  the source and p
-00001bf0: 726f 6365 7373 2069 7420 666f 7220 646f  rocess it for do
-00001c00: 776e 7374 7265 616d 2075 7365 2077 6974  wnstream use wit
-00001c10: 6820 5b6c 616e 6775 6167 6520 6d6f 6465  h [language mode
-00001c20: 6c73 5d28 6874 7470 733a 2f2f 656e 2e77  ls](https://en.w
-00001c30: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00001c40: 692f 4c61 7267 655f 6c61 6e67 7561 6765  i/Large_language
-00001c50: 5f6d 6f64 656c 292c 205b 7669 7369 6f6e  _model), [vision
-00001c60: 2074 7261 6e73 666f 726d 6572 735d 2868   transformers](h
-00001c70: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00001c80: 6469 612e 6f72 672f 7769 6b69 2f56 6973  dia.org/wiki/Vis
-00001c90: 696f 6e5f 7472 616e 7366 6f72 6d65 7229  ion_transformer)
-00001ca0: 2c20 6f72 205b 7669 7369 6f6e 2d6c 616e  , or [vision-lan
-00001cb0: 6775 6167 6520 6d6f 6465 6c73 5d28 6874  guage models](ht
-00001cc0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00001cd0: 6162 732f 3233 3034 2e30 3036 3835 292e  abs/2304.00685).
-00001ce0: 2054 6865 206f 7574 7075 7420 6672 6f6d   The output from
-00001cf0: 2074 6865 2070 6970 6520 6973 2061 2073   the pipe is a s
-00001d00: 656e 7369 626c 6520 6c69 7374 206f 6620  ensible list of 
-00001d10: 6d75 6c74 696d 6f64 616c 206d 6573 7361  multimodal messa
-00001d20: 6765 7320 7265 7072 6573 656e 7469 6e67  ges representing
-00001d30: 2063 6875 6e6b 7320 6f66 2074 6865 2065   chunks of the e
-00001d40: 7874 7261 6374 6564 2069 6e66 6f72 6d61  xtracted informa
-00001d50: 7469 6f6e 2c20 6361 7265 6675 6c6c 7920  tion, carefully 
-00001d60: 6372 6166 7465 6420 746f 2066 6974 2077  crafted to fit w
-00001d70: 6974 6869 6e20 636f 6e74 6578 7420 7769  ithin context wi
-00001d80: 6e64 6f77 7320 666f 7220 616e 7920 6d6f  ndows for any mo
-00001d90: 6465 6c73 2066 726f 6d20 5b67 656d 6d61  dels from [gemma
-00001da0: 2d37 625d 2868 7474 7073 3a2f 2f68 7567  -7b](https://hug
-00001db0: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
-00001dc0: 6c65 2f67 656d 6d61 2d37 6229 2074 6f20  le/gemma-7b) to 
-00001dd0: 5b47 5054 2d34 5d28 6874 7470 733a 2f2f  [GPT-4](https://
-00001de0: 6f70 656e 6169 2e63 6f6d 2f67 7074 2d34  openai.com/gpt-4
-00001df0: 292e 2054 6865 206d 6573 7361 6765 7320  ). The messages 
-00001e00: 7265 7475 726e 6564 2073 686f 756c 6420  returned should 
-00001e10: 6c6f 6f6b 206c 696b 6520 7468 6973 3a0d  look like this:.
-00001e20: 0a60 6060 6a73 6f6e 0d0a 5b0d 0a20 207b  .```json..[..  {
-00001e30: 0d0a 2020 2020 2272 6f6c 6522 3a20 2275  ..    "role": "u
-00001e40: 7365 7222 2c0d 0a20 2020 2022 636f 6e74  ser",..    "cont
-00001e50: 656e 7422 3a20 5b0d 0a20 2020 2020 207b  ent": [..      {
-00001e60: 0d0a 2020 2020 2020 2020 2274 7970 6522  ..        "type"
-00001e70: 3a20 2274 6578 7422 2c0d 0a20 2020 2020  : "text",..     
-00001e80: 2020 2022 7465 7874 223a 2022 2e2e 2e22     "text": "..."
-00001e90: 0d0a 2020 2020 2020 7d2c 0d0a 2020 2020  ..      },..    
-00001ea0: 2020 7b0d 0a20 2020 2020 2020 2022 7479    {..        "ty
-00001eb0: 7065 223a 2022 696d 6167 655f 7572 6c22  pe": "image_url"
-00001ec0: 2c0d 0a20 2020 2020 2020 2022 696d 6167  ,..        "imag
-00001ed0: 655f 7572 6c22 3a20 7b0d 0a20 2020 2020  e_url": {..     
-00001ee0: 2020 2020 2022 7572 6c22 3a20 2264 6174       "url": "dat
-00001ef0: 613a 696d 6167 652f 6a70 6567 3b62 6173  a:image/jpeg;bas
-00001f00: 6536 342c 2e2e 2e22 0d0a 2020 2020 2020  e64,..."..      
-00001f10: 2020 7d0d 0a20 2020 2020 207d 0d0a 2020    }..      }..  
-00001f20: 2020 5d0d 0a20 207d 0d0a 5d0d 0a60 6060    ]..  }..]..```
-00001f30: 0d0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
-00001f40: 2066 6565 6420 7468 6573 6520 6d65 7373   feed these mess
-00001f50: 6167 6573 2064 6972 6563 746c 7920 696e  ages directly in
-00001f60: 746f 2074 6865 206d 6f64 656c 2c20 6974  to the model, it
-00001f70: 2069 7320 696d 706f 7274 616e 7420 746f   is important to
-00001f80: 2062 6520 6d69 6e64 6675 6c20 6f66 2074   be mindful of t
-00001f90: 6865 2074 6f6b 656e 206c 696d 6974 2e0d  he token limit..
-00001fa0: 0a4f 7065 6e41 4920 646f 6573 206e 6f74  .OpenAI does not
-00001fb0: 2061 6c6c 6f77 2074 6f6f 206d 616e 7920   allow too many 
-00001fc0: 696d 6167 6573 2069 6e20 7468 6520 7072  images in the pr
-00001fd0: 6f6d 7074 2028 7365 6520 6469 7363 7573  ompt (see discus
-00001fe0: 7369 6f6e 205b 6865 7265 5d28 6874 7470  sion [here](http
-00001ff0: 733a 2f2f 636f 6d6d 756e 6974 792e 6f70  s://community.op
-00002000: 656e 6169 2e63 6f6d 2f74 2f67 7074 2d34  enai.com/t/gpt-4
-00002010: 2d76 6973 696f 6e2d 6d61 7869 6d75 6d2d  -vision-maximum-
-00002020: 616d 6f75 6e74 2d6f 662d 696d 6167 6573  amount-of-images
-00002030: 2f35 3733 3131 302f 3629 292c 2073 6f20  /573110/6)), so 
-00002040: 6c6f 6e67 2066 696c 6573 2073 686f 756c  long files shoul
-00002050: 6420 6265 2065 7874 7261 6374 6564 2077  d be extracted w
-00002060: 6974 6820 6074 6578 745f 6f6e 6c79 3d54  ith `text_only=T
-00002070: 7275 6560 2074 6f20 6176 6f69 6420 7468  rue` to avoid th
-00002080: 6973 2069 7373 7565 2c20 7768 696c 6520  is issue, while 
-00002090: 6c6f 6e67 2074 6578 7420 6669 6c65 7320  long text files 
-000020a0: 7368 6f75 6c64 2065 6974 6865 7220 6265  should either be
-000020b0: 2063 6f6d 7072 6573 7365 6420 6f72 2065   compressed or e
-000020c0: 6d62 6564 6465 6420 696e 2061 2052 4147  mbedded in a RAG
-000020d0: 2066 7261 6d65 776f 726b 2e0d 0a0d 0a54   framework.....T
-000020e0: 6865 2074 6578 7420 616e 6420 696d 6167  he text and imag
-000020f0: 6573 2066 726f 6d20 7468 6573 6520 6d65  es from these me
-00002100: 7373 6167 6573 206d 6179 2061 6c73 6f20  ssages may also 
-00002110: 6265 2070 7265 7061 7265 6420 666f 7220  be prepared for 
-00002120: 6120 7665 6374 6f72 2064 6174 6162 6173  a vector databas
-00002130: 6520 7769 7468 2060 7468 6570 6970 652e  e with `thepipe.
-00002140: 636f 7265 2e63 7265 6174 655f 6368 756e  core.create_chun
-00002150: 6b73 5f66 726f 6d5f 6d65 7373 6167 6573  ks_from_messages
-00002160: 6020 6f72 2066 6f72 2064 6f77 6e73 7472  ` or for downstr
-00002170: 6561 6d20 7573 6520 7769 7468 2052 4147  eam use with RAG
-00002180: 2066 7261 6d65 776f 726b 732e 205b 4c69   frameworks. [Li
-00002190: 7465 4c4c 4d5d 2868 7474 7073 3a2f 2f67  teLLM](https://g
-000021a0: 6974 6875 622e 636f 6d2f 4265 7272 6941  ithub.com/BerriA
-000021b0: 492f 6c69 7465 6c6c 6d29 2063 616e 2062  I/litellm) can b
-000021c0: 6520 7573 6564 2074 6f20 6561 7369 6c79  e used to easily
-000021d0: 2069 6e74 6567 7261 7465 2054 6865 2050   integrate The P
-000021e0: 6970 6520 7769 7468 2061 6e79 204c 4c4d  ipe with any LLM
-000021f0: 2070 726f 7669 6465 722e 200d 0a0d 0a49   provider. ....I
-00002200: 7420 7573 6573 2061 2076 6172 6965 7479  t uses a variety
-00002210: 206f 6620 6865 7572 6973 7469 6373 2066   of heuristics f
-00002220: 6f72 206f 7074 696d 616c 2070 6572 666f  or optimal perfo
-00002230: 726d 616e 6365 2077 6974 6820 7669 7369  rmance with visi
-00002240: 6f6e 2d6c 616e 6775 6167 6520 6d6f 6465  on-language mode
-00002250: 6c73 2c20 696e 636c 7564 696e 6720 4149  ls, including AI
-00002260: 2066 696c 6574 7970 6520 6465 7465 6374   filetype detect
-00002270: 696f 6e20 7769 7468 205b 6669 6c65 7479  ion with [filety
-00002280: 7065 2064 6574 6563 7469 6f6e 5d28 6874  pe detection](ht
-00002290: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
-000022a0: 2e67 6f6f 676c 6562 6c6f 672e 636f 6d2f  .googleblog.com/
-000022b0: 3230 3234 2f30 322f 6d61 6769 6b61 2d61  2024/02/magika-a
-000022c0: 692d 706f 7765 7265 642d 6661 7374 2d61  i-powered-fast-a
-000022d0: 6e64 2d65 6666 6963 6965 6e74 2d66 696c  nd-efficient-fil
-000022e0: 652d 7479 7065 2d69 6465 6e74 6966 6963  e-type-identific
-000022f0: 6174 696f 6e2e 6874 6d6c 292c 206f 7074  ation.html), opt
-00002300: 2d69 6e20 4149 205b 7461 626c 652c 2065  -in AI [table, e
-00002310: 7175 6174 696f 6e2c 2061 6e64 2066 6967  quation, and fig
-00002320: 7572 6520 6578 7472 6163 7469 6f6e 5d28  ure extraction](
-00002330: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
-00002340: 2f70 7269 6369 6e67 292c 2065 6666 6963  /pricing), effic
-00002350: 6965 6e74 205b 746f 6b65 6e20 636f 6d70  ient [token comp
-00002360: 7265 7373 696f 6e5d 2868 7474 7073 3a2f  ression](https:/
-00002370: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00002380: 3430 332e 3132 3936 3829 2c20 6175 746f  403.12968), auto
-00002390: 6d61 7469 6320 5b69 6d61 6765 2065 6e63  matic [image enc
-000023a0: 6f64 696e 675d 2868 7474 7073 3a2f 2f65  oding](https://e
-000023b0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-000023c0: 7769 6b69 2f42 6173 6536 3429 2c20 5b72  wiki/Base64), [r
-000023d0: 6572 616e 6b69 6e67 5d28 6874 7470 733a  eranking](https:
-000023e0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-000023f0: 3233 3130 2e30 3638 3339 2920 666f 7220  2310.06839) for 
-00002400: 5b6c 6f73 742d 696e 2d74 6865 2d6d 6964  [lost-in-the-mid
-00002410: 646c 655d 2868 7474 7073 3a2f 2f61 7278  dle](https://arx
-00002420: 6976 2e6f 7267 2f61 6273 2f32 3330 372e  iv.org/abs/2307.
-00002430: 3033 3137 3229 2065 6666 6563 7473 2c20  03172) effects, 
-00002440: 616e 6420 6d6f 7265 2c20 616c 6c20 7072  and more, all pr
-00002450: 652d 6275 696c 7420 746f 2077 6f72 6b20  e-built to work 
-00002460: 6f75 742d 6f66 2d74 6865 2d62 6f78 2e0d  out-of-the-box..
-00002470: 0a0d 0a21 5b44 656d 6f5d 2868 7474 7073  ...![Demo](https
-00002480: 3a2f 2f72 706e 7574 7a65 6d75 7462 7275  ://rpnutzemutbru
-00002490: 6d63 7a77 7675 652e 7375 7061 6261 7365  mczwvue.supabase
-000024a0: 2e63 6f2f 7374 6f72 6167 652f 7631 2f6f  .co/storage/v1/o
-000024b0: 626a 6563 742f 7075 626c 6963 2f61 7373  bject/public/ass
-000024c0: 6574 732f 6772 6164 6572 2e70 7925 3230  ets/grader.py%20
-000024d0: 2836 292e 706e 6729 0d0a 0d0a 0d0a 2323  (6).png)......##
-000024e0: 204c 6f63 616c 2049 6e73 7461 6c6c 6174   Local Installat
-000024f0: 696f 6e20 f09f 9ba0 efb8 8f0d 0a0d 0a54  ion ...........T
-00002500: 6865 2050 6970 6520 6861 6e64 6c65 7320  he Pipe handles 
-00002510: 6120 7769 6465 2061 7272 6179 206f 6620  a wide array of 
-00002520: 636f 6d70 6c65 7820 6669 6c65 7479 7065  complex filetype
-00002530: 732c 2061 6e64 2074 6875 7320 7265 7175  s, and thus requ
-00002540: 6972 6573 2069 6e73 7461 6c6c 6174 696f  ires installatio
-00002550: 6e20 6f66 206d 616e 7920 6469 6666 6572  n of many differ
-00002560: 656e 7420 7061 636b 6167 6573 2074 6f20  ent packages to 
-00002570: 6675 6e63 7469 6f6e 2e20 4974 2061 6c73  function. It als
-00002580: 6f20 7265 7175 6972 6573 2061 2076 6572  o requires a ver
-00002590: 7920 6361 7061 626c 6520 6d61 6368 696e  y capable machin
-000025a0: 6520 666f 7220 676f 6f64 2072 6573 706f  e for good respo
-000025b0: 6e73 6520 7469 6d65 732e 2046 6f72 2074  nse times. For t
-000025c0: 6869 7320 7265 6173 6f6e 2c20 7765 2068  his reason, we h
-000025d0: 6f73 7420 6974 2061 7320 616e 2041 5049  ost it as an API
-000025e0: 2074 6861 7420 776f 726b 7320 6f75 742d   that works out-
-000025f0: 6f66 2d74 6865 2d62 6f78 2e20 546f 2075  of-the-box. To u
-00002600: 7365 2054 6865 2050 6970 6520 6c6f 6361  se The Pipe loca
-00002610: 6c6c 7920 666f 7220 6672 6565 2069 6e73  lly for free ins
-00002620: 7465 6164 2c20 796f 7520 7769 6c6c 206e  tead, you will n
-00002630: 6565 6420 5b70 6c61 7977 7269 6768 745d  eed [playwright]
-00002640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002650: 636f 6d2f 6d69 6372 6f73 6f66 742f 706c  com/microsoft/pl
-00002660: 6179 7772 6967 6874 292c 205b 6374 6167  aywright), [ctag
-00002670: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00002680: 622e 636f 6d2f 756e 6976 6572 7361 6c2d  b.com/universal-
-00002690: 6374 6167 732f 292c 205b 7079 7465 7373  ctags/), [pytess
-000026a0: 6572 6163 745d 2868 7474 7073 3a2f 2f67  eract](https://g
-000026b0: 6974 6875 622e 636f 6d2f 682f 7079 7465  ithub.com/h/pyte
-000026c0: 7373 6572 6163 7429 2c20 616e 6420 7468  sseract), and th
-000026d0: 6520 6c6f 6361 6c20 7079 7468 6f6e 2072  e local python r
-000026e0: 6571 7569 7265 6d65 6e74 732c 2077 6869  equirements, whi
-000026f0: 6368 2064 6966 6665 7220 6672 6f6d 2074  ch differ from t
-00002700: 6865 206d 6f72 6520 6c69 6768 7477 6569  he more lightwei
-00002710: 6768 7420 4150 4920 7265 7175 6972 656d  ght API requirem
-00002720: 656e 7473 3a0d 0a0d 0a60 6060 6261 7368  ents:....```bash
-00002730: 0d0a 6769 7420 636c 6f6e 6520 6874 7470  ..git clone http
-00002740: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00002750: 6d63 662f 7468 6570 6970 650d 0a70 6970  mcf/thepipe..pip
-00002760: 2069 6e73 7461 6c6c 202d 7220 7265 7175   install -r requ
-00002770: 6972 656d 656e 7473 5f6c 6f63 616c 2e74  irements_local.t
-00002780: 7874 0d0a 6060 600d 0a0d 0a54 6970 2066  xt..```....Tip f
-00002790: 6f72 2077 696e 646f 7773 2075 7365 7273  or windows users
-000027a0: 3a20 496e 7374 616c 6c20 7468 6520 7079  : Install the py
-000027b0: 7468 6f6e 2d6c 6962 6d61 6769 6320 6269  thon-libmagic bi
-000027c0: 6e61 7269 6573 2077 6974 6820 6070 6970  naries with `pip
-000027d0: 2069 6e73 7461 6c6c 2070 7974 686f 6e2d   install python-
-000027e0: 6d61 6769 632d 6269 6e60 2e20 456e 7375  magic-bin`. Ensu
-000027f0: 7265 2074 6865 2060 7465 7373 6572 6163  re the `tesserac
-00002800: 742d 6f63 7260 2062 696e 6172 6965 7320  t-ocr` binaries 
-00002810: 616e 6420 7468 6520 6063 7461 6773 6020  and the `ctags` 
-00002820: 6269 6e61 7269 6573 2061 7265 2069 6e20  binaries are in 
-00002830: 796f 7572 2050 4154 482e 0d0a 0d0a 4e6f  your PATH.....No
-00002840: 7720 796f 7520 6361 6e20 7573 6520 5468  w you can use Th
-00002850: 6520 5069 7065 2077 6974 6820 5079 7468  e Pipe with Pyth
-00002860: 6f6e 3a0d 0a60 6060 6261 7368 0d0a 6672  on:..```bash..fr
-00002870: 6f6d 2074 6865 7069 7065 5f61 7069 2069  om thepipe_api i
-00002880: 6d70 6f72 7420 7468 6570 6970 650d 0a63  mport thepipe..c
-00002890: 6875 6e6b 7320 3d20 7468 6570 6970 652e  hunks = thepipe.
-000028a0: 6578 7472 6163 7428 2265 7861 6d70 6c65  extract("example
-000028b0: 2e70 6466 222c 206c 6f63 616c 3d54 7275  .pdf", local=Tru
-000028c0: 6529 0d0a 6060 600d 0a0d 0a6f 7220 6672  e)..```....or fr
-000028d0: 6f6d 2074 6865 2063 6f6d 6d61 6e64 206c  om the command l
-000028e0: 696e 653a 0d0a 6060 6062 6173 680d 0a74  ine:..```bash..t
-000028f0: 6865 7069 7065 2070 6174 682f 746f 2f66  hepipe path/to/f
-00002900: 6f6c 6465 7220 2d2d 6c6f 6361 6c0d 0a60  older --local..`
-00002910: 6060 0d0a 0d0a 4172 6775 6d65 6e74 7320  ``....Arguments 
-00002920: 6172 653a 0d0a 2d20 6073 6f75 7263 6560  are:..- `source`
-00002930: 2028 7265 7175 6972 6564 293a 2063 616e   (required): can
-00002940: 2062 6520 6120 6669 6c65 2070 6174 682c   be a file path,
-00002950: 2061 2055 524c 2c20 6f72 2061 2064 6972   a URL, or a dir
-00002960: 6563 746f 7279 2070 6174 682e 0d0a 2d20  ectory path...- 
-00002970: 606c 6f63 616c 6020 286f 7074 696f 6e61  `local` (optiona
-00002980: 6c29 3a20 5573 6520 7468 6520 6c6f 6361  l): Use the loca
-00002990: 6c20 7665 7273 696f 6e20 6f66 2054 6865  l version of The
-000029a0: 2050 6970 6520 696e 7374 6561 6420 6f66   Pipe instead of
-000029b0: 2074 6865 2068 6f73 7465 6420 4150 492e   the hosted API.
-000029c0: 0d0a 2d20 606d 6174 6368 6020 286f 7074  ..- `match` (opt
-000029d0: 696f 6e61 6c29 3a20 5375 6273 7472 696e  ional): Substrin
-000029e0: 6720 746f 206d 6174 6368 2066 696c 6573  g to match files
-000029f0: 2069 6e20 7468 6520 6469 7265 6374 6f72   in the director
-00002a00: 792e 2052 6567 6578 2069 7320 6e6f 7420  y. Regex is not 
-00002a10: 7965 7420 7375 7070 6f72 7465 642e 0d0a  yet supported...
-00002a20: 2d20 6069 676e 6f72 6560 2028 6f70 7469  - `ignore` (opti
-00002a30: 6f6e 616c 293a 2053 7562 7374 7269 6e67  onal): Substring
-00002a40: 2074 6f20 6967 6e6f 7265 2066 696c 6573   to ignore files
-00002a50: 2069 6e20 7468 6520 6469 7265 6374 6f72   in the director
-00002a60: 792e 2052 6567 6578 2069 7320 6e6f 7420  y. Regex is not 
-00002a70: 7965 7420 7375 7070 6f72 7465 642e 0d0a  yet supported...
-00002a80: 2d20 606c 696d 6974 6020 286f 7074 696f  - `limit` (optio
-00002a90: 6e61 6c29 3a20 5468 6520 746f 6b65 6e20  nal): The token 
-00002aa0: 6c69 6d69 7420 666f 7220 7468 6520 6f75  limit for the ou
-00002ab0: 7470 7574 2070 726f 6d70 742c 2064 6566  tput prompt, def
-00002ac0: 6175 6c74 7320 746f 2031 3030 4b2e 2050  aults to 100K. P
-00002ad0: 726f 6d70 7473 2065 7863 6565 6469 6e67  rompts exceeding
-00002ae0: 2074 6865 206c 696d 6974 2077 696c 6c20   the limit will 
-00002af0: 6265 2063 6f6d 7072 6573 7365 642e 2054  be compressed. T
-00002b00: 6869 7320 6d61 7920 6e6f 7420 776f 726b  his may not work
-00002b10: 2061 7320 6578 7065 6374 6564 2077 6974   as expected wit
-00002b20: 6820 7468 6520 4150 492c 2061 7320 6974  h the API, as it
-00002b30: 2069 7320 696e 2061 6374 6976 6520 6465   is in active de
-00002b40: 7665 6c6f 706d 656e 742e 0d0a 2d20 6061  velopment...- `a
-00002b50: 695f 6578 7472 6163 7469 6f6e 6020 286f  i_extraction` (o
-00002b60: 7074 696f 6e61 6c29 3a20 4578 7472 6163  ptional): Extrac
-00002b70: 7420 7461 626c 6573 2c20 6669 6775 7265  t tables, figure
-00002b80: 732c 2061 6e64 206d 6174 6820 6672 6f6d  s, and math from
-00002b90: 2050 4446 7320 7573 696e 6720 6f75 7220   PDFs using our 
-00002ba0: 6578 7472 6163 746f 722e 2049 6e63 7572  extractor. Incur
-00002bb0: 7320 6578 7472 6120 636f 7374 732e 0d0a  s extra costs...
-00002bc0: 2d20 6074 6578 745f 6f6e 6c79 6020 286f  - `text_only` (o
-00002bd0: 7074 696f 6e61 6c29 3a20 446f 206e 6f74  ptional): Do not
-00002be0: 2065 7874 7261 6374 2069 6d61 6765 7320   extract images 
-00002bf0: 6672 6f6d 2064 6f63 756d 656e 7473 206f  from documents o
-00002c00: 7220 7765 6273 6974 6573 2e20 4164 6469  r websites. Addi
-00002c10: 7469 6f6e 616c 6c79 2c20 696d 6167 6520  tionally, image 
-00002c20: 6669 6c65 7320 7769 6c6c 2062 6520 7265  files will be re
-00002c30: 7072 6573 656e 7465 6420 7769 7468 204f  presented with O
-00002c40: 4352 2069 6e73 7465 6164 206f 6620 6173  CR instead of as
-00002c50: 2069 6d61 6765 732e 0d0a 0d0a 2320 5370   images.....# Sp
-00002c60: 6f6e 736f 7273 0d0a 0d0a 3c61 2068 7265  onsors....<a hre
-00002c70: 663d 2268 7474 7073 3a2f 2f63 616c 2e63  f="https://cal.c
-00002c80: 6f6d 2f65 6d6d 6574 742d 6d63 662f 3330  om/emmett-mcf/30
-00002c90: 6d69 6e22 3e3c 696d 6720 616c 743d 2242  min"><img alt="B
-00002ca0: 6f6f 6b20 7573 2077 6974 6820 4361 6c2e  ook us with Cal.
-00002cb0: 636f 6d22 2073 7263 3d22 6874 7470 733a  com" src="https:
-00002cc0: 2f2f 6361 6c2e 636f 6d2f 626f 6f6b 2d77  //cal.com/book-w
-00002cd0: 6974 682d 6361 6c2d 6461 726b 2e73 7667  ith-cal-dark.svg
-00002ce0: 2220 2f3e 3c2f 613e 0d0a 0d0a 5468 616e  " /></a>....Than
-00002cf0: 6b20 796f 7520 746f 205b 4361 6c2e 636f  k you to [Cal.co
-00002d00: 6d5d 2868 7474 7073 3a2f 2f63 616c 2e63  m](https://cal.c
-00002d10: 6f6d 2f29 2066 6f72 2073 706f 6e73 6f72  om/) for sponsor
-00002d20: 696e 6720 7468 6973 2070 726f 6a65 6374  ing this project
-00002d30: 2e20 436f 6e74 6163 7420 656d 6d65 7474  . Contact emmett
-00002d40: 4074 6865 7069 2e70 6520 666f 7220 7370  @thepi.pe for sp
-00002d50: 6f6e 736f 7273 6869 7020 696e 666f 726d  onsorship inform
-00002d60: 6174 696f 6e2e                           ation.
+000014e0: 2020 207c 2060 2e69 7079 6e62 6020 2020     | `.ipynb`   
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00001510: 9d8c 2020 2020 2020 2020 2020 2020 2020  ..              
+00001520: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
+00001530: 2020 2020 2020 2020 7c20 4578 7472 6163          | Extrac
+00001540: 7473 2063 6f64 652c 206d 6172 6b64 6f77  ts code, markdow
+00001550: 6e2c 2061 6e64 2069 6d61 6765 7320 6672  n, and images fr
+00001560: 6f6d 204a 7570 7974 6572 206e 6f74 6562  om Jupyter noteb
+00001570: 6f6f 6b73 2020 2020 2020 2020 2020 2020  ooks            
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 2020 7c0d 0a7c 204d 6963 726f        |..| Micro
+000015a0: 736f 6674 2057 6f72 6420 446f 6375 6d65  soft Word Docume
+000015b0: 6e74 2020 2020 2020 2020 2020 2020 2020  nt              
+000015c0: 207c 2060 2e64 6f63 7860 2020 2020 2020   | `.docx`      
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+000015f0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+00001600: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001610: 2020 2020 2020 2020 207c 2045 7874 7261           | Extra
+00001620: 6374 7320 7465 7874 2061 6e64 2069 6d61  cts text and ima
+00001630: 6765 7320 6672 6f6d 2057 6f72 6420 646f  ges from Word do
+00001640: 6375 6d65 6e74 7320 2020 2020 2020 2020  cuments         
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001670: 0d0a 7c20 4d69 6372 6f73 6f66 7420 506f  ..| Microsoft Po
+00001680: 7765 7250 6f69 6e74 2050 7265 7365 6e74  werPoint Present
+00001690: 6174 696f 6e20 2020 2020 7c20 602e 7070  ation     | `.pp
+000016a0: 7478 6020 2020 2020 2020 2020 2020 2020  tx`             
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
+000016d0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+000016e0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+000016f0: 2020 7c20 4578 7472 6163 7473 2074 6578    | Extracts tex
+00001700: 7420 616e 6420 696d 6167 6573 2066 726f  t and images fro
+00001710: 6d20 506f 7765 7250 6f69 6e74 2070 7265  m PowerPoint pre
+00001720: 7365 6e74 6174 696f 6e73 2020 2020 2020  sentations      
+00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001740: 2020 2020 2020 2020 7c0d 0a7c 2056 6964          |..| Vid
+00001750: 656f 2020 2020 2020 2020 2020 2020 2020  eo              
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 207c 2060 2e6d 7034 602c 2060 2e61     | `.mp4`, `.a
+00001780: 7669 602c 2060 2e6d 6f76 602c 2060 2e77  vi`, `.mov`, `.w
+00001790: 6d76 6020 2020 2020 7c20 e29c 94ef b88f  mv`     | ......
+000017a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000017b0: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
+000017c0: 2020 2020 2020 207c 2045 7874 7261 6374         | Extract
+000017d0: 7320 6672 616d 6573 2066 726f 6d20 7669  s frames from vi
+000017e0: 6465 6f20 6669 6c65 733b 2073 7570 706f  deo files; suppo
+000017f0: 7274 7320 6672 616d 6520 6578 7472 6163  rts frame extrac
+00001800: 7469 6f6e 2061 6e64 204f 4352 2066 6f72  tion and OCR for
+00001810: 2074 6578 7420 6578 7472 6163 7469 6f6e   text extraction
+00001820: 2066 726f 6d20 6672 616d 6573 207c 0d0a   from frames |..
+00001830: 7c20 4175 6469 6f20 2020 2020 2020 2020  | Audio         
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 2020 7c20 602e 6d70 3360          | `.mp3`
+00001860: 2c20 602e 7761 7660 2020 2020 2020 2020  , `.wav`        
+00001870: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001880: 2020 2020 2020 2020 207c 20e2 9d8c 2020           | ...  
+00001890: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000018a0: 4578 7472 6163 7473 2074 6578 7420 6672  Extracts text fr
+000018b0: 6f6d 2061 7564 696f 2066 696c 6573 3b20  om audio files; 
+000018c0: 7375 7070 6f72 7473 2073 7065 6563 682d  supports speech-
+000018d0: 746f 2d74 6578 7420 636f 6e76 6572 7369  to-text conversi
+000018e0: 6f6e 2020 2020 2020 2020 7c20 0d0a 7c20  on        | ..| 
+000018f0: 5765 6273 6974 6520 2020 2020 2020 2020  Website         
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2020 2020 2020 7c20 5552 4c73 2028 696e        | URLs (in
+00001920: 7075 7473 2073 7461 7274 696e 6720 7769  puts starting wi
+00001930: 7468 2060 6874 7470 602c 2060 6874 7470  th `http`, `http
+00001940: 7360 2c20 6066 7470 6029 2020 2020 2020  s`, `ftp`)      
+00001950: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001970: 20e2 9c94 efb8 8f20 2020 207c 2045 7874   ......    | Ext
+00001980: 7261 6374 7320 7465 7874 2066 726f 6d20  racts text from 
+00001990: 7765 6220 7061 6765 2061 6c6f 6e67 2077  web page along w
+000019a0: 6974 6820 696d 6167 6520 286f 7220 696d  ith image (or im
+000019b0: 6167 6573 2069 6620 7363 726f 6c6c 6162  ages if scrollab
+000019c0: 6c65 293b 2074 6578 742d 6f6e 6c79 2065  le); text-only e
+000019d0: 7874 7261 6374 696f 6e20 6176 6169 6c61  xtraction availa
+000019e0: 626c 6520 2020 2020 2020 2020 207c 0d0a  ble          |..
+000019f0: 7c20 4769 7448 7562 2052 6570 6f73 6974  | GitHub Reposit
+00001a00: 6f72 7920 2020 2020 2020 2020 2020 2020  ory             
+00001a10: 2020 2020 2020 2020 7c20 4769 7448 7562          | GitHub
+00001a20: 2072 6570 6f20 5552 4c73 2028 696e 7075   repo URLs (inpu
+00001a30: 7473 2073 7461 7274 696e 6720 7769 7468  ts starting with
+00001a40: 2060 6874 7470 733a 2f2f 6769 7468 7562   `https://github
+00001a50: 2e63 6f6d 6020 6f72 2060 6874 7470 733a  .com` or `https:
+00001a60: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
+00001a70: 6029 2020 2020 2020 2020 2020 2020 2020  `)              
+00001a80: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00001a90: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+00001aa0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001ab0: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
+00001ac0: 7261 6374 7320 6672 6f6d 2047 6974 4875  racts from GitHu
+00001ad0: 6220 7265 706f 7369 746f 7269 6573 3b20  b repositories; 
+00001ae0: 7375 7070 6f72 7473 2062 7261 6e63 6820  supports branch 
+00001af0: 7370 6563 6966 6963 6174 696f 6e20 2020  specification   
+00001b00: 2020 2020 2020 7c0d 0a7c 2059 6f75 5475        |..| YouTu
+00001b10: 6265 2056 6964 656f 2020 2020 2020 2020  be Video        
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 207c 2059 6f75 5475 6265 2076 6964 656f   | YouTube video
+00001b40: 2055 524c 7320 2869 6e70 7574 7320 7374   URLs (inputs st
+00001b50: 6172 7469 6e67 2077 6974 6820 6068 7474  arting with `htt
+00001b60: 7073 3a2f 2f79 6f75 7475 6265 2e63 6f6d  ps://youtube.com
+00001b70: 6020 6f72 2060 6874 7470 733a 2f2f 7777  ` or `https://ww
+00001b80: 772e 796f 7574 7562 652e 636f 6d60 2920  w.youtube.com`) 
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
+00001bb0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+00001bc0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+00001bd0: 2020 207c 2045 7874 7261 6374 7320 6672     | Extracts fr
+00001be0: 616d 6573 2061 6e64 2074 7261 6e73 6372  ames and transcr
+00001bf0: 6970 7420 6672 6f6d 2059 6f75 5475 6265  ipt from YouTube
+00001c00: 2076 6964 656f 7320 696e 2070 6572 2d6d   videos in per-m
+00001c10: 696e 7574 6520 6368 756e 6b73 2020 2020  inute chunks    
+00001c20: 2020 2020 2020 7c0d 0a7c 205a 4950 2046        |..| ZIP F
+00001c30: 696c 6520 2020 2020 2020 2020 2020 2020  ile             
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 207c 2060 2e7a 6970 6020 2020 2020 2020   | `.zip`       
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+00001c80: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+00001c90: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001ca0: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+00001cb0: 6163 7473 2063 6f6e 7465 6e74 7320 6f66  acts contents of
+00001cc0: 205a 4950 2066 696c 6573 3b20 7375 7070   ZIP files; supp
+00001cd0: 6f72 7473 206e 6573 7465 6420 6469 7265  orts nested dire
+00001ce0: 6374 6f72 7920 6578 7472 6163 7469 6f6e  ctory extraction
+00001cf0: 2020 2020 207c 0d0a 0d0a 2323 2048 6f77       |....## How
+00001d00: 2069 7420 776f 726b 7320 f09f 9ba0 efb8   it works ......
+00001d10: 8f0d 0a0d 0a54 6865 2069 6e70 7574 2073  .....The input s
+00001d20: 6f75 7263 6520 6973 2065 6974 6865 7220  ource is either 
+00001d30: 6120 6669 6c65 2070 6174 682c 2061 2055  a file path, a U
+00001d40: 524c 2c20 6f72 2061 2064 6972 6563 746f  RL, or a directo
+00001d50: 7279 2e20 5468 6520 7069 7065 2077 696c  ry. The pipe wil
+00001d60: 6c20 6578 7472 6163 7420 696e 666f 726d  l extract inform
+00001d70: 6174 696f 6e20 6672 6f6d 2074 6865 2073  ation from the s
+00001d80: 6f75 7263 6520 616e 6420 7072 6f63 6573  ource and proces
+00001d90: 7320 6974 2066 6f72 2064 6f77 6e73 7472  s it for downstr
+00001da0: 6561 6d20 7573 6520 7769 7468 205b 6c61  eam use with [la
+00001db0: 6e67 7561 6765 206d 6f64 656c 735d 2868  nguage models](h
+00001dc0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00001dd0: 6469 612e 6f72 672f 7769 6b69 2f4c 6172  dia.org/wiki/Lar
+00001de0: 6765 5f6c 616e 6775 6167 655f 6d6f 6465  ge_language_mode
+00001df0: 6c29 2c20 5b76 6973 696f 6e20 7472 616e  l), [vision tran
+00001e00: 7366 6f72 6d65 7273 5d28 6874 7470 733a  sformers](https:
+00001e10: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00001e20: 7267 2f77 696b 692f 5669 7369 6f6e 5f74  rg/wiki/Vision_t
+00001e30: 7261 6e73 666f 726d 6572 292c 206f 7220  ransformer), or 
+00001e40: 5b76 6973 696f 6e2d 6c61 6e67 7561 6765  [vision-language
+00001e50: 206d 6f64 656c 735d 2868 7474 7073 3a2f   models](https:/
+00001e60: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00001e70: 3330 342e 3030 3638 3529 2e20 5468 6520  304.00685). The 
+00001e80: 6f75 7470 7574 2066 726f 6d20 7468 6520  output from the 
+00001e90: 7069 7065 2069 7320 6120 7365 6e73 6962  pipe is a sensib
+00001ea0: 6c65 206c 6973 7420 6f66 206d 756c 7469  le list of multi
+00001eb0: 6d6f 6461 6c20 6d65 7373 6167 6573 2072  modal messages r
+00001ec0: 6570 7265 7365 6e74 696e 6720 6368 756e  epresenting chun
+00001ed0: 6b73 206f 6620 7468 6520 6578 7472 6163  ks of the extrac
+00001ee0: 7465 6420 696e 666f 726d 6174 696f 6e2c  ted information,
+00001ef0: 2063 6172 6566 756c 6c79 2063 7261 6674   carefully craft
+00001f00: 6564 2074 6f20 6669 7420 7769 7468 696e  ed to fit within
+00001f10: 2063 6f6e 7465 7874 2077 696e 646f 7773   context windows
+00001f20: 2066 6f72 2061 6e79 206d 6f64 656c 7320   for any models 
+00001f30: 6672 6f6d 205b 6765 6d6d 612d 3762 5d28  from [gemma-7b](
+00001f40: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00001f50: 6163 652e 636f 2f67 6f6f 676c 652f 6765  ace.co/google/ge
+00001f60: 6d6d 612d 3762 2920 746f 205b 4750 542d  mma-7b) to [GPT-
+00001f70: 345d 2868 7474 7073 3a2f 2f6f 7065 6e61  4](https://opena
+00001f80: 692e 636f 6d2f 6770 742d 3429 2e20 5468  i.com/gpt-4). Th
+00001f90: 6520 6d65 7373 6167 6573 2072 6574 7572  e messages retur
+00001fa0: 6e65 6420 7368 6f75 6c64 206c 6f6f 6b20  ned should look 
+00001fb0: 6c69 6b65 2074 6869 733a 0d0a 6060 606a  like this:..```j
+00001fc0: 736f 6e0d 0a5b 0d0a 2020 7b0d 0a20 2020  son..[..  {..   
+00001fd0: 2022 726f 6c65 223a 2022 7573 6572 222c   "role": "user",
+00001fe0: 0d0a 2020 2020 2263 6f6e 7465 6e74 223a  ..    "content":
+00001ff0: 205b 0d0a 2020 2020 2020 7b0d 0a20 2020   [..      {..   
+00002000: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00002010: 7874 222c 0d0a 2020 2020 2020 2020 2274  xt",..        "t
+00002020: 6578 7422 3a20 222e 2e2e 220d 0a20 2020  ext": "..."..   
+00002030: 2020 207d 2c0d 0a20 2020 2020 207b 0d0a     },..      {..
+00002040: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00002050: 2269 6d61 6765 5f75 726c 222c 0d0a 2020  "image_url",..  
+00002060: 2020 2020 2020 2269 6d61 6765 5f75 726c        "image_url
+00002070: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
+00002080: 2275 726c 223a 2022 6461 7461 3a69 6d61  "url": "data:ima
+00002090: 6765 2f6a 7065 673b 6261 7365 3634 2c2e  ge/jpeg;base64,.
+000020a0: 2e2e 220d 0a20 2020 2020 2020 207d 0d0a  .."..        }..
+000020b0: 2020 2020 2020 7d0d 0a20 2020 205d 0d0a        }..    ]..
+000020c0: 2020 7d0d 0a5d 0d0a 6060 600d 0a49 6620    }..]..```..If 
+000020d0: 796f 7520 7761 6e74 2074 6f20 6665 6564  you want to feed
+000020e0: 2074 6865 7365 206d 6573 7361 6765 7320   these messages 
+000020f0: 6469 7265 6374 6c79 2069 6e74 6f20 7468  directly into th
+00002100: 6520 6d6f 6465 6c2c 2069 7420 6973 2069  e model, it is i
+00002110: 6d70 6f72 7461 6e74 2074 6f20 6265 206d  mportant to be m
+00002120: 696e 6466 756c 206f 6620 7468 6520 746f  indful of the to
+00002130: 6b65 6e20 6c69 6d69 742e 0d0a 4f70 656e  ken limit...Open
+00002140: 4149 2064 6f65 7320 6e6f 7420 616c 6c6f  AI does not allo
+00002150: 7720 746f 6f20 6d61 6e79 2069 6d61 6765  w too many image
+00002160: 7320 696e 2074 6865 2070 726f 6d70 7420  s in the prompt 
+00002170: 2873 6565 2064 6973 6375 7373 696f 6e20  (see discussion 
+00002180: 5b68 6572 655d 2868 7474 7073 3a2f 2f63  [here](https://c
+00002190: 6f6d 6d75 6e69 7479 2e6f 7065 6e61 692e  ommunity.openai.
+000021a0: 636f 6d2f 742f 6770 742d 342d 7669 7369  com/t/gpt-4-visi
+000021b0: 6f6e 2d6d 6178 696d 756d 2d61 6d6f 756e  on-maximum-amoun
+000021c0: 742d 6f66 2d69 6d61 6765 732f 3537 3331  t-of-images/5731
+000021d0: 3130 2f36 2929 2c20 736f 206c 6f6e 6720  10/6)), so long 
+000021e0: 6669 6c65 7320 7368 6f75 6c64 2062 6520  files should be 
+000021f0: 6578 7472 6163 7465 6420 7769 7468 2060  extracted with `
+00002200: 7465 7874 5f6f 6e6c 793d 5472 7565 6020  text_only=True` 
+00002210: 746f 2061 766f 6964 2074 6869 7320 6973  to avoid this is
+00002220: 7375 652c 2077 6869 6c65 206c 6f6e 6720  sue, while long 
+00002230: 7465 7874 2066 696c 6573 2073 686f 756c  text files shoul
+00002240: 6420 6569 7468 6572 2062 6520 636f 6d70  d either be comp
+00002250: 7265 7373 6564 206f 7220 656d 6265 6464  ressed or embedd
+00002260: 6564 2069 6e20 6120 5241 4720 6672 616d  ed in a RAG fram
+00002270: 6577 6f72 6b2e 0d0a 0d0a 5468 6520 7465  ework.....The te
+00002280: 7874 2061 6e64 2069 6d61 6765 7320 6672  xt and images fr
+00002290: 6f6d 2074 6865 7365 206d 6573 7361 6765  om these message
+000022a0: 7320 6d61 7920 616c 736f 2062 6520 7072  s may also be pr
+000022b0: 6570 6172 6564 2066 6f72 2061 2076 6563  epared for a vec
+000022c0: 746f 7220 6461 7461 6261 7365 2077 6974  tor database wit
+000022d0: 6820 6074 6865 7069 7065 2e63 6f72 652e  h `thepipe.core.
+000022e0: 6372 6561 7465 5f63 6875 6e6b 735f 6672  create_chunks_fr
+000022f0: 6f6d 5f6d 6573 7361 6765 7360 206f 7220  om_messages` or 
+00002300: 666f 7220 646f 776e 7374 7265 616d 2075  for downstream u
+00002310: 7365 2077 6974 6820 5241 4720 6672 616d  se with RAG fram
+00002320: 6577 6f72 6b73 2e20 5b4c 6974 654c 4c4d  eworks. [LiteLLM
+00002330: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002340: 2e63 6f6d 2f42 6572 7269 4149 2f6c 6974  .com/BerriAI/lit
+00002350: 656c 6c6d 2920 6361 6e20 6265 2075 7365  ellm) can be use
+00002360: 6420 746f 2065 6173 696c 7920 696e 7465  d to easily inte
+00002370: 6772 6174 6520 5468 6520 5069 7065 2077  grate The Pipe w
+00002380: 6974 6820 616e 7920 4c4c 4d20 7072 6f76  ith any LLM prov
+00002390: 6964 6572 2e20 0d0a 0d0a 4974 2075 7365  ider. ....It use
+000023a0: 7320 6120 7661 7269 6574 7920 6f66 2068  s a variety of h
+000023b0: 6575 7269 7374 6963 7320 666f 7220 6f70  euristics for op
+000023c0: 7469 6d61 6c20 7065 7266 6f72 6d61 6e63  timal performanc
+000023d0: 6520 7769 7468 2076 6973 696f 6e2d 6c61  e with vision-la
+000023e0: 6e67 7561 6765 206d 6f64 656c 732c 2069  nguage models, i
+000023f0: 6e63 6c75 6469 6e67 2041 4920 6669 6c65  ncluding AI file
+00002400: 7479 7065 2064 6574 6563 7469 6f6e 2077  type detection w
+00002410: 6974 6820 5b66 696c 6574 7970 6520 6465  ith [filetype de
+00002420: 7465 6374 696f 6e5d 2868 7474 7073 3a2f  tection](https:/
+00002430: 2f6f 7065 6e73 6f75 7263 652e 676f 6f67  /opensource.goog
+00002440: 6c65 626c 6f67 2e63 6f6d 2f32 3032 342f  leblog.com/2024/
+00002450: 3032 2f6d 6167 696b 612d 6169 2d70 6f77  02/magika-ai-pow
+00002460: 6572 6564 2d66 6173 742d 616e 642d 6566  ered-fast-and-ef
+00002470: 6669 6369 656e 742d 6669 6c65 2d74 7970  ficient-file-typ
+00002480: 652d 6964 656e 7469 6669 6361 7469 6f6e  e-identification
+00002490: 2e68 746d 6c29 2c20 6f70 742d 696e 2041  .html), opt-in A
+000024a0: 4920 5b74 6162 6c65 2c20 6571 7561 7469  I [table, equati
+000024b0: 6f6e 2c20 616e 6420 6669 6775 7265 2065  on, and figure e
+000024c0: 7874 7261 6374 696f 6e5d 2868 7474 7073  xtraction](https
+000024d0: 3a2f 2f74 6865 7069 2e70 652f 7072 6963  ://thepi.pe/pric
+000024e0: 696e 6729 2c20 6566 6669 6369 656e 7420  ing), efficient 
+000024f0: 5b74 6f6b 656e 2063 6f6d 7072 6573 7369  [token compressi
+00002500: 6f6e 5d28 6874 7470 733a 2f2f 6172 7869  on](https://arxi
+00002510: 762e 6f72 672f 6162 732f 3234 3033 2e31  v.org/abs/2403.1
+00002520: 3239 3638 292c 2061 7574 6f6d 6174 6963  2968), automatic
+00002530: 205b 696d 6167 6520 656e 636f 6469 6e67   [image encoding
+00002540: 5d28 6874 7470 733a 2f2f 656e 2e77 696b  ](https://en.wik
+00002550: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00002560: 4261 7365 3634 292c 205b 7265 7261 6e6b  Base64), [rerank
+00002570: 696e 675d 2868 7474 7073 3a2f 2f61 7278  ing](https://arx
+00002580: 6976 2e6f 7267 2f61 6273 2f32 3331 302e  iv.org/abs/2310.
+00002590: 3036 3833 3929 2066 6f72 205b 6c6f 7374  06839) for [lost
+000025a0: 2d69 6e2d 7468 652d 6d69 6464 6c65 5d28  -in-the-middle](
+000025b0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+000025c0: 672f 6162 732f 3233 3037 2e30 3331 3732  g/abs/2307.03172
+000025d0: 2920 6566 6665 6374 732c 2061 6e64 206d  ) effects, and m
+000025e0: 6f72 652c 2061 6c6c 2070 7265 2d62 7569  ore, all pre-bui
+000025f0: 6c74 2074 6f20 776f 726b 206f 7574 2d6f  lt to work out-o
+00002600: 662d 7468 652d 626f 782e 0d0a 0d0a 215b  f-the-box.....![
+00002610: 4465 6d6f 5d28 6874 7470 733a 2f2f 7270  Demo](https://rp
+00002620: 6e75 747a 656d 7574 6272 756d 637a 7776  nutzemutbrumczwv
+00002630: 7565 2e73 7570 6162 6173 652e 636f 2f73  ue.supabase.co/s
+00002640: 746f 7261 6765 2f76 312f 6f62 6a65 6374  torage/v1/object
+00002650: 2f70 7562 6c69 632f 6173 7365 7473 2f67  /public/assets/g
+00002660: 7261 6465 722e 7079 2532 3028 3629 2e70  rader.py%20(6).p
+00002670: 6e67 290d 0a0d 0a0d 0a23 2320 4c6f 6361  ng)......## Loca
+00002680: 6c20 496e 7374 616c 6c61 7469 6f6e 20f0  l Installation .
+00002690: 9f9b a0ef b88f 0d0a 0d0a 4966 2079 6f75  ..........If you
+000026a0: 2064 6f20 6e6f 7420 7769 7368 2074 6f20   do not wish to 
+000026b0: 7573 6520 6f75 7220 4150 492c 2079 6f75  use our API, you
+000026c0: 2061 7265 2077 656c 636f 6d65 2068 6f73   are welcome hos
+000026d0: 7420 5468 6520 5069 7065 2066 6f72 2079  t The Pipe for y
+000026e0: 6f75 7273 656c 6620 6c6f 6361 6c6c 792e  ourself locally.
+000026f0: 200d 0a49 6620 796f 7520 6368 6f6f 7365   ..If you choose
+00002700: 2074 6f20 646f 2074 6869 732c 2079 6f75   to do this, you
+00002710: 206d 7573 7420 696e 7374 616c 6c20 6120   must install a 
+00002720: 6e75 6d62 6572 206f 6620 6465 7065 6e64  number of depend
+00002730: 656e 6369 6573 2066 6f72 2074 6865 2063  encies for the c
+00002740: 6f64 6520 746f 2066 756e 6374 696f 6e20  ode to function 
+00002750: 636f 7272 6563 746c 792c 2073 6f6d 6520  correctly, some 
+00002760: 6f66 2077 6869 6368 206d 6179 2069 6e63  of which may inc
+00002770: 7572 2063 6f6d 7075 7465 2063 6f73 7473  ur compute costs
+00002780: 2061 6e64 2f6f 7220 7265 7175 6972 6520   and/or require 
+00002790: 6120 4750 5520 666f 7220 7265 6173 6f6e  a GPU for reason
+000027a0: 6162 6c65 2070 6572 666f 726d 616e 6365  able performance
+000027b0: 2e20 4164 6469 7469 6f6e 616c 2069 6e73  . Additional ins
+000027c0: 7461 6c6c 6564 2064 6570 656e 6465 6e63  talled dependenc
+000027d0: 6965 7320 6172 6520 7265 7175 6972 6564  ies are required
+000027e0: 3a20 7079 746f 7263 682c 2075 6e69 7665  : pytorch, unive
+000027f0: 7273 616c 2d63 7461 6773 2c20 706c 6179  rsal-ctags, play
+00002800: 7772 6967 6874 2c20 7079 7465 7373 6572  wright, pytesser
+00002810: 6163 742c 206c 6c6d 6c69 6e67 7561 2c20  act, llmlingua, 
+00002820: 6d6f 7669 6570 792c 2061 6e64 2070 7974  moviepy, and pyt
+00002830: 7562 652e 2054 6869 7320 696e 7374 616c  ube. This instal
+00002840: 6c61 7469 6f6e 2070 726f 6365 7373 2077  lation process w
+00002850: 696c 6c20 6465 7065 6e64 206f 6e20 796f  ill depend on yo
+00002860: 7572 2073 7973 7465 6d20 616e 6420 636f  ur system and co
+00002870: 6d70 7574 6520 6361 7061 6269 6c69 7469  mpute capabiliti
+00002880: 6573 2e20 4166 7465 7220 696e 7374 616c  es. After instal
+00002890: 6c69 6e67 2074 6865 6d2c 2066 6f6c 6c6f  ling them, follo
+000028a0: 7720 7468 6573 6520 7374 6570 7320 666f  w these steps fo
+000028b0: 7220 6120 6c6f 6361 6c20 7365 7475 703a  r a local setup:
+000028c0: 0d0a 0d0a 4172 6775 6d65 6e74 7320 6172  ....Arguments ar
+000028d0: 653a 0d0a 2d20 6073 6f75 7263 6560 2028  e:..- `source` (
+000028e0: 7265 7175 6972 6564 293a 2063 616e 2062  required): can b
+000028f0: 6520 6120 6669 6c65 2070 6174 682c 2061  e a file path, a
+00002900: 2055 524c 2c20 6f72 2061 2064 6972 6563   URL, or a direc
+00002910: 746f 7279 2070 6174 682e 0d0a 2d20 606c  tory path...- `l
+00002920: 6f63 616c 6020 286f 7074 696f 6e61 6c29  ocal` (optional)
+00002930: 3a20 5573 6520 7468 6520 6c6f 6361 6c20  : Use the local 
+00002940: 7665 7273 696f 6e20 6f66 2054 6865 2050  version of The P
+00002950: 6970 6520 696e 7374 6561 6420 6f66 2074  ipe instead of t
+00002960: 6865 2068 6f73 7465 6420 4150 492e 0d0a  he hosted API...
+00002970: 2d20 606d 6174 6368 6020 286f 7074 696f  - `match` (optio
+00002980: 6e61 6c29 3a20 5375 6273 7472 696e 6720  nal): Substring 
+00002990: 746f 206d 6174 6368 2066 696c 6573 2069  to match files i
+000029a0: 6e20 7468 6520 6469 7265 6374 6f72 792e  n the directory.
+000029b0: 2052 6567 6578 2069 7320 6e6f 7420 7965   Regex is not ye
+000029c0: 7420 7375 7070 6f72 7465 642e 0d0a 2d20  t supported...- 
+000029d0: 6069 676e 6f72 6560 2028 6f70 7469 6f6e  `ignore` (option
+000029e0: 616c 293a 2053 7562 7374 7269 6e67 2074  al): Substring t
+000029f0: 6f20 6967 6e6f 7265 2066 696c 6573 2069  o ignore files i
+00002a00: 6e20 7468 6520 6469 7265 6374 6f72 792e  n the directory.
+00002a10: 2052 6567 6578 2069 7320 6e6f 7420 7965   Regex is not ye
+00002a20: 7420 7375 7070 6f72 7465 642e 0d0a 2d20  t supported...- 
+00002a30: 606c 696d 6974 6020 286f 7074 696f 6e61  `limit` (optiona
+00002a40: 6c29 3a20 5468 6520 746f 6b65 6e20 6c69  l): The token li
+00002a50: 6d69 7420 666f 7220 7468 6520 6f75 7470  mit for the outp
+00002a60: 7574 2070 726f 6d70 742c 2064 6566 6175  ut prompt, defau
+00002a70: 6c74 7320 746f 2031 3030 4b2e 2050 726f  lts to 100K. Pro
+00002a80: 6d70 7473 2065 7863 6565 6469 6e67 2074  mpts exceeding t
+00002a90: 6865 206c 696d 6974 2077 696c 6c20 6265  he limit will be
+00002aa0: 2063 6f6d 7072 6573 7365 642e 2054 6869   compressed. Thi
+00002ab0: 7320 6d61 7920 6e6f 7420 776f 726b 2061  s may not work a
+00002ac0: 7320 6578 7065 6374 6564 2077 6974 6820  s expected with 
+00002ad0: 7468 6520 4150 492c 2061 7320 6974 2069  the API, as it i
+00002ae0: 7320 696e 2061 6374 6976 6520 6465 7665  s in active deve
+00002af0: 6c6f 706d 656e 742e 0d0a 2d20 6061 695f  lopment...- `ai_
+00002b00: 6578 7472 6163 7469 6f6e 6020 286f 7074  extraction` (opt
+00002b10: 696f 6e61 6c29 3a20 4578 7472 6163 7420  ional): Extract 
+00002b20: 7461 626c 6573 2c20 6669 6775 7265 732c  tables, figures,
+00002b30: 2061 6e64 206d 6174 6820 6672 6f6d 2050   and math from P
+00002b40: 4446 7320 7573 696e 6720 6f75 7220 6578  DFs using our ex
+00002b50: 7472 6163 746f 722e 2049 6e63 7572 7320  tractor. Incurs 
+00002b60: 6578 7472 6120 636f 7374 732e 0d0a 2d20  extra costs...- 
+00002b70: 6074 6578 745f 6f6e 6c79 6020 286f 7074  `text_only` (opt
+00002b80: 696f 6e61 6c29 3a20 446f 206e 6f74 2065  ional): Do not e
+00002b90: 7874 7261 6374 2069 6d61 6765 7320 6672  xtract images fr
+00002ba0: 6f6d 2064 6f63 756d 656e 7473 206f 7220  om documents or 
+00002bb0: 7765 6273 6974 6573 2e20 4164 6469 7469  websites. Additi
+00002bc0: 6f6e 616c 6c79 2c20 696d 6167 6520 6669  onally, image fi
+00002bd0: 6c65 7320 7769 6c6c 2062 6520 7265 7072  les will be repr
+00002be0: 6573 656e 7465 6420 7769 7468 204f 4352  esented with OCR
+00002bf0: 2069 6e73 7465 6164 206f 6620 6173 2069   instead of as i
+00002c00: 6d61 6765 732e 0d0a 0d0a 2320 5370 6f6e  mages.....# Spon
+00002c10: 736f 7273 0d0a 0d0a 3c61 2068 7265 663d  sors....<a href=
+00002c20: 2268 7474 7073 3a2f 2f63 616c 2e63 6f6d  "https://cal.com
+00002c30: 2f65 6d6d 6574 742d 6d63 662f 3330 6d69  /emmett-mcf/30mi
+00002c40: 6e22 3e3c 696d 6720 616c 743d 2242 6f6f  n"><img alt="Boo
+00002c50: 6b20 7573 2077 6974 6820 4361 6c2e 636f  k us with Cal.co
+00002c60: 6d22 2073 7263 3d22 6874 7470 733a 2f2f  m" src="https://
+00002c70: 6361 6c2e 636f 6d2f 626f 6f6b 2d77 6974  cal.com/book-wit
+00002c80: 682d 6361 6c2d 6461 726b 2e73 7667 2220  h-cal-dark.svg" 
+00002c90: 2f3e 3c2f 613e 0d0a 0d0a 5468 616e 6b20  /></a>....Thank 
+00002ca0: 796f 7520 746f 205b 4361 6c2e 636f 6d5d  you to [Cal.com]
+00002cb0: 2868 7474 7073 3a2f 2f63 616c 2e63 6f6d  (https://cal.com
+00002cc0: 2f29 2066 6f72 2073 706f 6e73 6f72 696e  /) for sponsorin
+00002cd0: 6720 7468 6973 2070 726f 6a65 6374 2e20  g this project. 
+00002ce0: 436f 6e74 6163 7420 656d 6d65 7474 4074  Contact emmett@t
+00002cf0: 6865 7069 2e70 6520 666f 7220 7370 6f6e  hepi.pe for spon
+00002d00: 736f 7273 6869 7020 696e 666f 726d 6174  sorship informat
+00002d10: 696f 6e2e                                ion.
```

### Comparing `thepipe_api-0.3.3/setup.py` & `thepipe_api-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.3.3',
+    version='0.3.4',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.3.3/tests/test_thepipe.py` & `thepipe_api-0.3.4/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.3/thepipe_api/compressor.py` & `thepipe_api-0.3.4/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.3/thepipe_api/core.py` & `thepipe_api-0.3.4/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.3/thepipe_api/extractor.py` & `thepipe_api-0.3.4/thepipe_api/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,17 @@
         if verbose: print_status(f"Extracted from {file_path}", status='success')
         return extraction
     except Exception as e:
         if verbose: print_status(f"Failed to extract from {file_path}: {e}", status='error')
         return [Chunk(path=file_path)]
 
 def detect_type(source: str) -> Optional[SourceTypes]:
-    if source.startswith("https://www.youtube.com"):
+    if source.startswith("https://www.youtube.com") or source.startswith("https://youtube.com"):
         return SourceTypes.YOUTUBE_VIDEO
-    if source.startswith("https://github.com"):
+    elif source.startswith("https://github.com") or source.startswith("https://www.github.com"):
         return SourceTypes.GITHUB
     elif source.startswith("http") or source.startswith("ftp."):
         return SourceTypes.URL
     elif source.endswith(".zip"):
         return SourceTypes.ZIP
     elif os.path.isdir(source) or source == '.' or source == './':
         return SourceTypes.DIR
@@ -348,23 +348,27 @@
             end_time = video.duration
         # extract frame at the middle of the chunk
         frame_time = (start_time + end_time) / 2
         frame = video.get_frame(frame_time)
         image = Image.fromarray(frame)
         # extract and transcribe audio for the current chunk
         audio_path = os.path.join(tempfile.gettempdir(), f"temp_audio_{i}.wav")
-        video.subclip(start_time, end_time).audio.write_audiofile(audio_path, codec='pcm_s16le')
-        result = model.transcribe(audio_path, verbose=verbose)
-        transcription = result['text']
+        audio = video.subclip(start_time, end_time).audio
+        if audio is None:
+            transcription = None
+        else:
+            audio.write_audiofile(audio_path, codec='pcm_s16le')
+            result = model.transcribe(audio_path, verbose=verbose)
+            transcription = result['text']
+            os.remove(audio_path)
         # add chunk
         if not text_only:
             chunks.append(Chunk(path=file_path, text=transcription, image=image, source_type=SourceTypes.VIDEO))
         else:
             chunks.append(Chunk(path=file_path, text=transcription, image=None, source_type=SourceTypes.VIDEO))
-        os.remove(audio_path)
     return chunks
 
 def extract_youtube(youtube_url: str, text_only: bool = False, verbose: bool = False) -> List[Chunk]:
     from pytube import YouTube # import only if needed
     temp_dir = "youtube_temp"
     filename = "temp_video.mp4"
     yt = YouTube(youtube_url)
```

### Comparing `thepipe_api-0.3.3/thepipe_api/thepipe.py` & `thepipe_api-0.3.4/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.3/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.3.4/thepipe_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,19 +26,19 @@
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a> <a href="https://discord.gg/bXfKeGs5qV">![Join discord](https://img.shields.io/discord/1227806200478044274?color=4f69ef&label=Discord&logo=discord&logoColor=ffffff)</a>
 
-### Feed PDFs, web pages, word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code ⚡
+### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-Language models with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that want to support comprehensive textual and visual understanding across a wide range of data sources. The Pipe is available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally to let you run the compute.
 
 ![Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/science_assistantpy2.png)
 
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
@@ -96,17 +96,17 @@
 | Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Video                                 | `.mp4`, `.avi`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames from video files; supports frame extraction and OCR for text extraction from frames |
 | Audio                                 | `.mp3`, `.wav`          | ✔️               | ❌                | Extracts text from audio files; supports speech-to-text conversion        | 
-| Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
-| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
-| YouTube Video                         | YouTube video URLs                      | ✔️               | ✔️                | Extracts text from YouTube videos; supports subtitles extraction          |
+| Website                               | URLs (inputs starting with `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| GitHub Repository                     | GitHub repo URLs (inputs starting with `https://github.com` or `https://www.github.com`)                          | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| YouTube Video                         | YouTube video URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)                     | ✔️               | ✔️                | Extracts frames and transcript from YouTube videos in per-minute chunks          |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## How it works 🛠️
 
 The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
 ```json
 [
@@ -135,33 +135,16 @@
 It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [table, equation, and figure extraction](https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
 
 
 ## Local Installation 🛠️
 
-The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
-
-```bash
-git clone https://github.com/emcf/thepipe
-pip install -r requirements_local.txt
-```
-
-Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH.
-
-Now you can use The Pipe with Python:
-```bash
-from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf", local=True)
-```
-
-or from the command line:
-```bash
-thepipe path/to/folder --local
-```
+If you do not wish to use our API, you are welcome host The Pipe for yourself locally. 
+If you choose to do this, you must install a number of dependencies for the code to function correctly, some of which may incur compute costs and/or require a GPU for reasonable performance. Additional installed dependencies are required: pytorch, universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This installation process will depend on your system and compute capabilities. After installing them, follow these steps for a local setup:
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Substring to match files in the directory. Regex is not yet supported.
 - `ignore` (optional): Substring to ignore files in the directory. Regex is not yet supported.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.3 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.4 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -11,126 +11,126 @@
 _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, web pages,
-word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code
-â¡ The Pipe is a multimodal-first tool for feeding files and web pages into
-vision-language models such as GPT-4V. It is best for LLM and RAG applications
-that require a deep understanding of tricky data sources. The Pipe is available
-as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
-[Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/
-object/public/assets/science_assistantpy2.png) ## Features ð - Extracts text
-and visuals from files or web pages ð - Outputs chunks optimized for
-multimodal LLMs and RAG frameworks ð¼ï¸ - Interpret complex PDFs, web pages,
-docs, videos, data, and more ð§  - Auto-compress prompts exceeding your chosen
-token limit ð¦ - Works even with missing file extensions, in-memory data
-streams ð¾ - Works with codebases, git repos, and custom integrations ð -
-Multi-threaded â¡ï¸ ## Getting Started ð The Pipe handles a wide array of
-complex filetypes, and thus has many dependencies that must be installed
-separately. It also requires a strong machine for good response times. For this
-reason, we host it as an API that works out-of-the-box. First, install The
-Pipe. ``` pip install thepipe_api ``` The Pipe is available as a hosted API, or
-it can be set up locally. An API key is recommended for out-of-the-box
-functionality (alternatively, see the local installation section). Ensure the
-`THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one
-here](https://thepi.pe). Now you can extract comprehensive text and visuals
-from any file: ```python from thepipe_api import thepipe messages =
-thepipe.extract("example.pdf") ``` Or websites: ```python messages =
-thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
-```python response = client.chat.completions.create( model="gpt-4-vision-
-preview", messages = messages, ) ``` ![Just call OpenAI](https://
-rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
-You can also use The Pipe from the command line. Here's how to recursively
-extract from a directory, matching only files containing a substring (in this
-example, typescript files) and ignore files containing other substrings (in
-this example, anything in the "tests" folder): ```bash thepipe path/to/folder -
--match tsx --ignore tests ``` ## Supported File Types ð | Source Type |
-Input types | Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð
-| |---------------------------------------|------------------------------------
-------|-------------------|------------------|---------------------------------
-------------------------| | Directory | Any `/path/to/directory` | âï¸ |
-âï¸ | Extracts from all files in directory, supports match and ignore
-patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸
-(varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are compressible
-with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸
-| â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text
-and images of each page; can use AI for extraction of table data and images
-within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts
-images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
-| â | Extracts data from spreadsheets; converts to text representation. For
-very large datasets, will only extract column names and types | | Jupyter
-Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
-Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
-Extracts text and images from Word documents | | Microsoft PowerPoint
-Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
-PowerPoint presentations | | Video | `.mp4`, `.avi`, `.mov`, `.wmv` | âï¸ |
-âï¸ | Extracts frames from video files; supports frame extraction and OCR
-for text extraction from frames | | Audio | `.mp3`, `.wav` | âï¸ | â |
-Extracts text from audio files; supports speech-to-text conversion | | Website
-| URLs (inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts
-text from web page along with image (or images if scrollable); text-only
-extraction available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸
-| Extracts from GitHub repositories; supports branch specification | | YouTube
-Video | YouTube video URLs | âï¸ | âï¸ | Extracts text from YouTube
-videos; supports subtitles extraction | | ZIP File | `.zip` | âï¸ | âï¸ |
-Extracts contents of ZIP files; supports nested directory extraction | ## How
-it works ð ï¸ The input source is either a file path, a URL, or a directory.
-The pipe will extract information from the source and process it for downstream
-use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
-[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
-[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
-pipe is a sensible list of multimodal messages representing chunks of the
-extracted information, carefully crafted to fit within context windows for any
-models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4]
-(https://openai.com/gpt-4). The messages returned should look like this:
-```json [ { "role": "user", "content": [ { "type": "text", "text": "..." },
-{ "type": "image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ]
-} ] ``` If you want to feed these messages directly into the model, it is
-important to be mindful of the token limit. OpenAI does not allow too many
-images in the prompt (see discussion [here](https://community.openai.com/t/gpt-
-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted
-with `text_only=True` to avoid this issue, while long text files should either
-be compressed or embedded in a RAG framework. The text and images from these
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) _!_[_J_o_i_n_ _d_i_s_c_o_r_d_]_(_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
+_1_2_2_7_8_0_6_2_0_0_4_7_8_0_4_4_2_7_4_?_c_o_l_o_r_=_4_f_6_9_e_f_&_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_f_f_f_f_f_f_)
+### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-
+Language models with one line of code â¡ The Pipe is a multimodal-first tool
+for feeding files and web pages into vision-language models such as GPT-4V. It
+is best for LLM and RAG applications that want to support comprehensive textual
+and visual understanding across a wide range of data sources. The Pipe is
+available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be
+set up locally to let you run the compute. ![Science assistant demo](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+science_assistantpy2.png) ## Features ð - Extracts text and visuals from
+files or web pages ð - Outputs chunks optimized for multimodal LLMs and RAG
+frameworks ð¼ï¸ - Interpret complex PDFs, web pages, docs, videos, data, and
+more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
+Works even with missing file extensions, in-memory data streams ð¾ - Works
+with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
+## Getting Started ð The Pipe handles a wide array of complex filetypes, and
+thus has many dependencies that must be installed separately. It also requires
+a strong machine for good response times. For this reason, we host it as an API
+that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
+``` The Pipe is available as a hosted API, or it can be set up locally. An API
+key is recommended for out-of-the-box functionality (alternatively, see the
+local installation section). Ensure the `THEPIPE_API_KEY` environment variable
+is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
+extract comprehensive text and visuals from any file: ```python from
+thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or
+websites: ```python messages = thepipe.extract("https://example.com") ``` Then
+feed it into GPT-4-Vision: ```python response = client.chat.completions.create
+( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
+(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory, matching only files containing a
+substring (in this example, typescript files) and ignore files containing other
+substrings (in this example, anything in the "tests" folder): ```bash thepipe
+path/to/folder --match tsx --ignore tests ``` ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
+`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts to text representation. For very large datasets, will only extract
+column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
+Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
+Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
+documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
+Extracts text and images from PowerPoint presentations | | Video | `.mp4`,
+`.avi`, `.mov`, `.wmv` | âï¸ | âï¸ | Extracts frames from video files;
+supports frame extraction and OCR for text extraction from frames | | Audio |
+`.mp3`, `.wav` | âï¸ | â | Extracts text from audio files; supports
+speech-to-text conversion | | Website | URLs (inputs starting with `http`,
+`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
+image (or images if scrollable); text-only extraction available | | GitHub
+Repository | GitHub repo URLs (inputs starting with `https://github.com` or
+`https://www.github.com`) | âï¸ | âï¸ | Extracts from GitHub
+repositories; supports branch specification | | YouTube Video | YouTube video
+URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)
+| âï¸ | âï¸ | Extracts frames and transcript from YouTube videos in per-
+minute chunks | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
+ZIP files; supports nested directory extraction | ## How it works ð ï¸ The
+input source is either a file path, a URL, or a directory. The pipe will
+extract information from the source and process it for downstream use with
+[language models](https://en.wikipedia.org/wiki/Large_language_model), [vision
+transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
+language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
+a sensible list of multimodal messages representing chunks of the extracted
+information, carefully crafted to fit within context windows for any models
+from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
+openai.com/gpt-4). The messages returned should look like this: ```json [
+{ "role": "user", "content": [ { "type": "text", "text": "..." }, { "type":
+"image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ] } ] ```
+If you want to feed these messages directly into the model, it is important to
+be mindful of the token limit. OpenAI does not allow too many images in the
+prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-
+maximum-amount-of-images/573110/6)), so long files should be extracted with
+`text_only=True` to avoid this issue, while long text files should either be
+compressed or embedded in a RAG framework. The text and images from these
 messages may also be prepared for a vector database with
 `thepipe.core.create_chunks_from_messages` or for downstream use with RAG
 frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily
 integrate The Pipe with any LLM provider. It uses a variety of heuristics for
 optimal performance with vision-language models, including AI filetype
 detection with [filetype detection](https://opensource.googleblog.com/2024/02/
 magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI
 [table, equation, and figure extraction](https://thepi.pe/pricing), efficient
 [token compression](https://arxiv.org/abs/2403.12968), automatic [image
 encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/
 abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172)
 effects, and more, all pre-built to work out-of-the-box. ![Demo](https://
 rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20
-(6).png) ## Local Installation ð ï¸ The Pipe handles a wide array of complex
-filetypes, and thus requires installation of many different packages to
-function. It also requires a very capable machine for good response times. For
-this reason, we host it as an API that works out-of-the-box. To use The Pipe
-locally for free instead, you will need [playwright](https://github.com/
-microsoft/playwright), [ctags](https://github.com/universal-ctags/),
-[pytesseract](https://github.com/h/pytesseract), and the local python
-requirements, which differ from the more lightweight API requirements: ```bash
-git clone https://github.com/emcf/thepipe pip install -r requirements_local.txt
-``` Tip for windows users: Install the python-libmagic binaries with `pip
-install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags`
-binaries are in your PATH. Now you can use The Pipe with Python: ```bash from
-thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
-``` or from the command line: ```bash thepipe path/to/folder --local ```
-Arguments are: - `source` (required): can be a file path, a URL, or a directory
-path. - `local` (optional): Use the local version of The Pipe instead of the
-hosted API. - `match` (optional): Substring to match files in the directory.
-Regex is not yet supported. - `ignore` (optional): Substring to ignore files in
-the directory. Regex is not yet supported. - `limit` (optional): The token
-limit for the output prompt, defaults to 100K. Prompts exceeding the limit will
-be compressed. This may not work as expected with the API, as it is in active
+(6).png) ## Local Installation ð ï¸ If you do not wish to use our API, you
+are welcome host The Pipe for yourself locally. If you choose to do this, you
+must install a number of dependencies for the code to function correctly, some
+of which may incur compute costs and/or require a GPU for reasonable
+performance. Additional installed dependencies are required: pytorch,
+universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This
+installation process will depend on your system and compute capabilities. After
+installing them, follow these steps for a local setup: Arguments are: -
+`source` (required): can be a file path, a URL, or a directory path. - `local`
+(optional): Use the local version of The Pipe instead of the hosted API. -
+`match` (optional): Substring to match files in the directory. Regex is not yet
+supported. - `ignore` (optional): Substring to ignore files in the directory.
+Regex is not yet supported. - `limit` (optional): The token limit for the
+output prompt, defaults to 100K. Prompts exceeding the limit will be
+compressed. This may not work as expected with the API, as it is in active
 development. - `ai_extraction` (optional): Extract tables, figures, and math
 from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
 not extract images from documents or websites. Additionally, image files will
 be represented with OCR instead of as images. # Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h
 _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
 Contact emmett@thepi.pe for sponsorship information.
```

