# Comparing `tmp/AL_Khatma_lib-1.0.0.tar.gz` & `tmp/AL_Khatma_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AL_Khatma_lib-1.0.0.tar", last modified: Sat Apr 22 09:53:01 2023, max compression
+gzip compressed data, was "AL_Khatma_lib-1.1.1.tar", last modified: Sun Apr 30 03:25:05 2023, max compression
```

## Comparing `AL_Khatma_lib-1.0.0.tar` & `AL_Khatma_lib-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-22 09:53:01.590073 AL_Khatma_lib-1.0.0/
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-04-16 18:02:45.000000 AL_Khatma_lib-1.0.0/LICENSE
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    29395 2023-04-22 09:53:01.590073 AL_Khatma_lib-1.0.0/PKG-INFO
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)    28884 2023-04-19 16:24:13.000000 AL_Khatma_lib-1.0.0/README.md
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      585 2023-04-22 09:52:01.000000 AL_Khatma_lib-1.0.0/pyproject.toml
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-04-22 09:53:01.590073 AL_Khatma_lib-1.0.0/setup.cfg
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-22 09:53:01.570072 AL_Khatma_lib-1.0.0/src/
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-22 09:53:01.590073 AL_Khatma_lib-1.0.0/src/AL_Khatma/
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     2426 2023-04-19 17:57:28.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma/__init__.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     7655 2023-04-19 17:57:18.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma/khatma.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)      637 2023-04-18 19:48:42.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma/log.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)    14597 2023-04-19 17:57:34.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma/quran.py
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-22 09:53:01.590073 AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    29395 2023-04-22 09:53:01.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      290 2023-04-22 09:53:01.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-04-22 09:53:01.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-04-22 09:53:01.000000 AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/top_level.txt
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-04-16 18:02:45.000000 AL_Khatma_lib-1.1.1/LICENSE
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    30117 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/PKG-INFO
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)    29605 2023-04-30 02:59:13.000000 AL_Khatma_lib-1.1.1/README.md
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      585 2023-04-30 03:24:31.000000 AL_Khatma_lib-1.1.1/pyproject.toml
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/setup.cfg
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.806463 AL_Khatma_lib-1.1.1/src/
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/src/AL_Khatma/
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1035 2023-04-30 03:24:36.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/__init__.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2746 2023-04-30 03:13:55.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/cheak.py
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)     7657 2023-04-30 02:51:02.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/khatma.py
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-04-30 02:22:42.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/log.py
+-rw-r--r--   0 oaokm     (1000) oaokm     (1000)    14667 2023-04-30 02:36:52.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/quran.py
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    30117 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      313 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/top_level.txt
```

### Comparing `AL_Khatma_lib-1.0.0/LICENSE` & `AL_Khatma_lib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-1.0.0/PKG-INFO` & `AL_Khatma_lib-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AL_Khatma_lib
-Version: 1.0.0
+Version: 1.1.1
 Summary: A library Specialized About Islamic
 Author-email: Osamah Awadh <osamahawadh01@gmail.com>
 Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
 Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,30 +29,30 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#التعامل_مع_المكتبة">التعامل مع المكتبة</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#المصادر">المصادر</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/UPDATE.md">التحديثات</a>
+  <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
 </p>
 
