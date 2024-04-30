# Comparing `tmp/helmet-1.0.4.tar.gz` & `tmp/helmet-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmet-1.0.4.tar", max compression
+gzip compressed data, was "helmet-1.0.5.tar", max compression
```

## Comparing `helmet-1.0.4.tar` & `helmet-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1279 2024-04-27 16:36:40.125625 helmet-1.0.4/README.md
--rw-r--r--   0        0        0      497 2024-04-27 16:36:40.125625 helmet-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2652 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/explainers/__init__.py
--rw-r--r--   0        0        0     5236 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/explainers/gradients.py
--rw-r--r--   0        0        0      630 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/explainers/perturbation.py
--rw-r--r--   0        0        0       49 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/model/__init__.py
--rw-r--r--   0        0        0     3680 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/model/base_lm.py
--rw-r--r--   0        0        0     5681 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/model/dec_lm.py
--rw-r--r--   0        0        0     3888 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/updater.py
--rw-r--r--   0        0        0       79 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/utils/constants.py
--rw-r--r--   0        0        0     3277 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/utils/types.py
--rw-r--r--   0        0        0      130 2024-04-27 16:36:40.125625 helmet-1.0.4/src/helmet/utils/utils.py
--rw-r--r--   0        0        0     2039 1970-01-01 00:00:00.000000 helmet-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1595 2024-04-30 07:26:25.313296 helmet-1.0.5/README.md
+-rw-r--r--   0        0        0      497 2024-04-30 07:26:25.313296 helmet-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2652 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/__init__.py
+-rw-r--r--   0        0        0     5236 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/gradients.py
+-rw-r--r--   0        0        0      630 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/perturbation.py
+-rw-r--r--   0        0        0       49 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/base_lm.py
+-rw-r--r--   0        0        0     6169 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/dec_lm.py
+-rw-r--r--   0        0        0     3949 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/updater.py
+-rw-r--r--   0        0        0       79 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/constants.py
+-rw-r--r--   0        0        0     3277 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/types.py
+-rw-r--r--   0        0        0      130 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/utils.py
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 helmet-1.0.5/PKG-INFO
```

### Comparing `helmet-1.0.4/README.md` & `helmet-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,10 +51,20 @@
 - Run experimental prompts
 -
 
 ## Running webapp locally
 
 For this, please check the `README`
 
