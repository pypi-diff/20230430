# Comparing `tmp/AudioProcessor-0.1.4.tar.gz` & `tmp/AudioProcessor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AudioProcessor-0.1.4.tar", last modified: Fri Apr 28 18:26:38 2023, max compression
+gzip compressed data, was "AudioProcessor-0.2.0.tar", last modified: Sun Apr 30 06:17:53 2023, max compression
```

## Comparing `AudioProcessor-0.1.4.tar` & `AudioProcessor-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:26:38.479807 AudioProcessor-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-28 18:26:38.462807 AudioProcessor-0.1.4/AudioProcessor/
--rw-rw-rw-   0        0        0     9513 2023-04-28 18:24:34.000000 AudioProcessor-0.1.4/AudioProcessor/AudioProcessor.py
--rw-rw-rw-   0        0        0       42 2023-04-28 18:26:06.000000 AudioProcessor-0.1.4/AudioProcessor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:26:38.477807 AudioProcessor-0.1.4/AudioProcessor.egg-info/
--rw-rw-rw-   0        0        0     3099 2023-04-28 18:26:38.000000 AudioProcessor-0.1.4/AudioProcessor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-28 18:26:38.000000 AudioProcessor-0.1.4/AudioProcessor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:26:38.000000 AudioProcessor-0.1.4/AudioProcessor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-28 18:26:38.000000 AudioProcessor-0.1.4/AudioProcessor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 18:26:38.000000 AudioProcessor-0.1.4/AudioProcessor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3099 2023-04-28 18:26:38.478807 AudioProcessor-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 18:26:38.479807 AudioProcessor-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-04-28 18:25:51.000000 AudioProcessor-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:17:53.446519 AudioProcessor-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:17:53.433562 AudioProcessor-0.2.0/AudioProcessor/
+-rw-rw-rw-   0        0        0    10415 2023-04-30 05:56:38.000000 AudioProcessor-0.2.0/AudioProcessor/AudioProcessor.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:26:06.000000 AudioProcessor-0.2.0/AudioProcessor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:17:53.444526 AudioProcessor-0.2.0/AudioProcessor.egg-info/
+-rw-rw-rw-   0        0        0     2537 2023-04-30 06:17:53.000000 AudioProcessor-0.2.0/AudioProcessor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-30 06:17:53.000000 AudioProcessor-0.2.0/AudioProcessor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:17:53.000000 AudioProcessor-0.2.0/AudioProcessor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-30 06:17:53.000000 AudioProcessor-0.2.0/AudioProcessor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 06:17:53.000000 AudioProcessor-0.2.0/AudioProcessor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-30 06:16:26.000000 AudioProcessor-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2537 2023-04-30 06:17:53.445523 AudioProcessor-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2012 2023-04-30 06:08:56.000000 AudioProcessor-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:17:53.446519 AudioProcessor-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-04-30 06:14:31.000000 AudioProcessor-0.2.0/setup.py
```

### Comparing `AudioProcessor-0.1.4/AudioProcessor/AudioProcessor.py` & `AudioProcessor-0.2.0/AudioProcessor/AudioProcessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,213 +1,259 @@
-import speech_recognition as sr
-from gtts import gTTS
-import pyaudio
-import wave
-import webrtcvad
 import os
+import logging
 import tempfile
+import wave
+from typing import List, Tuple, Union
+
+import pyaudio
 import pydub
+import pydub.effects
+import speech_recognition as sr
+import webrtcvad
+from gtts import gTTS
+
 
 class AudioProcessor:
-    def __init__(self, frame_duration_ms=30, sample_rate=16000, chunk_size=1024, vad_mode=2):
+    def __init__(
+        self,
+        frame_duration_ms: int = 30,
+        sample_rate: int = 16000,
+        chunk_size: int = 1024,
+        vad_mode: int = 2,
+        log_level: int = logging.WARNING,
+    ):
+        """Initialize the AudioProcessor class with the given parameters."""
+        if not isinstance(frame_duration_ms, int):
+            raise TypeError("frame_duration_ms must be an integer")
+        if frame_duration_ms < 0:
+            raise ValueError("frame_duration_ms cannot be negative")
         self.frame_duration_ms = frame_duration_ms
+
+        if not isinstance(sample_rate, int):
+            raise TypeError("sample_rate must be an integer")
+        if sample_rate < 0:
+            raise ValueError("sample_rate cannot be negative")
         self.sample_rate = sample_rate
