# Comparing `tmp/audclas-0.0.5.tar.gz` & `tmp/audclas-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audclas-0.0.5.tar", last modified: Wed Apr 19 15:41:14 2023, max compression
+gzip compressed data, was "audclas-0.0.6.tar", last modified: Sun Apr 30 13:38:51 2023, max compression
```

## Comparing `audclas-0.0.5.tar` & `audclas-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.683608 audclas-0.0.5/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1816 2023-04-19 15:41:14.683608 audclas-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-04-19 15:34:55.000000 audclas-0.0.5/README.md
--rw-rw-rw-   0        0        0      575 2023-04-19 15:29:23.000000 audclas-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 15:41:14.685137 audclas-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.648785 audclas-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.655734 audclas-0.0.5/src/audclas/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.682100 audclas-0.0.5/src/audclas/modules/
--rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.5/src/audclas/modules/audio_mini_encoder.py
--rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.5/src/audclas/modules/checkpoint.py
--rw-rw-rw-   0        0        0     4105 2023-04-18 14:21:32.000000 audclas-0.0.5/src/audclas/modules/dataset.py
--rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.5/src/audclas/modules/diffusion.py
--rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.5/src/audclas/modules/stft.py
--rw-rw-rw-   0        0        0     3157 2023-04-19 15:27:25.000000 audclas-0.0.5/src/audclas/tortoise_audio_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.675372 audclas-0.0.5/src/audclas.egg-info/
--rw-rw-rw-   0        0        0     1816 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 13:38:51.351309 audclas-0.0.6/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1846 2023-04-30 13:38:51.350311 audclas-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1377 2023-04-30 13:36:12.000000 audclas-0.0.6/README.md
+-rw-rw-rw-   0        0        0      575 2023-04-30 13:34:09.000000 audclas-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 13:38:51.351309 audclas-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 13:38:51.206258 audclas-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 13:38:51.239409 audclas-0.0.6/src/audclas/
+drwxrwxrwx   0        0        0        0 2023-04-30 13:38:51.348317 audclas-0.0.6/src/audclas/modules/
+-rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.6/src/audclas/modules/audio_mini_encoder.py
+-rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.6/src/audclas/modules/checkpoint.py
+-rw-rw-rw-   0        0        0     4195 2023-04-23 11:44:54.000000 audclas-0.0.6/src/audclas/modules/dataset.py
+-rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.6/src/audclas/modules/diffusion.py
+-rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.6/src/audclas/modules/stft.py
+-rw-rw-rw-   0        0        0     3303 2023-04-30 09:15:05.000000 audclas-0.0.6/src/audclas/tortoise_audio_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:38:51.279560 audclas-0.0.6/src/audclas.egg-info/
+-rw-rw-rw-   0        0        0     1846 2023-04-30 13:38:51.000000 audclas-0.0.6/src/audclas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-30 13:38:51.000000 audclas-0.0.6/src/audclas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 13:38:51.000000 audclas-0.0.6/src/audclas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-30 13:38:51.000000 audclas-0.0.6/src/audclas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 13:38:51.000000 audclas-0.0.6/src/audclas.egg-info/top_level.txt
```

### Comparing `audclas-0.0.5/LICENSE` & `audclas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audclas-0.0.5/PKG-INFO` & `audclas-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audclas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files.
 Author-email: Shmart <szprytnyd@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,23 +12,24 @@
 
 # AudClas
 
 Package that uses audio classification model extracted from neonbjb/DL-Art-School - for filtering fine audio files.
 
 # Classes
 
-Classifier returns one of 5 possible labels:
+Classifier model returns one of 6 possible labels:
 
 | label | class name |
 | ----- | ---------- |
 | 0     | fine       |
 | 1     | env_noise  |
 | 2     | music      |
 | 3     | two_voices |
 | 4     | reverb     |
+| -     | unknown    |
 
 # Installation
 
 `pip install audclas`
 
 # examples of usage
```

### Comparing `audclas-0.0.5/README.md` & `audclas-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # AudClas
 
 Package that uses audio classification model extracted from neonbjb/DL-Art-School - for filtering fine audio files.
 
 # Classes
 
-Classifier returns one of 5 possible labels:
+Classifier model returns one of 6 possible labels:
 
 | label | class name |
 | ----- | ---------- |
 | 0     | fine       |
 | 1     | env_noise  |
 | 2     | music      |
 | 3     | two_voices |
 | 4     | reverb     |
+| -     | unknown    |
 
 # Installation
 
 `pip install audclas`
 
 # examples of usage
