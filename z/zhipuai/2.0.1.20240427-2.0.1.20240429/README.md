# Comparing `tmp/zhipuai-2.0.1.20240427.tar.gz` & `tmp/zhipuai-2.0.1.20240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.0.1.20240427.tar", max compression
+gzip compressed data, was "zhipuai-2.0.1.20240429.tar", max compression
```

## Comparing `zhipuai-2.0.1.20240427.tar` & `zhipuai-2.0.1.20240429.tar`

### file list

```diff
@@ -1,45 +1,51 @@
--rw-r--r--   0        0        0     7371 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/README.md
--rw-r--r--   0        0        0     2979 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/pyproject.toml
--rw-r--r--   0        0        0      343 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/__init__.py
--rw-r--r--   0        0        0       23 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/__version__.py
--rw-r--r--   0        0        0    13562 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/_base_models.py
--rw-r--r--   0        0        0     2431 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/_client.py
--rw-r--r--   0        0        0      147 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3230 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      451 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0        0        0     4789 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1694 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/embeddings.py
--rw-r--r--   0        0        0     2463 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/files.py
--rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      311 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0     3757 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1885 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/api_resource/images.py
--rw-r--r--   0        0        0        0 2024-04-27 13:47:52.201318 zhipuai-2.0.1.20240427/zhipuai/core/__init__.py
--rw-r--r--   0        0        0      406 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_api.py
--rw-r--r--   0        0        0     6405 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_compat.py
--rw-r--r--   0        0        0     4484 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_base_type.py
--rw-r--r--   0        0        0     2038 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_errors.py
--rw-r--r--   0        0        0     1384 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_files.py
--rw-r--r--   0        0        0    13808 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_http_client.py
--rw-r--r--   0        0        0      713 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_jwt_token.py
--rw-r--r--   0        0        0     2346 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_request_opt.py
--rw-r--r--   0        0        0     3640 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_response.py
--rw-r--r--   0        0        0     4085 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_sse_client.py
--rw-r--r--   0        0        0     1451 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/__init__.py
--rw-r--r--   0        0        0     3858 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/_typing.py
--rw-r--r--   0        0        0    11363 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/core/_utils/_utils.py
--rw-r--r--   0        0        0        0 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/__init__.py
--rw-r--r--   0        0        0      557 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      885 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1257 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      434 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/embeddings.py
--rw-r--r--   0        0        0      538 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/file_object.py
--rw-r--r--   0        0        0      244 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1113 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1110 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      382 2024-04-27 13:47:52.205318 zhipuai-2.0.1.20240427/zhipuai/types/image.py
--rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 zhipuai-2.0.1.20240427/PKG-INFO
+-rw-r--r--   0        0        0     7810 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/README.md
+-rw-r--r--   0        0        0     3267 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/pyproject.toml
+-rw-r--r--   0        0        0      359 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/__version__.py
+-rw-r--r--   0        0        0     2435 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/_client.py
+-rw-r--r--   0        0        0      358 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0        0        0     3285 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0        0        0      464 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0        0        0     4591 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0        0        0     1757 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0        0        0     2422 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/files.py
+-rw-r--r--   0        0        0      188 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0       48 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/jobs/__init__.py
+-rw-r--r--   0        0        0     5537 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/jobs/jobs.py
+-rw-r--r--   0        0        0       77 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0     1309 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0     1948 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/api_resource/images.py
+-rw-r--r--   0        0        0     2040 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_api.py
+-rw-r--r--   0        0        0     6405 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_compat.py
+-rw-r--r--   0        0        0    13547 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_models.py
+-rw-r--r--   0        0        0     4551 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_type.py
+-rw-r--r--   0        0        0     2230 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_errors.py
+-rw-r--r--   0        0        0     1384 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_files.py
+-rw-r--r--   0        0        0    22877 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_http_client.py
+-rw-r--r--   0        0        0      713 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_jwt_token.py
+-rw-r--r--   0        0        0     3349 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_request_opt.py
+-rw-r--r--   0        0        0     3606 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_response.py
+-rw-r--r--   0        0        0     4085 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_sse_client.py
+-rw-r--r--   0        0        0     1451 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0        0        0     3858 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0        0        0    11363 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/_utils.py
+-rw-r--r--   0        0        0     2618 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/logs.py
+-rw-r--r--   0        0        0        0 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/__init__.py
+-rw-r--r--   0        0        0      568 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0        0        0      859 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1249 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      171 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0        0        0      426 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/embeddings.py
+-rw-r--r--   0        0        0      550 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/file_object.py
+-rw-r--r--   0        0        0      244 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0     1064 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      339 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0       53 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0      374 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/image.py
+-rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 zhipuai-2.0.1.20240429/PKG-INFO
```

### Comparing `zhipuai-2.0.1.20240427/README.md` & `zhipuai-2.0.1.20240429/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -149,76 +149,77 @@
         model="charglm-3",  # 填写需要调用的模型名称
         messages=[
             {
                 "role": "user",
                 "content": "请问你在做什么"
             }
         ],
-        extra_body={
-            "meta": {
-                "user_info": "我是陆星辰，是一个男性，是一位知名导演，也是苏梦远的合作导演。我擅长拍摄音乐题材的电影。苏梦远对我的态度是尊敬的，并视我为良师益友。",
-                "bot_info": "苏梦远，本名苏远心，是一位当红的国内女歌手及演员。在参加选秀节目后，凭借独特的嗓音及出众的舞台魅力迅速成名，进入娱乐圈。她外表美丽动人，但真正的魅力在于她的才华和勤奋。苏梦远是音乐学院毕业的优秀生，善于创作，拥有多首热门原创歌曲。除了音乐方面的成就，她还热衷于慈善事业，积极参加公益活动，用实际行动传递正能量。在工作中，她对待工作非常敬业，拍戏时总是全身心投入角色，赢得了业内人士的赞誉和粉丝的喜爱。虽然在娱乐圈，但她始终保持低调、谦逊的态度，深得同行尊重。在表达时，苏梦远喜欢使用“我们”和“一起”，强调团队精神。",
-                "bot_name": "苏梦远",
-                "user_name": "陆星辰"
-            },
-        }
+        meta={
+          "user_info": "我是陆星辰，是一个男性，是一位知名导演，也是苏梦远的合作导演。我擅长拍摄音乐题材的电影。苏梦远对我的态度是尊敬的，并视我为良师益友。",
+          "bot_info": "苏梦远，本名苏远心，是一位当红的国内女歌手及演员。在参加选秀节目后，凭借独特的嗓音及出众的舞台魅力迅速成名，进入娱乐圈。她外表美丽动人，但真正的魅力在于她的才华和勤奋。苏梦远是音乐学院毕业的优秀生，善于创作，拥有多首热门原创歌曲。除了音乐方面的成就，她还热衷于慈善事业，积极参加公益活动，用实际行动传递正能量。在工作中，她对待工作非常敬业，拍戏时总是全身心投入角色，赢得了业内人士的赞誉和粉丝的喜爱。虽然在娱乐圈，但她始终保持低调、谦逊的态度，深得同行尊重。在表达时，苏梦远喜欢使用“我们”和“一起”，强调团队精神。",
+          "bot_name": "苏梦远",
+          "user_name": "陆星辰"
+        },
     )
     print(response)
 test_completions_charglm()
 ```
 
 
 
 ### 异常处理
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `openai.APIConnectionError` is raised.
-
-When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `openai.APIStatusError` is raised, containing `status_code` and `response` properties.
-
-All errors inherit from `openai.APIError`.
+模块定义了一些统一的参数返回(例如:响应错误，网络超时错误)
 
+业务定义了http错误的响应类 (在接口返回，40x或者50x), 会抛出 `zhipuai.APIStatusError`  ,包含 `status_code` 和 `response` 属性. 它们都是继承 `zhipuai.APIStatusError`.
+其它Exception，属于不可预知的错误
 ```python