+
+        if not isinstance(chunk_size, int):
+            raise TypeError("chunk_size must be an integer")
+        if chunk_size < 0:
+            raise ValueError("chunk_size cannot be negative")
         self.chunk_size = chunk_size
+
+        if not isinstance(vad_mode, int):
+            raise TypeError("vad_mode must be an integer")
+        if vad_mode < 0 or vad_mode > 3:
+            raise ValueError("vad_mode must be an integer between 0 and 3")
         self.vad_mode = vad_mode
+
+        if not isinstance(log_level, int):
+            raise TypeError("log_level must be an integer")
+        if log_level < 0 or log_level > 50:
+            raise ValueError("log_level must be an integer between 0 and 50")
+
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(log_level)
+        handler = logging.StreamHandler()
+        handler.setFormatter(logging.Formatter(
+            "%(asctime)s %(levelname)s %(message)s"))
+        self.logger.addHandler(handler)
+
         self.recognizer = sr.Recognizer()
-        self.audio_interface = pyaudio.PyAudio()
         self.vad = webrtcvad.Vad()
-        self.vad.set_mode(vad_mode)
+        self.vad.set_mode(self.vad_mode)
+
+        # Initialize audio interface using a context manager to ensure proper cleanup
+        with pyaudio.PyAudio() as audio_interface:
+            self.audio_interface = audio_interface
+
+    def __enter__(self):
+        """Initialize the audio interface and return the AudioProcessor instance."""
+        self.audio_interface = pyaudio.PyAudio()
+        self.audio_stream = None
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Close the audio stream and terminate the audio interface upon exiting the context."""
+        if self.audio_stream is not None:
+            self.audio_stream.close()
+        self.audio_interface.terminate()
 
-    def record_audio(self, output_file_path):
+    def record_audio(self, output_file_path: str) -> bool:
         """Record audio from the microphone and save it to a .wav file."""
-        # Check if the output_file_path has a .wav extension
-        if not output_file_path.lower().endswith('.wav'):
-            print("Error: Output file path must have a .wav extension")
-            return
-        temp_file = tempfile.mktemp(".wav")
-        with sr.Microphone() as source:
-            print("Please speak now...")
-            audio = self.recognizer.listen(source)
-
-        self._save_audio_to_file(audio, temp_file)
-
-        # Convert the temporary file to the desired output format
-        with wave.open(temp_file, 'rb') as source_wave, \
-             wave.open(output_file_path, 'wb') as output_wave:
-            output_wave.setparams(source_wave.getparams())
-            output_wave.writeframes(source_wave.readframes(source_wave.getnframes()))
+        if not output_file_path.lower().endswith(".wav"):
+            self.logger.error("Output file path must have a .wav extension")
+            return False
+
+        with tempfile.NamedTemporaryFile(suffix=".wav", delete=False) as f:
+            temp_file = f.name
+
+        try:
+            with sr.Microphone() as source:
+                self.logger.info("Please speak now...")
+                audio = self.recognizer.listen(source)
+
+            self._save_audio_to_file(audio, temp_file)
+
+            with wave.open(temp_file, "rb") as source_wave, \
+                    wave.open(output_file_path, "wb") as output_wave:
+                output_wave.setparams(source_wave.getparams())
+                output_wave.writeframes(
+                    source_wave.readframes(source_wave.getnframes()))
 
-        print(f"Saved audio file: {output_file_path}")
-        os.remove(temp_file)
+            self.logger.info(f"Saved audio file: {output_file_path}")
+
+            os.remove(temp_file)
+
+        except sr.RequestError as e:
+            self.logger.error(
+                f"Failed to record audio due to a request error: {e}", exc_info=True)
+            return False
+        except sr.WaitTimeoutError:
+            self.logger.error(
+                "No audio detected within the timeout period", exc_info=True)
+            return False
+        except ValueError as e:
+            self.logger.error(
+                f"Failed to record audio due to an invalid argument: {str(e)}", exc_info=True)
+            return False
+        except Exception as e:
+            self.logger.error(
+                f"Failed to record audio due to an unexpected error: {e}", exc_info=True)
+            return False
+        return True
 
     def _save_audio_to_file(self, audio, file_path):
-        """Save the audio data to a .wav file."""
-        with open(file_path, "wb") as f:
+        """Save a SpeechRecognition AudioData object to a file."""
+        with open(file_path, 'wb') as f:
             f.write(audio.get_wav_data())
 
-    def audio_to_text(self, audio_file_path, **kwargs):
-        """Transcribe an audio file."""
+    def audio_to_text(self, audio_file_path: str, preprocess: bool = False, show_all: bool = False) -> Union[str, List[str]]:
+        """Convert the given audio file to text using Google Speech Recognition."""
         if not os.path.exists(audio_file_path):
-            print(f"Error: File not found ({audio_file_path})")
+            self.logger.error(f"Error: File not found ({audio_file_path})")
             return ""
-        file_ext = audio_file_path.split(".")[-1].lower()
 
-        if file_ext not in ["wav", "mp3", "flac"]:
-            print("Error: unsupported audio file format ({})".format(file_ext))
+        file_ext = os.path.splitext(audio_file_path)[-1].lower()
+
+        if file_ext not in [".wav", ".mp3", ".flac"]:
+            self.logger.error(
+                f"Error: unsupported audio file format ({file_ext})")
             return ""
 
         with sr.AudioFile(audio_file_path) as source:
             audio_text = self.recognizer.listen(source)
 
-        return self._process_audio_text(audio_text, **kwargs)
+        return self._process_audio_text(audio_text, preprocess=preprocess, show_all=show_all)
 
-    def _process_audio_text(self, audio_text, **kwargs):
-        """Process the audio_text and return the transcribed text."""
-        preprocess = kwargs.get("preprocess", False)
+    def _process_audio_text(self, audio_text, preprocess: bool = False, show_all: bool = False) -> Union[str, List[str]]:
+        """Preprocess the audio data and send it to Google Speech Recognition."""
         if preprocess:
-            frames = self._generate_frames(audio_text.get_raw_data(), self.sample_rate, self.frame_duration_ms)
-            segments = self._collect_voiced_segments(frames, self.vad, self.sample_rate)
+            frames = self._generate_frames(
+                audio_text.get_raw_data(), self.sample_rate, self.frame_duration_ms)
+            segments = self._collect_voiced_segments(
+                frames, self.vad, self.sample_rate)
             audio_text = b"".join(segments)
 
-        show_all = kwargs.get("show_all", False)
         try:
-            response = self.recognizer.recognize_google(audio_text, show_all=show_all)
+            response = self.recognizer.recognize_google(
+                audio_text, show_all=show_all)
             return self._parse_recognition_response(response, show_all)
         except (sr.UnknownValueError, sr.RequestError) as e:
-            print("Error: {}".format(e))
+            self.logger.error(f"Error: {e}")
             return ""
 
-    def _parse_recognition_response(self, response, show_all):
-        """Parse the response from the speech recognizer."""
+    def _parse_recognition_response(self, response, show_all: bool) -> Union[str, List[str]]:
+        """Parse the response from Google Speech Recognition and return the result as text."""
         if show_all:
-            text = [alternative['transcript'] for alternative in response['alternative']]
-            confidence = [alternative['confidence'] for alternative in response['alternative']]
-            print("Recognized text: {}".format(text))
-            print("Confidence scores: {}".format(confidence))
+            text = [alternative['transcript']
+                    for alternative in response['alternative']]
         else:
             text = response
-            print("Recognized text: {}".format(text))
 
         return text
 
-    def _process_recognized_audio(self, audio):
-        """Process the recognized audio and return the transcribed text."""
-        try:
-            text = self.recognizer.recognize_google(audio)
-            print("Recognized text: {}".format(text))
-        except sr.UnknownValueError as e:
-            print("Error: UnknownValueError - {}".format(e))
-            text = ""
-        except sr.RequestError as e:
-            print("Error: RequestError - {}".format(e))
-            text = ""
-
-        return text
-
-    def text_to_audio(self, text, audio_file_path, lang='en', volume=1.0, sample_rate=44100, bit_depth=16):
-        """Convert text to an audio file and play it."""
-        # Check if the output_file_path has a .wav extension
-        if not audio_file_path.lower().endswith('.wav'):
-            print("Error: Output file path must have a .wav extension")
+    def text_to_audio(
+        self,
+        text: str,
+        audio_file_path: str,
+        lang: str = 'en',
+        volume: float = 1.0,
+        sample_rate: int = 44100,
+        bit_depth: int = 16,
+    ) -> None:
+        """Convert the given text to an audio file using Google Text-to-Speech."""
+        if not audio_file_path.lower().endswith(".wav"):
+            self.logger.error("Output file path must have a .wav extension")
             return
+
         try:
             audio = gTTS(text=text, lang=lang, slow=False)
-            audio = audio.get_audio_data(rate=sample_rate, 
-                                        # multiply by 2 since the bit depth is in bytes and there are 2 bytes per sample for WAV files
-                                        width=bit_depth*2,  
-                                        normalize=False)
-            with wave.open(audio_file_path, 'wb') as wf:
-                wf.setnchannels(1)  # mono audio
-                wf.setsampwidth(bit_depth)  # bit depth in bytes
+            audio = audio.get_audio_data(
+                rate=sample_rate, width=bit_depth // 8, normalize=False)
+            with wave.open(audio_file_path, "wb") as wf:
+                wf.setnchannels(1)
+                wf.setsampwidth(bit_depth // 8)
                 wf.setframerate(sample_rate)
                 wf.writeframes(audio)
-            print(f"Saved audio file: {audio_file_path}")
+
+            self.logger.info(f"Saved audio file: {audio_file_path}")
+
         except Exception as e:
-            print(f"Error: {e}")
+            self.logger.error(f"Error: {e}")
             return
 
-        self._play_audio_file(audio_file_path, volume, normalize=True)
+        self._play_audio_file(audio_file_path,
+                              volume=volume)
 
-    def _play_audio_file(self, audio_file_path, volume=1.0, normalize=False):
-        """Play the audio file with the specified volume and optional normalization."""
+    def play_audio_file(self, audio_file_path: str, volume: float = 1.0) -> None:
+        """Play a given audio file, adjusting the volume as necessary."""
         if not os.path.exists(audio_file_path):
-            print(f"Error: File not found ({audio_file_path})")
+            self.logger.error(f"Error: File not found ({audio_file_path})")
             return
-        try:
-            with wave.open(audio_file_path, 'rb') as wf:
-                stream = self.audio_interface.open(format=self.audio_interface.get_format_from_width(wf.getsampwidth()),
-                                                    channels=wf.getnchannels(),
-                                                    rate=wf.getframerate(),
-                                                    output=True)
-                # Read and play the audio file in chunks
-                data = wf.readframes(self.chunk_size)
-                while data:
-                    adjusted_data = bytearray()
-                    for i in range(0, len(data), 2):
-                        audio_sample = int.from_bytes(data[i:i + 2], byteorder='little')
-                        audio_sample = int(audio_sample * volume)
-                        audio_sample = min(max(audio_sample, -32768), 32767)
-                        adjusted_data += audio_sample.to_bytes(2, byteorder='little')
-                    if normalize:
-                        audio_segment = pydub.AudioSegment(data=adjusted_data, sample_width=wf.getsampwidth(),
-                                                        frame_rate=wf.getframerate(), channels=wf.getnchannels())
-                        normalized_audio_segment = pydub.effects.normalize(audio_segment)
-                        normalized_data = normalized_audio_segment.raw_data
-                        stream.write(normalized_data)
-                    else:
-                        stream.write(bytes(adjusted_data))  # Convert bytearray to bytes
-                    data = wf.readframes(self.chunk_size)
-
-                # Close the stream
-                stream.stop_stream()
-                stream.close()
-        except Exception as e:
-            print(f"Error: {e}")
 
+        audio_segment = pydub.AudioSegment.from_wav(audio_file_path)
+        audio_segment = audio_segment + (20 * (volume - 1))
 
-    def _generate_frames(self, audio, sample_rate, frame_duration_ms):
-        frame_duration_s = frame_duration_ms / 1000
-        frame_size = int(frame_duration_s * sample_rate)
+        playback_temp = tempfile.NamedTemporaryFile(suffix=".wav")
+        audio_segment.export(playback_temp.name, format="wav")
+        playback_temp.seek(0)
+
+        with wave.open(playback_temp.name, "rb") as audio_file:
+            audio_stream = self.audio_interface.open(
+                format=self.audio_interface.get_format_from_width(
+                    audio_file.getsampwidth()),
+                channels=audio_file.getnchannels(),
+                rate=audio_file.getframerate(),
+                output=True
+            )
+
+            audio_data = audio_file.readframes(self.chunk_size)
+            while audio_data:
+                audio_stream.write(audio_data)
+                audio_data = audio_file.readframes(self.chunk_size)
+
+            audio_stream.stop_stream()
+            audio_stream.close()
+
+        playback_temp.close()
+
+    def _generate_frames(self, audio_data: bytes, sample_rate: int, frame_duration_ms: int) -> List[bytes]:
+        """Generate frames from raw audio data for Voice Activity Detection (VAD)."""
+        n = int(sample_rate * (frame_duration_ms / 1000.0) * 2)
         offset = 0
-        while offset < len(audio):
-            yield audio[offset:offset + frame_size]
-            offset += frame_size
-
-
-    def _collect_voiced_segments(self, frames, vad, sample_rate, ratio=2):
-        voiced_frames = [frame for frame in frames if vad.is_speech(frame.tobytes(), sample_rate)]
-
-        segments = []
-        start = 0
-        while start < len(voiced_frames):
-            end = start + 1
-            while end < len(voiced_frames) and end - start < ratio:
-                segment = b"".join(voiced_frames[start:end])
-                segments.append(segment)
-                end += 1
-            start = end
-
-        return segments
-
-# def main():
-#     audio_processor = AudioProcessor()
-
-#     # Test 1: Record audio from the microphone and save it to a .wav file
-#     print("\nTest 1: Record audio from the microphone and save it to a .wav file")
-#     output_audio_file_path = "recorded_audio.wav"
-#     audio_processor.record_audio(output_audio_file_path)
-
-#     # Test 2: Transcribe an audio file
-#     print("\nTest 2: Transcribe an audio file")
-#     audio_file_path = "Audio.wav"
-#     transcribed_text = audio_processor.audio_to_text(audio_file_path)
-#     print("Transcribed text: {}".format(transcribed_text))
-
-#     # Test 3: Text to audio and play it
-#     print("\nTest 3: Text to audio and play it")
-#     text = "This is a test for text to audio conversion."
-#     output_audio_file_path = "output_audio.wav"
-#     audio_processor.text_to_audio(text, output_audio_file_path)
-
-# if __name__ == "__main__":
-#     main()
+        timestamp = 0.0
+        duration = float(n) / sample_rate / 2.0
+        frames = []
+        while offset + n < len(audio_data):
+            frames.append(audio_data[offset:offset + n])
+            timestamp += duration
+            offset += n
+        return frames
+
+    def _collect_voiced_segments(self, frames: List[bytes], vad: webrtcvad.Vad, sample_rate: int) -> List[bytes]:
+        """Collect voiced segments from the frames using Voice Activity Detection (VAD)."""
+        voiced_segments = []
+        for frame in frames:
+            if vad.is_speech(frame, sample_rate):
+                voiced_segments.append(frame)
+        return voiced_segments
```

### Comparing `AudioProcessor-0.1.4/AudioProcessor.egg-info/PKG-INFO` & `AudioProcessor-0.2.0/AudioProcessor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,83 @@
 Metadata-Version: 2.1
 Name: AudioProcessor
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python package for recording, transcribing, and converting audio
 Home-page: https://github.com/TheWordSmith123/Audio-Processor
 Author: Andrew Horvath
 Author-email: drewfhorvath@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 AudioProcessor
 ==============
 
-`AudioProcessor` is a Python class that provides functionality for recording audio, transcribing audio to text, and converting text to audio.
+AudioProcessor is a Python library that provides a simple interface to perform various audio processing tasks such as recording, voice-to-text conversion, text-to-voice conversion, and audio playback.
 
-Class Methods
--------------
+Installation
+------------
 
-### `__init__(self, frame_duration_ms=30, sample_rate=16000, chunk_size=1024, vad_mode=2)`
+To use AudioProcessor, make sure you have the following packages installed:
 
-Initialize the `AudioProcessor` class.
+*   pyaudio
+*   pydub
+*   pydub.effects
+*   speech\_recognition
+*   webrtcvad
+*   gtts
 
-**Parameters:**
+You can install these packages using pip:
 
-*   `frame_duration_ms`: Frame duration in milliseconds (default: 30 ms)
-*   `sample_rate`: Audio sample rate (default: 16000 Hz)
-*   `chunk_size`: Audio chunk size for processing (default: 1024)
-*   `vad_mode`: Voice Activity Detection (VAD) mode (default: 2)
+`pip install pyaudio pydub speechrecognition webrtcvad gtts`
 
-### `record_audio(self, output_file_path)`
+Usage
+-----
 
-Record audio from the microphone and save it to a .wav file.
+To use AudioProcessor, simply import the `AudioProcessor` class and create an instance:
 
-**Parameters:**
+`from audio_processor import AudioProcessor  processor = AudioProcessor()`
 
-*   `output_file_path`: Output file path for the recorded audio
+### Recording audio
 
-### `audio_to_text(self, audio_file_path, **kwargs)`
+To record audio, use the `record_audio` method:
 
-Transcribe an audio file.
+`processor.record_audio("output_file.wav")`
 
-**Parameters:**
+This method records audio from the microphone and saves it to a .wav file.
 
-*   `audio_file_path`: Input audio file path
-*   `**kwargs`: Keyword arguments for preprocessing and other options
+### Voice-to-text conversion
 
-**Returns:**
+To convert an audio file to text, use the `audio_to_text` method:
 
-*   Transcribed text as a string
+`text = processor.audio_to_text("input_file.wav")`
 
-### `text_to_audio(self, text, audio_file_path, lang='en', volume=1.0, sample_rate=44100, bit_depth=16)`
+### Text-to-voice conversion
 
-Convert text to an audio file and play it.
+To convert text to an audio file, use the `text_to_audio` method:
 
-**Parameters:**
+`processor.text_to_audio("Hello world!", "output_file.wav")`
 
-*   `text`: Input text to convert to audio
-*   `audio_file_path`: Output audio file path
-*   `lang`: Language of the text (default: 'en')
-*   `volume`: Volume level of the output audio (default: 1.0)
-*   `sample_rate`: Audio sample rate (default: 44100 Hz)
-*   `bit_depth`: Audio bit depth (default: 16)
+### Audio playback
 
-Private Methods
----------------
+To play an audio file, use the `play_audio_file` method:
 
-These methods are used internally by the class and should not be called directly by the user.
+`processor.play_audio_file("input_file.wav")`
 
-### `_save_audio_to_file(self, audio, file_path)`
+Class Parameters
+----------------
 
-Save the audio data to a .wav file.
+The `AudioProcessor` class can be initialized with the following parameters:
 
-### `_process_audio_text(self, audio_text, **kwargs)`
+*   `frame_duration_ms`: (int) Frame duration in milliseconds for Voice Activity Detection (default: 30)
+*   `sample_rate`: (int) Sample rate of the audio in Hz (default: 16000)
+*   `chunk_size`: (int) Chunk size for audio playback (default: 1024)
+*   `vad_mode`: (int) Voice Activity Detection mode, an integer between 0 and 3 (default: 2)
+*   `log_level`: (int) Logging level, an integer between 0 and 50 (default: logging.WARNING)
 
-Process the audio\_text and return the transcribed text.
+License
+-------
 
-### `_parse_recognition_response(self, response, show_all)`
-
-Parse the response from the speech recognizer.
-
-### `_process_recognized_audio(self, audio)`
-
-Process the recognized audio and return the transcribed text.
-
-### `_play_audio_file(self, audio_file_path, volume=1.0, normalize=False)`
-
-Play the audio file with the specified volume and optional normalization.
-
-### `_generate_frames(self, audio, sample_rate, frame_duration_ms)`
-
-Generate audio frames from raw audio data.
-
-### `_collect_voiced_segments(self, frames, vad, sample_rate, ratio=2)`
-
-Collect voiced segments from audio frames using the Voice Activity Detection (VAD) algorithm.
+This project is licensed under the MIT License.
```

### Comparing `AudioProcessor-0.1.4/PKG-INFO` & `AudioProcessor-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,83 @@
 Metadata-Version: 2.1
 Name: AudioProcessor
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python package for recording, transcribing, and converting audio
 Home-page: https://github.com/TheWordSmith123/Audio-Processor
 Author: Andrew Horvath
 Author-email: drewfhorvath@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 AudioProcessor
 ==============
 
-`AudioProcessor` is a Python class that provides functionality for recording audio, transcribing audio to text, and converting text to audio.
+AudioProcessor is a Python library that provides a simple interface to perform various audio processing tasks such as recording, voice-to-text conversion, text-to-voice conversion, and audio playback.
 
-Class Methods
--------------
+Installation
+------------
 
-### `__init__(self, frame_duration_ms=30, sample_rate=16000, chunk_size=1024, vad_mode=2)`
+To use AudioProcessor, make sure you have the following packages installed:
 
-Initialize the `AudioProcessor` class.
+*   pyaudio
+*   pydub
+*   pydub.effects
+*   speech\_recognition
+*   webrtcvad
+*   gtts
 
-**Parameters:**
+You can install these packages using pip:
 
-*   `frame_duration_ms`: Frame duration in milliseconds (default: 30 ms)
-*   `sample_rate`: Audio sample rate (default: 16000 Hz)
-*   `chunk_size`: Audio chunk size for processing (default: 1024)
-*   `vad_mode`: Voice Activity Detection (VAD) mode (default: 2)
+`pip install pyaudio pydub speechrecognition webrtcvad gtts`
 
-### `record_audio(self, output_file_path)`
+Usage
+-----
 
-Record audio from the microphone and save it to a .wav file.
+To use AudioProcessor, simply import the `AudioProcessor` class and create an instance:
 
-**Parameters:**
+`from audio_processor import AudioProcessor  processor = AudioProcessor()`
 
-*   `output_file_path`: Output file path for the recorded audio
+### Recording audio
 
-### `audio_to_text(self, audio_file_path, **kwargs)`
+To record audio, use the `record_audio` method:
 
-Transcribe an audio file.
+`processor.record_audio("output_file.wav")`
 
-**Parameters:**
+This method records audio from the microphone and saves it to a .wav file.
 
-*   `audio_file_path`: Input audio file path
-*   `**kwargs`: Keyword arguments for preprocessing and other options
+### Voice-to-text conversion
 
-**Returns:**
+To convert an audio file to text, use the `audio_to_text` method:
 
-*   Transcribed text as a string
+`text = processor.audio_to_text("input_file.wav")`
 
-### `text_to_audio(self, text, audio_file_path, lang='en', volume=1.0, sample_rate=44100, bit_depth=16)`
+### Text-to-voice conversion
 
-Convert text to an audio file and play it.
+To convert text to an audio file, use the `text_to_audio` method:
 
-**Parameters:**
+`processor.text_to_audio("Hello world!", "output_file.wav")`
 
-*   `text`: Input text to convert to audio
-*   `audio_file_path`: Output audio file path
-*   `lang`: Language of the text (default: 'en')
-*   `volume`: Volume level of the output audio (default: 1.0)
-*   `sample_rate`: Audio sample rate (default: 44100 Hz)
-*   `bit_depth`: Audio bit depth (default: 16)
+### Audio playback
 
-Private Methods
----------------
+To play an audio file, use the `play_audio_file` method:
 
-These methods are used internally by the class and should not be called directly by the user.
+`processor.play_audio_file("input_file.wav")`
 
-### `_save_audio_to_file(self, audio, file_path)`
+Class Parameters
+----------------
 
-Save the audio data to a .wav file.
+The `AudioProcessor` class can be initialized with the following parameters:
 
-### `_process_audio_text(self, audio_text, **kwargs)`
+*   `frame_duration_ms`: (int) Frame duration in milliseconds for Voice Activity Detection (default: 30)
+*   `sample_rate`: (int) Sample rate of the audio in Hz (default: 16000)
+*   `chunk_size`: (int) Chunk size for audio playback (default: 1024)
+*   `vad_mode`: (int) Voice Activity Detection mode, an integer between 0 and 3 (default: 2)
+*   `log_level`: (int) Logging level, an integer between 0 and 50 (default: logging.WARNING)
 
-Process the audio\_text and return the transcribed text.
+License
+-------
 
-### `_parse_recognition_response(self, response, show_all)`
-
-Parse the response from the speech recognizer.
-
-### `_process_recognized_audio(self, audio)`
-
-Process the recognized audio and return the transcribed text.
-
-### `_play_audio_file(self, audio_file_path, volume=1.0, normalize=False)`
-
-Play the audio file with the specified volume and optional normalization.
-
-### `_generate_frames(self, audio, sample_rate, frame_duration_ms)`
-
-Generate audio frames from raw audio data.
-
-### `_collect_voiced_segments(self, frames, vad, sample_rate, ratio=2)`
-
-Collect voiced segments from audio frames using the Voice Activity Detection (VAD) algorithm.
+This project is licensed under the MIT License.
```

### Comparing `AudioProcessor-0.1.4/setup.py` & `AudioProcessor-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="AudioProcessor",
-    version="0.1.4",
+    version="0.2.0",
     packages=["AudioProcessor"],
     install_requires=[
         "speechrecognition",
         "gtts",
         "pyaudio",
         "wave",
         "webrtcvad",
```

