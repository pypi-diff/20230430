# Comparing `tmp/Scopul-1.0.4.tar.gz` & `tmp/Scopul-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scopul-1.0.4.tar", last modified: Sat Apr 15 15:08:01 2023, max compression
+gzip compressed data, was "Scopul-1.1.4.tar", last modified: Sun Apr 30 02:02:10 2023, max compression
```

## Comparing `Scopul-1.0.4.tar` & `Scopul-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.603704 Scopul-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      873 2023-04-15 15:08:01.604701 Scopul-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.4/README.md
--rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.4/long_desc.md
--rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      730 2023-04-15 15:08:01.605697 Scopul-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.562908 Scopul-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.589724 Scopul-1.0.4/src/Scopul/
--rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.4/src/Scopul/Sequence.py
--rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.4/src/Scopul/Tempo.py
--rw-rw-rw-   0        0        0      663 2023-04-15 00:33:29.000000 Scopul-1.0.4/src/Scopul/TimeSignature.py
--rw-rw-rw-   0        0        0      470 2023-04-15 14:56:04.000000 Scopul-1.0.4/src/Scopul/__init__.py
--rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.4/src/Scopul/config_musescore.py
--rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.4/src/Scopul/conversions.py
--rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.4/src/Scopul/helpers.py
--rw-rw-rw-   0        0        0    15321 2023-04-15 15:07:35.000000 Scopul-1.0.4/src/Scopul/scopul.py
--rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.4/src/Scopul/scopul_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.602707 Scopul-1.0.4/src/Scopul.egg-info/
--rw-rw-rw-   0        0        0      873 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 02:02:10.306022 Scopul-1.1.4/
+-rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      873 2023-04-30 02:02:10.307025 Scopul-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3163 2023-04-28 02:15:34.000000 Scopul-1.1.4/README.md
+-rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.1.4/long_desc.md
+-rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-30 02:02:10.309020 Scopul-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 02:02:10.226951 Scopul-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 02:02:10.277508 Scopul-1.1.4/src/Scopul/
+-rw-rw-rw-   0        0        0     2066 2023-04-29 00:49:09.000000 Scopul-1.1.4/src/Scopul/ChordProgression.py
+-rw-rw-rw-   0        0        0     4455 2023-04-27 02:44:37.000000 Scopul-1.1.4/src/Scopul/MusicalElements.py
+-rw-rw-rw-   0        0        0    15176 2023-04-29 00:25:00.000000 Scopul-1.1.4/src/Scopul/Sequence.py
+-rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.1.4/src/Scopul/Tempo.py
+-rw-rw-rw-   0        0        0      663 2023-04-15 00:33:29.000000 Scopul-1.1.4/src/Scopul/TimeSignature.py
+-rw-rw-rw-   0        0        0      505 2023-04-27 02:45:17.000000 Scopul-1.1.4/src/Scopul/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.1.4/src/Scopul/config_musescore.py
+-rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.1.4/src/Scopul/conversions.py
+-rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.1.4/src/Scopul/helpers.py
+-rw-rw-rw-   0        0        0    15943 2023-04-29 00:16:02.000000 Scopul-1.1.4/src/Scopul/scopul.py
+-rw-rw-rw-   0        0        0      560 2023-04-27 03:08:07.000000 Scopul-1.1.4/src/Scopul/scopul_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:02:10.303497 Scopul-1.1.4/src/Scopul.egg-info/
+-rw-rw-rw-   0        0        0      873 2023-04-30 02:02:10.000000 Scopul-1.1.4/src/Scopul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-30 02:02:10.000000 Scopul-1.1.4/src/Scopul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 02:02:10.000000 Scopul-1.1.4/src/Scopul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-30 02:02:10.000000 Scopul-1.1.4/src/Scopul.egg-info/top_level.txt
```

### Comparing `Scopul-1.0.4/LICENSE` & `Scopul-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.4/PKG-INFO` & `Scopul-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.4
+Version: 1.1.4
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Scopul-1.0.4/README.md` & `Scopul-1.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,34 +36,40 @@
 🟡 = In progress
 
 🟠 = To-Do
 
 🟢 = Done
 
 ### Things to look forward in the next major release, any suggestions will be appreciated