```

### Comparing `audclas-0.0.5/pyproject.toml` & `audclas-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "audclas"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `audclas-0.0.5/src/audclas/modules/audio_mini_encoder.py` & `audclas-0.0.6/src/audclas/modules/audio_mini_encoder.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.5/src/audclas/modules/checkpoint.py` & `audclas-0.0.6/src/audclas/modules/checkpoint.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.5/src/audclas/modules/dataset.py` & `audclas-0.0.6/src/audclas/modules/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # source: https://github.com/neonbjb/DL-Art-School
 
+import os
 import numpy as np
 import pathlib
 import torch
 import torchaudio
 
-from scipy.io.wavfile import read
-
-def find_audio_files(base_path, globs=['*.wav', '*.mp3', '*.flac']):
+def find_audio_files(base_path, globs=['*.wav', '*.mp3', '*.flac', '*.ogg']):
     path = pathlib.Path(base_path)
     paths = []
     for glob in globs:
         paths.extend([str(f) for f in path.rglob(glob)])
+    # return [path for path in paths if os.path.basename(path) > '33437.ogg']
     return paths
 
 def load_wav_to_torch(full_path):
     import scipy.io.wavfile
     sampling_rate, data = scipy.io.wavfile.read(full_path)
     if data.dtype == np.int32:
         norm_fix = 2 ** 31
@@ -31,15 +31,15 @@
     audiopath = str(audiopath)
     if raw_data is not None:
         # Assume the data is wav format. SciPy's reader can read raw WAV data from a BytesIO wrapper.
         audio, lsr = load_wav_to_torch(raw_data)
     else:
         if audiopath[-4:] == '.wav':
             audio, lsr = load_wav_to_torch(audiopath)
-        elif audiopath[-5:] == '.flac':
+        elif audiopath[-5:] == '.flac' or audiopath[-4:] == '.ogg':
             import soundfile as sf
             audio, lsr = sf.read(audiopath)
             audio = torch.FloatTensor(audio)
         elif audiopath[-4:] == '.mp3':
             # https://github.com/neonbjb/pyfastmp3decoder  - Definitely worth it.
             from pyfastmp3decoder.mp3decoder import load_mp3
             audio, lsr = load_mp3(audiopath, sampling_rate)
```

### Comparing `audclas-0.0.5/src/audclas/modules/diffusion.py` & `audclas-0.0.6/src/audclas/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.5/src/audclas/modules/stft.py` & `audclas-0.0.6/src/audclas/modules/stft.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.5/src/audclas/tortoise_audio_classifier.py` & `audclas-0.0.6/src/audclas/tortoise_audio_classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,31 +30,35 @@
             from huggingface_hub import hf_hub_download
             checkpoint = hf_hub_download(checkpoint_path, 'noisy_audio_clips_classifier.pth')
         self.classifier.load_state_dict(torch.load(checkpoint))
         self.stft = TacotronSTFT()
         if torch.cuda.is_available():
             self.classifier.cuda()
             self.stft.cuda()
+        
+        self.classifier.eval()
 
     def __call__(self, file_path):
         batch_item = AudioFolderDataset.get_batch_item(file_path)
         batch = default_collate([batch_item])
         _, labels = self.classify_batch(batch)
-        return to_label(labels[0])
+        return to_label(labels[0]) if labels is not None else 'unknown'
 
     def prepare_classify_dir_job(self, audio_dir: str, batch_size=16):
         dataset = AudioFolderDataset(audio_dir)
         data_loader = DataLoader(dataset, batch_size, shuffle=False, num_workers=os.cpu_count() - 1)
         def callback():
             try:
                 for batch in data_loader:
                     max_len = max(batch['samples'])
-                    batch['clip'] = batch['clip'][:, :max_len].cuda()
+                    batch['clip'] = batch['clip'][:, :max_len]
 
                     no_hifreq_data, labels = self.classify_batch(batch)
+                    if labels is None:
+                        continue
 
                     yield [(batch['path'][b], to_label(labels[b])) for b in range(labels.size(0)) if not no_hifreq_data[b]]
                         
             except:
                 print("Exception encountered. Will ignore and continue. Exception info follows.")
         return callback, len(data_loader)
```

### Comparing `audclas-0.0.5/src/audclas.egg-info/PKG-INFO` & `audclas-0.0.6/src/audclas.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audclas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files.
 Author-email: Shmart <szprytnyd@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,23 +12,24 @@
 
 # AudClas
 
 Package that uses audio classification model extracted from neonbjb/DL-Art-School - for filtering fine audio files.
 
 # Classes
 
-Classifier returns one of 5 possible labels:
+Classifier model returns one of 6 possible labels:
 
 | label | class name |
 | ----- | ---------- |
 | 0     | fine       |
 | 1     | env_noise  |
 | 2     | music      |
 | 3     | two_voices |
 | 4     | reverb     |
+| -     | unknown    |
 
 # Installation
 
 `pip install audclas`
 
 # examples of usage
```

