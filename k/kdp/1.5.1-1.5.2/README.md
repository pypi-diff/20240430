# Comparing `tmp/kdp-1.5.1.tar.gz` & `tmp/kdp-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-1.5.1.tar", max compression
+gzip compressed data, was "kdp-1.5.2.tar", max compression
```

## Comparing `kdp-1.5.1.tar` & `kdp-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-04-19 13:26:08.191996 kdp-1.5.1/LICENSE
--rw-r--r--   0        0        0     4114 2024-04-19 13:26:08.191996 kdp-1.5.1/README.md
--rw-r--r--   0        0        0   102413 2024-04-19 13:26:08.199996 kdp-1.5.1/docs/kdp_logo.png
--rw-r--r--   0        0        0      668 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/custom_layers.py
--rw-r--r--   0        0        0     5046 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/features.py
--rw-r--r--   0        0        0     8180 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/layers_factory.py
--rw-r--r--   0        0        0     3322 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/pipeline.py
--rw-r--r--   0        0        0    26856 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/processor.py
--rw-r--r--   0        0        0    14605 2024-04-19 13:26:08.199996 kdp-1.5.1/kdp/stats.py
--rw-r--r--   0        0        0     4034 2024-04-19 13:27:30.540485 kdp-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 kdp-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-30 14:16:46.250237 kdp-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4114 2024-04-30 14:16:46.250237 kdp-1.5.2/README.md
+-rw-r--r--   0        0        0   102413 2024-04-30 14:16:46.262237 kdp-1.5.2/docs/kdp_logo.png
+-rw-r--r--   0        0        0      763 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/__init__.py
+-rw-r--r--   0        0        0     4845 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/custom_layers.py
+-rw-r--r--   0        0        0     5046 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/features.py
+-rw-r--r--   0        0        0     8739 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/layers_factory.py
+-rw-r--r--   0        0        0     3322 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/pipeline.py
+-rw-r--r--   0        0        0    30444 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/processor.py
+-rw-r--r--   0        0        0    14605 2024-04-30 14:16:46.262237 kdp-1.5.2/kdp/stats.py
+-rw-r--r--   0        0        0     4034 2024-04-30 14:16:46.262237 kdp-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 kdp-1.5.2/PKG-INFO
```

### Comparing `kdp-1.5.1/LICENSE` & `kdp-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/README.md` & `kdp-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/docs/kdp_logo.png` & `kdp-1.5.2/docs/kdp_logo.png`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/kdp/__init__.py` & `kdp-1.5.2/kdp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # project plugin
 from kdp.features import CategoricalFeature, FeatureType, NumericalFeature, TextFeature
 from kdp.layers_factory import PreprocessorLayerFactory
 from kdp.pipeline import FeaturePreprocessor, Pipeline, ProcessingStep
-from kdp.processor import CategoryEncodingOptions, OutputModeOptions, PreprocessingModel
+from kdp.processor import (
+    CategoryEncodingOptions,
+    OutputModeOptions,
+    PreprocessingModel,
+    TransformerBlockPlacementOptions,
+)
 from kdp.stats import DatasetStatistics
 
 __all__ = [
     "ProcessingStep",
     "Pipeline",
     "FeaturePreprocessor",
     "FeatureType",
     "NumericalFeature",
     "CategoricalFeature",
     "TextFeature",
     "DatasetStatistics",
     "PreprocessorLayerFactory",
     "PreprocessingModel",
     "CategoryEncodingOptions",
+    "TransformerBlockPlacementOptions",
     "OutputModeOptions",
 ]
```

### Comparing `kdp-1.5.1/kdp/features.py` & `kdp-1.5.2/kdp/features.py`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/kdp/layers_factory.py` & `kdp-1.5.2/kdp/layers_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 
 import tensorflow as tf
 
