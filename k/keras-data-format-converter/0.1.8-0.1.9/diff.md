# Comparing `tmp/keras-data-format-converter-0.1.8.tar.gz` & `tmp/keras-data-format-converter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-data-format-converter-0.1.8.tar", max compression
+gzip compressed data, was "keras-data-format-converter-0.1.9.tar", max compression
```

## Comparing `keras-data-format-converter-0.1.8.tar` & `keras-data-format-converter-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-05-25 12:40:12.557908 keras-data-format-converter-0.1.8/LICENSE
--rw-r--r--   0        0        0     1833 2022-05-25 12:40:12.558163 keras-data-format-converter-0.1.8/README.md
--rw-r--r--   0        0        0       85 2022-11-13 12:50:54.945916 keras-data-format-converter-0.1.8/keras_data_format_converter/__init__.py
--rw-r--r--   0        0        0     3048 2022-12-01 18:06:07.158768 keras-data-format-converter-0.1.8/keras_data_format_converter/converterapi.py
--rw-r--r--   0        0        0        0 2022-05-25 12:40:12.558644 keras-data-format-converter-0.1.8/keras_data_format_converter/layers/__init__.py
--rw-r--r--   0        0        0        0 2022-05-25 12:40:12.558762 keras-data-format-converter-0.1.8/keras_data_format_converter/layers/confighandlers/__init__.py
--rw-r--r--   0        0        0      224 2022-09-20 13:07:37.196236 keras-data-format-converter-0.1.8/keras_data_format_converter/layers/confighandlers/dataformat.py
--rw-r--r--   0        0        0     1945 2022-11-13 12:50:54.953861 keras-data-format-converter-0.1.8/keras_data_format_converter/layers/layer_utils.py
--rw-r--r--   0        0        0     9767 2022-12-06 10:10:43.773250 keras-data-format-converter-0.1.8/keras_data_format_converter/modelconverter.py
--rw-r--r--   0        0        0      289 2022-05-25 12:40:12.559683 keras-data-format-converter-0.1.8/keras_data_format_converter/utils.py
--rw-r--r--   0        0        0      691 2022-12-06 10:22:54.871106 keras-data-format-converter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 keras-data-format-converter-0.1.8/setup.py
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 keras-data-format-converter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-25 12:40:12.557908 keras-data-format-converter-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1833 2022-05-25 12:40:12.558163 keras-data-format-converter-0.1.9/README.md
+-rw-r--r--   0        0        0       85 2022-11-13 12:50:54.945916 keras-data-format-converter-0.1.9/keras_data_format_converter/__init__.py
+-rw-r--r--   0        0        0     3152 2022-12-07 07:23:16.595845 keras-data-format-converter-0.1.9/keras_data_format_converter/converterapi.py
+-rw-r--r--   0        0        0        0 2022-05-25 12:40:12.558644 keras-data-format-converter-0.1.9/keras_data_format_converter/layers/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-25 12:40:12.558762 keras-data-format-converter-0.1.9/keras_data_format_converter/layers/confighandlers/__init__.py
+-rw-r--r--   0        0        0      224 2022-09-20 13:07:37.196236 keras-data-format-converter-0.1.9/keras_data_format_converter/layers/confighandlers/dataformat.py
+-rw-r--r--   0        0        0     1945 2022-11-13 12:50:54.953861 keras-data-format-converter-0.1.9/keras_data_format_converter/layers/layer_utils.py
+-rw-r--r--   0        0        0     9767 2022-12-06 10:10:43.773250 keras-data-format-converter-0.1.9/keras_data_format_converter/modelconverter.py
+-rw-r--r--   0        0        0      289 2022-05-25 12:40:12.559683 keras-data-format-converter-0.1.9/keras_data_format_converter/utils.py
+-rw-r--r--   0        0        0      691 2022-12-07 07:27:08.847528 keras-data-format-converter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 keras-data-format-converter-0.1.9/setup.py
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 keras-data-format-converter-0.1.9/PKG-INFO
```

### Comparing `keras-data-format-converter-0.1.8/LICENSE` & `keras-data-format-converter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-data-format-converter-0.1.8/README.md` & `keras-data-format-converter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `keras-data-format-converter-0.1.8/keras_data_format_converter/converterapi.py` & `keras-data-format-converter-0.1.9/keras_data_format_converter/converterapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,18 @@
         else:
             new_input_tensor = tf.keras.Input(new_input_shape, name=k_input.name, batch_size=k_input.shape[0])
         back_to_channel_first_perm_values = calculate_permute_values(new_input_tensor.shape, to_channel_first=True)
         permute_after = Permute(back_to_channel_first_perm_values)(new_input_tensor)
         new_inputs.append(new_input_tensor)
         new_old_inputs.append(permute_after)
 
+    # clear the old inbound_nodes
+    for layer in k_model.layers:
+        layer.inbound_nodes.clear()
+
     new_outputs = []
     new_old_outputs = k_model.call(new_old_inputs)
     if not isinstance(new_old_outputs, list):
         new_old_outputs = [new_old_outputs]
     for output in new_old_outputs:
         perm_values = calculate_permute_values(output.shape, to_channel_first=False)
         new_outputs.append(Permute(perm_values)(output))
```