-![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange)
---| --|
+![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI](https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://img.shields.io/github/repo-size/oaokm/AL-Khatma)
+--| --| -- | --| 
 
 
 ## **بيان**
 في يوم الثالث من أبريل من عام 2023 الموافق الثاني عشر من رمضان لعام 1444 هـ في هذا اليوم بدأت الفكرة وبعدها قمت بتطبيق الفكرة وبناء أول API لي.
 
 وفي اليوم التاسع عشر من أبريل من عام 2023 الموافق الثامن والعشرون من رمضان لعام 1444 هـ وبتوفيق من الله لقد أنهيت النسخة الأولى من هذا المشروع ولله الحمد.
 وأشكر أخي وأختي اللذانِ دعمني وحفزاني لأتمّ هذا المشروع ❤️
 
 
 ## فكرة_الختمة
-**الختمة** هو مشروع مفتوح المصدر تم بناءه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
+**الختمة** هو مشروع مفتوح المصدر تم بنائه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
 وتتمتع المكتبة بعدّة حزمّ، وأهمها:
 
 * **حزمة القرأن الكريم**:.
   * استخراج جميع الأيات القرآنية وكاقة معلوماتها.
   * إمكانية البحث عن الأيات الكريمة.
   * إمكانية تحميل صور صفحات القرآن الكريم.
   * المكتبة مزودة بعدّة لغات. ومنها:
@@ -89,21 +89,31 @@
 
 **الطريقة الثانية**: تحميلها من المتصفح بصيغة ملف مضعوط `.zip`
 
 
 ### التحميل عن طريق **pypi**
 
 ```sh
-$ pip install AL-Khatma
+$ pip install AL-Khatma-lib
 ```
 **أو**
 ```sh
-$ pip3 install AL-Khatma
+$ pip3 install AL-Khatma-lib
 ```
 
+#### تحميل الملفات الهامة
+الملفات الهامة هي ملف اللغة وبعض الملفات التي تساعد عمل البرنامج، بكتابة الأمر التالي:
+
+```py
+>>> import AL_Khatma
+>>> AL_Khatma.Download_DATA()
+```
+وأنتظر إلى أن تتم عملية التحميل بنجاح
+
+
 ## **التعامل_مع_المكتبة**
 
 حاليا هنالك حزمتين، وهي:
 
 * حزمة القرآن الكريم
 * حزمة تختيم القرآن الكريم
 
@@ -366,22 +376,23 @@
 
 > **معلومة مساعدة**: خاصية `return_imge` يمكن أستخدامها في بناء البوتات، كبوت في التليجرام مثلًا. بدلًا من أن تخزم محتوى الصورة في القرص الصلب، يمكون في متغير قائمة (list).
 
 > **ملاحظة مهمة(1)**: في حال عدم إتصالك بالإنترنت فإن هذه الميزة لن تعمل، ويرجى التحقق من إتصالك للإنترنت.
 
 > **ملاحظة مهمة(2)**: خيار `type` هو نوع أو شكل الصفحة التي تريدها، وحاليا هنالك فقط شكلان فقط، ويمكن الاطلاع عليه [بالضغط هنا لرؤية الخيارات المتاح](https://github.com/oaokm/AL-Khatma/blob/main/DATA/quran_books.json).
 
+> **ملاحظة مهمة(3)**: عندما تضع المسار التي ستنزل فيها الصور يجب أن تضع المسار الكامل كما هو موضح في المثال
 
 طريقة كتابة الأمر كالتالي:
 
 ```py
 >>> from AL_Khatma.quran import Quran
 >>> quran = Quran() # استدعاء الكائن
->>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
-# Download Pages From Quran ... 
+>>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
+# Download Pages From Quran | [/home/oaokm/Pictures/Quran] 
 100%|███████████████████████████████████████| 3/3 [00:01<00:00,  1.69it/s]
 ```
 <p align="center">
   <img src="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/Pictures/Screenshot_for_page_pic.png" alt="picture_screenshot">
 </p>
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 1.0.0 Summary: A library
+Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 1.1.1 Summary: A library
 Specialized About Islamic Author-email: Osamah Awadh
 gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
 URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
                               Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª
 ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://
-img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) --| --| ##
+img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
+(https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
+img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
 Ø§ÙÙÙØ±Ø© ÙØ¨ÙØ§Ø¡ Ø£ÙÙ API ÙÙ. ÙÙÙ Ø§ÙÙÙÙ Ø§ÙØªØ§Ø³Ø¹ Ø¹Ø´Ø±
 ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ ÙØ§ÙØ¹Ø´Ø±ÙÙ
 ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙØ¨ØªÙÙÙÙ ÙÙ Ø§ÙÙÙ ÙÙØ¯
 Ø£ÙÙÙØª Ø§ÙÙØ³Ø®Ø© Ø§ÙØ£ÙÙÙ ÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ ÙÙÙÙ
 Ø§ÙØ­ÙØ¯. ÙØ£Ø´ÙØ± Ø£Ø®Ù ÙØ£Ø®ØªÙ Ø§ÙÙØ°Ø§ÙÙ Ø¯Ø¹ÙÙÙ
 ÙØ­ÙØ²Ø§ÙÙ ÙØ£ØªÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ â¤ï¸ ## ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©
-**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¡Ù
+**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¦Ù
 ÙØªÙØ­ÙØ¯ Ø§ÙÙØªØ¹ÙÙØ§Øª Ø§ÙÙØªØ¹ÙÙØ© Ø¨Ø§ÙØ¯ÙØ§ÙØ©
 Ø§ÙØ¥Ø³ÙØ§ÙÙØ© (ÙØ§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙØ ÙØ§ÙØ£Ø­Ø§Ø¯ÙØ«
 Ø§ÙØ´Ø±ÙÙØ© Ø ÙØ§ÙØªÙØ³ÙØ±Ø ÙØ§ÙØ£Ø¯Ø¹ÙØ©Ø ÙØºÙØ±ÙØ§) ÙÙ
 ÙÙØ§Ù ÙØ§Ø­Ø¯. ÙØªØªÙØªØ¹ Ø§ÙÙÙØªØ¨Ø© Ø¨Ø¹Ø¯ÙØ© Ø­Ø²ÙÙØ
 ÙØ£ÙÙÙØ§: * **Ø­Ø²ÙØ© Ø§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙ**:. * Ø§Ø³ØªØ®Ø±Ø§Ø¬
 Ø¬ÙÙØ¹ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±Ø¢ÙÙØ© ÙÙØ§ÙØ© ÙØ¹ÙÙÙØ§ØªÙØ§. *
 Ø¥ÙÙØ§ÙÙØ© Ø§ÙØ¨Ø­Ø« Ø¹Ù Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ©. * Ø¥ÙÙØ§ÙÙØ©
@@ -42,36 +44,40 @@
 Ø¹ÙÙØ§ ÙÙ Ø§ÙØ¥ØµØ¯Ø§Ø±Ø§Øª Ø§ÙÙØ§Ø¯ÙØ© -Ø¥Ù Ø´Ø§Ø¡ Ø§ÙÙÙ- ##
 **ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©** ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù Ø·Ø±ÙÙ **Github**
 **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ£ÙÙÙ**: Ø¹Ù Ø·Ø±ÙÙ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±: *
 Ø¥ÙØ´Ø§Ø¡ ÙÙÙ Ø¨Ø£Ø³Ù **`AL_Khatma`** * Ø§ÙØªØ­ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±
 ÙØ£ÙØªØ¨ ÙØ°Ø§ Ø§ÙØ£ÙØ±: ```sh S git clone https://github.com/oaokm/AL-
 Khatma ``` **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ«Ø§ÙÙØ©**: ØªØ­ÙÙÙÙØ§ ÙÙ
 Ø§ÙÙØªØµÙØ­ Ø¨ØµÙØºØ© ÙÙÙ ÙØ¶Ø¹ÙØ· `.zip` ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù
-Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma ``` **Ø£Ù** ```sh $ pip3
-install AL-Khatma ``` ## **Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§
-ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ *
-Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø±
-Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ
-Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§ ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma
->>> AL_Khatma.__version__ '1.0.0' ``` ### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬
-Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©** Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ
-Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ÙÙ `Quran
-().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ©
-Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list) ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯
-Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ© ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª
-Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§. ```py
-Quran.show_block_aya( self, verses_no:int, verses_number:list, orderly=False,
-): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§
-ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ© verses_no(int):
-Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number(list): ÙÙ
-Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ Ø¨ÙØªØ§Ø¨Ø©
-Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly(bool):
-Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ ÙÙÙÙ
-ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§ Ø³ÙØ±Ø©
-Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
+Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma-lib ``` **Ø£Ù** ```sh $ pip3
+install AL-Khatma-lib ``` #### ØªØ­ÙÙÙ Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ©
+Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ© ÙÙ ÙÙÙ Ø§ÙÙØºØ© ÙØ¨Ø¹Ø¶ Ø§ÙÙÙÙØ§Øª
+Ø§ÙØªÙ ØªØ³Ø§Ø¹Ø¯ Ø¹ÙÙ Ø§ÙØ¨Ø±ÙØ§ÙØ¬Ø Ø¨ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ±
+Ø§ÙØªØ§ÙÙ: ```py >>> import AL_Khatma >>> AL_Khatma.Download_DATA() ```
+ÙØ£ÙØªØ¸Ø± Ø¥ÙÙ Ø£Ù ØªØªÙ Ø¹ÙÙÙØ© Ø§ÙØªØ­ÙÙÙ Ø¨ÙØ¬Ø§Ø­ ##
+**Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§ ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ
+ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ * Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø©
+Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§
+ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma >>> AL_Khatma.__version__ '1.0.0' ```
+### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©**
+Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ÙÙ `Quran().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ
+Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list)
+ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯ Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ©
+ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§.
+```py Quran.show_block_aya( self, verses_no:int, verses_number:list,
+orderly=False, ): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ
+Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§ ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ©
+verses_no(int): Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number
+(list): ÙÙ Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ
+Ø¨ÙØªØ§Ø¨Ø© Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly
+(bool): Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ
+ÙÙÙÙ ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§
+Ø³ÙØ±Ø© Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
 Ø§ÙØ¨Ø±ÙØ§ÙØ¬ Ø³ÙØ¹ÙØ¯ ÙÙ 7 Ø¹ÙØ§ØµØ± Ø¯Ø§Ø®Ù Ø§ÙÙØ§Ø¦ÙØ©. ÙÙÙ
 Ø¹ÙØµØ± ÙØ­ØªÙÙ Ø¹ÙÙ ÙØ¹ÙÙÙØ§Øª ÙÙØ£ÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ±
 Ø§ÙÙØ§ÙÙØ³ (dict) ÙÙÙÙÙ Ø´ÙÙÙ ÙØ§ÙØªØ§ÙÙ: ```json // Form JSON
 File 'main.json' (Arabic + English) // { "ID": 1, "Name": "Ø§ÙÙÙØ§ØªÙØ­Ø©",
 "Transliteration": "Al-FÄtiá¸¥ah", "translation": "The Opener", "type":
 "meccan", "total_verses": 7, "verses_no": 1, "jozz": 1, "page": 1,
 "verses_number": 1, "line_start": 2, "line_end": 2, "verses_text":
@@ -329,19 +335,22 @@
 (list). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(1)**: ÙÙ Ø­Ø§Ù Ø¹Ø¯Ù Ø¥ØªØµØ§ÙÙ
 Ø¨Ø§ÙØ¥ÙØªØ±ÙØª ÙØ¥Ù ÙØ°Ù Ø§ÙÙÙØ²Ø© ÙÙ ØªØ¹ÙÙØ ÙÙØ±Ø¬Ù
 Ø§ÙØªØ­ÙÙ ÙÙ Ø¥ØªØµØ§ÙÙ ÙÙØ¥ÙØªØ±ÙØª. > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©
 (2)**: Ø®ÙØ§Ø± `type` ÙÙ ÙÙØ¹ Ø£Ù Ø´ÙÙ Ø§ÙØµÙØ­Ø© Ø§ÙØªÙ
 ØªØ±ÙØ¯ÙØ§Ø ÙØ­Ø§ÙÙØ§ ÙÙØ§ÙÙ ÙÙØ· Ø´ÙÙØ§Ù ÙÙØ·Ø ÙÙÙÙÙ
 Ø§ÙØ§Ø·ÙØ§Ø¹ Ø¹ÙÙÙ [Ø¨Ø§ÙØ¶ØºØ· ÙÙØ§ ÙØ±Ø¤ÙØ© Ø§ÙØ®ÙØ§Ø±Ø§Øª
 Ø§ÙÙØªØ§Ø­](https://github.com/oaokm/AL-Khatma/blob/main/DATA/
-quran_books.json). Ø·Ø±ÙÙØ© ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>>
-from AL_Khatma.quran import Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡
-Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures',
-'quran') # ÙØªØ§Ø¨Ø© Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages
-From Quran ...
+quran_books.json). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(3)**: Ø¹ÙØ¯ÙØ§ ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙØªÙ Ø³ØªÙØ²Ù ÙÙÙØ§ Ø§ÙØµÙØ± ÙØ¬Ø¨ Ø£Ù ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙÙØ§ÙÙ ÙÙØ§ ÙÙ ÙÙØ¶Ø­ ÙÙ Ø§ÙÙØ«Ø§Ù Ø·Ø±ÙÙØ©
+ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>> from AL_Khatma.quran import
+Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1,
+2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # ÙØªØ§Ø¨Ø©
+Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages From Quran | [/home/
+oaokm/Pictures/Quran]
 100%|âââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:01<00:00, 1.69it/s] ```
                              [picture_screenshot]
 ### ØªÙØ³ÙÙ ØµÙØ­Ø§Øª Ø§ÙÙØ±Ø¢Ù ÙÙ Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
 Ø§ÙÙØ±ÙÙØ Ø·Ø±ÙÙØ© ÙØªÙØ³ÙÙ Ø§ÙØµÙØ­Ø§Øª Ø¨ÙØ¯Ù ØªØ®ØªÙÙ
 Ø§ÙÙØ±Ø¢ÙØ ÙØªÙØ²ÙØ¹ Ø§ÙØªÙØ³ÙÙ Ø¹ÙÙ Ø§ÙØµÙØ­Ø§Øª. ```py >>>
 from AL_Khatma.khatma import khatma # Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙØ­Ø²ÙØ© >>> k =
```

### Comparing `AL_Khatma_lib-1.0.0/README.md` & `AL_Khatma_lib-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#التعامل_مع_المكتبة">التعامل مع المكتبة</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#المصادر">المصادر</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/UPDATE.md">التحديثات</a>
+  <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
 </p>
 
-![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange)
---| --|
+![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI](https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://img.shields.io/github/repo-size/oaokm/AL-Khatma)
+--| --| -- | --| 
 
 
 ## **بيان**
 في يوم الثالث من أبريل من عام 2023 الموافق الثاني عشر من رمضان لعام 1444 هـ في هذا اليوم بدأت الفكرة وبعدها قمت بتطبيق الفكرة وبناء أول API لي.
 
 وفي اليوم التاسع عشر من أبريل من عام 2023 الموافق الثامن والعشرون من رمضان لعام 1444 هـ وبتوفيق من الله لقد أنهيت النسخة الأولى من هذا المشروع ولله الحمد.
 وأشكر أخي وأختي اللذانِ دعمني وحفزاني لأتمّ هذا المشروع ❤️
 
 
 ## فكرة_الختمة
-**الختمة** هو مشروع مفتوح المصدر تم بناءه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
+**الختمة** هو مشروع مفتوح المصدر تم بنائه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
 وتتمتع المكتبة بعدّة حزمّ، وأهمها:
 
 * **حزمة القرأن الكريم**:.
   * استخراج جميع الأيات القرآنية وكاقة معلوماتها.
   * إمكانية البحث عن الأيات الكريمة.
   * إمكانية تحميل صور صفحات القرآن الكريم.
   * المكتبة مزودة بعدّة لغات. ومنها:
@@ -75,21 +75,31 @@
 
 **الطريقة الثانية**: تحميلها من المتصفح بصيغة ملف مضعوط `.zip`
 
 
 ### التحميل عن طريق **pypi**
 
 ```sh
-$ pip install AL-Khatma
+$ pip install AL-Khatma-lib
 ```
 **أو**
 ```sh
-$ pip3 install AL-Khatma
+$ pip3 install AL-Khatma-lib
 ```
 
+#### تحميل الملفات الهامة
+الملفات الهامة هي ملف اللغة وبعض الملفات التي تساعد عمل البرنامج، بكتابة الأمر التالي:
+
+```py
+>>> import AL_Khatma
+>>> AL_Khatma.Download_DATA()
+```
+وأنتظر إلى أن تتم عملية التحميل بنجاح
+
+
 ## **التعامل_مع_المكتبة**
 
 حاليا هنالك حزمتين، وهي:
 
 * حزمة القرآن الكريم
 * حزمة تختيم القرآن الكريم
 
@@ -352,22 +362,23 @@
 
 > **معلومة مساعدة**: خاصية `return_imge` يمكن أستخدامها في بناء البوتات، كبوت في التليجرام مثلًا. بدلًا من أن تخزم محتوى الصورة في القرص الصلب، يمكون في متغير قائمة (list).
 
 > **ملاحظة مهمة(1)**: في حال عدم إتصالك بالإنترنت فإن هذه الميزة لن تعمل، ويرجى التحقق من إتصالك للإنترنت.
 
 > **ملاحظة مهمة(2)**: خيار `type` هو نوع أو شكل الصفحة التي تريدها، وحاليا هنالك فقط شكلان فقط، ويمكن الاطلاع عليه [بالضغط هنا لرؤية الخيارات المتاح](https://github.com/oaokm/AL-Khatma/blob/main/DATA/quran_books.json).
 
+> **ملاحظة مهمة(3)**: عندما تضع المسار التي ستنزل فيها الصور يجب أن تضع المسار الكامل كما هو موضح في المثال
 
 طريقة كتابة الأمر كالتالي:
 
 ```py
 >>> from AL_Khatma.quran import Quran
 >>> quran = Quran() # استدعاء الكائن
->>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
-# Download Pages From Quran ... 
+>>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
+# Download Pages From Quran | [/home/oaokm/Pictures/Quran] 
 100%|███████████████████████████████████████| 3/3 [00:01<00:00,  1.69it/s]
 ```
 <p align="center">
   <img src="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/Pictures/Screenshot_for_page_pic.png" alt="picture_screenshot">
 </p>
 
 
@@ -405,8 +416,8 @@
 * [الأيات القرأنية باللغات الأخرى](https://github.com/risan/quran-json)
 * مصادر تحميل صفحات القرآن الكريم:
   * [الموقع الرسمي لأيات لجامعة الملك سعود](https://quran.ksu.edu.sa/ayat/)
   * [موقع الباحث القرآني](https://tafsir.app/)
 
 
 ## **الترخيص**
-ترخيص هو: إم آي تي ([MIT © Osamah Awadh](https://github.com/oaokm/AL-Khatma/blob/main/LICENSE))
+ترخيص هو: إم آي تي ([MIT © Osamah Awadh](https://github.com/oaokm/AL-Khatma/blob/main/LICENSE))
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
                               Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª
 ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://
-img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) --| --| ##
+img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
+(https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
+img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
 Ø§ÙÙÙØ±Ø© ÙØ¨ÙØ§Ø¡ Ø£ÙÙ API ÙÙ. ÙÙÙ Ø§ÙÙÙÙ Ø§ÙØªØ§Ø³Ø¹ Ø¹Ø´Ø±
 ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ ÙØ§ÙØ¹Ø´Ø±ÙÙ
 ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙØ¨ØªÙÙÙÙ ÙÙ Ø§ÙÙÙ ÙÙØ¯
 Ø£ÙÙÙØª Ø§ÙÙØ³Ø®Ø© Ø§ÙØ£ÙÙÙ ÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ ÙÙÙÙ
 Ø§ÙØ­ÙØ¯. ÙØ£Ø´ÙØ± Ø£Ø®Ù ÙØ£Ø®ØªÙ Ø§ÙÙØ°Ø§ÙÙ Ø¯Ø¹ÙÙÙ
 ÙØ­ÙØ²Ø§ÙÙ ÙØ£ØªÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ â¤ï¸ ## ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©
-**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¡Ù
+**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¦Ù
 ÙØªÙØ­ÙØ¯ Ø§ÙÙØªØ¹ÙÙØ§Øª Ø§ÙÙØªØ¹ÙÙØ© Ø¨Ø§ÙØ¯ÙØ§ÙØ©
 Ø§ÙØ¥Ø³ÙØ§ÙÙØ© (ÙØ§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙØ ÙØ§ÙØ£Ø­Ø§Ø¯ÙØ«
 Ø§ÙØ´Ø±ÙÙØ© Ø ÙØ§ÙØªÙØ³ÙØ±Ø ÙØ§ÙØ£Ø¯Ø¹ÙØ©Ø ÙØºÙØ±ÙØ§) ÙÙ
 ÙÙØ§Ù ÙØ§Ø­Ø¯. ÙØªØªÙØªØ¹ Ø§ÙÙÙØªØ¨Ø© Ø¨Ø¹Ø¯ÙØ© Ø­Ø²ÙÙØ
 ÙØ£ÙÙÙØ§: * **Ø­Ø²ÙØ© Ø§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙ**:. * Ø§Ø³ØªØ®Ø±Ø§Ø¬
 Ø¬ÙÙØ¹ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±Ø¢ÙÙØ© ÙÙØ§ÙØ© ÙØ¹ÙÙÙØ§ØªÙØ§. *
 Ø¥ÙÙØ§ÙÙØ© Ø§ÙØ¨Ø­Ø« Ø¹Ù Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ©. * Ø¥ÙÙØ§ÙÙØ©
@@ -35,36 +37,40 @@
 Ø¹ÙÙØ§ ÙÙ Ø§ÙØ¥ØµØ¯Ø§Ø±Ø§Øª Ø§ÙÙØ§Ø¯ÙØ© -Ø¥Ù Ø´Ø§Ø¡ Ø§ÙÙÙ- ##
 **ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©** ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù Ø·Ø±ÙÙ **Github**
 **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ£ÙÙÙ**: Ø¹Ù Ø·Ø±ÙÙ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±: *
 Ø¥ÙØ´Ø§Ø¡ ÙÙÙ Ø¨Ø£Ø³Ù **`AL_Khatma`** * Ø§ÙØªØ­ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±
 ÙØ£ÙØªØ¨ ÙØ°Ø§ Ø§ÙØ£ÙØ±: ```sh S git clone https://github.com/oaokm/AL-
 Khatma ``` **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ«Ø§ÙÙØ©**: ØªØ­ÙÙÙÙØ§ ÙÙ
 Ø§ÙÙØªØµÙØ­ Ø¨ØµÙØºØ© ÙÙÙ ÙØ¶Ø¹ÙØ· `.zip` ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù
-Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma ``` **Ø£Ù** ```sh $ pip3
-install AL-Khatma ``` ## **Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§
-ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ *
-Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø±
-Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ
-Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§ ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma
->>> AL_Khatma.__version__ '1.0.0' ``` ### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬
-Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©** Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ
-Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ÙÙ `Quran
-().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ©
-Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list) ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯
-Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ© ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª
-Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§. ```py
-Quran.show_block_aya( self, verses_no:int, verses_number:list, orderly=False,
-): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§
-ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ© verses_no(int):
-Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number(list): ÙÙ
-Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ Ø¨ÙØªØ§Ø¨Ø©
-Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly(bool):
-Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ ÙÙÙÙ
-ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§ Ø³ÙØ±Ø©
-Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
+Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma-lib ``` **Ø£Ù** ```sh $ pip3
+install AL-Khatma-lib ``` #### ØªØ­ÙÙÙ Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ©
+Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ© ÙÙ ÙÙÙ Ø§ÙÙØºØ© ÙØ¨Ø¹Ø¶ Ø§ÙÙÙÙØ§Øª
+Ø§ÙØªÙ ØªØ³Ø§Ø¹Ø¯ Ø¹ÙÙ Ø§ÙØ¨Ø±ÙØ§ÙØ¬Ø Ø¨ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ±
+Ø§ÙØªØ§ÙÙ: ```py >>> import AL_Khatma >>> AL_Khatma.Download_DATA() ```
+ÙØ£ÙØªØ¸Ø± Ø¥ÙÙ Ø£Ù ØªØªÙ Ø¹ÙÙÙØ© Ø§ÙØªØ­ÙÙÙ Ø¨ÙØ¬Ø§Ø­ ##
+**Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§ ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ
+ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ * Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø©
+Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§
+ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma >>> AL_Khatma.__version__ '1.0.0' ```
+### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©**
+Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ÙÙ `Quran().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ
+Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list)
+ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯ Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ©
+ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§.
+```py Quran.show_block_aya( self, verses_no:int, verses_number:list,
+orderly=False, ): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ
+Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§ ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ©
+verses_no(int): Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number
+(list): ÙÙ Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ
+Ø¨ÙØªØ§Ø¨Ø© Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly
+(bool): Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ
+ÙÙÙÙ ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§
+Ø³ÙØ±Ø© Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
 Ø§ÙØ¨Ø±ÙØ§ÙØ¬ Ø³ÙØ¹ÙØ¯ ÙÙ 7 Ø¹ÙØ§ØµØ± Ø¯Ø§Ø®Ù Ø§ÙÙØ§Ø¦ÙØ©. ÙÙÙ
 Ø¹ÙØµØ± ÙØ­ØªÙÙ Ø¹ÙÙ ÙØ¹ÙÙÙØ§Øª ÙÙØ£ÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ±
 Ø§ÙÙØ§ÙÙØ³ (dict) ÙÙÙÙÙ Ø´ÙÙÙ ÙØ§ÙØªØ§ÙÙ: ```json // Form JSON
 File 'main.json' (Arabic + English) // { "ID": 1, "Name": "Ø§ÙÙÙØ§ØªÙØ­Ø©",
 "Transliteration": "Al-FÄtiá¸¥ah", "translation": "The Opener", "type":
 "meccan", "total_verses": 7, "verses_no": 1, "jozz": 1, "page": 1,
 "verses_number": 1, "line_start": 2, "line_end": 2, "verses_text":
@@ -322,19 +328,22 @@
 (list). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(1)**: ÙÙ Ø­Ø§Ù Ø¹Ø¯Ù Ø¥ØªØµØ§ÙÙ
 Ø¨Ø§ÙØ¥ÙØªØ±ÙØª ÙØ¥Ù ÙØ°Ù Ø§ÙÙÙØ²Ø© ÙÙ ØªØ¹ÙÙØ ÙÙØ±Ø¬Ù
 Ø§ÙØªØ­ÙÙ ÙÙ Ø¥ØªØµØ§ÙÙ ÙÙØ¥ÙØªØ±ÙØª. > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©
 (2)**: Ø®ÙØ§Ø± `type` ÙÙ ÙÙØ¹ Ø£Ù Ø´ÙÙ Ø§ÙØµÙØ­Ø© Ø§ÙØªÙ
 ØªØ±ÙØ¯ÙØ§Ø ÙØ­Ø§ÙÙØ§ ÙÙØ§ÙÙ ÙÙØ· Ø´ÙÙØ§Ù ÙÙØ·Ø ÙÙÙÙÙ
 Ø§ÙØ§Ø·ÙØ§Ø¹ Ø¹ÙÙÙ [Ø¨Ø§ÙØ¶ØºØ· ÙÙØ§ ÙØ±Ø¤ÙØ© Ø§ÙØ®ÙØ§Ø±Ø§Øª
 Ø§ÙÙØªØ§Ø­](https://github.com/oaokm/AL-Khatma/blob/main/DATA/
-quran_books.json). Ø·Ø±ÙÙØ© ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>>
-from AL_Khatma.quran import Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡
-Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures',
-'quran') # ÙØªØ§Ø¨Ø© Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages
-From Quran ...
+quran_books.json). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(3)**: Ø¹ÙØ¯ÙØ§ ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙØªÙ Ø³ØªÙØ²Ù ÙÙÙØ§ Ø§ÙØµÙØ± ÙØ¬Ø¨ Ø£Ù ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙÙØ§ÙÙ ÙÙØ§ ÙÙ ÙÙØ¶Ø­ ÙÙ Ø§ÙÙØ«Ø§Ù Ø·Ø±ÙÙØ©
+ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>> from AL_Khatma.quran import
+Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1,
+2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # ÙØªØ§Ø¨Ø©
+Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages From Quran | [/home/
+oaokm/Pictures/Quran]
 100%|âââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:01<00:00, 1.69it/s] ```
                              [picture_screenshot]
 ### ØªÙØ³ÙÙ ØµÙØ­Ø§Øª Ø§ÙÙØ±Ø¢Ù ÙÙ Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
 Ø§ÙÙØ±ÙÙØ Ø·Ø±ÙÙØ© ÙØªÙØ³ÙÙ Ø§ÙØµÙØ­Ø§Øª Ø¨ÙØ¯Ù ØªØ®ØªÙÙ
 Ø§ÙÙØ±Ø¢ÙØ ÙØªÙØ²ÙØ¹ Ø§ÙØªÙØ³ÙÙ Ø¹ÙÙ Ø§ÙØµÙØ­Ø§Øª. ```py >>>
 from AL_Khatma.khatma import khatma # Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙØ­Ø²ÙØ© >>> k =
```

### Comparing `AL_Khatma_lib-1.0.0/pyproject.toml` & `AL_Khatma_lib-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AL_Khatma_lib"
-version = "1.0.0"
+version = "1.1.1"
 authors = [
   { name="Osamah Awadh", email="osamahawadh01@gmail.com" },
 ]
 description = "A library Specialized About Islamic"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `AL_Khatma_lib-1.0.0/src/AL_Khatma/khatma.py` & `AL_Khatma_lib-1.1.1/src/AL_Khatma/khatma.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from quran import Quran
-from log import log
+from .quran import Quran
+from .log import log
 from tqdm import tqdm
 
 class khatma:
     def __init__(self, days:int):
         log(
             f"{__file__} > khatma | Status The Class",
             f"True, days(int): {days}"
```

### Comparing `AL_Khatma_lib-1.0.0/src/AL_Khatma/quran.py` & `AL_Khatma_lib-1.1.1/src/AL_Khatma/quran.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import AL_Khatma
-from log import log
+from .log import log
 import json
 import requests
 import os
 from tqdm import tqdm
 import urllib3
 from time import perf_counter
 
+__main_path__ = os.path.dirname(__file__)
 
 class Quran:
     def __init__(self, lang='main'):
         """
         Quran(class): 
         lang: اللغة التي تريد عرضها
         """
         try:
             #* قراءة ملف اللغات
-            os.chdir(path=AL_Khatma.__main_path__)
+            os.chdir(path=__main_path__)
             self.quran = json.load(open(f"./DATA/Language/{lang}.json", "r", encoding="utf8"))
             log(
                 f'{__file__} > Quran | Status JSON File ', 
                 f'Read: True, Language: {lang}'
                 ).write_message()
         except FileNotFoundError as e:
             #* في حال طلب المستخدم استعراض اللغات
@@ -239,25 +240,26 @@
                     f"Error(keyError): {e}"
                 ).write_message()
                 print(f'[ Quran > page_pic | KeyError ]: {e}')
             #* في حالة إذا كان خاصية (return_imge) مفعلة يتم تسجيل محتويات الصورة كبِّت(صيغة ثنائية)
             pics = list()
             
             #? هنا تبدأ عملية الوصول للصفحات وتحميلها
-            print("# Download Pages From Quran ... ")
+            PATH = f'{path}/{name_folder}'
+            print(f"# Download Pages From Quran | [{os.path.abspath(PATH)}]")
             for p in tqdm(page):
                 #? التحقق من إذا كان المدخل لا يتخطى عدد صفحات القرأن
                 if p <= 604:
                     #* عملية الإتصال بالموقع لسحب الصورة الصفحة
                     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
                     url    = web_pic.format(p)
                     r_page = requests.get(url=url, verify=False)
                     
                     #* عملية إنشاء ملف تمهيدًا لتحميل الصفحات
-                    PATH = f'{path}/{name_folder}'
+                    
                     #? في حال كان خيار return_imge مفعل فسوف يتم تحميل الصور كبٍّت(النظام الثنائي)
                     if return_imge:
                         pics.append([p, r_page.content])
                     else:
                         #! في حال إذا الملف الذي أدخل المستخدم غير موجود على القرص سيتم تنزيل مباشرًا
                         if not os.path.exists(PATH):
                             os.makedirs(PATH)
```

### Comparing `AL_Khatma_lib-1.0.0/src/AL_Khatma_lib.egg-info/PKG-INFO` & `AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AL-Khatma-lib
-Version: 1.0.0
+Version: 1.1.1
 Summary: A library Specialized About Islamic
 Author-email: Osamah Awadh <osamahawadh01@gmail.com>
 Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
 Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,30 +29,30 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#التعامل_مع_المكتبة">التعامل مع المكتبة</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#المصادر">المصادر</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/UPDATE.md">التحديثات</a>
+  <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
 </p>
 
-![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange)
---| --|
+![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI](https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://img.shields.io/github/repo-size/oaokm/AL-Khatma)
+--| --| -- | --| 
 
 
 ## **بيان**
 في يوم الثالث من أبريل من عام 2023 الموافق الثاني عشر من رمضان لعام 1444 هـ في هذا اليوم بدأت الفكرة وبعدها قمت بتطبيق الفكرة وبناء أول API لي.
 
 وفي اليوم التاسع عشر من أبريل من عام 2023 الموافق الثامن والعشرون من رمضان لعام 1444 هـ وبتوفيق من الله لقد أنهيت النسخة الأولى من هذا المشروع ولله الحمد.
 وأشكر أخي وأختي اللذانِ دعمني وحفزاني لأتمّ هذا المشروع ❤️
 
 
 ## فكرة_الختمة
-**الختمة** هو مشروع مفتوح المصدر تم بناءه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
+**الختمة** هو مشروع مفتوح المصدر تم بنائه لتوحيد المتعلقات المتعلقة بالديانة الإسلامية (كالقرأن الكريم، والأحاديث الشريفة ، والتفسير، والأدعية، وغيرها) في مكان واحد.
 وتتمتع المكتبة بعدّة حزمّ، وأهمها:
 
 * **حزمة القرأن الكريم**:.
   * استخراج جميع الأيات القرآنية وكاقة معلوماتها.
   * إمكانية البحث عن الأيات الكريمة.
   * إمكانية تحميل صور صفحات القرآن الكريم.
   * المكتبة مزودة بعدّة لغات. ومنها:
@@ -89,21 +89,31 @@
 
 **الطريقة الثانية**: تحميلها من المتصفح بصيغة ملف مضعوط `.zip`
 
 
 ### التحميل عن طريق **pypi**
 
 ```sh
-$ pip install AL-Khatma
+$ pip install AL-Khatma-lib
 ```
 **أو**
 ```sh
-$ pip3 install AL-Khatma
+$ pip3 install AL-Khatma-lib
 ```
 
+#### تحميل الملفات الهامة
+الملفات الهامة هي ملف اللغة وبعض الملفات التي تساعد عمل البرنامج، بكتابة الأمر التالي:
+
+```py
+>>> import AL_Khatma
+>>> AL_Khatma.Download_DATA()
+```
+وأنتظر إلى أن تتم عملية التحميل بنجاح
+
+
 ## **التعامل_مع_المكتبة**
 
 حاليا هنالك حزمتين، وهي:
 
 * حزمة القرآن الكريم
 * حزمة تختيم القرآن الكريم
 
@@ -366,22 +376,23 @@
 
 > **معلومة مساعدة**: خاصية `return_imge` يمكن أستخدامها في بناء البوتات، كبوت في التليجرام مثلًا. بدلًا من أن تخزم محتوى الصورة في القرص الصلب، يمكون في متغير قائمة (list).
 
 > **ملاحظة مهمة(1)**: في حال عدم إتصالك بالإنترنت فإن هذه الميزة لن تعمل، ويرجى التحقق من إتصالك للإنترنت.
 
 > **ملاحظة مهمة(2)**: خيار `type` هو نوع أو شكل الصفحة التي تريدها، وحاليا هنالك فقط شكلان فقط، ويمكن الاطلاع عليه [بالضغط هنا لرؤية الخيارات المتاح](https://github.com/oaokm/AL-Khatma/blob/main/DATA/quran_books.json).
 
+> **ملاحظة مهمة(3)**: عندما تضع المسار التي ستنزل فيها الصور يجب أن تضع المسار الكامل كما هو موضح في المثال
 
 طريقة كتابة الأمر كالتالي:
 
 ```py
 >>> from AL_Khatma.quran import Quran
 >>> quran = Quran() # استدعاء الكائن
->>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
-# Download Pages From Quran ... 
+>>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # كتابة جميع المعطيات اللازمة
+# Download Pages From Quran | [/home/oaokm/Pictures/Quran] 
 100%|███████████████████████████████████████| 3/3 [00:01<00:00,  1.69it/s]
 ```
 <p align="center">
   <img src="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/Pictures/Screenshot_for_page_pic.png" alt="picture_screenshot">
 </p>
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 1.0.0 Summary: A library
+Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 1.1.1 Summary: A library
 Specialized About Islamic Author-email: Osamah Awadh
 gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
 URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
                               Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª
 ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https://
-img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) --| --| ##
+img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
+(https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
+img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
 Ø§ÙÙÙØ±Ø© ÙØ¨ÙØ§Ø¡ Ø£ÙÙ API ÙÙ. ÙÙÙ Ø§ÙÙÙÙ Ø§ÙØªØ§Ø³Ø¹ Ø¹Ø´Ø±
 ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ ÙØ§ÙØ¹Ø´Ø±ÙÙ
 ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙØ¨ØªÙÙÙÙ ÙÙ Ø§ÙÙÙ ÙÙØ¯
 Ø£ÙÙÙØª Ø§ÙÙØ³Ø®Ø© Ø§ÙØ£ÙÙÙ ÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ ÙÙÙÙ
 Ø§ÙØ­ÙØ¯. ÙØ£Ø´ÙØ± Ø£Ø®Ù ÙØ£Ø®ØªÙ Ø§ÙÙØ°Ø§ÙÙ Ø¯Ø¹ÙÙÙ
 ÙØ­ÙØ²Ø§ÙÙ ÙØ£ØªÙÙ ÙØ°Ø§ Ø§ÙÙØ´Ø±ÙØ¹ â¤ï¸ ## ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©
-**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¡Ù
+**Ø§ÙØ®ØªÙØ©** ÙÙ ÙØ´Ø±ÙØ¹ ÙÙØªÙØ­ Ø§ÙÙØµØ¯Ø± ØªÙ Ø¨ÙØ§Ø¦Ù
 ÙØªÙØ­ÙØ¯ Ø§ÙÙØªØ¹ÙÙØ§Øª Ø§ÙÙØªØ¹ÙÙØ© Ø¨Ø§ÙØ¯ÙØ§ÙØ©
 Ø§ÙØ¥Ø³ÙØ§ÙÙØ© (ÙØ§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙØ ÙØ§ÙØ£Ø­Ø§Ø¯ÙØ«
 Ø§ÙØ´Ø±ÙÙØ© Ø ÙØ§ÙØªÙØ³ÙØ±Ø ÙØ§ÙØ£Ø¯Ø¹ÙØ©Ø ÙØºÙØ±ÙØ§) ÙÙ
 ÙÙØ§Ù ÙØ§Ø­Ø¯. ÙØªØªÙØªØ¹ Ø§ÙÙÙØªØ¨Ø© Ø¨Ø¹Ø¯ÙØ© Ø­Ø²ÙÙØ
 ÙØ£ÙÙÙØ§: * **Ø­Ø²ÙØ© Ø§ÙÙØ±Ø£Ù Ø§ÙÙØ±ÙÙ**:. * Ø§Ø³ØªØ®Ø±Ø§Ø¬
 Ø¬ÙÙØ¹ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±Ø¢ÙÙØ© ÙÙØ§ÙØ© ÙØ¹ÙÙÙØ§ØªÙØ§. *
 Ø¥ÙÙØ§ÙÙØ© Ø§ÙØ¨Ø­Ø« Ø¹Ù Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ©. * Ø¥ÙÙØ§ÙÙØ©
@@ -42,36 +44,40 @@
 Ø¹ÙÙØ§ ÙÙ Ø§ÙØ¥ØµØ¯Ø§Ø±Ø§Øª Ø§ÙÙØ§Ø¯ÙØ© -Ø¥Ù Ø´Ø§Ø¡ Ø§ÙÙÙ- ##
 **ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©** ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù Ø·Ø±ÙÙ **Github**
 **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ£ÙÙÙ**: Ø¹Ù Ø·Ø±ÙÙ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±: *
 Ø¥ÙØ´Ø§Ø¡ ÙÙÙ Ø¨Ø£Ø³Ù **`AL_Khatma`** * Ø§ÙØªØ­ Ø³Ø·Ø± Ø§ÙØ£ÙØ§ÙØ±
 ÙØ£ÙØªØ¨ ÙØ°Ø§ Ø§ÙØ£ÙØ±: ```sh S git clone https://github.com/oaokm/AL-
 Khatma ``` **Ø§ÙØ·Ø±ÙÙØ© Ø§ÙØ«Ø§ÙÙØ©**: ØªØ­ÙÙÙÙØ§ ÙÙ
 Ø§ÙÙØªØµÙØ­ Ø¨ØµÙØºØ© ÙÙÙ ÙØ¶Ø¹ÙØ· `.zip` ### Ø§ÙØªØ­ÙÙÙ Ø¹Ù
-Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma ``` **Ø£Ù** ```sh $ pip3
-install AL-Khatma ``` ## **Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§
-ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ *
-Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø±
-Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ
-Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§ ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma
->>> AL_Khatma.__version__ '1.0.0' ``` ### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬
-Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©** Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ
-Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ ÙÙ `Quran
-().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ©
-Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list) ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯
-Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ© ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª
-Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§. ```py
-Quran.show_block_aya( self, verses_no:int, verses_number:list, orderly=False,
-): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§
-ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ© verses_no(int):
-Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number(list): ÙÙ
-Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ Ø¨ÙØªØ§Ø¨Ø©
-Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly(bool):
-Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ ÙÙÙÙ
-ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§ Ø³ÙØ±Ø©
-Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
+Ø·Ø±ÙÙ **pypi** ```sh $ pip install AL-Khatma-lib ``` **Ø£Ù** ```sh $ pip3
+install AL-Khatma-lib ``` #### ØªØ­ÙÙÙ Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ©
+Ø§ÙÙÙÙØ§Øª Ø§ÙÙØ§ÙØ© ÙÙ ÙÙÙ Ø§ÙÙØºØ© ÙØ¨Ø¹Ø¶ Ø§ÙÙÙÙØ§Øª
+Ø§ÙØªÙ ØªØ³Ø§Ø¹Ø¯ Ø¹ÙÙ Ø§ÙØ¨Ø±ÙØ§ÙØ¬Ø Ø¨ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ±
+Ø§ÙØªØ§ÙÙ: ```py >>> import AL_Khatma >>> AL_Khatma.Download_DATA() ```
+ÙØ£ÙØªØ¸Ø± Ø¥ÙÙ Ø£Ù ØªØªÙ Ø¹ÙÙÙØ© Ø§ÙØªØ­ÙÙÙ Ø¨ÙØ¬Ø§Ø­ ##
+**Ø§ÙØªØ¹Ø§ÙÙ_ÙØ¹_Ø§ÙÙÙØªØ¨Ø©** Ø­Ø§ÙÙØ§ ÙÙØ§ÙÙ Ø­Ø²ÙØªÙÙØ
+ÙÙÙ: * Ø­Ø²ÙØ© Ø§ÙÙØ±Ø¢Ù Ø§ÙÙØ±ÙÙ * Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ### **Ø·Ø¨Ø§Ø¹Ø© Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø©** ÙØ·Ø¨Ø§Ø¹Ø©
+Ø¥ØµØ¯Ø§Ø± Ø§ÙÙÙØªØ¨Ø© ÙØ¬Ø¨ Ø¹ÙÙÙ Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙÙØªØ¨Ø© ÙÙØ§
+ÙÙ ÙÙØ¶Ø­: ```py >>> import AL_Khatma >>> AL_Khatma.__version__ '1.0.0' ```
+### **Ø·Ø±ÙÙØ© Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³ÙØ± Ø§ÙÙØ±Ø¢ÙÙØ© Ø§ÙÙØ±ÙÙØ©**
+Ø§ÙØ£ÙØ± Ø§ÙØ°Ù ÙÙÙÙ Ø¨Ø£Ø³ØªØ®Ø±Ø§Ø¬ ÙØ­ØªÙÙ Ø§ÙÙØ±Ø¢Ù
+Ø§ÙÙØ±ÙÙ ÙÙ `Quran().show_block_aya`. ÙÙØ°Ø§ Ø§ÙØ£ÙØ± ÙÙÙÙ
+Ø¨Ø¥Ø±Ø¬Ø§Ø¹ ÙÙ ÙÙÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ± Ø§ÙÙØ§Ø¦ÙØ©(list)
+ÙØªÙÙÙ Ø¯Ø§Ø¦ÙØ§ Ø¹Ø¯Ø¯ Ø§ÙØ¹ÙØ§ØµØ± ÙÙ Ø§ÙÙØ§Ø¦ÙØ© ÙØ³Ø§ÙÙØ©
+ÙØ¹Ø¯Ø¯ Ø§ÙØ£ÙØ§Øª Ø§ÙÙØ±ÙÙØ© ÙÙØ³ÙØ±Ø© Ø§ÙØªÙ Ø£Ø³ØªØ¯Ø¹ÙØªÙØ§.
+```py Quran.show_block_aya( self, verses_no:int, verses_number:list,
+orderly=False, ): """ show_block_aya(func): ÙÙ Ø¯Ø§ÙØ© ØªÙÙÙ
+Ø¨Ø¥Ø³ØªØ®Ø±Ø§Ø¬ ÙØ§ ÙØ¯Ø±Ø¯Ù Ø§ÙÙØ³ØªØ®Ø¯Ù ÙÙ ÙÙÙ Ø§ÙÙØºØ©
+verses_no(int): Ø£Ø³ØªØ®Ø±Ø§Ø¬ Ø§ÙØ³Ø±ÙØ© Ø§ÙØªÙ ØªØ±ÙØ¯ÙØ§ verses_number
+(list): ÙÙ Ø­Ø§ÙØ© Ø£ÙÙ ØªØ±Ø¯ ØµÙØ±Ø© Ø¨Ø¹ÙÙÙØ§ ÙÙÙÙÙ Ø°ÙÙ
+Ø¨ÙØªØ§Ø¨Ø© Ø±ÙÙ Ø£ÙØªÙØ§. ÙÙÙÙÙ Ø£Ù ØªØ¬Ø¹ÙØ¹Ø§ ÙØ§Ø±ØºØ© orderly
+(bool): Ø¥Ø°Ø§ Ø£Ø±Ø¯Øª Ø£Ù ØªØ±Ù Ø§ÙÙØªÙØ¬Ø© ÙØ·Ø¨ÙØ¹Ø© Ø¨Ø´ÙÙ
+ÙÙÙÙ ÙØ±Ø§Ø¡ØªÙØ§ """ ``` > **ÙØ«ÙØ§ ÙÙØªÙØ¶ÙØ­**: ÙÙØ«ÙØ§
+Ø³ÙØ±Ø© Ø§ÙÙØ§ØªØ­Ø© Ø¹Ø¯Ø¯ Ø£ÙØ§ØªÙØ§ 7 ÙØ¹ Ø§ÙØ¨Ø³ÙÙØ© ÙØ¥Ù
 Ø§ÙØ¨Ø±ÙØ§ÙØ¬ Ø³ÙØ¹ÙØ¯ ÙÙ 7 Ø¹ÙØ§ØµØ± Ø¯Ø§Ø®Ù Ø§ÙÙØ§Ø¦ÙØ©. ÙÙÙ
 Ø¹ÙØµØ± ÙØ­ØªÙÙ Ø¹ÙÙ ÙØ¹ÙÙÙØ§Øª ÙÙØ£ÙØ© Ø¹ÙÙ Ø´ÙÙ ÙØªØºÙØ±
 Ø§ÙÙØ§ÙÙØ³ (dict) ÙÙÙÙÙ Ø´ÙÙÙ ÙØ§ÙØªØ§ÙÙ: ```json // Form JSON
 File 'main.json' (Arabic + English) // { "ID": 1, "Name": "Ø§ÙÙÙØ§ØªÙØ­Ø©",
 "Transliteration": "Al-FÄtiá¸¥ah", "translation": "The Opener", "type":
 "meccan", "total_verses": 7, "verses_no": 1, "jozz": 1, "page": 1,
 "verses_number": 1, "line_start": 2, "line_end": 2, "verses_text":
@@ -329,19 +335,22 @@
 (list). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(1)**: ÙÙ Ø­Ø§Ù Ø¹Ø¯Ù Ø¥ØªØµØ§ÙÙ
 Ø¨Ø§ÙØ¥ÙØªØ±ÙØª ÙØ¥Ù ÙØ°Ù Ø§ÙÙÙØ²Ø© ÙÙ ØªØ¹ÙÙØ ÙÙØ±Ø¬Ù
 Ø§ÙØªØ­ÙÙ ÙÙ Ø¥ØªØµØ§ÙÙ ÙÙØ¥ÙØªØ±ÙØª. > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©
 (2)**: Ø®ÙØ§Ø± `type` ÙÙ ÙÙØ¹ Ø£Ù Ø´ÙÙ Ø§ÙØµÙØ­Ø© Ø§ÙØªÙ
 ØªØ±ÙØ¯ÙØ§Ø ÙØ­Ø§ÙÙØ§ ÙÙØ§ÙÙ ÙÙØ· Ø´ÙÙØ§Ù ÙÙØ·Ø ÙÙÙÙÙ
 Ø§ÙØ§Ø·ÙØ§Ø¹ Ø¹ÙÙÙ [Ø¨Ø§ÙØ¶ØºØ· ÙÙØ§ ÙØ±Ø¤ÙØ© Ø§ÙØ®ÙØ§Ø±Ø§Øª
 Ø§ÙÙØªØ§Ø­](https://github.com/oaokm/AL-Khatma/blob/main/DATA/
-quran_books.json). Ø·Ø±ÙÙØ© ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>>
-from AL_Khatma.quran import Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡
-Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1, 2 , 48], 'm-madinah_ksu', '~/Pictures',
-'quran') # ÙØªØ§Ø¨Ø© Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages
-From Quran ...
+quran_books.json). > **ÙÙØ§Ø­Ø¸Ø© ÙÙÙØ©(3)**: Ø¹ÙØ¯ÙØ§ ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙØªÙ Ø³ØªÙØ²Ù ÙÙÙØ§ Ø§ÙØµÙØ± ÙØ¬Ø¨ Ø£Ù ØªØ¶Ø¹
+Ø§ÙÙØ³Ø§Ø± Ø§ÙÙØ§ÙÙ ÙÙØ§ ÙÙ ÙÙØ¶Ø­ ÙÙ Ø§ÙÙØ«Ø§Ù Ø·Ø±ÙÙØ©
+ÙØªØ§Ø¨Ø© Ø§ÙØ£ÙØ± ÙØ§ÙØªØ§ÙÙ: ```py >>> from AL_Khatma.quran import
+Quran >>> quran = Quran() # Ø§Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙÙØ§Ø¦Ù >>> quran.page_pic([1,
+2 , 48], 'm-madinah_ksu', '/home/oaokm/Pictures', 'quran') # ÙØªØ§Ø¨Ø©
+Ø¬ÙÙØ¹ Ø§ÙÙØ¹Ø·ÙØ§Øª Ø§ÙÙØ§Ø²ÙØ© # Download Pages From Quran | [/home/
+oaokm/Pictures/Quran]
 100%|âââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:01<00:00, 1.69it/s] ```
                              [picture_screenshot]
 ### ØªÙØ³ÙÙ ØµÙØ­Ø§Øª Ø§ÙÙØ±Ø¢Ù ÙÙ Ø­Ø²ÙØ© ØªØ®ØªÙÙ Ø§ÙÙØ±Ø¢Ù
 Ø§ÙÙØ±ÙÙØ Ø·Ø±ÙÙØ© ÙØªÙØ³ÙÙ Ø§ÙØµÙØ­Ø§Øª Ø¨ÙØ¯Ù ØªØ®ØªÙÙ
 Ø§ÙÙØ±Ø¢ÙØ ÙØªÙØ²ÙØ¹ Ø§ÙØªÙØ³ÙÙ Ø¹ÙÙ Ø§ÙØµÙØ­Ø§Øª. ```py >>>
 from AL_Khatma.khatma import khatma # Ø£Ø³ØªØ¯Ø¹Ø§Ø¡ Ø§ÙØ­Ø²ÙØ© >>> k =
```