+- Deletion of elements (Only addition is currently supported)🟠
+- Create and add parts, consisting of multiple other Scopul Musical Elements🟠
 - Chord extraction: Allow the extraction of chord progressions from the MIDI file.🟠
 - Key detection: Implement a function to detect the key of the MIDI file.🟠
 - Melody extraction: Allow the extraction of the melody from the MIDI file.🟠
 - Harmonic analysis: Provide harmonic analysis of the MIDI file by identifying chords and their progressions.🟠
 
 ### Things for the distant future, any suggestions will be appreciated
 - Drum track extraction: Allow the extraction of the drum track from the MIDI file.🟠
 - Quantization: Implement a function to quantize the notes in the MIDI file to a particular grid size.🟠
 - MIDI file validation: Implement a function to validate the structure of the MIDI file and detect any errors.🟠
 - Export to other formats: Allow the export of the MIDI data to other formats such as CSV, JSON, or XML.🟠
 
+## Bugs
+- A lot of the MIDI to PDF conversions are still throwing errors
+- PDFs and XMLs are not generating with title
+
 ## Links
 Documentation - [https://swayamsahoo11742.github.io/](https://swayamsahoo11742.github.io/)
 
 Documentation Source Code - [https://github.com/SwayamSahoo11742/SwayamSahoo11742.github.io/](https://github.com/SwayamSahoo11742/SwayamSahoo11742.github.io/)
 
 PyPi - [https://pypi.org/project/scopul/](https://pypi.org/project/scopul/)
 
 GitHub - [https://github.com/SwayamSahoo11742/Scopul/](https://github.com/SwayamSahoo11742/Scopul/)
 
 ## Credits
 Thanks to [Music21](https://web.mit.edu/music21/doc/) and [MuseScore](https://musescore.org/en/download) for making this possible
 
 ## Contact or Help us!
-If you encounter any bugs, kindly send me an email at swayamsa01@gmail.com. If you have any suggestions or would like to contribute to the improvement of the code, including efficiency and best practices, feel free to reach out to me via email or create a pull request. I most likely won’t be actively adding and developing this project, but I will still implement any sugegstions that are fit.
+If you have any questions, kindly send an email to swayamsa01@gmail.com. If you have any suggestions or would like to contribute to the improvement of the code, including efficiency and best practices, feel free to reach out to me via email or create a pull request. I most likely won’t be actively adding and developing this project, but I will still implement any sugegstions that are fit.
 
 Thank you very much!
```

### Comparing `Scopul-1.0.4/setup.cfg` & `Scopul-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 636f 7075 6c0d 0a76 6572 7369   = Scopul..versi
-00000020: 6f6e 203d 2031 2e30 2e34 0d0a 6175 7468  on = 1.0.4..auth
+00000020: 6f6e 203d 2031 2e31 2e34 0d0a 6175 7468  on = 1.1.4..auth
 00000030: 6f72 203d 2053 7761 7961 6d20 5361 686f  or = Swayam Saho
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 7377 6179 616d 7361 3031 4067 6d61  = swayamsa01@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 4120 4d49 4449 2066 696c  ion = A MIDI fil
 00000080: 6520 616e 616c 797a 6572 2077 6869 6368  e analyzer which
 00000090: 2061 6c6c 6f77 7320 796f 7520 746f 2067   allows you to g
```

### Comparing `Scopul-1.0.4/src/Scopul/Sequence.py` & `Scopul-1.1.4/src/Scopul/Sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,124 @@
 import music21
-from Scopul.scopul_exception import InvalidMusicElementError
+from Scopul.MusicalElements import Note, Rest, Chord
+from Scopul.ChordProgression import ChordProgression
+from Scopul.scopul_exception import InvalidMusicElementError, PercussionChordifyError
 from Scopul.conversions import note_to_number
 from collections.abc import Iterable
 from Scopul.helpers import sublist
+from Scopul import TimeSignature, Tempo
 import re
+from copy import deepcopy
 
 
 class Part:
     """A class representing the a part in a score.
     EX: A flute part
+
+     Args
+        part: Can be an iterbale consisting of Scopul musical elements OR a music21 part object
     """
 
-    def __init__(self, part) -> None:
-        self._part = part
-        self.name = part.partName
+    def __init__(self, part: Iterable | music21.stream.Part) -> None:
+        if not isinstance(part, music21.stream.Part):
+            p = music21.stream.Part()
+            for ele in part:
+                if isinstance(ele, Note):
+                    p.append(music21.note.Note(ele.name, velocity=ele.velocity, duration=music21.duration.Duration(ele.length)))
+                if isinstance(ele, Rest):
+                    p.append(music21.note.Rest(ele.length))
+                if isinstance(ele, Chord):
+                    c = music21.chord.Chord()
+                    for nt in ele.notes:
+                        c.add(music21.note.Note(nt.name, velocity=nt.velocity, duration=music21.duration.Duration(nt.length)))
+                    p.append(c)
+
+            self._part = p 
+            self.name = p.partName
+        else:
+            self._part= part
+            self.name = part.partName
 
     @property
     def sequence(self):
         sequence = []
         # Looping through the part
-        for element in self._part.recurse():
-            # Setting the class and appending depending on the type of symbol
-            if isinstance(element, music21.note.Note):
-                sequence.append(Note(element))
-            elif isinstance(element, music21.chord.Chord):
-                sequence.append(Chord(element))
-            elif isinstance(element, music21.note.Rest):
-                sequence.append(Rest(element))
-        
+        if isinstance(self._part, music21.stream.Part):
+            for element in self._part.recurse():
+                # Setting the class and appending depending on the type of symbol
+                if isinstance(element, music21.note.Note):
+                    sequence.append(Note(element))
+                elif isinstance(element, music21.chord.Chord):
+                    sequence.append(Chord(element))
+                elif isinstance(element, music21.note.Rest):
+                    sequence.append(Rest(element))
         return sequence
 
 
+    # =========================================================================================== METHODS ====================================================================================================================
+    def get_chord_progression(self):
+        try:
+            return ChordProgression(self)
+        except AttributeError:
+            raise PercussionChordifyError("Cannot get chord progression for Percussion part")
+        
+    def delete(self, index: int = 0):
+        """Deletes a object at the index of self.sequence
+            Args:
+                index: an in
+        """
+        self._part.pop(index)
+        
+    def insert(self, element, measure_number: int = None, position: int = 0):
+        """Inserts a musical element into the current part at a certain location
+
+            Args:
+                element: a Note, Rest or Chord object
+                measure_number: an int
+                position: an int, the offset of the note within the measure
+            Returns:
+                None
+            
+        """
+        if not isinstance(element, (Note, Rest, Chord, TimeSignature, Tempo)):
+            raise ValueError(f"{type(element)} is not a Scopul musical element (Notes, Rests, Chords, Tempo, TimeSignature)")
+        
+        if not measure_number:
+            # If no measure number is provided, add the element to the last measure in the part
+            measure_number = self.sequence[-1].measure
+
+        new_part = music21.stream.Stream()
+
+        # copying into new part with modified time
+        element_added = False
+        for measure in self._part.getElementsByClass("Measure"):
+
+            if measure.number == measure_number and not element_added:
+                measure.insert(position, deepcopy(element.music21))
+                element_added = True
+
+            new_part.append(measure)
+
+        new_part = new_part.makeMeasures()
+        self._part.replace(self._part, new_part)
 
     # Note list
-    def get_notes(self, seq: list) -> list:
+    def get_notes(self) -> list:
         """Retrieves all the notes in a given sequence
 
         Args:
             seq: a list of Scopul musical symbols (Rest, Chord, Note)
 
         Returns:
             a list of note objects extracted from the list
 
         Raises:
             InvalidMusicElementError: if found a type that is not Rest, Note or Chord
         """
+        seq = self.sequence
         # Notes list
         notes = []
 
         # If not a iterable, raise error
         if not isinstance(seq, Iterable):
             raise TypeError(
                 "Not an iterable. Include a iterable object of Scopul Rests, Chords or Note"
@@ -64,31 +134,32 @@
             # Append to list
             if isinstance(element, Note):
                 notes.append(element)
 
         return notes
 
     # Gets a count of notes
-    def get_note_count(self, seq: list) -> int:
+    def get_note_count(self) -> int:
         """Retrieves the number of notes"""
-        return len(self.get_notes(seq))
+        return len(self.get_notes())
 
     # Note list
-    def get_rests(self, seq: list) -> list:
+    def get_rests(self) -> list:
         """Retrieves all the notes in a given sequence
 
         Args:
             seq: a list of Scopul musical symbols (Rest, Chord, Note)
 
         Returns:
             a list of rest objects extracted from the list
 
         Raises:
             InvalidMusicElementError: if found a type that is not Rest, Note or Chord
         """
+        seq = self.sequence
         # rests list
         rests = []
 
         # If not a iterable, raise error
         if not isinstance(seq, Iterable):
             raise TypeError(
                 "Not an iterable. Include a iterable object of Scopul Rests, Chords or Note"
@@ -104,32 +175,33 @@
             # Append to list
             if isinstance(element, Note):
                 rests.append(element)
 
         return rests
 
     # Gets a count of rests
-    def get_rest_count(self, seq: list) -> int:
+    def get_rest_count(self) -> int:
         """Retrieves the number of rests"""
-        return len(self.get_rests(seq))
+        return len(self.get_rests())
 
         # Note list
 
-    def get_chords(self, seq: list) -> list:
+    def get_chords(self) -> list:
         """Retrieves all the chords in a given sequence
 
         Args:
             seq: a list of Scopul musical symbols (Rest, Chord, Note)
 
         Returns:
             a list of chords objects extracted from the list
 
         Raises:
             InvalidMusicElementError: if found a type that is not Rest, Note or Chord
         """
+        seq = self.sequence
         # chords list
         chords = []
 
         # If not a iterable, raise error
         if not isinstance(seq, Iterable):
             raise TypeError(
                 "Not an iterable. Include a iterable object of Scopul Rests, Chords or Note"
@@ -145,17 +217,17 @@
             # Append to list
             if isinstance(element, Note):
                 chords.append(element)
 
         return chords
 
     # Gets a count of notes
-    def get_chord_count(self, seq: list) -> int:
+    def get_chord_count(self) -> int:
         """Retrieves the number of notes"""
-        return len(self.get_chords(seq))
+        return len(self.get_chords())
 
     def get_measure(self, measures: int | list):
         """Fetches the contents of a measure.
 
         Retrieves about chords, notes and rest objects in the sequence
 
         Args:
@@ -201,26 +273,27 @@
 
         # Incorrect type
         else:
             raise TypeError(
                 f"get_measure only accepts int or iterable, instead got {type(measures)}"
             )
 
-    def get_highest_note(self, seq: list):
+    def get_highest_note(self):
         """Retrieves all the chords in a given sequence
 
         Args:
             seq: a list of Scopul musical symbols (Rest, Chord, Note)
 
         Returns:
             a list of chords objects extracted from the list
 
         Raises:
             InvalidMusicElementError: if found a type that is not Rest, Note or Chord
         """
+        seq = self.sequence
         # highest note
         highest = 0
 
         # If not a list, raise error
         if not isinstance(seq, Iterable):
             raise TypeError(
                 "Not a list. Include a list of Scopul Rests, Chords or Note"
@@ -333,149 +406,7 @@
             if match:
                 final_list.append(sequence)
 
         # Return the list of rhythmic patterns
         return final_list
 
 
-# A container class, whose job is to store data nicely
-class Note:
-    """A Class for all the notes"""
-
-    def __init__(self, m21=None, name=None, length=None, velocity=None, measure=None) -> None:
-        """
-        A class representing a music note.
-
-        Args:
-            note: A music21 note object (optional).
-            name: A string representing the name of the note in 'note octave' format (optional).
-            length: A float or int representing the length of the note (optional).
-
-        Raises:
-            ValueError: If name is provided but is not in 'note octave' format.
-            TypeError: If length is provided but is not a float or int.
-        """
-
-        if m21 is not None:
-            self.music21 = m21
-            self._measure = m21.measureNumber
-            self._velocity = m21.volume.velocity
-        else:
-            self.music21 = music21.note.Note(name, quarterLength=length)
-            self._measure = velocity
-            self._velocity = measure
-
-        if name and not re.search(r"[a-zA-z][1-9]", name):
-            raise ValueError(
-                "name expects a note name in 'note octave' format, ex: 'A1' 'C4'"
-            )
-        self._name = name if name else self.music21.pitch.nameWithOctave
-
-        if length and not isinstance(length, (int, float)):
-            raise TypeError("length only accepts ints and floats")
-        self._length = length if length else self.music21.duration.quarterLength
-
-    @property
-    def name(self):
-        """Returns the note in 'letter-name octave' format.
-
-        Example:
-            C4
-            D5
-            B-4
-        """
-        return self._name
-
-    @property
-    def measure(self):
-        """Returns an int representing the measure"""
-        return self._measure
-
-    @property
-    def velocity(self):
-        """Returns an int representing velocity of the note"""
-        return self._velocity
-
-    @property
-    def length(self):
-        """Returns a str representing the length of the note
-
-        Example:
-            "quarter"
-
-        """
-        return self._length
-
-# A container class, whose job is to store data nicely
-class Rest:
-    """A Class for all the rests"""
-
-    def __init__(self, m21=None, length=None, measure=None) -> None:
-
-        if length and isinstance(length, (int, float)):
-            self._length = length
-        else:
-            self._length = m21.duration.quarterLength
-
-        if m21 is not None:
-            self.music21 = m21
-            self._measure = m21.measureNumber
-        else:
-            self._measure = measure
-            self.music21 = music21.note.Rest(quarterlength=length)
-
-    @property
-    def length(self):
-        """Returns a str, indicating the length of the rest
-
-        Example:
-            "whole"
-        """
-        return self._length
-
-    @property
-    def measure(self):
-        """Returns an int, representing the measure number"""
-        return self._measure
-
-# A container class, whose job is to store data nicely
-class Chord:
-    """A Class to represent a chord (multiple notes at once)"""
-
-    def __init__(self, m21=None, notes: list = None, measure=None) -> None:
-        if isinstance(m21, music21.chord.Chord):
-            self.music21 = m21
-            self._notes = [Note(note) for note in list(m21.notes)]
-            self._measure = m21.measureNumber
-            self._length = m21.duration.quarterLength
-        # if chord is not a music21 chord object
-        else:
-            notes = [note.music21 for note in notes]
-            self.music21 = music21.chord.Chord(notes)
-            self._notes = [Note(note) for note in notes]
-            self._measure = measure
-            self._length = notes[0].duration.quarterLength
-
-    @property
-    def length(self):
-        """Returns a str, representing the length of the chord
-
-        Example:
-            "eighth"
-        """
-        return self._length
-
-    @property
-    def measure(self):
-        """Returns an int, representing the measure number"""
-        return self._measure
-
-    @property
-    def notes(self):
-        """Retrieves a list of notes in a chord
-
-        Returns;
-            A list, consisting of Note objects. For example:
-
-            [Note Object, Note Object]
-        """
-        return self._notes
```

### Comparing `Scopul-1.0.4/src/Scopul/TimeSignature.py` & `Scopul-1.1.4/src/Scopul/TimeSignature.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.4/src/Scopul/conversions.py` & `Scopul-1.1.4/src/Scopul/conversions.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.4/src/Scopul/helpers.py` & `Scopul-1.1.4/src/Scopul/helpers.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.4/src/Scopul/scopul.py` & `Scopul-1.1.4/src/Scopul/scopul.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from Scopul.scopul_exception import (
     InvalidFileFormatError,
     InvalidMusicElementError,
     NoMusePathError,
     MeasureNotFoundException,
 )
 from mido import bpm2tempo, tempo2bpm, MidiFile
-
+from deprecated import deprecated
 # Setting up music21 with MuseScore
 from Scopul.TimeSignature import TimeSignature
 from Scopul.Tempo import Tempo
 from Scopul.Sequence import Part, Rest, Chord, Note
 from Scopul.helpers import get_tempos
+import subprocess
 
 
 class Scopul:
     def __init__(self, audio):
         self.construct(audio)
 
     # Time Signature (time_sig)
@@ -41,35 +42,49 @@
                     TimeSignature(
                         value=meta_message.ratioString,
                         measure=meta_message.measureNumber,
                     )
                 )
 
         return sig_list
+    
+    @property
+    def key(self):
+        s = stream.Stream()
+        for part in self.music21.parts:
+            try:
+                part.analyze('key')
+            except AttributeError:
+                continue
+
+            s.insert(part)
+        key_sig = s.analyze('key')
+        # print the key signature
+        return f"{key_sig.tonic.name} {key_sig.mode}"
 
     # Midi File (midi)
     @property
-    def audio(self):
+    def path(self):
         """Retrieves your midi file."""
-        return self._audio
+        return self._path
 
     @property
     def parts(self) -> list:
         """Retrieves a list of Part objects
 
         Example:
             [Part Object 1, Part Object 2]
         """
         return self._parts
 
     # Midi File setter
-    @audio.setter
-    def audio(self, audio) -> None:
+    @path.setter
+    def path(self, path) -> None:
         """Allows to reconstruct the object to change accordingly to a new midi"""
-        self.construct(audio)
+        self.construct(path)
 
     @property
     def tempo_list(self):
         """Fetches the tempo list in bpm format
 
         Fetches the time signatures in bpm with both measure numbers and the tempo
 
@@ -82,169 +97,160 @@
     def get_audio_length(self) -> int:
         """Returns the audio length"""
         return MidiFile(self._audio).length
     
     # Generate a pdf
     def generate_pdf(
         self,
-        output: str,
         fp: str = "",
         title: str = "Scop",
         overwrite: bool = False,
-        remove_defects: bool = False,
     ) -> None:
+
         """Generates a pdf of the midi
 
         Creates a pdf by turning it into musicxml then to pdf
 
         Args:
             output: a str that represents the name of the file
             fp: a str that represents the file path as to where to save the pdf. Default is '', which will save to the current working directory
             overwrite: a boolean, indicates whether to overwrite files or not
-            remove_defects: a boolean, indicates whether to remove defective parts or not
 
         Returns:
             None, just generates a pdf in the path specified with the name specified
 
         Raises:
             FileExistsError: if overwrite is False and there is a file at the same path
         """
 
+        if fp == "":
+            fp = self.path
+
         # Looking for muse score path
         try:
-            env = environment.Environment()
-            env["musicxmlPath"] = os.environ["MUSESCORE_PATH"]
-            env["musescoreDirectPNGPath"] = os.environ["MUSESCORE_PATH"]
+            mspath = os.environ["MUSESCORE_PATH"]
         except:
             raise NoMusePathError(
                 "Path to musescore not set. please set using config_musescore()"
             )
 
         # checking for existence of the path
         if not pathlib.Path(os.environ["MUSESCORE_PATH"]).exists():
             raise FileNotFoundError(
                 f"MuseScore path at {os.environ['MUSESCORE_PATH']} not found. Please check to see if it exists"
             )
 
         # Check for correct file format
-        ext = pathlib.Path(output).suffix
+        ext = pathlib.Path(fp).suffix
         if ext != ".pdf":
             raise InvalidFileFormatError(f"Expected .pdf, got {ext}")
 
         midi = self.music21
 
-        if remove_defects:
-            for part in midi.parts:
-                try:
-                    part.write("musicxml.pdf")
-                except:
-                    midi.remove(part)
-
         # Check for overwrite
         if overwrite:
-            if pathlib.Path(fp + output).exists():
-                os.remove(fp + output)
+            if pathlib.Path(fp).exists():
+                os.remove(fp)
         # If not overwrite
         else:
-            if pathlib.Path(fp + output).exists():
+            if pathlib.Path(fp).exists():
                 raise FileExistsError(
-                    f"{fp + output} already exists. To overwrite, set overwrite=True"
+                    f"{fp} already exists. To overwrite, set overwrite=True"
                 )
 
         # Creates the pdf and deletes the musicxml file
-        midi.metadata.title = title
-        midi.write("musicxml.pdf", fp=fp)
-        os.rename(fp + ".musicxml.pdf", fp + output)
-        os.remove(fp + ".musicxml.musicxml")
+        self.generate_musicxml(fp=fp.replace(".pdf", ".xml"),title=title,overwrite=True)
+        subprocess.run(f'"{mspath}" -o "{fp}" "{fp.replace(".pdf", ".xml")}" -T "{title}" 0')
+        os.remove(fp.replace(".pdf", ".xml"))
 
     def generate_musicxml(
         self,
-        output: str,
         fp: str = "",
         overwrite: bool = False,
-        remove_defects: bool = False,
+        title = 'scop',
     ) -> None:
         """Generates a musicxml of the midi
 
         Args:
             output: a str that represents the name of the file
             fp: a str that represents the file path as to where to save the pdf. Default is '', which will save to the current working directory
             overwrite: a boolean, indicates whether to overwrite files or not
-            remove_defects: a boolean, indicates whether to remove defective parts or not
 
         Returns:
             None, just generates a pdf in the path specified with the name specified
 
         Raises:
             FileExistsError: if overwrite is False and there is a file at the same path
         """
+        if fp == "":
+            fp = self.path
 
         # Looking for muse score path
         try:
-            env = environment.Environment()
-            env["musicxmlPath"] = os.environ["MUSESCORE_PATH"]
-            env["musescoreDirectPNGPath"] = os.environ["MUSESCORE_PATH"]
+            mspath = os.environ["MUSESCORE_PATH"]
         except:
             raise NoMusePathError(
                 "Path to musescore not set. please set using config_musescore()"
             )
 
         # Checking for existence of the path
         if not pathlib.Path(os.environ["MUSESCORE_PATH"]):
             raise FileNotFoundError(
                 f"MuseScore path at {os.environ['MUSESCORE_PATH']} not found. Please check to see if it exists"
             )
 
         # Check for correct file format
-        ext = pathlib.Path(output).suffix
+        ext = pathlib.Path(fp).suffix
         if ext != ".xml":
             raise InvalidFileFormatError(f"Expected .xml, got {ext}")
 
-        midi = self.music21
-
         # Check for overwrite
         if overwrite:
-            if pathlib.Path(fp + output).exists():
-                os.remove(fp + output)
+            if pathlib.Path(fp).exists():
+                os.remove(fp)
 
         # If not overwrite
         else:
-            if pathlib.Path(fp + output).exists():
+            if pathlib.Path(fp).exists():
                 raise FileExistsError(
-                    f"{fp + output} already exists. To overwrite, set overwrite=True"
+                    f"{fp} already exists. To overwrite, set overwrite=True"
                 )
 
-        if remove_defects:
-            for part in midi.parts:
-                try:
-                    part.write("musicxml.pdf")
-                except:
-                    midi.remove(part)
 
         # Creates the pdf and deletes the musicxml file
-        self.music21.write("musicxml.xml", fp=fp)
-        os.rename(fp + ".musicxml.musicxml", fp + output)
+        subprocess.run(f'"{mspath}" -o "{fp}" "{self.path}" -T {title} 0')
+
+        # Open the file and read all the lines into a list
+        with open(fp, 'r') as file:
+            lines = file.readlines()
+
+        # Insert the new line at index 3
+        lines.insert(3, f'<movement-title>{title}</movement-title>\n')
+
+        # Open the file in write mode and write the modified lines back to the file
+        with open(fp, 'w') as file:
+            file.writelines(lines)
 
     # (Re)constructor
-    def construct(self, audio) -> None:
+    def construct(self, path) -> None:
         """Constructor function to reconstruct the object
 
         Can also be called with a setter to the midi property. For example:
 
         testmidi.music21 = "test.mid"
 
         """
 
-        self._audio = audio
-        self.music21 = converter.parse(audio)
+        self._path = path
+        self.music21 = converter.parse(path).makeMeasures()
         self._parts = []
         for part in self.music21.parts:
             self._parts.append(Part(part))
 
-    def save_midi(self, output, fp="", overwrite=False):
+    def save_midi(self, fp=None, overwrite=True):
         """
         Save the MIDI file to the specified output file path.
 
         Args:
             self: A reference to the current object.
             output (str): The name of the MIDI output file.
             fp (str, optional): The path to the directory where the output file will be saved. Defaults to the current directory.
@@ -253,55 +259,70 @@
         Raises:
             InvalidFileFormatError: If the output file has an invalid file extension.
             FileExistsError: If the output file already exists and overwrite is set to False.
 
         Returns:
             None
         """
+
+        if not fp:
+            fp = self.path
         # Check for correct file format
-        ext = pathlib.Path(output).suffix
+        ext = pathlib.Path(fp).suffix
         if ext != ".mid":
             raise InvalidFileFormatError(f"Expected .mid, got {ext}")
 
         midi = self.music21
 
         # Check for overwrite
         if overwrite:
-            if pathlib.Path(fp + output).exists():
-                os.remove(fp + output)
+            if pathlib.Path(fp).exists():
+                os.remove(fp)
 
         # If not overwrite
         else:
-            if pathlib.Path(fp + output).exists():
+            if pathlib.Path(fp).exists():
                 raise FileExistsError(
-                    f"{fp + output} already exists. To overwrite, set overwrite=True"
+                    f"{fp} already exists. To overwrite, set overwrite=True"
                 )
 
-        midi.write("midi", fp=fp + output)
 
+        midi.write("midi", fp=fp)
+    
+    def append_part(self, part: Part) -> None:
+        """Appends a Scopul Part to the object
+
+        Args:
+            part: a Part object
+        
+        Returns:
+            None
+        """
+        self._parts.append(part._part)
+
+
+# ---------------------------------------------------DEPRECATED-------------------------------------------------------------------------------
+
+    @deprecated(reason="add_tempo(), add_note() and add_TimeSignature() are deprecated. Use Part.insert() instead")
     def add_tempo(self, bpm_tempo: int, part, measure_number: int = 1):
         """
         Adds a metronome mark at the specified measure in a part object.
-
         Args:
             part: A Scopul Part object representing a musical part.
             measure_number: An integer specifying the measure number where the
                 metronome mark should be added.
             tempo: A floating point number representing the tempo in beats per
                 minute (BPM) for the metronome mark.
-
         Returns:
             None.
-
         Raises:
             TypeError: If part is not a Scopul part object
             ValueError: If measure_number is not a positive integer
             ValueError: If tempo is not a positive number.
             MeasureNotFoundError: If given measure does not exist
-
         If a metronome mark already exists at the specified location, its tempo
         will be updated to the new tempo value
         """
         # Checking if part is a scopul part
         if not isinstance(part, Part):
             raise TypeError("Provided part is not a Scopul Part object")
 
@@ -342,25 +363,23 @@
                 ),
             ):
                 new_part.append(element)
 
         new_part = new_part.makeMeasures()
         self.music21.replace(part, new_part)
 
+    @deprecated(reason="add_tempo(), add_note() and add_TimeSignature() are deprecated. Use Part.insert() instead")
     def add_TimeSignature(self, time_sig: str, part, measure_number: int = 1) -> None:
         """A method to add a timesignature to a piece
-
         Args:
             time_sig: a str object representing the int. For example - "3/4"
             part: the Part object you want to modify
             measure: an int, representing the measure number you want to add this time signature. Default is one
-
         Returns:
             None, only modifies the midi
-
         """
         # Getting the Music21 converter object and the Muic21 part object
         midi_file = self.music21
         part = part._part
 
         # Looking for measure
         if part[-1].measureNumber < measure_number:
@@ -389,29 +408,27 @@
                 ),
             ):
                 new_part.append(element)
 
         new_part = new_part.makeMeasures()
         midi_file.replace(part, new_part)
 
+    @deprecated(reason="add_tempo(), add_note() and add_TimeSignature() are deprecated. Use Part.insert() instead")
     def add_note(self, element, part, measure_number=None, position=0):
         """Add a musical element (Note, Rest, or Chord) to a measure in the given part.
-
         Args:
             element: A Scopul musical element (Note, Rest, or Chord) to add to the measure.
             part: A music21 Part object representing the part to add the element to.
             measure_number (optional): An integer specifying the measure number to add the element to.
                 If not provided, the element will be added to the last measure in the part.
             position (optional): An integer specifying the position within the measure to add the element.
                 Defaults to 0 (the beginning of the measure).
-
         Raises:
             ValueError: If the given element is not a Scopul musical element (Note, Rest, or Chord),
                 or if no measure is found with the given measure number.
-
         Returns:
             None
         """
         if not isinstance(element, (Note, Rest, Chord)):
             raise ValueError("Not a Scopul musical element (Notes, Rests, Chords)")
         
         if not measure_number:
@@ -429,12 +446,7 @@
                 element_added = True
 
             new_part.append(measure)
 
         new_part = new_part.makeMeasures()
         self.music21.replace(part, new_part)
 
-        
-        
-
-
-
```

### Comparing `Scopul-1.0.4/src/Scopul.egg-info/PKG-INFO` & `Scopul-1.1.4/src/Scopul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.4
+Version: 1.1.4
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

