# Comparing `tmp/AIsketcher-0.0.0.1-py3-none-any.whl.zip` & `tmp/AIsketcher-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3101 bytes, number of entries: 6
--rw-r--r--  2.0 unx      442 b- defN 23-May-19 07:55 AIsketcher/__init__.py
--rw-r--r--  2.0 unx     2776 b- defN 23-May-19 07:38 AIsketcher/modelPipe.py
--rw-r--r--  2.0 unx     1094 b- defN 23-May-19 07:56 AIsketcher-0.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 07:56 AIsketcher-0.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-19 07:56 AIsketcher-0.0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      476 b- defN 23-May-19 07:56 AIsketcher-0.0.0.1.dist-info/RECORD
-6 files, 4891 bytes uncompressed, 2237 bytes compressed:  54.3%
+Zip file size: 3138 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      466 b- defN 23-May-19 08:06 AIsketcher/__init__.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-May-19 09:35 AIsketcher/modelPipe.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-May-19 09:39 AIsketcher-0.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 09:39 AIsketcher-0.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-19 09:39 AIsketcher-0.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      476 b- defN 23-May-19 09:39 AIsketcher-0.0.0.2.dist-info/RECORD
+6 files, 5107 bytes uncompressed, 2274 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: AIsketcher/__init__.py
 Comment: 
 
 Filename: AIsketcher/modelPipe.py
 Comment: 
 
-Filename: AIsketcher-0.0.0.1.dist-info/METADATA
+Filename: AIsketcher-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: AIsketcher-0.0.0.1.dist-info/WHEEL
+Filename: AIsketcher-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: AIsketcher-0.0.0.1.dist-info/top_level.txt
+Filename: AIsketcher-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: AIsketcher-0.0.0.1.dist-info/RECORD
+Filename: AIsketcher-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AIsketcher/__init__.py

```diff
@@ -8,15 +8,16 @@
 for dependency in hard_dependencies:
     try:
         __import__(dependency)
     except ImportError as e:
         missing_dependencies.append(f"{dependency}: {e}")
 
 from AIsketcher.modelPipe import (
-    img2img
+    img2img,
+    translate_language
 )
 
 #__all__ = ["get_cer",
 #           "get_wer"]
```

## AIsketcher/modelPipe.py

```diff
@@ -14,15 +14,15 @@
     default_prompt = "(8k, best quality, masterpiece:1.2), (realistic, photo-realistic:1.37), ultra-detailed,"
     negative_prompt = "NSFW, lowres, ((bad anatomy)), ((bad hands)), text, missing finger, extra digits, fewer digits, blurry, ((mutated hands and fingers)), (poorly drawn face), ((mutation)), ((deformed face)), (ugly), ((bad proportions)), ((extra limbs)), extra face, (double head), (extra head), ((extra feet)), monster, logo, cropped, worst quality, low quality, normal quality, jpeg, humpbacked, long body, long neck, ((jpeg artifacts))"
 
     # resize image for fitting stable diffusion 800 x 800
     res_img = resize_image(img_path,800)
     np_image = np.array(res_img)
 
-    #Prompt Translate
+    #prompt Translate
     if trans_info is not None :
         input_prompt = default_prompt + translate_language(prompt, trans_info)
     else:
         input_prompt = default_prompt + prompt
 
 
     canny_image = cv2.Canny(np_image, low, high)
@@ -34,26 +34,28 @@
         input_prompt,
         negative_prompt=negative_prompt,
         num_inference_steps=num_steps,
         guidance_scale=guidance_scale,
         generator=torch.manual_seed(seed),
         image=canny_image
     ).images[0]
-
+    # resizing to original image size
     resized_out_image = out_image.resize(image.size)
     return image, canny_image, resized_out_image
 
 def resize_image(image_path, pixels):
   image = Image.open(image_path)
   image.thumbnail((pixels,pixels), Image.ANTIALIAS)
   return image
 
 def translate_language(input, trans_info):
-    if trans_info.iam_access :
-        translate = boto3.client(service_name='translate', region_name=trans_info.region_name, use_ssl=True)
-    elif trans_info.iam_access is False:
-        translate = boto3.client(service_name='translate', region_name=trans_info.region_name, use_ssl=True, aws_access_key_id=trans_info.aws_access_key_id, aws_secret_access_key=trans_info.aws_secret_access_key)
+    if 'iam_access' in trans_info and trans_info['iam_access']:
+        translate = boto3.client(service_name='translate', region_name=trans_info['region_name'], use_ssl=True)
+    elif 'iam_access' in trans_info and not trans_info['iam_access']:
+        translate = boto3.client(service_name='translate', region_name=trans_info['region_name'], use_ssl=True,
+                                 aws_access_key_id=trans_info['aws_access_key_id'], aws_secret_access_key=trans_info['aws_secret_access_key'])
     else:
-        translate = boto3.client(service_name='translate', region_name=trans_info.region_name, use_ssl=True, aws_access_key_id=trans_info.aws_access_key_id, aws_secret_access_key=trans_info.aws_secret_access_key)
+        translate = boto3.client(service_name='translate', region_name=trans_info['region_name'], use_ssl=True,
+                                 aws_access_key_id=trans_info['aws_access_key_id'], aws_secret_access_key=trans_info['aws_secret_access_key'])
 
-    prompt = translate.translate_text(Text=input, SourceLanguageCode=trans_info.SourceLanguageCode, TargetLanguageCode=trans_info.TargetLanguageCode)['TranslatedText']
+    prompt = translate.translate_text(Text=input, SourceLanguageCode=trans_info['SourceLanguageCode'], TargetLanguageCode=trans_info['TargetLanguageCode'])['TranslatedText']
     return prompt
```

## Comparing `AIsketcher-0.0.0.1.dist-info/METADATA` & `AIsketcher-0.0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: AIsketcher
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Text-to-image generation using Huggingface stable diffusion ControlNet conditioning and AWS Translate's prompt translation function package
 Home-page: https://github.com/hyeonsangjeon/AIsketcher
 Author: hyeonsangjeon
 Author-email: wingnut0310@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-contrib-python
 Requires-Dist: diffusers
 Requires-Dist: transformers
+Requires-Dist: boto3
 
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://raw.githubusercontent.com/hyeonsangjeon/youtube-dl-nas/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/ai-sketcher)](https://pepy.tech/project/ai-sketcher)
 #ai-sketcher
 
 
 
@@ -25,15 +26,14 @@
 
 ```text
 
 ```
 ```python
 
 
-# prints: wer -> 0.0
 ```
 
 
 
 ### References 
 - `[1]`.
 - `[2]`.
```