+## Credits
+
+Some inspiration has been drawn from a couple of other tools:
+
+- [Interpret-ml](https://github.com/kayoyin/interpret-lm)
+- [Ecco](https://github.com/jalammar/ecco)
+- [Phoenix](https://github.com/Arize-ai/phoenix)
+- [Inseq](https://github.com/inseq-team/inseq)
+- [Ferret](https://github.com/g8a9/ferret)
+
 ## License
 
 `helmet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `helmet-1.0.4/src/helmet/__init__.py` & `helmet-1.0.5/src/helmet/__init__.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.4/src/helmet/explainers/gradients.py` & `helmet-1.0.5/src/helmet/explainers/gradients.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.4/src/helmet/explainers/perturbation.py` & `helmet-1.0.5/src/helmet/explainers/perturbation.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.4/src/helmet/model/base_lm.py` & `helmet-1.0.5/src/helmet/model/base_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,25 @@
 
     def normalize(self, attr):
         l2_norm = np.linalg.norm(attr)
         l2_normalized_matrix = attr / l2_norm
         return l2_normalized_matrix
 
     def update_run(self, run: Run):
-        update_app(self.platform_url, "/runs", run.dict())
+        id = update_app(self.platform_url, "/runs", run.dict())
+        return id
 
     def update_explainer_model(self):
         b = {
             "model_checkpoint": self.model_checkpoint,
             "model": self.model.config.model_type,
             "tokenizer": self.tokenizer.name_or_path,
             "model_type": self.model_type
         }
-        update_app(self.platform_url, "/update_model", b)
+        id = update_app(self.platform_url, "/update_model", b)
 
     def reset_model(self):
         self.model.eval()
         self.model.zero_grad()
 
 
     @abstractmethod
```

### Comparing `helmet-1.0.4/src/helmet/model/dec_lm.py` & `helmet-1.0.5/src/helmet/model/dec_lm.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,44 +25,51 @@
         except Exception as e:
             print(e)
             raise KeyError("embeddings must be specified in model_config")
 
         super().__init__(model_checkpoint, model, tokenizer, self.model_type, url, project_id, embeddings, device)
     
     def forward(self, inputs, generation_args, **kwargs) -> Tuple[list, AlternativesExplanation]:
-        ids = self.to_device(inputs["input_ids"])
-
-        input_len = len(ids[0])
         amount_potentials = 5
+        inputs_ = self.to_device(inputs)
+
+        input_len = len(inputs_["input_ids"][0])
 
         output = self.model.generate(
-            input_ids=ids, 
+            **inputs_, 
             return_dict_in_generate=True,
             output_scores=True, # this gets the scores, while logits are unprocessed.
+            # num_beams=5,
+            no_repeat_ngram_size=2,
+            # num_return_sequences=5,
+            # early_stopping=True,
             **generation_args,
         )
 
-        output = output.to_tuple() #0 it tokens, 1 is scores
-        outputIds = output[0]
-        scores = output[1]
-
-        alternatives_per_token = []
-        # for i in range(len(scores)):
-        #     scores = scores[i]
-        #     top_k = scores.topk(amount_potentials, dim=1)
-        #     top_k_scores = top_k.values.detach().flatten().tolist()
-        #     top_k_indices = top_k.indices
-
-        #     tokens = self.tokenizer.convert_ids_to_tokens(top_k_indices.detach().flatten(), skip_special_tokens=True)
-        #     res = [{"token": token, "score": score} for token, score in zip(tokens, top_k_scores)]
-        #     alternatives_per_token.append(res)
-        
-        outs = outputIds[0].detach().cpu().numpy()
+        outputIds = output.sequences[0] #first of 5 sequence outputs
+        outs = outputIds.detach().cpu().numpy()
         output_token_ids = outs[input_len:]
         print("output_token_ids", output_token_ids)
+
+        scores = output.scores
+
+        alternatives_per_token = []
+        for i in range(len(scores)):
+            local_scores = scores[i][0] #only for the final sequence, thus [0]
+            # Scores is now a tensor of shape (vocab_size)
+            top_k = local_scores.topk(amount_potentials) 
+            top_k_scores = top_k.values.detach().flatten().tolist()
+            #  normalize scores
+            top_k_scores = self.normalize(top_k_scores)
+            top_k_indices = top_k.indices
+
+            tokens = self.tokenizer.convert_ids_to_tokens(top_k_indices.detach().flatten(), skip_special_tokens=True)
+            res = [{"token": token, "score": score} for token, score in zip(tokens, top_k_scores)]
+            alternatives_per_token.append(res)
+
         
         return output_token_ids, AlternativesExplanation(alternatives_per_token)
     
     def predict(self, prompt, generation_args, groundtruth=None, *args, **kwargs):
         print("start of the predict function")
         start = time.time()
         input = self._encode_text(prompt)
@@ -76,17 +83,17 @@
         print("Predicted output:", output_str)
         
         end = time.time()
         execution_time = end - start
 
         formatted_run = self._format_run(input_str, output_str, [alternatives], execution_time, groundtruth=groundtruth)
 
-        self.update_run(formatted_run)
+        id = self.update_run(formatted_run)
 
-        return output_str
+        return output_str, id
 
     def saliency_explainer(self, id: str, **kwargs) -> SaliencyExplanation:
         run: Run = self.get_run(id)
         input = self._encode_text(run.input.prompt)
         output_token_ids = self.tokenizer.convert_tokens_to_ids(run.output.tokens)
         
         input_ids = input["input_ids"][0]
@@ -106,35 +113,38 @@
             gradients = input_x_gradient(base_saliency_matrix, base_embd_matrix, normalize=True)
             result.append(gradients)
             print("finished token", idx, "of", total_length)
 
         explanation = SaliencyExplanation(input_attributions=result)
         run.explanations.append(explanation)
 
-        self.update_run(run)
+        id = self.update_run(run)
 
         return explanation
     
     def contrastive_explainer(self, id: str, alternative_str: str, **kwargs) -> ContrastiveExplanation:
         run: Run = self.get_run(id)
         input = self._tokenize(run.input.prompt)
         alternative_output = self._encode_text(alternative_str)
         output_token_ids = self.tokenizer.convert_tokens_to_ids(run.output.tokens)
 
-        input_ids = input["input_ids"][0]
-        attention_mask = input["attention_mask"]
+        input_ids = self.to_device(input["input_ids"][0])
+        attention_mask = self.to_device(input["attention_mask"])
         
         output_id = output_token_ids[0]
 
-        alternative_id = alternative_output["input_ids"][0][0] # not sure why we need this
+        alternative_id = alternative_output["input_ids"][0]
+        if len(alternative_id) > 1:
+            print("Warning: alternative output has more than one token, using the first one")
+            alternative_id = alternative_id[0]
         saliency_matrix, base_embd_matrix = analyze_token(self, input_ids, attention_mask, correct=output_id, foil=alternative_id)
         gradients = input_x_gradient(saliency_matrix, base_embd_matrix, normalize=True)
 
         alternative_output_str = self.tokenizer.decode(alternative_id, skip_special_tokens=True)
         
         explanation = ContrastiveExplanation(contrastive_input=alternative_output_str, attributions=gradients)
         run.explanations.append(explanation)
 
-        self.update_run(run)
+        id = self.update_run(run)
 
         return explanation
```

### Comparing `helmet-1.0.4/src/helmet/updater.py` & `helmet-1.0.5/src/helmet/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
     body: dict: the body of the request """
     
     if url is None or route is None:
         raise ValueError(f"url cannot be None url: {url} route:{route}")
     try :
         r = requests.post(f"{url}{route}", json=serialize(body))
         r.raise_for_status()
-        print("updated app, result: ", r.json())
+        res = r.json()
+        print("updated app, result: ", res)
+        return res.get("insertedId", None)
         
     except Exception as e:
         print(e)
         raise ValueError(f"Failed to get app. Is it running? url: {url} route: {route}")
     
 
 def get_run(url: str, run_id: str) -> Run | None:
```

### Comparing `helmet-1.0.4/src/helmet/utils/types.py` & `helmet-1.0.5/src/helmet/utils/types.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.4/PKG-INFO` & `helmet-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmet
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Jeroen
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -73,11 +73,21 @@
 - Run experimental prompts
 -
 
 ## Running webapp locally
 
 For this, please check the `README`
 
+## Credits
+
+Some inspiration has been drawn from a couple of other tools:
+
+- [Interpret-ml](https://github.com/kayoyin/interpret-lm)
+- [Ecco](https://github.com/jalammar/ecco)
+- [Phoenix](https://github.com/Arize-ai/phoenix)
+- [Inseq](https://github.com/inseq-team/inseq)
+- [Ferret](https://github.com/g8a9/ferret)
+
 ## License
 
 `helmet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