-from kdp.custom_layers import CastToFloat32Layer, TextPreprocessingLayer
+from kdp.custom_layers import CastToFloat32Layer, TextPreprocessingLayer, TransformerBlock
 
 
 class PreprocessorLayerFactory:
     @staticmethod
     def create_layer(layer_class, name: str = None, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a layer, automatically filtering kwargs based on the provided layer_class.
 
@@ -248,7 +248,24 @@
             An instance of the CastToFloat32Layer layer.
         """
         return PreprocessorLayerFactory.create_layer(
             layer_class=CastToFloat32Layer,
             name=name,
             **kwargs,
         )
+
+    @staticmethod
+    def transformer_block_layer(name: str = "transformer", **kwargs: dict) -> tf.keras.layers.Layer:
+        """Create a TransformerBlock layer.
+
+        Args:
+            name: The name of the layer.
+            **kwargs: Additional keyword arguments to pass to the layer constructor.
+
+        Returns:
+            An instance of the TransformerBlock layer.
+        """
+        return PreprocessorLayerFactory.create_layer(
+            layer_class=TransformerBlock,
+            name=name,
+            **kwargs,
+        )
```

### Comparing `kdp-1.5.1/kdp/pipeline.py` & `kdp-1.5.2/kdp/pipeline.py`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/kdp/processor.py` & `kdp-1.5.2/kdp/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 
 class TextVectorizerOutputOptions(auto):
     TF_IDF = "tf_idf"
     INT = "int"
     MULTI_HOT = "multi_hot"
 
 
+class TransformerBlockPlacementOptions(auto):
+    CATEGORICAL = "categorical"
+    ALL_FEATURES = "all_features"
+
+
 # testing conversion
 class FeatureSpaceConverter:
     def __init__(self):
         """Initialize the FeatureSpaceConverter class."""
         self.features_space = {}
         self.numeric_features = []
         self.categorical_features = []
@@ -102,14 +107,19 @@
         batch_size: int = 50_000,
         feature_crosses: list[tuple[str, str, int]] = None,
         features_stats_path: str = None,
         output_mode: str = OutputModeOptions.CONCAT,
         overwrite_stats: bool = False,
         log_to_file: bool = False,
         features_specs: dict[str, FeatureType | str] = None,
+        transfo_nr_blocks: int = None,
+        transfo_nr_heads: int = 3,
+        transfo_ff_units: int = 16,
+        transfo_dropout_rate: float = 0.25,
+        transfo_placement: str = TransformerBlockPlacementOptions.CATEGORICAL,
     ) -> None:
         """Initialize a preprocessing model.
 
         Args:
             features_stats (dict[str, Any]): A dictionary containing the statistics of the features.
             path_data (str): The path to the data from which estimate the statistics.
             batch_size (int): The batch size for the data iteration for stats estimation.
@@ -117,29 +127,42 @@
                 A list of tuples containing the names of the features to be crossed,
                 and nr_bins to be used for hashing.
             features_stats_path (str): The path where to save/load features statistics.
             output_mode (str): The output mode of the model (concat | dict).
             overwrite_stats (bool): A boolean indicating whether to overwrite the statistics.
             log_to_file (bool): A boolean indicating whether to log to a file.
             features_specs (dict[str, FeatureType | str]): A dictionary containing the features and their types.
+            transfo_nr_blocks (int): The number of transformer blocks for the transformer block
+                (default=None, transformer block is disabled).
+            transfo_nr_heads (int): The number of heads for the transformer block (categorical variables).
+            transfo_ff_units (int): The number of feed forward units for the transformer
+            transfo_dropout_rate (float): The dropout rate for the transformer block (default=0.25).
+            transfo_placement (str): The placement of the transformer block (categorical | all_features).
         """
         self.path_data = path_data
         self.batch_size = batch_size or 50_000
         self.features_stats = features_stats or {}
         self.features_specs = features_specs or {}
         self.features_stats_path = features_stats_path or "features_stats.json"
         self.feature_crosses = feature_crosses or []
         self.output_mode = output_mode
         self.overwrite_stats = overwrite_stats
+        # transformer blocks controll
+        self.transfo_nr_blocks = transfo_nr_blocks
+        self.transfo_nr_heads = transfo_nr_heads
+        self.transfo_ff_units = transfo_ff_units
+        self.transfo_dropout_rate = transfo_dropout_rate
+        self.transfo_placement = transfo_placement
 
         # PLACEHOLDERS
         self.preprocessors = {}
         self.inputs = {}
         self.signature = {}
         self.outputs = {}
+        self.outputs_categorical = {}
 
         if log_to_file:
             logger.info("Logging to file enabled 🗂️")
             logger.add("PreprocessModel.log")
 
         # formatting features specs info
         self._init_features_specs(features_specs=features_specs)
@@ -318,19 +341,14 @@
                     mean=mean,
                     variance=variance,
                     name=f"norm_{feature_name}",
                 )
         # defining the pipeline input layer
         _output_pipeline = preprocessor.chain(input_layer=input_layer)
 
-        # adjusting output
-        # if _feature.feature_type == FeatureType.FLOAT_DISCRETIZED:
-        # Cast the crossed feature to float32
-        # _output_pipeline = tf.cast(_output_pipeline, tf.float32)
-
         # defining output
         self.outputs[feature_name] = _output_pipeline
 
     def _add_pipeline_categorical(self, feature_name: str, input_layer, stats: dict) -> None:
         """Add a categorical preprocessing step to the pipeline.
 
         Args:
@@ -398,16 +416,17 @@
             )
 
         # we need to flatten the categorical feature
         preprocessor.add_processing_step(
             layer_creator=PreprocessorLayerFactory.flatten_layer,
             name=f"flatten_{feature_name}",
         )
+
         # adding outputs