### Comparing `keras-data-format-converter-0.1.8/keras_data_format_converter/layers/layer_utils.py` & `keras-data-format-converter-0.1.9/keras_data_format_converter/layers/layer_utils.py`

 * *Files identical despite different names*

### Comparing `keras-data-format-converter-0.1.8/keras_data_format_converter/modelconverter.py` & `keras-data-format-converter-0.1.9/keras_data_format_converter/modelconverter.py`

 * *Files identical despite different names*

### Comparing `keras-data-format-converter-0.1.8/pyproject.toml` & `keras-data-format-converter-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keras-data-format-converter"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generates equal keras models with the desired data format"
 readme = "README.md"
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.8.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `keras-data-format-converter-0.1.8/setup.py` & `keras-data-format-converter-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras_require = \
 {':platform_machine == "arm64"': ['tensorflow-macos==2.8.0'],
  ':platform_machine == "x86_64"': ['tensorflow==2.8.0',
                                    'tensorflow-addons>=0.17.1,<0.18.0']}
 
 setup_kwargs = {
     'name': 'keras-data-format-converter',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Generates equal keras models with the desired data format',
     'long_description': '# Keras data format converter\n\nGenerates equal keras models with the desired data format  \n\n\n## Requirements\ntensorflow >= 2.0\n\n\n## API\n`convert_channels_first_to_last(model: keras.Model, inputs_to_transpose: List[str] = None, verbose: bool = False) -> keras.Model`\n\n`convert_channels_last_to_first(model: tf.keras.Model, inputs_to_transpose: List[str] = None, verbose: bool = False) \\\n        -> tf.keras.Model`\n\n`model`: Keras model to convert\n\n`inputs_to_transpose`: list of input names that need to be transposed due tothe data foramt changing  \n\n`verbose`: detailed output\n\n## Getting started\n\n```python\nfrom tensorflow import keras\nfrom keras_data_format_converter import convert_channels_last_to_first\n\n# Load Keras model\nkeras_model = keras.models.load_model("my_image_model")\n\n# Call the converter (image_input is an input that needs to be transposed, can be different for your model)\nconverted_model = convert_channels_last_to_first(keras_model, ["image_input"])\n```\n\n## Supported Layers with Special handling\n- [X] Normalization layers\n- [x] Permute\n- [x] Reshape\n- [x] Concatenate\n- [ ] Dot\n- [ ] MultiHeadAttention\n- [ ] TFOpLambda (Inserted by the Functional API construction whenever users call\n  a supported TF symbol on KerasTensors, see [here](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/keras/layers/core.py#L1284) at Tensorflow repo for more info)\n\n## Unsupported Layers due to lack of data_format property\n- Cropping1D\n- Upsampling1D\n- Zeropadding1D\n- All layers in tensorflow.keras.preprocessing\n\n## How to deploy\n- Create a new release version on GitHub\n- Update parameters in setup.py (usually `version` and `download_url`)\n- Run `python setup.py sdist` in root directory\n- Run `pip install twine`\n- Run `twine upload dist/*`\n \n\n\n## License\nThis software is covered by MIT License.\n',
     'author': 'dorhar',
     'author_email': 'doron.harnoy@tensorleap.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `keras-data-format-converter-0.1.8/PKG-INFO` & `keras-data-format-converter-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-data-format-converter
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generates equal keras models with the desired data format
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