-import openai
-from openai import OpenAI
-
-client = OpenAI()
-
+from zhipuai import ZhipuAI
+import zhipuai
+client = ZhipuAI()  # 填写您自己的APIKey
 try:
-    client.fine_tunes.create(
-        training_file="file-XGinujblHPwGLSztz8cPS8XY",
-    )
-except openai.APIConnectionError as e:
-    print("The server could not be reached")
-    print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except openai.RateLimitError as e:
-    print("A 429 status code was received; we should back off a bit.")
-except openai.APIStatusError as e:
-    print("Another non-200-range status code was received")
-    print(e.status_code)
-    print(e.response)
+  response = client.chat.completions.create(
+    model="glm-4",  # 填写需要调用的模型名称
+    messages=[
+      {"role": "user", "content": "作为一名营销专家，请为我的产品创作一个吸引人的slogan"},
+      {"role": "assistant", "content": "当然，为了创作一个吸引人的slogan，请告诉我一些关于您产品的信息"},
+      {"role": "user", "content": "智谱AI开放平台"},
+      {"role": "assistant", "content": "智启未来，谱绘无限一智谱AI，让创新触手可及!"},
+      {"role": "user", "content": "创造一个更精准、吸引人的slogan"}
+    ]
+  )
+  print(response)
+ 
+except zhipuai.APIStatusError as err:
+  print(err) 
+except zhipuai.APITimeoutError as err:
+  print(err) 
 ```
 
 Error codes are as followed:
 
 | Status Code | Error Type                 |
-| ----------- | -------------------------- |
-| 400         | `BadRequestError`          |
-| 401         | `AuthenticationError`      |
-| 403         | `PermissionDeniedError`    |
-| 404         | `NotFoundError`            |
-| 422         | `UnprocessableEntityError` |
-| 429         | `RateLimitError`           |
-| >=500       | `InternalServerError`      |
-| N/A         | `APIConnectionError`       |
+|-------------| -------------------------- |
+| 400         | `APIRequestFailedError`          |
+| 401         | `APIAuthenticationError`      |
+| 429         | `APIReachLimitError`           |
+| 500         | `APIInternalError`      |
+| 503         | `APIServerFlowExceedError`      |
+| N/A         | `APIStatusError`       |
 
 
 
 ### 更新日志
 
+`2024-4-29` 
+- 一些 `python3.7` 的代码适配问题， 
+- 接口失败重试机制，通过 `retry` 参数控制重试次数，默认为3次
+- 接口超时策略调整，通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
+- 对话模块增加超拟人大模型参数支持，`model="charglm-3"`, `meta`参数支持
+  
 `2024-4-23` 
 - 一些兼容 `pydantic<3,>=1.9.0 ` 的代码，
 - 报文处理的业务请求参数和响应参数可通过配置扩充
 - 兼容了一些参数 `top_p:1`,`temperture:0`(do_sample重写false，参数top_p temperture不生效)
 - 图像理解部分，  image_url参数base64内容包含 `data:image/jpeg;base64`兼容
 - 删除jwt认证逻辑
```

### Comparing `zhipuai-2.0.1.20240427/pyproject.toml` & `zhipuai-2.0.1.20240429/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 [tool.poetry]
 name = "zhipuai"
