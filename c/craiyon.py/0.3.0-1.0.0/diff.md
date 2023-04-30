# Comparing `tmp/craiyon.py-0.3.0.tar.gz` & `tmp/craiyon.py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craiyon.py-0.3.0.tar", last modified: Mon Mar 13 17:44:58 2023, max compression
+gzip compressed data, was "craiyon.py-1.0.0.tar", last modified: Sun Apr 30 18:15:04 2023, max compression
```

## Comparing `craiyon.py-0.3.0.tar` & `craiyon.py-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 17:44:58.741175 craiyon.py-0.3.0/
--rw-rw-rw-   0        0        0    11546 2022-07-30 06:08:39.000000 craiyon.py-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     9082 2023-03-13 17:44:58.741175 craiyon.py-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     8618 2023-03-13 17:38:54.000000 craiyon.py-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 17:44:58.709968 craiyon.py-0.3.0/craiyon/
--rw-rw-rw-   0        0        0      103 2023-03-13 16:55:35.000000 craiyon.py-0.3.0/craiyon/__init__.py
--rw-rw-rw-   0        0        0     5137 2023-03-13 17:16:43.000000 craiyon.py-0.3.0/craiyon/craiyon.py
--rw-rw-rw-   0        0        0     1599 2023-03-13 16:55:35.000000 craiyon.py-0.3.0/craiyon/craiyon_utils.py
--rw-rw-rw-   0        0        0     2984 2023-03-13 17:14:39.000000 craiyon.py-0.3.0/craiyon/templates.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:44:58.725552 craiyon.py-0.3.0/craiyon.py.egg-info/
--rw-rw-rw-   0        0        0     9082 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-13 17:44:58.000000 craiyon.py-0.3.0/craiyon.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-03-13 17:44:58.741175 craiyon.py-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-03-13 16:55:35.000000 craiyon.py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:15:04.495058 craiyon.py-1.0.0/
+-rw-rw-rw-   0        0        0    11546 2022-07-30 06:08:39.000000 craiyon.py-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    10541 2023-04-30 18:15:04.495058 craiyon.py-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10077 2023-04-30 18:10:20.000000 craiyon.py-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 18:15:04.457941 craiyon.py-1.0.0/craiyon/
+-rw-rw-rw-   0        0        0      103 2023-04-30 17:02:03.000000 craiyon.py-1.0.0/craiyon/__init__.py
+-rw-rw-rw-   0        0        0     9575 2023-04-30 17:28:28.000000 craiyon.py-1.0.0/craiyon/craiyon.py
+-rw-rw-rw-   0        0        0     1599 2023-03-13 16:55:35.000000 craiyon.py-1.0.0/craiyon/craiyon_utils.py
+-rw-rw-rw-   0        0        0     2103 2023-04-30 17:23:43.000000 craiyon.py-1.0.0/craiyon/templates.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:15:04.494059 craiyon.py-1.0.0/craiyon.py.egg-info/
+-rw-rw-rw-   0        0        0    10541 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 18:15:04.000000 craiyon.py-1.0.0/craiyon.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-04-30 18:15:04.497057 craiyon.py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-04-30 17:02:13.000000 craiyon.py-1.0.0/setup.py
```

### Comparing `craiyon.py-0.3.0/LICENSE` & `craiyon.py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craiyon.py-0.3.0/PKG-INFO` & `craiyon.py-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craiyon.py
-Version: 0.3.0
+Version: 1.0.0
 Summary: API Wrapper for craiyon.com (DAL-E-MINI). Generate awesome images from text tokens.
 Home-page: https://github.com/FireHead90544/craiyon.py
 Author: Rudransh Joshi
 Author-email: rudranshjoshi1806@gmail.com
 License: Apache License 2.0
 Project-URL: Issue tracker, https://github.com/FireHead90544/craiyon.py/issues
 Platform: any
@@ -48,60 +48,64 @@
 
 ```shell
   pip install -U craiyon.py
 ```
 
 Or just manually clone the repository and build the wheel
 
-## Craiyon v2 vs v1
+## Versioning
 
-The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v2.
-A quick comparison between the two is given below:
+The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v3.
+The v2 model has been removed from the api, so the model class around it is also deprecated by commenting it out.
+A quick comparison is given below:
 
 | Model | Speed | Quality | API_URL | Import Name |
 |:-----:|:-----:|:-------:|:-------:|:-----------:|
