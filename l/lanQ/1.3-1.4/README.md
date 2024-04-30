# Comparing `tmp/lanQ-1.3.tar.gz` & `tmp/lanQ-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.3.tar", last modified: Mon Apr 15 09:16:29 2024, max compression
+gzip compressed data, was "lanQ-1.4.tar", last modified: Tue Apr 30 03:42:58 2024, max compression
```

## Comparing `lanQ-1.3.tar` & `lanQ-1.4.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.360690 lanQ-1.3/
--rw-rw-rw-   0        0        0      192 2024-04-15 09:16:29.358695 lanQ-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7459 2024-04-15 09:15:37.000000 lanQ-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.357697 lanQ-1.3/lanQ.egg-info/
--rw-rw-rw-   0        0        0      192 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.355704 lanQ-1.3/lanQ_rule/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.3/lanQ_rule/__init__.py
--rw-rw-rw-   0        0        0     3981 2024-04-11 02:54:19.000000 lanQ-1.3/lanQ_rule/base.py
--rw-rw-rw-   0        0        0    16420 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/common_rule.py
--rw-rw-rw-   0        0        0     1471 2024-04-11 02:54:19.000000 lanQ-1.3/lanQ_rule/const.py
--rw-rw-rw-   0        0        0      985 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/model_rule.py
--rw-rw-rw-   0        0        0     1156 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/prompt_rule.py
--rw-rw-rw-   0        0        0       42 2024-04-15 09:16:29.360690 lanQ-1.3/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-04-15 09:15:46.000000 lanQ-1.3/setup.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 03:42:58.954318 lanQ-1.4/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      185 2024-04-30 03:42:58.954318 lanQ-1.4/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     7763 2024-04-19 03:19:52.000000 lanQ-1.4/README.md
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 03:42:58.954318 lanQ-1.4/lanQ.egg-info/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      185 2024-04-30 03:42:58.000000 lanQ-1.4/lanQ.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      226 2024-04-30 03:42:58.000000 lanQ-1.4/lanQ.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-04-30 03:42:58.000000 lanQ-1.4/lanQ.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       10 2024-04-30 03:42:58.000000 lanQ-1.4/lanQ.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 03:42:58.954318 lanQ-1.4/lanQ_rule/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4/lanQ_rule/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    16072 2024-04-30 03:21:14.000000 lanQ-1.4/lanQ_rule/common_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      991 2024-04-30 03:33:53.000000 lanQ-1.4/lanQ_rule/model_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1153 2024-04-24 03:44:27.000000 lanQ-1.4/lanQ_rule/prompt_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-04-30 03:42:58.954318 lanQ-1.4/setup.cfg
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      392 2024-04-30 03:42:47.000000 lanQ-1.4/setup.py
```

### Comparing `lanQ-1.3/README.md` & `lanQ-1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,213 @@
-# lanQ v1.2
-
-English | [简体中文](README_ZH.md)
-
-Language quality evaluation tool.
-
-## Run it
-
-Clone the project into your environment.
-
-```
-git clone ssh://git@gitlab.pjlab.org.cn:1122/qa/lanq.git
-```
-
-Install the requirement packages.
-
-```
-pip install -r requirements.txt
-```
-
-Add the test data file `test_data.json` into `data/predictions` directory.  
-Then execute `main.py` with parameter `-i`.
-
-```
-python main.py -i test_data.json
-```
-
-You will get the result file `data_predictions_test_data.json` in `data/results`.
-
-If you want to test files in directory, you just need to change to file name to directory name in `data/predictions`, such as:
-
-```
-python main.py -i directory_name
-```
-
-## Data format
-
-There are 2 data format supported.  
-One is model type, contain `id`, `prompt` and `prediction` keys, as follows:  
-
-```
-{"id": "0", "prompt": "how old are you?", "prediction": "I am 8 years old."}
-```
-
-Another is data type, have `id` and `content` keys, such as:
-
-```
-{"id":"Bl1b6P41SlcCHv8gfhLy","content":"秦始皇嬴政，从此结束了贵族王侯专政的王国时代，进入了君主专制的帝国时代。"}
-```
-
-No matter what data format is, each line of data is `json` type and each data file only has one format data.   
-Besides, data exits in data file with `jsonline` style, refering to `test_data1.json` or `test_data2.json`.
-
-## Reading result
-
-The file in `data/results` directory has format as follows:
-
-```
-{
-    "score": 50.0,
-    "num_good": 1,
-    "num_bad": 1,
-    "total": 2,
-    "ERROR_RULE_COLON_END": {
-        "count": 1,
-        "ratio": 0.5,
-        "detail": [
-            {
-                "id": "0",
-                "error_reason": "冒号结尾"
-            }
-        ]
-    },
-}
-```
-
-key name | description
--|-
-`score` | `num_good` / `total`, means the quality of data.  
-`num_good` | the count of good data.  
-`num_bad` | the count of bad data, which has some error.  
-`total` | the count of all data.  
-`ERROR_RULE_COLON_END` | the error name.  
-`count` | the number of error appearance.    
-`ratio` | `count` / `total`, means the ratio of error appearance.  
-`detail` | the information of error.  
-`id` | the data id with error.  
-`error_reason` | the reason why judge the data has error. 
-
-## How to Use
-
-First, you should install the package.
-
-```
-pip install lanQ
-```
-
-After installing the tool in python environment, wo can import it in our project as follows.
-
-```
-from lanQ_rule import common_rule
-```
-
-At this time, we can use all functions in `common_rule.py`. The parameter `content` is must `string` type, such as:
-
-```
-common_bracket_unmatch(content)
-```
-
-We will get a result, which is a json type and has a key `error_status`.  
-If `error_status` is `True`, which means content has problem, the result will have other 2 keys: `error_type` and `error_reason`, for example:  
-
-```
-{
-   'error_status': True, 
-   'error_type': 'ERROR_RULE_COLON_END', 
-   'error_reason': '冒号结尾'
-}
-```
-
-## Upload 
-
-Update the version number in `setup.py`
-
-```
-setup(
-    name="lanQ",
-    version="x.y",
-    ...
-)
-```
-
-Make a .tar file for using in other project. 
-You will get a .tar file in `lanQ/dist/`
-
-```
-python .\setup.py sdist
-```
-
-Upload the .tar file to Internet.
-
-```
-twine upload .\dist\lanQ-x.y.tar.gz
-```
-
-## Summary of Quality Functions
-
-The Category in below table is the same name `.py` file in `lanQ/lanQ_rule/` path.  
-Function's name are arranged in alphabetical order.
-
-Function Name | Description                                             | Category | Version
--|---------------------------------------------------------|----------|-
-common_anti_crawler_zh | check weather the content contains anti crawl text |  common  |  1.2
-common_bracket_unmatch | check whether bracket is matches                        | common   | 1.0
-common_chaos_en | check whether content has English messy code            | common   | 1.0
-common_chaos_symbol | check whether content has a lot of meaningless words    | common   | 1.0
-common_chaos_zh | check whether content has Chinese messy code            | common   | 1.0
-common_check_photo | check whether content has photo | common | 1.2
-common_colon_end | check whether the last char is ':'                      | common   | 1.0
-common_content_null | check whether content is null | common   | 1.0
-common_doc_repeat | check whether content repeats                           | common   | 1.0
-common_ellipsis_ratio   |  check whether ratio of lines end with ellipsis is bigger than 75% | common | 1.2
-common_emoj_characters | check whether content contains emoji charactors | common | 1.2
-common_enter_more | check whether content has more than 8 continious enter | common   | 1.0
-common_enter_ratio_more | check whether enter / content is more than 25% | common   | 1.0
-common_html_entity | check whether content has html entity | common | 1.2
-common_img_html_tag | check whether content has img tag or html tag | common | 1.2
-common_invalid_web | check whether the content is invalid | common | 1.2 
-common_invisible_char | check whether content has invisible char | common | 1.2
-common_joint_special_symbol | check if there are special symbols composed of multiple symbols spliced together | common | 1.2
-common_language_mixed | check whether content is mixed in Chinese and English   | common   | 1.0
-common_license_key | check if the content contains license key| common | 1.2
-common_no_punc | check whether content has paragraph without punctuations | common   | 1.0
-common_space_more | check whether content has more than 500 space | common   | 1.0
-common_special_character | check whether special char in content, such as '�'      | common   | 1.0
-common_special_mark | check if the content contains special mark | common |1.2
-common_unconverted_symbol | check if the content contains special symbols for conversion failure | common | 1.2
-common_underscore_length | check whether the content contains underscores whose length is longer than 15 | common | 1.2
-common_url_only | check whether content is all urls | common   | 1.0
-common_word_stuck | check whether words are stuck | common   | 1.0
-model_advertisement | check whether content has model advertisement | model    | 1.0
-model_watermark | check whether content has watermark | model    | 1.0
-prompt_chinese_produce_english | check whether chinese prompt produce english prediction | prompt   | 1.0
-prompt_english_produce_chinese | check whether english prompt produce chinese prediction | prompt   | 1.0
-
-## RoadMap
- - 1.5:
-   - 支持多种数据格式的convert
- - 1.4:
-   - 增加函数的可配置性
-
-## Release Notes
- - 1.3:
-   - 重新组织 config.py 对外开放用户配置接口
-   - 添加 error 比例
-   - main 与 convert 模块批量处理
- - 1.2:
-   - 更新 main 与 config 模块，使用 callable 组织函数
-   - common_rule 添加 v1.2 新规则
-   - 新增 convert 目录，支持 stringline 转化；
-   - readme 补充使用方法与数据类型
- - 1.1:
-   - 新增 base.py 抽取基础功能;
-   - functions 按字母顺序排列
- - 1.0:   
-   - 新增 1.0 functions;  
-   - 新增 common_rule 模块;  
-   - 新增 model_rule 模块;  
-   - 新增 prompt_rule 模块;  
-   - 新增 convert 功能;
-   - 新增 main.py 支持本质运行。
+# lanQ v1.2
+
+English | [简体中文](README_ZH.md)
+
+Language quality evaluation tool.
+
+## Run it
+
+Clone the project into your environment.
+
+```
+git clone ssh://git@gitlab.pjlab.org.cn:1122/qa/lanq.git
+```
+
+Install the requirement packages.
+
+```
+pip install -r requirements.txt
+```
+
+Add the test data file `test_data.json` into `data/predictions` directory.  
+Then execute `main.py` with parameter `-i`.
+
+```
+python main.py -i test_data.json
+```
+
+You will get the result file `data_predictions_test_data.json` in `data/results`.
+
+If you want to test files in directory, you just need to change to file name to directory name in `data/predictions`, such as:
+
+```
+python main.py -i directory_name
+```
+
+## Data format
+
+There are 2 data format supported.  
+One is model type, contain `id`, `prompt` and `prediction` keys, as follows:  
+
+```
+{"id": "0", "prompt": "how old are you?", "prediction": "I am 8 years old."}
+```
+
+Another is data type, have `id` and `content` keys, such as:
+
+```
+{"id":"Bl1b6P41SlcCHv8gfhLy","content":"秦始皇嬴政，从此结束了贵族王侯专政的王国时代，进入了君主专制的帝国时代。"}
+```
+
+No matter what data format is, each line of data is `json` type and each data file only has one format data.   
+Besides, data exits in data file with `jsonline` style, refering to `test_data1.json` or `test_data2.json`.
+
+## Reading result
+
+The file in `data/results` directory has format as follows:
+
+```
+{
+    "score": 50.0,
+    "num_good": 1,
+    "num_bad": 1,
+    "total": 2,
+    "ERROR_RULE_COLON_END": {
+        "count": 1,
+        "ratio": 0.5,
+        "detail": [
+            {
+                "id": "0",
+                "error_reason": "冒号结尾"
+            }
+        ]
+    },
+}
+```
+
+key name | description
+-|-
+`score` | `num_good` / `total`, means the quality of data.  
+`num_good` | the count of good data.  
+`num_bad` | the count of bad data, which has some error.  
+`total` | the count of all data.  
+`ERROR_RULE_COLON_END` | the error name.  
+`count` | the number of error appearance.    
+`ratio` | `count` / `total`, means the ratio of error appearance.  
+`detail` | the information of error.  
+`id` | the data id with error.  
+`error_reason` | the reason why judge the data has error. 
+
+## How to Use
+
+First, you should install the package.
+
+```
+pip install lanQ
+```
+
+After installing the tool in python environment, wo can import it in our project as follows.
+
+```
+from lanQ_rule import common_rule
+```
+
+At this time, we can use all functions in `common_rule.py`. The parameter `content` is must `string` type, such as:
+
+```
+common_bracket_unmatch(content)
+```
+
+We will get a result, which is a json type and has a key `error_status`.  
+If `error_status` is `True`, which means content has problem, the result will have other 2 keys: `error_type` and `error_reason`, for example:  
+
+```
+{
+   'error_status': True, 
+   'error_type': 'ERROR_RULE_COLON_END', 
+   'error_reason': '冒号结尾'
+}
+```
+
+## Upload 
+
+Update the version number in `setup.py`
+
+```
+setup(
+    name="lanQ",
+    version="x.y",
+    ...
+)
+```
+
+Make a .tar file for using in other project. 
+You will get a .tar file in `lanQ/dist/`
+
+```
+python .\setup.py sdist
+```
+
+Upload the .tar file to Internet.
+
+```
+twine upload .\dist\lanQ-x.y.tar.gz
+```
+
+## Summary of Quality Functions
+
+The Category in below table is the same name `.py` file in `lanQ/lanQ_rule/` path.  
+Function's name are arranged in alphabetical order.
+
+Function Name | Error Rule | Description                                             | Category 
+-|-|---------------------------------------------------------|----------
+common_anti_crawler_zh | ERROR_CRAWL_ANTI | check weather the content contains anti crawl text |  common  
+common_bracket_unmatch | ERROR_BRACKET_UNMATCH | check whether bracket is matches                        | common   
+common_chaos_en | ERROR_CHAOS_EN | check whether content has English messy code            | common   
+common_chaos_symbol |ERROR_CHAOS_SYMBOL | check whether content has a lot of meaningless words    | common   
+common_chaos_zh | ERROR_CHAOS_ZH | check whether content has Chinese messy code            | common   
+common_check_photo | ERROR_CHECK_PHOTO | check whether content has photo | common 
+common_colon_end | ERROR_RULE_COLON_END | check whether the last char is ':'                      | common   
+common_content_null | ERROR_CONTENT_NULL | check whether content is null | common   
+common_doc_repeat | ERROR_DOC_REPEAT | check whether content repeats                           | common   
+common_ellipsis_ratio | ERROR_ELLIPSIS_RATIO |  check whether ratio of lines end with ellipsis is bigger than 75% | common 
+common_emoj_characters | ERROR_EMOJ_CHAR | check whether content contains emoji charactors | common 
+common_enter_more | ERROR_ENTER_MORE | check whether content has more than 8 continious enter | common   
+common_enter_ratio_more | ERROR_ENTER_RATIO_MORE | check whether enter / content is more than 25% | common   
+common_html_entity | ERROR_HTML_ENTITY | check whether content has html entity | common 
+common_img_html_tag | ERROR_IMG_HTML_TAG | check whether content has img tag or html tag | common 
+common_invalid_web | ERROR_INVALID_WEB | check whether the content is invalid | common  
+common_invisible_char | ERROR_INVISIBLE_CHAR | check whether content has invisible char | common 
+common_joint_special_symbol | ERROR_JOINT_SPECIAL_SYMBOL | check if there are special symbols composed of multiple symbols spliced together | common 
+common_language_mixed | ERROR_LANGUAGE_MIXED | check whether content is mixed in Chinese and English   | common   
+common_license_key | ERROR_LICENSE_KEY | check if the content contains license key| common 
+common_no_punc | ERROR_NO_PUNC | check whether content has paragraph without punctuations | common   
+common_space_more | ERROR_SPACE_MORE | check whether content has more than 500 space | common   
+common_special_character | ERROR_SPECIAL_CHARACTER | check whether special char in content, such as '�'      | common   
+common_special_mark | ERROR_SPECIAL_MARK | check if the content contains special mark | common |1.2
+common_unconverted_symbol | ERROR_UNCONVERTED_SYMBOL | check if the content contains special symbols for conversion failure | common 
+common_underscore_length | ERROR_UNDERSCORE_LENGTH | check whether the content contains underscores whose length is longer than 15 | common 
+common_url_only | ERROR_URL_ONLY | check whether content is all urls | common   
+common_word_stuck | ERROR_WORD_STUCK | check whether words are stuck | common   
+model_advertisement | ERROR_ADVERTISEMENT | check whether content has model advertisement | model    
+model_watermark | ERROR_WATERMARK | check whether content has watermark | model    
+prompt_chinese_produce_english | ERROR_CHINESE_PRODUCE_ENGLISH | check whether chinese prompt produce english prediction | prompt   
+prompt_english_produce_chinese | ERROR_ENGLISH_PRODUCE_CHINESE | check whether english prompt produce chinese prediction | prompt   
+
+## RoadMap
+ - 1.6:
+   - add benchmark for rules
+ - 1.5:
+   - add convert for different data type
+ - 1.4:
+   - add config of functions
+
+## Release Notes
+ - 1.3:
+   - reorganize `config.py`, let user can configure
+   - add error ratio
+   - `main.py` and `convert` support input directory
+ - 1.2:
+   - add v1.2 rules
+   - update `main.py` and `config` module, use callable type to organize functions
+   - add convert folder, support stringline type
+   - `readme` add usage and data type
+ - 1.1:
+   - add `base.py` contain base functions
+   - sort functions by alphabetic order
+ - 1.0:   
+   - add 1.0 functions
+   - add common_rule module
+   - add model_rule module 
+   - add prompt_rule module
+   - add convert function
+   - add `main.py`
```

### Comparing `lanQ-1.3/lanQ_rule/common_rule.py` & `lanQ-1.4/lanQ_rule/common_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,431 +1,428 @@
-import re
-import os
-import sys
-import numpy
-import jieba
-import string
-import langid
-import textstat
-import unicodedata
-import zhon.hanzi
-from collections import Counter
-from hanziconv import HanziConv
-
-sys.path.append(os.path.dirname(__file__))
-
-from base import *
-from const import *
-
-def common_anti_crawler_zh(content: str) -> dict:
-    """from lvkai"""
-    res = {'error_status': False}
-    line_num = 50
-    content_lines = [l.strip() for l in content.split("\n") if len(l.strip())]
-    max_jieba_ratio = 0
-    for line in content_lines:
-        line = get_real_text(line)
-        char_num = len(line)
-        word_num = 0
-        if len(line) > line_num:
-            seg_list = jieba.cut(line, cut_all=True)
-            for word in seg_list:
-                if len(word) == 1:
-                    word_num += 1
-            max_jieba_ratio = max(max_jieba_ratio, word_num / char_num)
-    if max_jieba_ratio > 0.8:
-        res["error_status"] = True
-        res["error_type"][ERROR_CRAWL_ANTI] = ERROR_CRAWL_ANTI
-        res["error_reason"][ERROR_CRAWL_ANTI] = "包含反爬文本"
-    return res
-
-def common_bracket_unmatch(content: str) -> dict:
-    """check whether bracket matches"""
-    res = {'error_status': False}
-    bracket_types = [("[", "]"), ("{", "}"), ("【", "】"), ("《", "》")]
-    for open_bracket, close_bracket in bracket_types:
-        if content.count(open_bracket) != content.count(close_bracket):
-            res["error_status"] = True
-            res["error_type"][ERROR_BRACKET_UNMATCH] = ERROR_BRACKET_UNMATCH
-            res["error_reason"][ERROR_BRACKET_UNMATCH] = "括号数量不一致"
-    return res
-
-def common_chaos_en(content: str) -> dict:
-    """check whether content has English messy code"""
-    res = {'error_status': False}
-    lan = langid.classify(content)[0]
-    if lan != 'en':
-        return res
-    s = normalize(content)
-    str_len = len(s)
-    seg_len = len(list(jieba.cut(s)))
-    num_bytes = len(content.encode('utf-8'))
-    tokens_len = int(num_bytes * 0.248)
-    if str_len == 0 or seg_len == 0 or tokens_len < 50:
-        return res
-    if str_len / seg_len <= 1.2:
-        res["error_status"] = True
-        res["error_type"] = ERROR_CHAOS_EN
-        res['error_reason'] = '英文乱码'
-    return res
-
-def common_chaos_symbol(content: str) -> dict:
-    """check whether content has a lot of meaningless words"""
-    res = {'error_status': False}
-    pattern = r'[0-9a-zA-Z\u4e00-\u9fa5]'
-    s = re.sub(pattern, '', content)
-    str_len = len(content)
-    symbol_len = len(s)
-    if str_len == 0 or symbol_len == 0:
-        return res
-    if symbol_len / str_len > 0.5:
-        res["error_status"] = True
-        res["error_type"] = ERROR_CHAOS_SYMBOL
-        res['error_reason'] = '大量非正文内容'
-    return res
-
-def common_chaos_zh(content: str) -> dict:
-    """check whether content has Chinese messy code"""
-    res = {'error_status': False}
-    lan = langid.classify(content)[0]
-    if lan != 'zh':
-        return res
-    s = normalize(content)
-    pattern = r'[a-zA-Zāáǎàēéěèīíǐìōóǒòūúǔùǖǘǚǜ\n\s]'
-    s = re.sub(pattern, '', s)
-    s_simplified = HanziConv.toSimplified(s)
-    str_len = len(s)
-    seg_len = len(list(jieba.cut(s_simplified)))
-    num_bytes = len(content.encode('utf-8'))
-    tokens_len = int(num_bytes * 0.248)
-    if str_len == 0 or seg_len == 0 or tokens_len < 50:
-        return res
-    if str_len / seg_len <= 1.1:
-        res["error_status"] = True
-        res["error_type"] = ERROR_CHAOS_ZH
-        res['error_reason'] = '中文乱码'
-    return res
-
-def common_check_photo(content: str) -> dict:
-    """check whether content has photo"""
-    res = {'error_status': False}
-    pattern = '!\[\]\(http[s]?://.*?jpeg "\n"\)'
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_CHECK_PHOTO
-        res['error_reason'] = matches
-    return res
-
-def common_colon_end(content: str) -> dict:
-    """check whether the last char is ':'"""
-    res = {'error_status': False}
-    if len(content) <= 0:
-        return res
-    if content[-1] == ':':
-        res['error_status'] = True
-        res['error_type'] = ERROR_RULE_COLON_END
-        res['error_reason'] = '冒号结尾'
-    return res
-
-def common_content_null(content: str) -> dict:
-    """check whether content is null"""
-    res = {'error_status': False}
-    count = len(content.strip())
-    if count == 0:
-        res["error_status"] = True
-        res["error_type"] = ERROR_CONTENT_NULL
-        res['error_reason'] = '内容为空'
-    return res
-
-def common_doc_repeat(content: str) -> dict:
-    """check whether content repeats"""
-    res = {'error_status': False}
-    repeat_score = base_rps_frac_chars_in_dupe_ngrams(6, content)
-    if repeat_score >= 80:
-        res["error_status"] = True
-        res["error_type"] = ERROR_DOC_REPEAT
-        res['error_reason'] = '文本重复度过高： ' + str(repeat_score)
-    return res
-
-def common_ellipsis_ratio(content: str) -> dict:
-    """check whether ratio of lines end with ellipsis is bigger than 75%"""
-    res = {'error_status': False}
-    lines = content.split("\n")
-    non_empty_lines = 0
-    ellipsis_lines = 0
-    for line in lines:
-        if line.strip() != "":
-            non_empty_lines += 1
-            if (
-                line.strip().endswith("。。。")
-                or line.strip().endswith("…")
-                or line.strip().endswith("。。。。。。")
-                or line.strip().endswith("……")
-            ):
-                ellipsis_lines += 1
-    if non_empty_lines != 0:
-        ellipsis_ratio = ellipsis_lines / non_empty_lines
-        if ellipsis_ratio >0.75:
-            res["error_status"] = True
-            res['error_type'][ERROR_ELLIPSIS_RATIO] = ERROR_ELLIPSIS_RATIO
-            res["error_reason"][ERROR_ELLIPSIS_RATIO] = "省略号结尾行占比超过75%" 
-    return res
-
-def common_emoj_characters(content: str) -> dict:
-    """check whether content contains emoji charactors"""
-    res = {'error_status': False}
-    emoj_chars_pattern = r"U\+26[0-F][0-D]|U\+273[3-4]|U\+1F[3-6][0-4][0-F]|U\+1F6[8-F][0-F]"
-    matches = re.search(emoj_chars_pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"][ERROR_EMOJ_CHAR] = ERROR_EMOJ_CHAR
-        res["error_reason"][ERROR_EMOJ_CHAR] = "包含emoji符号"
-    return res
-
-def common_enter_more(content: str) -> dict:
-    """check whether content has more than 8 continious enter"""
-    res = {'error_status': False}
-    pattern = r'\n{8,}|\r{8,}'
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_ENTER_MORE
-        res['error_reason'] = '存在连续8个回车'
-    return res
-
-def common_enter_ratio_more(content: str) -> dict:
-    """check whether enter / content is more than 25%"""
-    res = {'error_status': False}
-    enter_count = content.count('\n')
-    count = len(content)
-    if count == 0:
-        return res
-    ratio = enter_count / count * 100
-    if ratio >= 25:
-        res["error_status"] = True
-        res["error_type"] = ERROR_ENTER_RATIO_MORE
-        res['error_reason'] = '回车超过正文25%'
-    return res
-
-def common_html_entity(content: str) -> dict:
-    """check whether content has html entity"""
-    res = {'error_status': False}
-    entities = [
-        "nbsp",
-        "lt",
-        "gt",
-        "amp",
-        "quot",
-        "apos",
-        "hellip",
-        "ndash",
-        "mdash",
-        "lsquo",
-        "rsquo",
-        "ldquo",
-        "rdquo",
-    ]
-    full_entities_1 = [f"&{entity}；" for entity in entities]
-    full_entities_2 = [f"&{entity};" for entity in entities]
-    full_entities_3 = [f"＆{entity};" for entity in entities]
-    full_entities_4 = [f"＆{entity}；" for entity in entities]
-    full_entities = (
-        full_entities_1 + full_entities_2 + full_entities_3 + full_entities_4
-    )
-    # half_entity_1 = [f"{entity}；" for entity in entities]
-    half_entity_2 = [f"＆{entity}" for entity in entities]
-    half_entity_3 = [f"&{entity}" for entity in entities]
-    # half_entity_4 = [f"{entity};" for entity in entities]
-    half_entities = half_entity_2 + half_entity_3
-    # maked_entities = [f"{entity}" for entity in entities]
-    all_entities = full_entities + half_entities
-
-    pattern = '|'.join(all_entities)
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_HTML_ENTITY
-        res['error_reason'] = matches
-    return res
-
-def common_img_html_tag(content: str) -> dict:
-    """check whether content has img or html tag"""
-    res = {'error_status': False}
-    pattern = r"(<img[^>]*>)|<p[^>]*>(.*?)<\/p>|<o:p[^>]*>(.*?)<\/o:p>"
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_IMG_HTML_TAG
-        res['error_reason'] = matches
-    return res
-
-def common_invalid_web(content: str) -> dict:
-    """check whether the content is invalid"""
-    res = {'error_status': False}
-    invalid_list = ["404 - Page not found\nThe requested page does not exist (or has been deleted).\nIf you typed a URL by hand, or used a bookmark, please double check the address that you used.\nIf you see this page, and the error persists, please contact Customer Care and provide details about the action you tried to perform."]
-    for item in invalid_list:
-        if item in content:
-            res["error_status"] = True
-            res["error_type"][ERROR_INVALID_WEB] = ERROR_INVALID_WEB
-            res["error_reason"][ERROR_INVALID_WEB] = "content内容为404"
-    return res
-
-def common_invisible_char(content: str) -> dict:
-    """check whether content has invisible char"""
-    res = {'error_status': False}
-    pattern = r"[\u2000-\u200F\u202F\u205F\u3000\uFEFF\u00A0\u2060-\u206F\uFEFF\xa0]"
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_INVISIBLE_CHAR
-        res['error_reason'] = matches
-    return res
-
-def common_joint_special_symbol(content: str) -> dict:
-    """check if there are special symbols composed of multiple symbols spliced together"""
-    res = {'error_status': False}
-    pattern = r"&#247;|\? :"
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"][ERROR_JOINT_SPECIAL_SYMBOL] = ERROR_JOINT_SPECIAL_SYMBOL
-        res["error_reason"][ERROR_JOINT_SPECIAL_SYMBOL] = "包含多个符号拼接组成的特殊符号"
-    return res
-
-def common_language_mixed(content: str) -> dict:
-    """check whether content is mixed in Chinese and English"""
-    res = {'error_status': False}
-    s = normalize(content)
-    en_len = len(re.findall(r'[a-zA-Z]', s))
-    zh_len = len(re.findall(r'[\u4e00-\u9fa5]', s))
-    count_len = len(s)
-    if count_len == 0:
-        return res
-    if en_len / count_len >= 0.5 and zh_len / count_len >= 0.1:
-        res["error_status"] = True
-        res["error_type"] = ERROR_LANGUAGE_MIXED
-        res['error_reason'] = '中英文混杂'
-    return res
-
-def common_license_key(content: str) -> dict:
-    """check if the content contains license key"""
-    res = {'error_status': False}
-    # 定义三个模式对应于上述的三种格式
-    pattern = r"(License|破解)|" + "|".join([
-    "[A-Z0-9]{47}",  # 字母数字混合
-    "[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}",  # 分段的字母数字混合
-    "[A-Z0-9]{4}-\d{8}-[A-Z0-9]{4}"  # 含有特定信息的许可证密钥，例如产品ID和购买日期
-    ])
-    match = re.search(pattern, content, re.I)  # re.I使匹配对大小写不敏感
-    if match:
-        res["error_status"] = True
-        res["error_type"][ERROR_LICENSE_KEY] = ERROR_LICENSE_KEY
-        res["error_reason"][ERROR_LICENSE_KEY] = "包含license key"
-    return res
-
-def common_no_punc(content: str) -> dict:
-    """check whether content has paragraph without punctuations"""
-    res = {'error_status': False}
-    paragraphs = content.split('\n')
-    max_word_count = 0
-    for paragraph in paragraphs:
-        if len(paragraph) == 0:
-            continue
-        sentences = re.split(r'[-–.!?,;•、。！？，；·]', paragraph)
-        for sentence in sentences:
-            words = sentence.split()
-            word_count = len(words)
-            if word_count > max_word_count:
-                max_word_count = word_count
-    text_stat_res = textstat.flesch_reading_ease(content)
-    if int(max_word_count) > 56 and text_stat_res < 20:
-        res["error_status"] = True
-        res["error_type"] = ERROR_NO_PUNC
-        res['error_reason'] = '段落无标点'
-    return res
-
-def common_space_more(content: str) -> dict:
-    """check whether content has more than 500 consecutive spaces"""
-    res = {'error_status': False}
-    pattern = r' {500,}'
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_SPACE_MORE
-        res['error_reason'] = '存在连续500个空格'
-    return res
-
-def common_special_character(content: str) -> dict:
-    res = {'error_status': False}
-    pattern = r"[�□\^]|\{\/U\}"
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_SPECIAL_CHARACTER
-        res['error_reason'] = matches
-    return res
-
-def common_special_mark(content: str) -> dict:
-    """check if the content contains special mark"""
-    res = {'error_status': False}
-    pattern = r'keyboard_arrow_(left|right)'
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"][ERROR_SPECIAL_MARK] = ERROR_SPECIAL_MARK
-        res["error_reason"][ERROR_SPECIAL_MARK] = "元素包含特殊标记"
-    return res
-
-def common_unconverted_symbol(content: str) -> dict:
-    """check if the content contains special symbols for conversion failure"""
-    res = {'error_status': False}
-    pattern = r'u200e'
-    matches = re.findall(pattern, content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"][ERROR_UNCONVERTED_SYMBOL] = ERROR_UNCONVERTED_SYMBOL
-        res["error_reason"][ERROR_UNCONVERTED_SYMBOL] = "包含转换失败的特殊符号"
-    return res
-
-def common_underscore_length(content: str) -> dict:
-    """check whether the content contains underscores whose length is longer than 15"""
-    res = {'error_status': False}
-    max_underscore_count = 0
-    for char in content:
-        if char == '_':
-            underscore_count += 1
-            if underscore_count > max_underscore_count:
-                max_underscore_count = underscore_count
-        else:
-            underscore_count = 0
-    if max_underscore_count >= 15:
-        res["error_status"] = True
-        res["error_type"][ERROR_UNDERSCORE_LENGTH] = ERROR_UNDERSCORE_LENGTH
-        res["error_reason"][ERROR_UNDERSCORE_LENGTH] = "下划线长度大于15"
-    return res
-
-def common_url_only(content: str) -> dict:
-    """check whether content is all urls"""
-    res = {'error_status': False}
-    pattern = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'  # noqa
-    s = re.sub(pattern, '', content)
-    count = len(s.strip())
-    if count == 0:
-        res["error_status"] = True
-        res["error_type"] = ERROR_URL_ONLY
-        res['error_reason'] = '内容只有url'
-    return res
-
-def common_word_stuck(content: str) -> dict:
-    """check whether words are stuck"""
-    res = {'error_status': False}
-    words = re.findall(r'[a-zA-Z]+', content)
-    max_word_len = 0
-    for word in words:
-        if len(word) > max_word_len:
-            max_word_len = len(word)
-    if max_word_len > 45:
-        res["error_status"] = True
-        res["error_type"] = ERROR_WORD_STUCK
-        res['error_reason'] = '英文单词黏连'
+import os
+import sys
+import jieba
+import langid
+import textstat
+from hanziconv import HanziConv
+
+sys.path.append(os.path.dirname(__file__))
+
+import lanQ_rule.config.customize as cm
+from lanQ_rule.base_func.base import *
+from lanQ_rule.config.const import *
+
+def common_anti_crawler_zh(content: str) -> dict:
+    """from lvkai"""
+    res = {'error_status': False}
+    line_num = 50
+    content_lines = [l.strip() for l in content.split("\n") if len(l.strip())]
+    max_jieba_ratio = 0
+    for line in content_lines:
+        line = get_real_text(line)
+        char_num = len(line)
+        word_num = 0
+        if len(line) > line_num:
+            seg_list = jieba.cut(line, cut_all=True)
+            for word in seg_list:
+                if len(word) == 1:
+                    word_num += 1
+            max_jieba_ratio = max(max_jieba_ratio, word_num / char_num)
+    if max_jieba_ratio > cm.common_anti_crawler_zh['threshold']:
+        res["error_status"] = True
+        res["error_type"][ERROR_CRAWL_ANTI] = ERROR_CRAWL_ANTI
+        res["error_reason"][ERROR_CRAWL_ANTI] = "包含反爬文本"
+    return res
+
+def common_bracket_unmatch(content: str) -> dict:
+    """check whether bracket matches"""
+    res = {'error_status': False}
+    bracket_types = [("[", "]"), ("{", "}"), ("【", "】"), ("《", "》")]
+    for open_bracket, close_bracket in bracket_types:
+        if content.count(open_bracket) != content.count(close_bracket):
+            res["error_status"] = True
+            res["error_type"][ERROR_BRACKET_UNMATCH] = ERROR_BRACKET_UNMATCH
+            res["error_reason"][ERROR_BRACKET_UNMATCH] = "括号数量不一致"
+    return res
+
+def common_chaos_en(content: str) -> dict:
+    """check whether content has English messy code"""
+    res = {'error_status': False}
+    af_en = delete_punc_en(content)
+    af_ch = delte_punc_ch(af_en)
+    str_len = len(af_ch)
+    language = langid.classify(content)[0]
+    if language == "en":
+        seg_len = len(list(jieba.cut(af_ch)))
+        if str_len == 0 or seg_len == 0 or get_tokens(content, language) < 50:
+            return res
+        if str_len / seg_len > 1.2:
+            return res
+        else:
+            res["error_status"] = True
+            res["error_type"] = ERROR_CHAOS_EN
+            res["error_reason"] = '英文乱码'
+            return res
+    else:
+        return res
+
+def common_chaos_symbol(content: str) -> dict:
+    """check whether content has a lot of meaningless words"""
+    res = {'error_status': False}
+    pattern = r'[0-9a-zA-Z\u4e00-\u9fa5]'
+    s = re.sub(pattern, '', content)
+    str_len = len(content)
+    symbol_len = len(s)
+    if str_len == 0 or symbol_len == 0:
+        return res
+    if symbol_len / str_len > 0.5:
+        res["error_status"] = True
+        res["error_type"] = ERROR_CHAOS_SYMBOL
+        res['error_reason'] = '大量非正文内容'
+    return res
+
+def common_chaos_zh(content: str) -> dict:
+    """check whether content has Chinese messy code"""
+    res = {'error_status': False}
+    lan = langid.classify(content)[0]
+    if lan != 'zh':
+        return res
+    s = normalize(content)
+    pattern = r'[a-zA-Zāáǎàēéěèīíǐìōóǒòūúǔùǖǘǚǜ\n\s]'
+    s = re.sub(pattern, '', s)
+    s_simplified = HanziConv.toSimplified(s)
+    str_len = len(s)
+    seg_len = len(list(jieba.cut(s_simplified)))
+    num_bytes = len(content.encode('utf-8'))
+    tokens_len = int(num_bytes * 0.248)
+    if str_len == 0 or seg_len == 0 or tokens_len < 50:
+        return res
+    if str_len / seg_len <= 1.1:
+        res["error_status"] = True
+        res["error_type"] = ERROR_CHAOS_ZH
+        res['error_reason'] = '中文乱码'
+    return res
+
+def common_check_photo(content: str) -> dict:
+    """check whether content has photo"""
+    res = {'error_status': False}
+    pattern = '!\[\]\(http[s]?://.*?jpeg "\n"\)'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_CHECK_PHOTO
+        res['error_reason'] = matches
+    return res
+
+def common_colon_end(content: str) -> dict:
+    """check whether the last char is ':'"""
+    res = {'error_status': False}
+    if len(content) <= 0:
+        return res
+    if content[-1] == ':':
+        res['error_status'] = True
+        res['error_type'] = ERROR_RULE_COLON_END
+        res['error_reason'] = '冒号结尾'
+    return res
+
+def common_content_null(content: str) -> dict:
+    """check whether content is null"""
+    res = {'error_status': False}
+    count = len(content.strip())
+    if count == 0:
+        res["error_status"] = True
+        res["error_type"] = ERROR_CONTENT_NULL
+        res['error_reason'] = '内容为空'
+    return res
+
+def common_doc_repeat(content: str) -> dict:
+    """check whether content repeats"""
+    res = {'error_status': False}
+    repeat_score = base_rps_frac_chars_in_dupe_ngrams(6, content)
+    if repeat_score >= 80:
+        res["error_status"] = True
+        res["error_type"] = ERROR_DOC_REPEAT
+        res['error_reason'] = '文本重复度过高： ' + str(repeat_score)
+    return res
+
+def common_ellipsis_ratio(content: str) -> dict:
+    """check whether ratio of lines end with ellipsis is bigger than 75%"""
+    res = {'error_status': False}
+    lines = content.split("\n")
+    non_empty_lines = 0
+    ellipsis_lines = 0
+    for line in lines:
+        if line.strip() != "":
+            non_empty_lines += 1
+            if (
+                line.strip().endswith("。。。")
+                or line.strip().endswith("…")
+                or line.strip().endswith("。。。。。。")
+                or line.strip().endswith("……")
+            ):
+                ellipsis_lines += 1
+    if non_empty_lines != 0:
+        ellipsis_ratio = ellipsis_lines / non_empty_lines
+        if ellipsis_ratio >0.75:
+            res["error_status"] = True
+            res['error_type'][ERROR_ELLIPSIS_RATIO] = ERROR_ELLIPSIS_RATIO
+            res["error_reason"][ERROR_ELLIPSIS_RATIO] = "省略号结尾行占比超过75%" 
+    return res
+
+def common_emoj_characters(content: str) -> dict:
+    """check whether content contains emoji charactors"""
+    res = {'error_status': False}
+    emoj_chars_pattern = r"U\+26[0-F][0-D]|U\+273[3-4]|U\+1F[3-6][0-4][0-F]|U\+1F6[8-F][0-F]"
+    matches = re.search(emoj_chars_pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"][ERROR_EMOJ_CHAR] = ERROR_EMOJ_CHAR
+        res["error_reason"][ERROR_EMOJ_CHAR] = "包含emoji符号"
+    return res
+
+def common_enter_more(content: str) -> dict:
+    """check whether content has more than 8 continious enter"""
+    res = {'error_status': False}
+    pattern = r'\n{8,}|\r{8,}'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_ENTER_MORE
+        res['error_reason'] = '存在连续8个回车'
+    return res
+
+def common_enter_ratio_more(content: str) -> dict:
+    """check whether enter / content is more than 25%"""
+    res = {'error_status': False}
+    enter_count = content.count('\n')
+    count = len(content)
+    if count == 0:
+        return res
+    ratio = enter_count / count * 100
+    if ratio >= 25:
+        res["error_status"] = True
+        res["error_type"] = ERROR_ENTER_RATIO_MORE
+        res['error_reason'] = '回车超过正文25%'
+    return res
+
+def common_html_entity(content: str) -> dict:
+    """check whether content has html entity"""
+    res = {'error_status': False}
+    entities = [
+        "nbsp",
+        "lt",
+        "gt",
+        "amp",
+        "quot",
+        "apos",
+        "hellip",
+        "ndash",
+        "mdash",
+        "lsquo",
+        "rsquo",
+        "ldquo",
+        "rdquo",
+    ]
+    full_entities_1 = [f"&{entity}；" for entity in entities]
+    full_entities_2 = [f"&{entity};" for entity in entities]
+    full_entities_3 = [f"＆{entity};" for entity in entities]
+    full_entities_4 = [f"＆{entity}；" for entity in entities]
+    full_entities = (
+        full_entities_1 + full_entities_2 + full_entities_3 + full_entities_4
+    )
+    # half_entity_1 = [f"{entity}；" for entity in entities]
+    half_entity_2 = [f"＆{entity}" for entity in entities]
+    half_entity_3 = [f"&{entity}" for entity in entities]
+    # half_entity_4 = [f"{entity};" for entity in entities]
+    half_entities = half_entity_2 + half_entity_3
+    # maked_entities = [f"{entity}" for entity in entities]
+    all_entities = full_entities + half_entities
+
+    pattern = '|'.join(all_entities)
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_HTML_ENTITY
+        res['error_reason'] = matches
+    return res
+
+def common_img_html_tag(content: str) -> dict:
+    """check whether content has img or html tag"""
+    res = {'error_status': False}
+    pattern = r"(<img[^>]*>)|<p[^>]*>(.*?)<\/p>|<o:p[^>]*>(.*?)<\/o:p>"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_IMG_HTML_TAG
+        res['error_reason'] = matches
+    return res
+
+def common_invalid_web(content: str) -> dict:
+    """check whether the content is invalid"""
+    res = {'error_status': False}
+    invalid_list = ["404 - Page not found\nThe requested page does not exist (or has been deleted).\nIf you typed a URL by hand, or used a bookmark, please double check the address that you used.\nIf you see this page, and the error persists, please contact Customer Care and provide details about the action you tried to perform."]
+    for item in invalid_list:
+        if item in content:
+            res["error_status"] = True
+            res["error_type"][ERROR_INVALID_WEB] = ERROR_INVALID_WEB
+            res["error_reason"][ERROR_INVALID_WEB] = "content内容为404"
+    return res
+
+def common_invisible_char(content: str) -> dict:
+    """check whether content has invisible char"""
+    res = {'error_status': False}
+    pattern = r"[\u2000-\u200F\u202F\u205F\u3000\uFEFF\u00A0\u2060-\u206F\uFEFF\xa0]"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_INVISIBLE_CHAR
+        res['error_reason'] = matches
+    return res
+
+def common_joint_special_symbol(content: str) -> dict:
+    """check if there are special symbols composed of multiple symbols spliced together"""
+    res = {'error_status': False}
+    pattern = r"&#247;|\? :"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"][ERROR_JOINT_SPECIAL_SYMBOL] = ERROR_JOINT_SPECIAL_SYMBOL
+        res["error_reason"][ERROR_JOINT_SPECIAL_SYMBOL] = "包含多个符号拼接组成的特殊符号"
+    return res
+
+def common_language_mixed(content: str) -> dict:
+    """check whether content is mixed in Chinese and English"""
+    res = {'error_status': False}
+    s = normalize(content)
+    en_len = len(re.findall(r'[a-zA-Z]', s))
+    zh_len = len(re.findall(r'[\u4e00-\u9fa5]', s))
+    count_len = len(s)
+    if count_len == 0:
+        return res
+    if en_len / count_len >= 0.5 and zh_len / count_len >= 0.1:
+        res["error_status"] = True
+        res["error_type"] = ERROR_LANGUAGE_MIXED
+        res['error_reason'] = '中英文混杂'
+    return res
+
+def common_license_key(content: str) -> dict:
+    """check if the content contains license key"""
+    res = {'error_status': False}
+    # 定义三个模式对应于上述的三种格式
+    pattern = r"(License|破解)|" + "|".join([
+    "[A-Z0-9]{47}",  # 字母数字混合
+    "[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}",  # 分段的字母数字混合
+    "[A-Z0-9]{4}-\d{8}-[A-Z0-9]{4}"  # 含有特定信息的许可证密钥，例如产品ID和购买日期
+    ])
+    match = re.search(pattern, content, re.I)  # re.I使匹配对大小写不敏感
+    if match:
+        res["error_status"] = True
+        res["error_type"][ERROR_LICENSE_KEY] = ERROR_LICENSE_KEY
+        res["error_reason"][ERROR_LICENSE_KEY] = "包含license key"
+    return res
+
+def common_no_punc(content: str) -> dict:
+    """check whether content has paragraph without punctuations"""
+    res = {'error_status': False}
+    paragraphs = content.split('\n')
+    max_word_count = 0
+    for paragraph in paragraphs:
+        if len(paragraph) == 0:
+            continue
+        sentences = re.split(r'[-–.!?,;•、。！？，；·]', paragraph)
+        for sentence in sentences:
+            words = sentence.split()
+            word_count = len(words)
+            if word_count > max_word_count:
+                max_word_count = word_count
+    text_stat_res = textstat.flesch_reading_ease(content)
+    if int(max_word_count) > 56 and text_stat_res < 20:
+        res["error_status"] = True
+        res["error_type"] = ERROR_NO_PUNC
+        res['error_reason'] = '段落无标点'
+    return res
+
+def common_space_more(content: str) -> dict:
+    """check whether content has more than 500 consecutive spaces"""
+    res = {'error_status': False}
+    pattern = r' {500,}'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_SPACE_MORE
+        res['error_reason'] = '存在连续500个空格'
+    return res
+
+def common_special_character(content: str) -> dict:
+    res = {'error_status': False}
+    pattern = r"[�□\^]|\{\/U\}"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_SPECIAL_CHARACTER
+        res['error_reason'] = matches
+    return res
+
+def common_special_mark(content: str) -> dict:
+    """check if the content contains special mark"""
+    res = {'error_status': False}
+    pattern = r'keyboard_arrow_(left|right)'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"][ERROR_SPECIAL_MARK] = ERROR_SPECIAL_MARK
+        res["error_reason"][ERROR_SPECIAL_MARK] = "元素包含特殊标记"
+    return res
+
+def common_unconverted_symbol(content: str) -> dict:
+    """check if the content contains special symbols for conversion failure"""
+    res = {'error_status': False}
+    pattern = r'u200e'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"][ERROR_UNCONVERTED_SYMBOL] = ERROR_UNCONVERTED_SYMBOL
+        res["error_reason"][ERROR_UNCONVERTED_SYMBOL] = "包含转换失败的特殊符号"
+    return res
+
+def common_underscore_length(content: str) -> dict:
+    """check whether the content contains underscores whose length is longer than 15"""
+    res = {'error_status': False}
+    max_underscore_count = 0
+    for char in content:
+        if char == '_':
+            underscore_count += 1
+            if underscore_count > max_underscore_count:
+                max_underscore_count = underscore_count
+        else:
+            underscore_count = 0
+    if max_underscore_count >= 15:
+        res["error_status"] = True
+        res["error_type"][ERROR_UNDERSCORE_LENGTH] = ERROR_UNDERSCORE_LENGTH
+        res["error_reason"][ERROR_UNDERSCORE_LENGTH] = "下划线长度大于15"
+    return res
+
+def common_url_only(content: str) -> dict:
+    """check whether content is all urls"""
+    res = {'error_status': False}
+    pattern = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'  # noqa
+    s = re.sub(pattern, '', content)
+    count = len(s.strip())
+    if count == 0:
+        res["error_status"] = True
+        res["error_type"] = ERROR_URL_ONLY
+        res['error_reason'] = '内容只有url'
+    return res
+
+def common_word_stuck(content: str) -> dict:
+    """check whether words are stuck"""
+    res = {'error_status': False}
+    words = re.findall(r'[a-zA-Z]+', content)
+    max_word_len = 0
+    for word in words:
+        if len(word) > max_word_len:
+            max_word_len = len(word)
+    if max_word_len > 45:
+        res["error_status"] = True
+        res["error_type"] = ERROR_WORD_STUCK
+        res['error_reason'] = '英文单词黏连'
     return res
```