-version = "2.0.1.20240427"
+version = "2.0.1.20240429"
 description = "A SDK library for accessing big model apis from ZhipuAI"
 authors = ["Zhipu AI"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12,!=3.9.7"
+python = ">=3.7.1,<3.12,!=3.9.7 "
 httpx = ">=0.23.0"
 pydantic = ">=1.9.0,<3.0"
 cachetools = ">=4.2.2"
 pyjwt = "~=2.8.0"
 
+
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-dotenv = "^0.5.2"
 duckdb-engine = "^0.9.2"
 pytest-watcher = "^0.2.6"
 freezegun = "^1.2.2"
 responses = "^0.22.0"
-pytest-asyncio = "^0.23.2"
+pytest-asyncio = { version = "^0.23.2", python = "^3.8" }
 lark = "^1.1.5"
-pandas = "^2.0.0"
-pytest-mock  = "^3.10.0"
+pandas = { version = "^2.0.0", python = "^3.8" }
+pytest-mock = "^3.10.0"
 pytest-socket = "^0.6.0"
-syrupy = "^4.0.2"
+syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
 requests-mock = "^1.11.0"
 
 [tool.poetry.group.test_langchain.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-dotenv = "^0.5.2"
 duckdb-engine = "^0.9.2"
 pytest-watcher = "^0.2.6"
 freezegun = "^1.2.2"
 responses = "^0.22.0"
-pytest-asyncio = "^0.23.2"
+pytest-asyncio = { version = "^0.23.2", python = "^3.8" }
 lark = "^1.1.5"
-pandas = "^2.0.0"
-pytest-mock  = "^3.10.0"
+pandas = { version = "^2.0.0", python = "^3.8" }
+pytest-mock = "^3.10.0"
 pytest-socket = "^0.6.0"
-syrupy = "^4.0.2"
+syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
 requests-mock = "^1.11.0"
-langchain = "0.1.5"
+langchain = { version = "0.1.5", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
 
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
@@ -62,17 +63,17 @@
 # merge-conflicts
 extended_testing = [
     "langchain",
 ]
 
 [tool.ruff.lint]
 select = [
-    "E",  # pycodestyle
-    "F",  # pyflakes
-    "I",  # isort
+    "E", # pycodestyle
+    "F", # pyflakes
+    "I", # isort
     "T201", # print
 ]
 
 
 [tool.coverage.run]
 omit = [
     "tests/*",
@@ -99,11 +100,11 @@
     "requires: mark tests as requiring a specific library",
     "scheduled: mark tests to run in scheduled testing",
     "compile: mark placeholder test used to compile integration tests without running them"
 ]
 asyncio_mode = "auto"
 
 # https://python-poetry.org/docs/repositories/
-#[[tool.poetry.source]]
-#name = "tsinghua"
-#url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
-#priority = "default"
+[[tool.poetry.source]]
+name = "tsinghua"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
+priority = "default"
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/_base_models.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_base_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     runtime_checkable,
 )
 
 import pydantic
 import pydantic.generics
 from pydantic.fields import FieldInfo
 from pydantic import root_validator
-from .core._base_type import (
+from ._base_type import (
     IncEx,
     ModelT,
 )
-from .core._utils import is_list, is_mapping, parse_date, parse_datetime
-from .core._base_compat import (
+from ._utils import is_list, is_mapping, parse_date, parse_datetime
+from ._base_compat import (
     PYDANTIC_V2,
     ConfigDict,
     GenericModel as BaseGenericModel,
     get_args,
     is_union,
     parse_obj,
     get_origin,
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/_client.py` & `zhipuai-2.0.1.20240429/zhipuai/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Union, Mapping
 
 from typing_extensions import override
 
 from .core import _jwt_token
-from .core._errors import ZhipuAIError
-from .core._http_client import HttpClient, ZHIPUAI_DEFAULT_MAX_RETRIES
-from .core._base_type import NotGiven, NOT_GIVEN
+from .core import ZhipuAIError
+from .core import HttpClient, ZHIPUAI_DEFAULT_MAX_RETRIES
+from .core import NotGiven, NOT_GIVEN
 from . import api_resource
 import os
 import httpx
 from httpx import Timeout
 
 
 class ZhipuAI(HttpClient):
@@ -38,27 +38,28 @@
             base_url = os.environ.get("ZHIPUAI_BASE_URL")
         if base_url is None:
             base_url = f"https://open.bigmodel.cn/api/paas/v4"
         from .__version__ import __version__
         super().__init__(
             version=__version__,
             base_url=base_url,
+            max_retries=max_retries,
             timeout=timeout,
             custom_httpx_client=http_client,
             custom_headers=custom_headers,
         )
         self.chat = api_resource.chat.Chat(self)
         self.images = api_resource.images.Images(self)
         self.embeddings = api_resource.embeddings.Embeddings(self)
         self.files = api_resource.files.Files(self)
         self.fine_tuning = api_resource.fine_tuning.FineTuning(self)
 
     @property
     @override
-    def _auth_headers(self) -> dict[str, str]:
+    def auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
         # return {"Authorization": f"{_jwt_token.generate_token(api_key)}"}
         return {"Authorization": f"{api_key}"}
 
     def __del__(self) -> None:
         if (not hasattr(self, "_has_custom_http_client")
                 or not hasattr(self, "close")
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/async_completions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 from typing_extensions import Literal
 
-from ...core._base_api import BaseAPI
-from ...core._base_type import NotGiven, NOT_GIVEN, Headers, Body
-from ...core._http_client import make_request_options
+from ...core import BaseAPI
+from ...core import NotGiven, NOT_GIVEN, Headers, Body
+from ...core import make_request_options
 from ...types.chat.async_chat_completion import AsyncTaskStatus, AsyncCompletion
 
 if TYPE_CHECKING:
     from ..._client import ZhipuAI
 
 
 class AsyncCompletions(BaseAPI):
@@ -30,14 +30,15 @@
             max_tokens: int | NotGiven = NOT_GIVEN,
             seed: int | NotGiven = NOT_GIVEN,
             messages: Union[str, List[str], List[int], List[List[int]], None],
             stop: Optional[Union[str, List[str], None]] | NotGiven = NOT_GIVEN,
             sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
             tools: Optional[object] | NotGiven = NOT_GIVEN,
             tool_choice: str | NotGiven = NOT_GIVEN,
+            meta: Optional[Dict[str,str]] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
             extra_body: Body | None = None,
             disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncTaskStatus:
         _cast_type = AsyncTaskStatus
 
@@ -54,20 +55,21 @@
                 "max_tokens": max_tokens,
                 "seed": seed,
                 "messages": messages,
                 "stop": stop,
                 "sensitive_word_check": sensitive_word_check,
                 "tools": tools,
                 "tool_choice": tool_choice,
+                "meta": meta,
             },
             options=make_request_options(
                 extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
-            enable_stream=False,
+            stream=False,
         )
 
     def retrieve_completion_result(
         self,
         id: str,
         extra_headers: Headers | None = None,
         extra_body: Body | None = None,
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/completions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 import logging
 from typing_extensions import Literal
 
-from ...core._base_api import BaseAPI
-from ...core._base_type import NotGiven, NOT_GIVEN, Headers, Query, Body
-from ...core._http_client import make_request_options
-from ...core._sse_client import StreamResponse
+from ...core import BaseAPI
+from ...core import NotGiven, NOT_GIVEN, Headers, Query, Body
+from ...core import make_request_options
+from ...core import StreamResponse
 from ...types.chat.chat_completion import Completion
 from ...types.chat.chat_completion_chunk import ChatCompletionChunk
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..._client import ZhipuAI
@@ -35,48 +35,40 @@
             max_tokens: int | NotGiven = NOT_GIVEN,
             seed: int | NotGiven = NOT_GIVEN,
             messages: Union[str, List[str], List[int], object, None],
             stop: Optional[Union[str, List[str], None]] | NotGiven = NOT_GIVEN,
             sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
             tools: Optional[object] | NotGiven = NOT_GIVEN,
             tool_choice: str | NotGiven = NOT_GIVEN,
+            meta: Optional[Dict[str,str]] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
             extra_body: Body | None = None,
-            disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | StreamResponse[ChatCompletionChunk]:
-        _cast_type = Completion
-        _stream_cls = StreamResponse[ChatCompletionChunk]
-        if disable_strict_validation:
-            _cast_type = object
-            _stream_cls = StreamResponse[object]
-
-        print(f"temperature:{temperature}")
-        print(f"top_p:{top_p}")
+        logger.info(f"temperature:{temperature}, top_p:{top_p}")
         if temperature is not None and temperature != NOT_GIVEN:
 
             if temperature <= 0:
                 do_sample = False
                 temperature = 0.01
-                logger.warning("取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
+                logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
             if temperature >= 1:
                 do_sample = False
                 temperature = 0.99
-                logger.warning("取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
+                logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
         if top_p is not None and top_p != NOT_GIVEN:
 
             if top_p >= 1:
                 top_p = 0.99
-                logger.warning("取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
+                logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
             if top_p <= 0:
                 top_p = 0.01
-                logger.warning("取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
+                logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
 
-        print(f"temperature:{temperature}")
-        print(f"top_p:{top_p}")
+        logger.info(f"temperature:{temperature}, top_p:{top_p}")
         if isinstance(messages, List):
             for item in messages:
                 if item.get('content'):
                     item['content'] = self._drop_prefix_image_data(item['content'])
 
         return self._post(
             "/chat/completions",
@@ -90,21 +82,22 @@
                 "seed": seed,
                 "messages": messages,
                 "stop": stop,
                 "sensitive_word_check": sensitive_word_check,
                 "stream": stream,
                 "tools": tools,
                 "tool_choice": tool_choice,
+                "meta": meta,
             },
             options=make_request_options(
                 extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
-            cast_type=_cast_type,
-            enable_stream=stream or False,
-            stream_cls=_stream_cls,
+            cast_type=Completion,
+            stream=stream or False,
+            stream_cls=StreamResponse[ChatCompletionChunk],
         )
 
     def _drop_prefix_image_data(self, content: Union[str,List[dict]]) -> Union[str,List[dict]]:
         """
         删除 ;base64, 前缀
         :param image_data:
         :return:
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/api_resource/embeddings.py` & `zhipuai-2.0.1.20240429/zhipuai/api_resource/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 from __future__ import annotations
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 
-from ..core._base_api import BaseAPI
-from ..core._base_type import NotGiven, NOT_GIVEN, Headers
-from ..core._http_client import make_request_options
-from ..types.embeddings import EmbeddingsResponded
+from ..core import BaseAPI
+from ..core import NotGiven, NOT_GIVEN, Headers, Body
+from ..core import make_request_options
+from ..types.image import ImagesResponded
 
 if TYPE_CHECKING:
     from .._client import ZhipuAI
 
 
-class Embeddings(BaseAPI):
+class Images(BaseAPI):
     def __init__(self, client: "ZhipuAI") -> None:
         super().__init__(client)
 
-    def create(
+    def generations(
             self,
             *,
-            input: Union[str, List[str], List[int], List[List[int]]],
-            model: Union[str],
-            encoding_format: str | NotGiven = NOT_GIVEN,
+            prompt: str,
+            model: str | NotGiven = NOT_GIVEN,
+            n: Optional[int] | NotGiven = NOT_GIVEN,
+            quality: Optional[str] | NotGiven = NOT_GIVEN,
+            response_format: Optional[str] | NotGiven = NOT_GIVEN,
+            size: Optional[str] | NotGiven = NOT_GIVEN,
+            style: Optional[str] | NotGiven = NOT_GIVEN,
             user: str | NotGiven = NOT_GIVEN,
-            sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
+            request_id: Optional[str] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
             extra_body: Body | None = None,
             disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> EmbeddingsResponded:
-        _cast_type = EmbeddingsResponded
+    ) -> ImagesResponded:
+        _cast_type = ImagesResponded
         if disable_strict_validation:
             _cast_type = object
         return self._post(
-            "/embeddings",
+            "/images/generations",
             body={
-                "input": input,
+                "prompt": prompt,
                 "model": model,
-                "encoding_format": encoding_format,
+                "n": n,
+                "quality": quality,
+                "response_format": response_format,
+                "size": size,
+                "style": style,
                 "user": user,
-                "sensitive_word_check": sensitive_word_check,
+                "request_id": request_id,
             },
             options=make_request_options(
                 extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
-            enable_stream=False,
+            stream=False,
         )
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/api_resource/files.py` & `zhipuai-2.0.1.20240429/zhipuai/api_resource/files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import httpx
 
-from ..core._base_api import BaseAPI
-from ..core._base_type import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
-from ..core._files import is_file_content
-from ..core._http_client import (
+from ..core import BaseAPI
+from ..core import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
+from ..core import is_file_content
+from ..core import (
     make_request_options,
 )
 from ..types.file_object import FileObject, ListOfFileObject
 
 if TYPE_CHECKING:
     from .._client import ZhipuAI
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/api_resource/images.py` & `zhipuai-2.0.1.20240429/zhipuai/api_resource/embeddings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 from __future__ import annotations
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 
-from ..core._base_api import BaseAPI
-from ..core._base_type import NotGiven, NOT_GIVEN, Headers, Body
-from ..core._http_client import make_request_options
-from ..types.image import ImagesResponded
+from ..core import BaseAPI
+from ..core import NotGiven, NOT_GIVEN, Headers
+from ..core import make_request_options
+from ..types.embeddings import EmbeddingsResponded
 
 if TYPE_CHECKING:
     from .._client import ZhipuAI
 
 
-class Images(BaseAPI):
+class Embeddings(BaseAPI):
     def __init__(self, client: "ZhipuAI") -> None:
         super().__init__(client)
 
-    def generations(
+    def create(
             self,
             *,
-            prompt: str,
-            model: str | NotGiven = NOT_GIVEN,
-            n: Optional[int] | NotGiven = NOT_GIVEN,
-            quality: Optional[str] | NotGiven = NOT_GIVEN,
-            response_format: Optional[str] | NotGiven = NOT_GIVEN,
-            size: Optional[str] | NotGiven = NOT_GIVEN,
-            style: Optional[str] | NotGiven = NOT_GIVEN,
+            input: Union[str, List[str], List[int], List[List[int]]],
+            model: Union[str],
+            encoding_format: str | NotGiven = NOT_GIVEN,
             user: str | NotGiven = NOT_GIVEN,
+            request_id: Optional[str] | NotGiven = NOT_GIVEN,
+            sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
             extra_body: Body | None = None,
             disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ImagesResponded:
-        _cast_type = ImagesResponded
+    ) -> EmbeddingsResponded:
+        _cast_type = EmbeddingsResponded
         if disable_strict_validation:
             _cast_type = object
         return self._post(
-            "/images/generations",
+            "/embeddings",
             body={
-                "prompt": prompt,
+                "input": input,
                 "model": model,
-                "n": n,
-                "quality": quality,
-                "response_format": response_format,
-                "size": size,
-                "style": style,
+                "encoding_format": encoding_format,
                 "user": user,
+                "request_id": request_id,
+                "sensitive_word_check": sensitive_word_check,
             },
             options=make_request_options(
                 extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
-            enable_stream=False,
+            stream=False,
         )
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_base_compat.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_base_compat.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_base_type.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_base_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,14 +130,17 @@
     __orig_bases__: tuple[_GenericAlias]
 
 
 class _GenericAlias(Protocol):
     __origin__: type[object]
 
 
+class HttpxSendArgs(TypedDict, total=False):
+    auth: httpx.Auth
+
 # for user input files
 if TYPE_CHECKING:
     FileContent = Union[IO[bytes], bytes, PathLike[str]]
 else:
     FileContent = Union[IO[bytes], bytes, PathLike]
 
 FileTypes = Union[
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_errors.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class ZhipuAIError(Exception):
     def __init__(self, message: str, ) -> None:
         super().__init__(message)
 
 
-class APIStatusError(Exception):
+class APIStatusError(ZhipuAIError):
     response: httpx.Response
     status_code: int
 
     def __init__(self, message: str, *, response: httpx.Response) -> None:
         super().__init__(message)
         self.response = response
         self.status_code = response.status_code
@@ -47,15 +47,15 @@
     ...
 
 
 class APIServerFlowExceedError(APIStatusError):
     ...
 
 
-class APIResponseError(Exception):
+class APIResponseError(ZhipuAIError):
     message: str
     request: httpx.Request
     json_data: object
 
     def __init__(self, message: str, request: httpx.Request, json_data: object):
         self.message = message
         self.request = request
@@ -78,13 +78,15 @@
             request=response.request,
             json_data=json_data
         )
         self.response = response
         self.status_code = response.status_code
 
 
-class APITimeoutError(Exception):
-    request: httpx.Request
+class APIConnectionError(APIResponseError):
+    def __init__(self, *, message: str = "Connection error.", request: httpx.Request) -> None:
+        super().__init__(message, request, json_data=None)
 
-    def __init__(self, request: httpx.Request):
-        self.request = request
-        super().__init__("Request Timeout")
+
+class APITimeoutError(APIConnectionError):
+    def __init__(self, request: httpx.Request) -> None:
+        super().__init__(message="Request timed out.", request=request)
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_files.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_http_client.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_http_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,80 +3,115 @@
 
 import inspect
 from typing import (
     Any,
     Type,
     Union,
     cast,
-    Mapping, TypeVar, Dict,
+    Mapping,
+    TypeVar,
+    Dict,
+    overload
 )
 
+from random import random
+import time
 import httpx
 import pydantic
 from httpx import URL, Timeout
 
 from . import _errors
-from ._base_compat import parse_obj
-from ._base_type import NotGiven, ResponseT, Body, Headers, NOT_GIVEN, RequestFiles, Query, Data, Omit, AnyMapping, \
-    ModelBuilderProtocol
-from ._errors import APIResponseValidationError, APIStatusError, APITimeoutError
+from ._base_type import (
+    NotGiven,
+    ResponseT,
+    Body,
+    Headers,
+    NOT_GIVEN,
+    RequestFiles,
+    Query,
+    Data,
+    Omit,
+    AnyMapping,
+    ModelBuilderProtocol,
+    HttpxSendArgs,
+)
+from ._errors import APIResponseValidationError, APIStatusError, APITimeoutError, APIConnectionError
 from ._files import make_httpx_files
-from ._request_opt import ClientRequestParam, UserRequestInput
+from ._request_opt import FinalRequestOptions, UserRequestInput
 from ._response import HttpResponse
 from ._sse_client import StreamResponse
-from ._utils import flatten, is_mapping
-from .._base_models import construct_type
-
+from ._utils import flatten, is_mapping, is_given
+from ._base_models import construct_type
+import logging
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 
+log: logging.Logger = logging.getLogger(__name__)
+
 
 headers = {
     "Accept": "application/json",
     "Content-Type": "application/json; charset=UTF-8",
 }
 
 
 from httpx._config import DEFAULT_TIMEOUT_CONFIG as HTTPX_DEFAULT_TIMEOUT
-
+RAW_RESPONSE_HEADER = "X-Stainless-Raw-Response"
 ZHIPUAI_DEFAULT_TIMEOUT = httpx.Timeout(timeout=300.0, connect=8.0)
 ZHIPUAI_DEFAULT_MAX_RETRIES = 3
 ZHIPUAI_DEFAULT_LIMITS = httpx.Limits(max_connections=50, max_keepalive_connections=10)
 
+INITIAL_RETRY_DELAY = 0.5
+MAX_RETRY_DELAY = 8.0
 
 class HttpClient:
     _client: httpx.Client
     _version: str
     _base_url: URL
-
+    max_retries: int
     timeout: Union[float, Timeout, None]
     _limits: httpx.Limits
     _has_custom_http_client: bool
     _default_stream_cls: type[StreamResponse[Any]] | None = None
 
     def __init__(
             self,
             *,
             version: str,
             base_url: URL,
+            max_retries: int = ZHIPUAI_DEFAULT_MAX_RETRIES,
             timeout: Union[float, Timeout, None],
+            limits: Limits | None = None,
             custom_httpx_client: httpx.Client | None = None,
             custom_headers: Mapping[str, str] | None = None,
     ) -> None:
-        if timeout is None or isinstance(timeout, NotGiven):
+        if limits is not None:
+            warnings.warn(
+                "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
+                category=DeprecationWarning,
+                stacklevel=3,
+            )
+            if http_client is not None:
+                raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
+        else:
+            limits = ZHIPUAI_DEFAULT_LIMITS
+
+        if not is_given(timeout):
             if custom_httpx_client and custom_httpx_client.timeout != HTTPX_DEFAULT_TIMEOUT:
                 timeout = custom_httpx_client.timeout
             else:
                 timeout = ZHIPUAI_DEFAULT_TIMEOUT
-        self.timeout = cast(Timeout, timeout)
+        self.max_retries = max_retries
+        self.timeout = timeout
+        self._limits = limits
         self._has_custom_http_client = bool(custom_httpx_client)
         self._client = custom_httpx_client or httpx.Client(
             base_url=base_url,
             timeout=self.timeout,
-            limits=ZHIPUAI_DEFAULT_LIMITS,
+            limits=limits,
         )
         self._version = version
         url = URL(url=base_url)
         if not url.raw_path.endswith(b"/"):
             url = url.copy_with(raw_path=url.raw_path + b"/")
         self._base_url = url
         self._custom_headers = custom_headers or {}
@@ -95,43 +130,76 @@
         return \
             {
                 "Accept": "application/json",
                 "Content-Type": "application/json; charset=UTF-8",
                 "ZhipuAI-SDK-Ver": self._version,
                 "source_type": "zhipu-sdk-python",
                 "x-request-sdk": "zhipu-sdk-python",
-                **self._auth_headers,
+                **self.auth_headers,
                 **self._custom_headers,
             }
+    @property
+    def custom_auth(self) -> httpx.Auth | None:
+        return None
 
     @property
-    def _auth_headers(self):
+    def auth_headers(self):
         return {}
 
-    def _prepare_headers(self, request_param: ClientRequestParam) -> httpx.Headers:
-        custom_headers = request_param.headers or {}
+    def _prepare_headers(self, options: FinalRequestOptions) -> httpx.Headers:
+        custom_headers = options.headers or {}
         headers_dict = _merge_mappings(self._default_headers, custom_headers)
 
         httpx_headers = httpx.Headers(headers_dict)
 
         return httpx_headers
 
+    def _remaining_retries(
+            self,
+            remaining_retries: Optional[int],
+            options: FinalRequestOptions,
+    ) -> int:
+        return remaining_retries if remaining_retries is not None else options.get_max_retries(self.max_retries)
+
+    def _calculate_retry_timeout(
+            self,
+            remaining_retries: int,
+            options: FinalRequestOptions,
+            response_headers: Optional[httpx.Headers] = None,
+    ) -> float:
+        max_retries = options.get_max_retries(self.max_retries)
+
+        # If the API asks us to wait a certain amount of time (and it's a reasonable amount), just do what it says.
+        # retry_after = self._parse_retry_after_header(response_headers)
+        # if retry_after is not None and 0 < retry_after <= 60:
+        #     return retry_after
+
+        nb_retries = max_retries - remaining_retries
+
+        # Apply exponential backoff, but not more than the max.
+        sleep_seconds = min(INITIAL_RETRY_DELAY * pow(2.0, nb_retries), MAX_RETRY_DELAY)
+
+        # Apply some jitter, plus-or-minus half a second.
+        jitter = 1 - 0.25 * random()
+        timeout = sleep_seconds * jitter
+        return timeout if timeout >= 0 else 0
+
     def _build_request(
             self,
-            request_param: ClientRequestParam
+            options: FinalRequestOptions
     ) -> httpx.Request:
         kwargs: dict[str, Any] = {}
-        headers = self._prepare_headers(request_param)
-        url = self._prepare_url(request_param.url)
-        json_data = request_param.json_data
-        if request_param.extra_json is not None:
+        headers = self._prepare_headers(options)
+        url = self._prepare_url(options.url)
+        json_data = options.json_data
+        if options.extra_json is not None:
             if json_data is None:
-                json_data = cast(Body, request_param.extra_json)
+                json_data = cast(Body, options.extra_json)
             elif is_mapping(json_data):
-                json_data = _merge_mappings(json_data, request_param.extra_json)
+                json_data = _merge_mappings(json_data, options.extra_json)
             else:
                 raise RuntimeError(f"Unexpected JSON data type, {type(json_data)}, cannot merge with `extra_body`")
 
         content_type = headers.get("Content-Type")
         # multipart/form-data; boundary=---abc--
         if headers.get("Content-Type") == "multipart/form-data":
             if "boundary" not in content_type:
@@ -140,20 +208,20 @@
                 headers.pop("Content-Type")
 
             if json_data:
                 kwargs["data"] = self._make_multipartform(json_data)
 
         return self._client.build_request(
             headers=headers,
-            timeout=self.timeout if isinstance(request_param.timeout, NotGiven) else request_param.timeout,
-            method=request_param.method,
+            timeout=self.timeout if isinstance(options.timeout, NotGiven) else options.timeout,
+            method=options.method,
             url=url,
             json=json_data,
-            files=request_param.files,
-            params=request_param.params,
+            files=options.files,
+            params=options.params,
             **kwargs,
         )
 
     def _object_to_formfata(self, key: str, value: Data | Mapping[object, object]) -> list[tuple[str, str]]:
         items = []
 
         if isinstance(value, Mapping):
@@ -193,24 +261,24 @@
         return serialized
 
     def _parse_response(
             self,
             *,
             cast_type: Type[ResponseT],
             response: httpx.Response,
-            enable_stream: bool,
-            request_param: ClientRequestParam,
+            stream: bool,
+            options: FinalRequestOptions,
             stream_cls: type[StreamResponse[Any]] | None = None,
     ) -> HttpResponse:
 
         http_response = HttpResponse(
             raw_response=response,
             cast_type=cast_type,
             client=self,
-            enable_stream=enable_stream,
+            stream=stream,
             stream_cls=stream_cls
         )
         return http_response.parse()
 
     def _process_response_data(
             self,
             *,
@@ -229,14 +297,52 @@
             if inspect.isclass(cast_type) and issubclass(cast_type, ModelBuilderProtocol):
                 return cast(ResponseT, cast_type.build(response=response, data=data))
 
             return cast(ResponseT, construct_type(type_=cast_type, value=data))
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(response=response, json_data=data) from err
 
+    def _should_stream_response_body(self, request: httpx.Request) -> bool:
+        return request.headers.get(RAW_RESPONSE_HEADER) == "stream"  # type: ignore[no-any-return]
+
+    def _should_retry(self, response: httpx.Response) -> bool:
+        # Note: this is not a standard header
+        should_retry_header = response.headers.get("x-should-retry")
+
+        # If the server explicitly says whether or not to retry, obey.
+        if should_retry_header == "true":
+            log.debug("Retrying as header `x-should-retry` is set to `true`")
+            return True
+        if should_retry_header == "false":
+            log.debug("Not retrying as header `x-should-retry` is set to `false`")
+            return False
+
+        # Retry on request timeouts.
+        if response.status_code == 408:
+            log.debug("Retrying due to status code %i", response.status_code)
+            return True
+
+        # Retry on lock timeouts.
+        if response.status_code == 409:
+            log.debug("Retrying due to status code %i", response.status_code)
+            return True
+
+        # Retry on rate limits.
+        if response.status_code == 429:
+            log.debug("Retrying due to status code %i", response.status_code)
+            return True
+
+        # Retry internal errors.
+        if response.status_code >= 500:
+            log.debug("Retrying due to status code %i", response.status_code)
+            return True
+
+        log.debug("Not retrying")
+        return False
+
     def is_closed(self) -> bool:
         return self._client.is_closed
 
     def close(self):
         self._client.close()
 
     def __enter__(self):
@@ -244,121 +350,296 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def request(
             self,
             cast_type: Type[ResponseT],
-            params: ClientRequestParam,
+            options: FinalRequestOptions,
+            remaining_retries: Optional[int] = None,
             *,
-            enable_stream: bool = False,
-            stream_cls: type[StreamResponse[Any]] | None = None,
+            stream: bool = False,
+            stream_cls: type[StreamResponse] | None = None,
+    ) -> ResponseT | StreamResponse:
+        return self._request(
+            cast_type=cast_type,
+            options=options,
+            stream=stream,
+            stream_cls=stream_cls,
+            remaining_retries=remaining_retries,
+        )
+
+    def _request(
+            self,
+            *,
+            cast_type: Type[ResponseT],
+            options: FinalRequestOptions,
+            remaining_retries: int | None,
+            stream: bool,
+            stream_cls: type[StreamResponse] | None,
     ) -> ResponseT | StreamResponse:
-        request = self._build_request(params)
 
+        retries = self._remaining_retries(remaining_retries, options)
+        request = self._build_request(options)
+
+        kwargs: HttpxSendArgs = {}
+        if self.custom_auth is not None:
+            kwargs["auth"] = self.custom_auth
         try:
             response = self._client.send(
                 request,
-                stream=enable_stream,
+                stream=stream or self._should_stream_response_body(request=request),
+                **kwargs,
             )
-            response.raise_for_status()
         except httpx.TimeoutException as err:
+            log.debug("Encountered httpx.TimeoutException", exc_info=True)
+
+            if retries > 0:
+                return self._retry_request(
+                    options,
+                    cast_type,
+                    retries,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                    response_headers=None,
+                )
+
+            log.debug("Raising timeout error")
             raise APITimeoutError(request=request) from err
-        except httpx.HTTPStatusError as err:
-            err.response.read()
-            # raise err
+        except Exception as err:
+            log.debug("Encountered Exception", exc_info=True)
+
+            if retries > 0:
+                return self._retry_request(
+                    options,
+                    cast_type,
+                    retries,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                    response_headers=None,
+                )
+
+            log.debug("Raising connection error")
+            raise APIConnectionError(request=request) from err
+
+        log.debug(
+            'HTTP Request: %s %s "%i %s"', request.method, request.url, response.status_code, response.reason_phrase
+        )
+
+        try:
+            response.raise_for_status()
+        except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
+            log.debug("Encountered httpx.HTTPStatusError", exc_info=True)
+
+            if retries > 0 and self._should_retry(err.response):
+                err.response.close()
+                return self._retry_request(
+                    options,
+                    cast_type,
+                    retries,
+                    err.response.headers,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                )
+
+            # If the response is streamed then we need to explicitly read the response
+            # to completion before attempting to access the response text.
+            if not err.response.is_closed:
+                err.response.read()
+
+            log.debug("Re-raising status error")
             raise self._make_status_error(err.response) from None
 
-        except Exception as err:
-            raise err
 
         return self._parse_response(
             cast_type=cast_type,
-            request_param=params,
+            options=options,
             response=response,
-            enable_stream=enable_stream,
+            stream=stream,
+            stream_cls=stream_cls,
+        )
+
+    def _retry_request(
+            self,
+            options: FinalRequestOptions,
+            cast_type: Type[ResponseT],
+            remaining_retries: int,
+            response_headers: httpx.Headers | None,
+            *,
+            stream: bool,
+            stream_cls: type[StreamResponse] | None,
+    ) -> ResponseT | StreamResponse:
+        remaining = remaining_retries - 1
+        if remaining == 1:
+            log.debug("1 retry left")
+        else:
+            log.debug("%i retries left", remaining)
+
+        timeout = self._calculate_retry_timeout(remaining, options, response_headers)
+        log.info("Retrying request to %s in %f seconds", options.url, timeout)
+
+        # In a synchronous context we are blocking the entire thread. Up to the library user to run the client in a
+        # different thread if necessary.
+        time.sleep(timeout)
+
+        return self._request(
+            options=options,
+            cast_type=cast_type,
+            remaining_retries=remaining,
+            stream=stream,
             stream_cls=stream_cls,
         )
 
+    @overload
+    def get(
+            self,
+            path: str,
+            *,
+            cast_type: Type[ResponseT],
+            options: UserRequestInput = {},
+            stream: Literal[False] = False,
+    ) -> ResponseT:
+        ...
+
+    @overload
     def get(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             options: UserRequestInput = {},
-            enable_stream: bool = False,
+            stream: Literal[True],
+            stream_cls: type[StreamResponse],
+    ) -> StreamResponse:
+        ...
+
+    @overload
+    def get(
+            self,
+            path: str,
+            *,
+            cast_type: Type[ResponseT],
+            options: UserRequestInput = {},
+            stream: bool,
+            stream_cls: type[StreamResponse] | None = None,
     ) -> ResponseT | StreamResponse:
-        opts = ClientRequestParam.construct(method="get", url=path, **options)
-        return self.request(
-            cast_type=cast_type, params=opts,
-            enable_stream=enable_stream
-        )
+        ...
+
+    def get(
+            self,
+            path: str,
+            *,
+            cast_type: Type[ResponseT],
+            options: UserRequestInput = {},
+            stream: bool = False,
+            stream_cls: type[StreamResponse] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
+        opts = FinalRequestOptions.construct(method="get", url=path, **options)
+        return cast(ResponseT, self.request(cast_type, opts, stream=stream, stream_cls=stream_cls))
 
+    @overload
     def post(
             self,
             path: str,
             *,
+            cast_type: Type[ResponseT],
             body: Body | None = None,
+            options: UserRequestInput = {},
+            files: RequestFiles | None = None,
+            stream: Literal[False] = False,
+    ) -> ResponseT:
+        ...
+
+    @overload
+    def post(
+            self,
+            path: str,
+            *,
             cast_type: Type[ResponseT],
+            body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
-            enable_stream: bool = False,
-            stream_cls: type[StreamResponse[Any]] | None = None,
+            stream: Literal[True],
+            stream_cls: type[StreamResponse],
+    ) -> StreamResponse:
+        ...
+
+    @overload
+    def post(
+            self,
+            path: str,
+            *,
+            cast_type: Type[ResponseT],
+            body: Body | None = None,
+            options: UserRequestInput = {},
+            files: RequestFiles | None = None,
+            stream: bool,
+            stream_cls: type[StreamResponse] | None = None,
     ) -> ResponseT | StreamResponse:
-        opts = ClientRequestParam.construct(method="post", json_data=body, files=make_httpx_files(files), url=path,
-                                            **options)
+        ...
 
-        return self.request(
-            cast_type=cast_type, params=opts,
-            enable_stream=enable_stream,
-            stream_cls=stream_cls
+    def post(
+            self,
+            path: str,
+            *,
+            cast_type: Type[ResponseT],
+            body: Body | None = None,
+            options: UserRequestInput = {},
+            files: RequestFiles | None = None,
+            stream: bool = False,
+            stream_cls: type[StreamResponse[Any]] | None = None,
+    ) -> ResponseT | StreamResponse:
+        opts = FinalRequestOptions.construct(
+            method="post", url=path, json_data=body, files=make_httpx_files(files), **options
         )
 
+        return cast(ResponseT,  self.request(cast_type, opts, stream=stream, stream_cls=stream_cls))
+
     def patch(
             self,
             path: str,
             *,
-            body: Body | None = None,
             cast_type: Type[ResponseT],
+            body: Body | None = None,
             options: UserRequestInput = {},
     ) -> ResponseT:
-        opts = ClientRequestParam.construct(method="patch", url=path, json_data=body, **options)
+        opts = FinalRequestOptions.construct(method="patch", url=path, json_data=body, **options)
 
         return self.request(
-            cast_type=cast_type, params=opts,
+            cast_type=cast_type, options=opts,
         )
 
     def put(
             self,
             path: str,
             *,
-            body: Body | None = None,
             cast_type: Type[ResponseT],
+            body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
     ) -> ResponseT | StreamResponse:
-        opts = ClientRequestParam.construct(method="put", url=path, json_data=body, files=make_httpx_files(files),
+        opts = FinalRequestOptions.construct(method="put", url=path, json_data=body, files=make_httpx_files(files),
                                             **options)
 
         return self.request(
-            cast_type=cast_type, params=opts,
+            cast_type=cast_type, options=opts,
         )
 
     def delete(
             self,
             path: str,
             *,
-            body: Body | None = None,
             cast_type: Type[ResponseT],
+            body: Body | None = None,
             options: UserRequestInput = {},
     ) -> ResponseT | StreamResponse:
-        opts = ClientRequestParam.construct(method="delete", url=path, json_data=body, **options)
+        opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
 
         return self.request(
-            cast_type=cast_type, params=opts,
+            cast_type=cast_type, options=opts,
         )
 
     def _make_status_error(self, response) -> APIStatusError:
         response_text = response.text.strip()
         status_code = response.status_code
         error_msg = f"Error code: {status_code}, with error text {response_text}"
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_jwt_token.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_response.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 
 import httpx
 import logging
 from typing_extensions import ParamSpec, get_origin, get_args
 
 from ._base_type import NoneType
 from ._sse_client import StreamResponse
-from .._base_models import is_basemodel
+from ._base_models import is_basemodel
 
 if TYPE_CHECKING:
     from ._http_client import HttpClient
 
 P = ParamSpec("P")
 R = TypeVar("R")
 log: logging.Logger = logging.getLogger(__name__)
 
 class HttpResponse(Generic[R]):
     _cast_type: type[R]
     _client: "HttpClient"
     _parsed: R | None
-    _enable_stream: bool
+    _stream: bool
     _stream_cls: type[StreamResponse[Any]]
     http_response: httpx.Response
 
     def __init__(
             self,
             *,
             raw_response: httpx.Response,
             cast_type: type[R],
             client: "HttpClient",
-            enable_stream: bool = False,
+            stream: bool = False,
             stream_cls: type[StreamResponse[Any]] | None = None,
     ) -> None:
         self._cast_type = cast_type
         self._client = client
         self._parsed = None
         self._stream_cls = stream_cls
-        self._enable_stream = enable_stream
+        self._stream = stream
         self.http_response = raw_response
 
     def parse(self) -> R:
         self._parsed = self._parse()
         return self._parsed
 
     def _parse(self) -> R:
-        if self._enable_stream:
+        if self._stream:
             self._parsed = cast(
                 R,
                 self._stream_cls(
                     cast_type=cast(type, get_args(self._stream_cls)[0]),
                     response=self.http_response,
                     client=self._client
                 )
@@ -71,15 +71,15 @@
                 try:
                     data = http_response.json()
                 except Exception as exc:
                     log.debug("Could not read JSON from response data due to %s - %s", type(exc), exc)
                 else:
                     return self._client._process_response_data(
                         data=data,
-                        cast_to=cast_type,  # type: ignore
+                        cast_type=cast_type,  # type: ignore
                         response=http_response,
                     )
 
             return http_response.text
 
         data = http_response.json()
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_sse_client.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_utils/__init__.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_utils/_typing.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/core/_utils/_utils.py` & `zhipuai-2.0.1.20240429/zhipuai/core/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import List, Optional, Union, Dict, Any
+from typing import List, Optional
 
-from ..._base_models import BaseModel
+from ...core import BaseModel
 
 __all__ = ["Completion", "CompletionUsage"]
 
 
 class Function(BaseModel):
     arguments: str
     name: str
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Dict, Any
 
-from ..._base_models import BaseModel
+from ...core import BaseModel
 
 __all__ = [
     "ChatCompletionChunk",
     "Choice",
     "ChoiceDelta",
     "ChoiceDeltaFunctionCall",
     "ChoiceDeltaToolCall",
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/types/file_object.py` & `zhipuai-2.0.1.20240429/zhipuai/types/file_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, List
 
-from .._base_models import BaseModel
+from ..core import BaseModel
 
-__all__ = ["FileObject"]
+__all__ = ["FileObject", "ListOfFileObject"]
 
 
 class FileObject(BaseModel):
 
     id: Optional[str] = None
     bytes: Optional[int] = None
     created_at: Optional[int] = None
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Union, Optional, Dict, Any
-from typing_extensions import Literal
 
-from ..._base_models import BaseModel
+from ...core import BaseModel
 
 __all__ = ["FineTuningJob", "Error", "Hyperparameters", "ListOfFineTuningJob" ]
 
 
 class Error(BaseModel):
     code: str
     message: str
@@ -40,15 +39,13 @@
     status: str
 
     trained_tokens: Optional[int] = None
 
     training_file: str
 
     validation_file: Optional[str] = None
-    extra_json: Dict[str, Any]
 
 
 class ListOfFineTuningJob(BaseModel):
     object: Optional[str] = None
     data: List[FineTuningJob]
     has_more: Optional[bool] = None
-    extra_json: Dict[str, Any]
```

### Comparing `zhipuai-2.0.1.20240427/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Union, Optional
-from typing_extensions import Literal
 
-from ..._base_models import BaseModel
+from ...core import BaseModel
 
 __all__ = ["FineTuningJobEvent", "Metric", "JobEvent"]
 
 
 class Metric(BaseModel):
     epoch: Optional[Union[str, int, float]] = None
     current_steps: Optional[int] = None
```

### Comparing `zhipuai-2.0.1.20240427/PKG-INFO` & `zhipuai-2.0.1.20240429/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.0.1.20240427
+Version: 2.0.1.20240429
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Author: Zhipu AI
-Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.12.*
+Requires-Python: >=3.7, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.12.*
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
 Provides-Extra: extended-testing
 Requires-Dist: cachetools (>=4.2.2)
 Requires-Dist: httpx (>=0.23.0)
@@ -167,76 +168,77 @@
         model="charglm-3",  # 填写需要调用的模型名称
         messages=[
             {
                 "role": "user",
                 "content": "请问你在做什么"
             }
         ],
-        extra_body={
-            "meta": {
-                "user_info": "我是陆星辰，是一个男性，是一位知名导演，也是苏梦远的合作导演。我擅长拍摄音乐题材的电影。苏梦远对我的态度是尊敬的，并视我为良师益友。",
-                "bot_info": "苏梦远，本名苏远心，是一位当红的国内女歌手及演员。在参加选秀节目后，凭借独特的嗓音及出众的舞台魅力迅速成名，进入娱乐圈。她外表美丽动人，但真正的魅力在于她的才华和勤奋。苏梦远是音乐学院毕业的优秀生，善于创作，拥有多首热门原创歌曲。除了音乐方面的成就，她还热衷于慈善事业，积极参加公益活动，用实际行动传递正能量。在工作中，她对待工作非常敬业，拍戏时总是全身心投入角色，赢得了业内人士的赞誉和粉丝的喜爱。虽然在娱乐圈，但她始终保持低调、谦逊的态度，深得同行尊重。在表达时，苏梦远喜欢使用“我们”和“一起”，强调团队精神。",
-                "bot_name": "苏梦远",
-                "user_name": "陆星辰"
-            },
-        }
+        meta={
+          "user_info": "我是陆星辰，是一个男性，是一位知名导演，也是苏梦远的合作导演。我擅长拍摄音乐题材的电影。苏梦远对我的态度是尊敬的，并视我为良师益友。",
+          "bot_info": "苏梦远，本名苏远心，是一位当红的国内女歌手及演员。在参加选秀节目后，凭借独特的嗓音及出众的舞台魅力迅速成名，进入娱乐圈。她外表美丽动人，但真正的魅力在于她的才华和勤奋。苏梦远是音乐学院毕业的优秀生，善于创作，拥有多首热门原创歌曲。除了音乐方面的成就，她还热衷于慈善事业，积极参加公益活动，用实际行动传递正能量。在工作中，她对待工作非常敬业，拍戏时总是全身心投入角色，赢得了业内人士的赞誉和粉丝的喜爱。虽然在娱乐圈，但她始终保持低调、谦逊的态度，深得同行尊重。在表达时，苏梦远喜欢使用“我们”和“一起”，强调团队精神。",
+          "bot_name": "苏梦远",
+          "user_name": "陆星辰"
+        },
     )
     print(response)
 test_completions_charglm()
 ```
 
 
 
 ### 异常处理
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `openai.APIConnectionError` is raised.
-
-When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `openai.APIStatusError` is raised, containing `status_code` and `response` properties.
-
-All errors inherit from `openai.APIError`.
+模块定义了一些统一的参数返回(例如:响应错误，网络超时错误)
 
+业务定义了http错误的响应类 (在接口返回，40x或者50x), 会抛出 `zhipuai.APIStatusError`  ,包含 `status_code` 和 `response` 属性. 它们都是继承 `zhipuai.APIStatusError`.
+其它Exception，属于不可预知的错误
 ```python
-import openai
-from openai import OpenAI
-
-client = OpenAI()
-
+from zhipuai import ZhipuAI
+import zhipuai
+client = ZhipuAI()  # 填写您自己的APIKey
 try:
-    client.fine_tunes.create(
-        training_file="file-XGinujblHPwGLSztz8cPS8XY",
-    )
-except openai.APIConnectionError as e:
-    print("The server could not be reached")
-    print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except openai.RateLimitError as e:
-    print("A 429 status code was received; we should back off a bit.")
-except openai.APIStatusError as e:
-    print("Another non-200-range status code was received")
-    print(e.status_code)
-    print(e.response)
+  response = client.chat.completions.create(
+    model="glm-4",  # 填写需要调用的模型名称
+    messages=[
+      {"role": "user", "content": "作为一名营销专家，请为我的产品创作一个吸引人的slogan"},
+      {"role": "assistant", "content": "当然，为了创作一个吸引人的slogan，请告诉我一些关于您产品的信息"},
+      {"role": "user", "content": "智谱AI开放平台"},
+      {"role": "assistant", "content": "智启未来，谱绘无限一智谱AI，让创新触手可及!"},
+      {"role": "user", "content": "创造一个更精准、吸引人的slogan"}
+    ]
+  )
+  print(response)
+ 
+except zhipuai.APIStatusError as err:
+  print(err) 
+except zhipuai.APITimeoutError as err:
+  print(err) 
 ```
 
 Error codes are as followed:
 
 | Status Code | Error Type                 |
-| ----------- | -------------------------- |
-| 400         | `BadRequestError`          |
-| 401         | `AuthenticationError`      |
-| 403         | `PermissionDeniedError`    |
-| 404         | `NotFoundError`            |
-| 422         | `UnprocessableEntityError` |
-| 429         | `RateLimitError`           |
-| >=500       | `InternalServerError`      |
-| N/A         | `APIConnectionError`       |
+|-------------| -------------------------- |
+| 400         | `APIRequestFailedError`          |
+| 401         | `APIAuthenticationError`      |
+| 429         | `APIReachLimitError`           |
+| 500         | `APIInternalError`      |
+| 503         | `APIServerFlowExceedError`      |
+| N/A         | `APIStatusError`       |
 
 
 
 ### 更新日志
 
+`2024-4-29` 
+- 一些 `python3.7` 的代码适配问题， 
+- 接口失败重试机制，通过 `retry` 参数控制重试次数，默认为3次
+- 接口超时策略调整，通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
+- 对话模块增加超拟人大模型参数支持，`model="charglm-3"`, `meta`参数支持
+  
 `2024-4-23` 
 - 一些兼容 `pydantic<3,>=1.9.0 ` 的代码，
 - 报文处理的业务请求参数和响应参数可通过配置扩充
 - 兼容了一些参数 `top_p:1`,`temperture:0`(do_sample重写false，参数top_p temperture不生效)
 - 图像理解部分，  image_url参数base64内容包含 `data:image/jpeg;base64`兼容
 - 删除jwt认证逻辑
```

