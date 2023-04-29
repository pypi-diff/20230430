# Comparing `tmp/ersciyt-1.4.tar.gz` & `tmp/ersciyt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.4.tar", last modified: Fri Apr 28 21:21:14 2023, max compression
+gzip compressed data, was "ersciyt-1.5.tar", last modified: Sat Apr 29 22:10:30 2023, max compression
```

## Comparing `ersciyt-1.4.tar` & `ersciyt-1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:21:14.981562 ersciyt-1.4/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-28 21:21:07.000000 ersciyt-1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 21:21:07.000000 ersciyt-1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 21:21:14.981562 ersciyt-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-28 21:21:07.000000 ersciyt-1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:21:14.980563 ersciyt-1.4/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:21:14.981562 ersciyt-1.4/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/models.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     7380 2023-04-28 21:21:07.000000 ersciyt-1.4/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:21:14.980563 ersciyt-1.4/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 21:21:14.000000 ersciyt-1.4/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-28 21:21:14.000000 ersciyt-1.4/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:21:14.000000 ersciyt-1.4/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-28 21:21:14.000000 ersciyt-1.4/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 21:21:14.000000 ersciyt-1.4/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-28 21:21:14.982563 ersciyt-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-28 21:21:07.000000 ersciyt-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.815107 ersciyt-1.5/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-29 22:10:25.000000 ersciyt-1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-29 22:10:25.000000 ersciyt-1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-29 22:10:30.815107 ersciyt-1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-29 22:10:25.000000 ersciyt-1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.813107 ersciyt-1.5/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.815107 ersciyt-1.5/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/models.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.814108 ersciyt-1.5/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-29 22:10:30.816108 ersciyt-1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-29 22:10:25.000000 ersciyt-1.5/setup.py
```

### Comparing `ersciyt-1.4/LICENSE` & `ersciyt-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.4/PKG-INFO` & `ersciyt-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.4
+Version: 1.5
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.4/README.md` & `ersciyt-1.5/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.4/ersciyt/views.py` & `ersciyt-1.5/ersciyt/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.shortcuts import render
 from django.conf import settings
-from pytube import YouTube
+#from pytube import YouTube
 import os,subprocess
 from django.http import HttpResponse,FileResponse
-from youtube_transcript_api import YouTubeTranscriptApi
-from youtube_transcript_api.formatters import WebVTTFormatter
+#from youtube_transcript_api import YouTubeTranscriptApi
+#from youtube_transcript_api.formatters import WebVTTFormatter
 #pip install googletrans==4.0.0-rc1
 #from googletrans import Translator
 import re
 
 
 def ytdwn(request,link):
     try:        
@@ -36,17 +36,18 @@
         response['Content-Length'] = os.path.getsize(media_dir + '/' + file)
         response['Content-Disposition'] = 'filename=%s' % fn
         os.remove(media_dir + '/' + file)
         '''
         return response
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
-
+'''
 def sub(request,lang,link):
     try:
+        
         video = YouTube('https://www.youtube.com/watch?v=%s' % link)
         stream = video.streams.get_highest_resolution()
         media_dir=os.path.join(settings.BASE_DIR,'ytdown','media')
         stream.download(output_path=media_dir,filename='a.mp4')
 
         #srt=YouTubeTranscriptApi.get_transcript(link)
         transcripts = YouTubeTranscriptApi.list_transcripts(link)
@@ -102,43 +103,30 @@
         response['Content-Length'] = os.path.getsize(media_dir + '/out.mp4')
         response['Content-Disposition'] = 'attachment; filename=%s' % fn
         os.remove(media_dir + '/a.mp4')
         os.remove(media_dir + '/out.mp4')
         return response
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
-
-def ytlink(request):
+'''
+def vid(request):
     try:
-        link=''
-        if request.method == 'GET' and 'url' in request.GET:
-            txt = request.GET['url']
-            arr = txt.split("watch%3Fv%3D");
-            arr1 = arr[-1].split("watch?v=");
-            arr2 = arr1[-1].split("&");
-            link = arr2[0];
-
-        video = YouTube('https://www.youtube.com/watch?v=%s' % link)
-        stream = video.streams.get_highest_resolution()
-        media_dir=os.path.join(settings.BASE_DIR,'ytdown','media')
-        file = str(link)
-        stream.download(output_path=media_dir,filename=file)
-        tmp4=open(media_dir + '/' + file , 'rb')
+        link=request.GET['url']
+        os.system('yt-dlp  -f 18 -o a.mp4 {}'.format(link))        
+        tmp4=open('a.mp4' , 'rb')
         tmp5=tmp4.read()
         tmp4.close()
-        fn=stream.default_filename
-        fn=re.sub(r"\s+", '_', fn)
         response=HttpResponse(tmp5, content_type='video/mp4')
-        response['Content-Length'] = os.path.getsize(media_dir + '/' + file)
-        response['Content-Disposition'] = 'attachment; filename=%s' % fn
-        os.remove(media_dir + '/' + file)
+        response['Content-Length'] = os.path.getsize('a.mp4')
+        response['Content-Disposition'] = 'filename=a.mp4'
+        os.remove('a.mp4')
         return response
     except:
         return HttpResponse ('Youtube Url Is Mistake!!')
-
+'''
 def ytmp3(request,link):
     try:
         video = YouTube('https://www.youtube.com/watch?v=%s' % link)
         stream = video.streams.filter(only_audio=True).first()
         media_dir=os.path.join(settings.BASE_DIR,'ytdown','media')
         file = str(link)
         stream.download(output_path=media_dir,filename=file)
@@ -152,30 +140,22 @@
         response['Content-Length'] = os.path.getsize(media_dir + '/m1.mp3')
         response['Content-Disposition'] = 'attachment; filename=%s' % fn
         os.remove(media_dir + '/' + file)
         os.remove(media_dir + '/m1.mp3')
         return response
     except:
         return HttpResponse (video.description)
-
+'''
 
 def helping(request):
     try:
         return HttpResponse ('''
         <p>Use address of youtube after watch like - for download video -  :<br>
-        <b> YourSiteName/ytlink?url=https://www.youtube.com/watch?v=xazlZh1lTpM</b><br>
+        <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         link name like - for play in firefox -  : <br>
-        <b>YourSiteName/xazlZh1lTpM</b><br>
-        and<br>
-        for download Mp3 Audio : <br>
-        <b>YourSiteName/mp3/xazlZh1lTpM</b><br>
-        for download A-B Cutting Video (from 00:30 to 00:70) : <br>
-        <b>YourSiteName/ab/00300070/xazlZh1lTpM</b><br>
-        for Subtitle the video (for any language enter language code like en,fa,it ) : <br>
-        <b>YourSiteName/en/xazlZh1lTpM</b><br>
-        <br>
-        <a href="/static/epg_youtube4.xpi">YouTube Firefox Addon</a></br>
+        <b>YourSiteName/xazlZh1lTpM</b><br>        
+        <a href="/static/ersci_viddown2.xpi">video download firefox Addon</a></br>
         </p>
         ''')
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.4/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.5/ersciyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.4
+Version: 1.5
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.4/setup.cfg` & `ersciyt-1.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.4
+version = 1.5
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
@@ -19,14 +19,12 @@
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	django
 	yt-dlp
-	pytube3
-	youtube-transcript-api
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