-| v2 | Faster (<1m) | Good | https://api.craiyon.com/draw | Craiyon |
-| v1 | Slower (~1.5m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
+| v3 | Fast (~50s) | Best | https://api.craiyon.com/v3 | Craiyon |
+| v2 (Removed) | Fastest (<45s) | Good | https://api.craiyon.com/draw | CraiyonV2 |
+| v1 | Slow (~1m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
 
 
 ## Usage / Examples
 
 ### 
 
 **Generate and save the images**
 
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
-result = generator.generate("Photorealistic image of shrek eating earth")
+result = generator.generate("Photorealistic image of shrek eating earth", negative_prompt="spoon", model_type="art")
+print(result.description) # Description about the generated images # >>> Shrek devouring planet Earth with a sinister grin
 result.save_images() # Saves the generated images to 'current working directory/generated', you can also provide a custom path
 ```
-![image](https://user-images.githubusercontent.com/55452780/181876989-38872ca2-c3d5-4891-9bd4-cf4e4b26b91e.png)
+![image](https://user-images.githubusercontent.com/55452780/235368810-bbeda283-d0d5-43b4-a1af-d5fdeab7cadb.png)
 
 **Use the images in your code without saving**
 
 ```py
 from craiyon import Craiyon, craiyon_utils
 from PIL import Image # pip install pillow
 from io import BytesIO
 import base64
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Professional photo of Obama flashing a flag with his last name") # Generates 9 images by default and you cannot change that
+print(result.description) # >>> Obama holding up a flag with his last name, smiling confidently
 images = craiyon_utils.encode_base64(result.images)
 for i in images:
     image = Image.open(BytesIO(base64.decodebytes(i)))
     # To convert the .webp images to .jpg or .png, you can proceed like this
     # image.convert("RGB").save("image.jpg", "JPEG") # For ".jpg" images
     # image.convert("RGBA").save("image.png", "PNG") # For ".png" images
     
     # Use the PIL's Image object as per your needs
 ```
-![image](https://user-images.githubusercontent.com/55452780/181877028-740bee12-432d-4019-b74e-a17f53b79987.png)
+![image](https://user-images.githubusercontent.com/55452780/235368949-05e4d215-5f29-4aea-a059-e6ad62b1ee2c.png)
 
 **Just get the Direct Image URLs**
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Photorealistic image of shrek eating earth")
@@ -169,39 +173,54 @@
         
     await ctx.reply(files=images1) # Reply to the user with all 9 images in 1 message
         
 
 bot.run("your_token_here")
 ```
 
+## Generation parameters
+
+```py
+# These parameters are only supported by the v3 model
+from craiyon import Craiyon
+generator = Craiyon()
+result = generator.generate("prompt here", negative_prompt="cap", model_type="art") # The negative prompt and model type are optional parameters
+# Negative prompt helps filtering out certain things from the images that will be generated, defaults to empty string ""
+# Model type can be "art", "drawing", "photo" and "none", defaults to "none". It does as it's name suggests.
+
+# result.description returns a brief description generated by craiyon about the generated images
+# result.images returns the list of images generated (v3 returns the image links, v1 returns the base64 image data)
+# result.model returns the model version
+```
+
 ## Specify custom tokens/model versions
 
 ```py
 
-from craiyon import Craiyon # Importing the v2 model
+from craiyon import Craiyon # Importing the v3 model
 
 # api_token and model_version are not required, but recommended
 generator = Craiyon(api_token="your-token-here", model_version="api-model-version")
 
 # ...rest is the same stuff as above
 ```
 
 ### api_token
 * If you bought a paid subscription to Craiyon.com, you would know that the watermark is removed. If you wish to have the watermark removed from the generated images in your application as well, you can specify a token here. 
 * To find your token: Open Google Chrome, go to craiyon.com (make sure you're logged in), Press F12, go to the Network tab, make sure the record button looks like a red circle at the top-left. Put your prompt in the text box and press the orange "Draw" button. Two "draw" items should appear on the left, under "name". One of them will have a "Payload" tab next to "Headers" and "Preview", as well as above "General". Click it, and your token is listed there.
 
 ### model_version
 * Since Craiyon is still training their V2 model, it is improving every day. We recommend putting your own model version here to get the newest and best model they have at the moment.
-* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument for the generate() function as a string and you're ready!
+* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument while instantiating the `Craiyon` class and you're ready!
 * While this is recommended, it is not required. If you do not pass a custom model version, this value will automatically default to "35s5hfwn9n78gb06", which is Craiyon's newest model as of March 10, 2023.
 
 ## Backwards Compatibility
 This library is fully backwards-compatible with older versions.
 
-If you were previously using this library before we added support for Craiyon's V2 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V2 model by reading the code samples above.
+If you were previously using this library before we added support for Craiyon's V3 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V3 model by reading the code samples above. Please note that the v2 model used to work earlier, but Craiyon completely removed their v2 model from the api and there are no traces of it left, so we currently removed the CraiyonV2 class. Please use either the v1 or v3 model instead.
 
 
 ## Todo
 
 None!
 
 ## Contributing
```

### Comparing `craiyon.py-0.3.0/README.md` & `craiyon.py-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,60 +35,64 @@
 
 ```shell
   pip install -U craiyon.py
 ```
 
 Or just manually clone the repository and build the wheel
 
-## Craiyon v2 vs v1
+## Versioning
 
-The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v2.
-A quick comparison between the two is given below:
+The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v3.
+The v2 model has been removed from the api, so the model class around it is also deprecated by commenting it out.
+A quick comparison is given below:
 
 | Model | Speed | Quality | API_URL | Import Name |
 |:-----:|:-----:|:-------:|:-------:|:-----------:|
-| v2 | Faster (<1m) | Good | https://api.craiyon.com/draw | Craiyon |
-| v1 | Slower (~1.5m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
+| v3 | Fast (~50s) | Best | https://api.craiyon.com/v3 | Craiyon |
+| v2 (Removed) | Fastest (<45s) | Good | https://api.craiyon.com/draw | CraiyonV2 |
+| v1 | Slow (~1m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
 
 
 ## Usage / Examples
 
 ### 
 
 **Generate and save the images**
 
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
-result = generator.generate("Photorealistic image of shrek eating earth")
+result = generator.generate("Photorealistic image of shrek eating earth", negative_prompt="spoon", model_type="art")
+print(result.description) # Description about the generated images # >>> Shrek devouring planet Earth with a sinister grin
 result.save_images() # Saves the generated images to 'current working directory/generated', you can also provide a custom path
 ```
-![image](https://user-images.githubusercontent.com/55452780/181876989-38872ca2-c3d5-4891-9bd4-cf4e4b26b91e.png)
+![image](https://user-images.githubusercontent.com/55452780/235368810-bbeda283-d0d5-43b4-a1af-d5fdeab7cadb.png)
 
 **Use the images in your code without saving**
 
 ```py
 from craiyon import Craiyon, craiyon_utils
 from PIL import Image # pip install pillow
 from io import BytesIO
 import base64
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Professional photo of Obama flashing a flag with his last name") # Generates 9 images by default and you cannot change that
+print(result.description) # >>> Obama holding up a flag with his last name, smiling confidently
 images = craiyon_utils.encode_base64(result.images)
 for i in images:
     image = Image.open(BytesIO(base64.decodebytes(i)))
     # To convert the .webp images to .jpg or .png, you can proceed like this
     # image.convert("RGB").save("image.jpg", "JPEG") # For ".jpg" images
     # image.convert("RGBA").save("image.png", "PNG") # For ".png" images
     
     # Use the PIL's Image object as per your needs
 ```
-![image](https://user-images.githubusercontent.com/55452780/181877028-740bee12-432d-4019-b74e-a17f53b79987.png)
+![image](https://user-images.githubusercontent.com/55452780/235368949-05e4d215-5f29-4aea-a059-e6ad62b1ee2c.png)
 
 **Just get the Direct Image URLs**
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Photorealistic image of shrek eating earth")
@@ -156,39 +160,54 @@
         
     await ctx.reply(files=images1) # Reply to the user with all 9 images in 1 message
         
 
 bot.run("your_token_here")
 ```
 
+## Generation parameters
+
+```py
+# These parameters are only supported by the v3 model
+from craiyon import Craiyon
+generator = Craiyon()
+result = generator.generate("prompt here", negative_prompt="cap", model_type="art") # The negative prompt and model type are optional parameters
+# Negative prompt helps filtering out certain things from the images that will be generated, defaults to empty string ""
+# Model type can be "art", "drawing", "photo" and "none", defaults to "none". It does as it's name suggests.
+
+# result.description returns a brief description generated by craiyon about the generated images
+# result.images returns the list of images generated (v3 returns the image links, v1 returns the base64 image data)
+# result.model returns the model version
+```
+
 ## Specify custom tokens/model versions
 
 ```py
 
-from craiyon import Craiyon # Importing the v2 model
+from craiyon import Craiyon # Importing the v3 model
 
 # api_token and model_version are not required, but recommended
 generator = Craiyon(api_token="your-token-here", model_version="api-model-version")
 
 # ...rest is the same stuff as above
 ```
 
 ### api_token
 * If you bought a paid subscription to Craiyon.com, you would know that the watermark is removed. If you wish to have the watermark removed from the generated images in your application as well, you can specify a token here. 
 * To find your token: Open Google Chrome, go to craiyon.com (make sure you're logged in), Press F12, go to the Network tab, make sure the record button looks like a red circle at the top-left. Put your prompt in the text box and press the orange "Draw" button. Two "draw" items should appear on the left, under "name". One of them will have a "Payload" tab next to "Headers" and "Preview", as well as above "General". Click it, and your token is listed there.
 
 ### model_version
 * Since Craiyon is still training their V2 model, it is improving every day. We recommend putting your own model version here to get the newest and best model they have at the moment.
-* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument for the generate() function as a string and you're ready!
+* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument while instantiating the `Craiyon` class and you're ready!
 * While this is recommended, it is not required. If you do not pass a custom model version, this value will automatically default to "35s5hfwn9n78gb06", which is Craiyon's newest model as of March 10, 2023.
 
 ## Backwards Compatibility
 This library is fully backwards-compatible with older versions.
 
-If you were previously using this library before we added support for Craiyon's V2 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V2 model by reading the code samples above.
+If you were previously using this library before we added support for Craiyon's V3 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V3 model by reading the code samples above. Please note that the v2 model used to work earlier, but Craiyon completely removed their v2 model from the api and there are no traces of it left, so we currently removed the CraiyonV2 class. Please use either the v1 or v3 model instead.
 
 
 ## Todo
 
 None!
 
 ## Contributing
```

### Comparing `craiyon.py-0.3.0/craiyon/craiyon_utils.py` & `craiyon.py-1.0.0/craiyon/craiyon_utils.py`

 * *Files identical despite different names*

### Comparing `craiyon.py-0.3.0/craiyon.py.egg-info/PKG-INFO` & `craiyon.py-1.0.0/craiyon.py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craiyon.py
-Version: 0.3.0
+Version: 1.0.0
 Summary: API Wrapper for craiyon.com (DAL-E-MINI). Generate awesome images from text tokens.
 Home-page: https://github.com/FireHead90544/craiyon.py
 Author: Rudransh Joshi
 Author-email: rudranshjoshi1806@gmail.com
 License: Apache License 2.0
 Project-URL: Issue tracker, https://github.com/FireHead90544/craiyon.py/issues
 Platform: any
@@ -48,60 +48,64 @@
 
 ```shell
   pip install -U craiyon.py
 ```
 
 Or just manually clone the repository and build the wheel
 
-## Craiyon v2 vs v1
+## Versioning
 
-The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v2.
-A quick comparison between the two is given below:
+The api wrapper has separate classes revolving around each model, i.e, the Craiyon v1 and v3.
+The v2 model has been removed from the api, so the model class around it is also deprecated by commenting it out.
+A quick comparison is given below:
 
 | Model | Speed | Quality | API_URL | Import Name |
 |:-----:|:-----:|:-------:|:-------:|:-----------:|
-| v2 | Faster (<1m) | Good | https://api.craiyon.com/draw | Craiyon |
-| v1 | Slower (~1.5m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
+| v3 | Fast (~50s) | Best | https://api.craiyon.com/v3 | Craiyon |
+| v2 (Removed) | Fastest (<45s) | Good | https://api.craiyon.com/draw | CraiyonV2 |
+| v1 | Slow (~1m) | Average | https://backend.craiyon.com/generate | CraiyonV1 |
 
 
 ## Usage / Examples
 
 ### 
 
 **Generate and save the images**
 
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
-result = generator.generate("Photorealistic image of shrek eating earth")
+result = generator.generate("Photorealistic image of shrek eating earth", negative_prompt="spoon", model_type="art")
+print(result.description) # Description about the generated images # >>> Shrek devouring planet Earth with a sinister grin
 result.save_images() # Saves the generated images to 'current working directory/generated', you can also provide a custom path
 ```
-![image](https://user-images.githubusercontent.com/55452780/181876989-38872ca2-c3d5-4891-9bd4-cf4e4b26b91e.png)
+![image](https://user-images.githubusercontent.com/55452780/235368810-bbeda283-d0d5-43b4-a1af-d5fdeab7cadb.png)
 
 **Use the images in your code without saving**
 
 ```py
 from craiyon import Craiyon, craiyon_utils
 from PIL import Image # pip install pillow
 from io import BytesIO
 import base64
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Professional photo of Obama flashing a flag with his last name") # Generates 9 images by default and you cannot change that
+print(result.description) # >>> Obama holding up a flag with his last name, smiling confidently
 images = craiyon_utils.encode_base64(result.images)
 for i in images:
     image = Image.open(BytesIO(base64.decodebytes(i)))
     # To convert the .webp images to .jpg or .png, you can proceed like this
     # image.convert("RGB").save("image.jpg", "JPEG") # For ".jpg" images
     # image.convert("RGBA").save("image.png", "PNG") # For ".png" images
     
     # Use the PIL's Image object as per your needs
 ```
-![image](https://user-images.githubusercontent.com/55452780/181877028-740bee12-432d-4019-b74e-a17f53b79987.png)
+![image](https://user-images.githubusercontent.com/55452780/235368949-05e4d215-5f29-4aea-a059-e6ad62b1ee2c.png)
 
 **Just get the Direct Image URLs**
 ```py
 from craiyon import Craiyon
 
 generator = Craiyon() # Instantiates the api wrapper
 result = generator.generate("Photorealistic image of shrek eating earth")
@@ -169,39 +173,54 @@
         
     await ctx.reply(files=images1) # Reply to the user with all 9 images in 1 message
         
 
 bot.run("your_token_here")
 ```
 
+## Generation parameters
+
+```py
+# These parameters are only supported by the v3 model
+from craiyon import Craiyon
+generator = Craiyon()
+result = generator.generate("prompt here", negative_prompt="cap", model_type="art") # The negative prompt and model type are optional parameters
+# Negative prompt helps filtering out certain things from the images that will be generated, defaults to empty string ""
+# Model type can be "art", "drawing", "photo" and "none", defaults to "none". It does as it's name suggests.
+
+# result.description returns a brief description generated by craiyon about the generated images
+# result.images returns the list of images generated (v3 returns the image links, v1 returns the base64 image data)
+# result.model returns the model version
+```
+
 ## Specify custom tokens/model versions
 
 ```py
 
-from craiyon import Craiyon # Importing the v2 model
+from craiyon import Craiyon # Importing the v3 model
 
 # api_token and model_version are not required, but recommended
 generator = Craiyon(api_token="your-token-here", model_version="api-model-version")
 
 # ...rest is the same stuff as above
 ```
 
 ### api_token
 * If you bought a paid subscription to Craiyon.com, you would know that the watermark is removed. If you wish to have the watermark removed from the generated images in your application as well, you can specify a token here. 
 * To find your token: Open Google Chrome, go to craiyon.com (make sure you're logged in), Press F12, go to the Network tab, make sure the record button looks like a red circle at the top-left. Put your prompt in the text box and press the orange "Draw" button. Two "draw" items should appear on the left, under "name". One of them will have a "Payload" tab next to "Headers" and "Preview", as well as above "General". Click it, and your token is listed there.
 
 ### model_version
 * Since Craiyon is still training their V2 model, it is improving every day. We recommend putting your own model version here to get the newest and best model they have at the moment.
-* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument for the generate() function as a string and you're ready!
+* To get the model version, follow the steps for the api_token listed above, except copy the "version" instead of the "token". Then, just pass it in as an argument while instantiating the `Craiyon` class and you're ready!
 * While this is recommended, it is not required. If you do not pass a custom model version, this value will automatically default to "35s5hfwn9n78gb06", which is Craiyon's newest model as of March 10, 2023.
 
 ## Backwards Compatibility
 This library is fully backwards-compatible with older versions.
 
-If you were previously using this library before we added support for Craiyon's V2 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V2 model by reading the code samples above.
+If you were previously using this library before we added support for Craiyon's V3 model and you wish to continue using the old V1 model, simply change the name of the class `Craiyon` to `CraiyonV1`! Otherwise, you can update your application to the V3 model by reading the code samples above. Please note that the v2 model used to work earlier, but Craiyon completely removed their v2 model from the api and there are no traces of it left, so we currently removed the CraiyonV2 class. Please use either the v1 or v3 model instead.
 
 
 ## Todo
 
 None!
 
 ## Contributing
```

### Comparing `craiyon.py-0.3.0/setup.py` & `craiyon.py-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(name='craiyon.py',
-      version='0.3.0',
+      version='1.0.0',
       description='API Wrapper for craiyon.com (DAL-E-MINI). Generate awesome images from text tokens.',
       long_description=readme,
       long_description_content_type="text/markdown",
       url='https://github.com/FireHead90544/craiyon.py',
       project_urls={
         "Issue tracker": "https://github.com/FireHead90544/craiyon.py/issues",
       },
```