-        self.outputs[feature_name] = preprocessor.chain(input_layer=input_layer)
+        self.outputs_categorical[feature_name] = preprocessor.chain(input_layer=input_layer)
 
     def _add_pipeline_text(self, feature_name: str, input_layer, stats: dict) -> None:
         """Add a text preprocessing step to the pipeline.
 
         Args:
             feature_name (str): The name of the feature to be preprocessed.
             input_layer: The input layer for the feature.
@@ -451,15 +470,17 @@
             )
             # for concatenation we need the same format
             # so the cast to float 32 is necessary
             preprocessor.add_processing_step(
                 layer_creator=PreprocessorLayerFactory.cast_to_float32_layer,
                 name=f"cast_to_float_{feature_name}",
             )
-        self.outputs[feature_name] = preprocessor.chain(input_layer=input_layer)
+        # adding outputs
+        self.outputs_categorical[feature_name] = preprocessor.chain(input_layer=input_layer)
+        # self.outputs[feature_name] = preprocessor.chain(input_layer=input_layer)
 
     def _add_pipeline_cross(self) -> None:
         """Add a crossing preprocessing step to the pipeline.
 
         Args:
             stats (dict): A dictionary containing the metadata of the feature, including
                 the list of features it is crossed with and the depth of the crossing.
@@ -496,17 +517,64 @@
         """Preparing the outputs of the model.
 
         Note:
             Two outputs are possible based on output_model variable.
         """
         logger.info("Building preprocessor Model")
         if self.output_mode == OutputModeOptions.CONCAT:
+            # getting all features to concatenate
             self.features_to_concat = list(self.outputs.values())
-            self.concat = tf.keras.layers.Concatenate(axis=-1)
-            self.outputs = self.concat(self.features_to_concat)
+            self.features_cat_to_concat = list(self.outputs_categorical.values())
+
+            # Concatenate numerical features
+            concat_num = tf.keras.layers.Concatenate(
+                name="ConcatenateNumeric",
+                axis=-1,
+            )(self.features_to_concat)
+
+            # Concatenate categorical features
+            concat_cat = tf.keras.layers.Concatenate(
+                name="ConcatenateCategorical",
+                axis=-1,
+            )(self.features_cat_to_concat)
+
+            # adding transformer layers
+            if self.transfo_nr_blocks and self.transfo_placement == TransformerBlockPlacementOptions.CATEGORICAL:
+                logger.info(f"Adding transformer blocks CATEGORICAL: #{self.transfo_nr_blocks}")
+                for block_idx in range(self.transfo_nr_blocks):
+                    concat_cat = PreprocessorLayerFactory.transformer_block_layer(
+                        dim_model=concat_cat.shape[1],
+                        num_heads=self.transfo_nr_heads,
+                        ff_units=self.transfo_ff_units,
+                        dropout_rate=self.transfo_dropout_rate,
+                        name=f"transformer_block_{block_idx}_{self.transfo_nr_heads}heads",
+                    )(concat_cat)
+
+            # Combine concatenated numerical and categorical features
+            logger.info("Concatenating all features")
+            self.outputs = tf.keras.layers.Concatenate(
+                name="ConcatenateAllFeatures",
+                axis=-1,
+            )([concat_num, concat_cat])
+
+            # TODO: check shape mismatch here (Inputs have incompatible shapes. Received shapes (1, 141) and (1, 4))
+            if self.transfo_nr_blocks and self.transfo_placement == TransformerBlockPlacementOptions.ALL_FEATURES:
+                _transfor_input_shape = self.outputs.shape[1]
+                logger.info(
+                    f"Adding transformer blocks ALL_FEATURES: #{self.transfo_nr_blocks}",
+                )
+                for block_idx in range(self.transfo_nr_blocks):
+                    self.outputs = PreprocessorLayerFactory.transformer_block_layer(
+                        dim_model=_transfor_input_shape,
+                        num_heads=self.transfo_nr_heads,
+                        ff_units=self.transfo_ff_units,
+                        dropout_rate=self.transfo_dropout_rate,
+                        name=f"transformer_block_{block_idx}_{self.transfo_nr_heads}heads",
+                    )(self.outputs)
+
             logger.info("Concatenating outputs mode enabled")
         else:
             outputs = OrderedDict([(k, None) for k in self.inputs if k in self.outputs])
             outputs.update(OrderedDict(self.outputs))
             self.outputs = outputs
             logger.info("OrderedDict outputs mode enabled")
```

### Comparing `kdp-1.5.1/kdp/stats.py` & `kdp-1.5.2/kdp/stats.py`

 * *Files identical despite different names*

### Comparing `kdp-1.5.1/pyproject.toml` & `kdp-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kdp"
-version = "1.5.1"
+version = "1.5.2"
 documentation = "http://piotrlaczkowski.github.io/keras-data-processor/"
 repository = "https://github.com/piotrlaczkowski/keras-data-processor"
 description = "Data Preprocessing model based on Keras preprocessing layers"
 authors = ["piotrlaczkowski <piotr.laczkowski@gmail.com>"]
 readme = "README.md"
 include = ["docs/kdp_logo.png"]
```

### Comparing `kdp-1.5.1/PKG-INFO` & `kdp-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp
-Version: 1.5.1
+Version: 1.5.2
 Summary: Data Preprocessing model based on Keras preprocessing layers
 Home-page: https://github.com/piotrlaczkowski/keras-data-processor
 Author: piotrlaczkowski
 Author-email: piotr.laczkowski@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

