# Comparing `tmp/musiclang-0.8.2.tar.gz` & `tmp/musiclang-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclang-0.8.2.tar", last modified: Mon Apr 24 08:43:15 2023, max compression
+gzip compressed data, was "musiclang-0.8.3.tar", last modified: Sun Apr 30 13:59:12 2023, max compression
```

## Comparing `musiclang-0.8.2.tar` & `musiclang-0.8.3.tar`

### file list

```diff
@@ -1,213 +1,215 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-04-24 08:43:11.000000 musiclang-0.8.2/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5238 2023-04-24 08:43:15.869644 musiclang-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3620 2023-04-24 08:43:11.000000 musiclang-0.8.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.841644 musiclang-0.8.2/musiclang/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.845644 musiclang-0.8.2/musiclang/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/analyze/augmented_net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/chord_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/feature_representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/inference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/input_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/keydistance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/output_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/score_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/midi_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15745 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/pattern_analyzer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/pattern_sampler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/roman_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/score_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/score_formatter_elements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/to_musiclang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/voice_separation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/library.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/arranger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/arranger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/arranger_trainer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/composer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       39 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6139 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/auto_composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/harmony.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/predictors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/huggin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/windowed.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/tokenizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/tokenizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/tokenizers/chord_tokenizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.853644 musiclang-0.8.2/musiclang/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/base_transformer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.853644 musiclang-0.8.2/musiclang/transform/chord/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/chord/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/chord/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/arrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/patternator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18038 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/dynamics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/dynamics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/dynamics/dynamizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/features/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/features/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/features/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/generators/rythm_generator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/mask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/melody/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/basics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/continuation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/filler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/merger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/note/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/note/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/note/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/orchestrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/epic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/nocturne.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/score/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/transform/score_merger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score_merger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score_merger/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/transform/structure_graphs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/structure_graphs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/structure_graphs/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/transformer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/utils_random.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/arrange_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/arrange_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/skyline_algorithm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40204 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/element.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/elements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/bar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/beat.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/element.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/free_text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/rhythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/time_signature.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/tonality.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/voice_leading.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/voicing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14137 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26909 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/note_pitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8464 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/ornementation.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/midi_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_code.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_midi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_mxl.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/pitches/pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/properties/note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/rhythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/score_rythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/utils_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32073 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/score.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/sequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/sequence_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/time_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/time_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/time_utils/time_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/tonality.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.841644 musiclang-0.8.2/musiclang.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5238 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6111 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-04-24 08:43:13.000000 musiclang-0.8.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-24 08:43:15.869644 musiclang-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2023-04-24 08:43:13.000000 musiclang-0.8.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/test_analyze.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/test_score_formatter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/predict/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/predict/test_auto_composer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_mask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transform_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transforms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/out/test_to_midi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/pitches/test_pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/properties/test_note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/rythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/rythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/rythm/test_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_absolute_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_bass_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chord_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chromatic_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_drum_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_extensions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5540 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_score.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.005807 musiclang-0.8.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-04-30 13:59:08.000000 musiclang-0.8.3/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5253 2023-04-30 13:59:12.001807 musiclang-0.8.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-04-30 13:59:08.000000 musiclang-0.8.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.985807 musiclang-0.8.3/musiclang/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.985807 musiclang-0.8.3/musiclang/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/analyze/augmented_net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/chord_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/feature_representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/inference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/input_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/keydistance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/output_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/score_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/augmented_net/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/midi_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16589 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/pattern_analyzer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/pattern_sampler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/roman_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/score_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/score_formatter_elements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/to_musiclang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/analyze/voice_separation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/library.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/predict/arranger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/arranger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/arranger/arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/arranger/arranger_trainer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/arranger/melody_arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6092 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/arranger/melody_arranger_trainer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/predict/composer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       39 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/composer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6139 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/composer/auto_composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/composer/composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/composer/harmony.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/predict/predictors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/predictors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/predictors/huggin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/predictors/windowed.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/predict/tokenizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/tokenizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/predict/tokenizers/chord_tokenizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1559 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/base_transformer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.989807 musiclang-0.8.3/musiclang/transform/chord/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/chord/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/chord/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/arrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/patternator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18039 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/composing/voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/dynamics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/dynamics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/dynamics/dynamizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/features/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/features/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/features/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/generators/rythm_generator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/mask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/melody/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/melody/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/melody/basics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/melody/continuation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/melody/filler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/merger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/note/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/note/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/note/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/orchestrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/orchestrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/orchestrations/epic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/orchestrations/nocturne.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/score/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/score/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/score/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/score_merger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/score_merger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/score_merger/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.993807 musiclang-0.8.3/musiclang/transform/structure_graphs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/structure_graphs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/structure_graphs/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/transformer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/transform/utils_random.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/arrange_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/arrange_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/arrange_utils/arrange_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/arrange_utils/skyline_algorithm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41769 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/element.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/elements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/bar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/beat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/element.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/free_text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/rhythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/time_signature.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/tonality.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/voice_leading.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/elements/voicing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14138 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27070 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/note_pitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8474 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/ornementation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/midi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/to_code.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/to_midi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/out/to_mxl.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/pitches/pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/properties/note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/rhythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/rhythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/rhythm/metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/rhythm/score_rythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/rhythm/utils_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34870 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/score.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.997807 musiclang-0.8.3/musiclang/write/sequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/sequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/sequence/sequence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/sequence/sequence_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/musiclang/write/time_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/time_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/time_utils/time_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-04-30 13:59:08.000000 musiclang-0.8.3/musiclang/write/tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:11.985807 musiclang-0.8.3/musiclang.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5253 2023-04-30 13:59:11.000000 musiclang-0.8.3/musiclang.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6211 2023-04-30 13:59:11.000000 musiclang-0.8.3/musiclang.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-30 13:59:11.000000 musiclang-0.8.3/musiclang.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-30 13:59:11.000000 musiclang-0.8.3/musiclang.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-30 13:59:11.000000 musiclang-0.8.3/musiclang.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-04-30 13:59:10.000000 musiclang-0.8.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-30 13:59:12.005807 musiclang-0.8.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2023-04-30 13:59:10.000000 musiclang-0.8.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/analyze/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/analyze/test_analyze.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/analyze/test_score_formatter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/composing/test_counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/composing/test_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/composing/test_voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/predict/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/predict/test_auto_composer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/test_mask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/test_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/test_transform_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/transform/test_transforms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/out/test_to_midi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/pitches/test_pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/properties/test_note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:12.001807 musiclang-0.8.3/tests/write/rythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/rythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/rythm/test_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_absolute_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_bass_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_chord_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_chromatic_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_drum_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_extensions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5994 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_score.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-04-30 13:59:08.000000 musiclang-0.8.3/tests/write/test_tonality.py
```

### Comparing `musiclang-0.8.2/LICENSE.md` & `musiclang-0.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/PKG-INFO` & `musiclang-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.2
+Version: 0.8.3
 Summary: A python package for music notation and generation
 Home-page: UNKNOWN
 Author: Florian GARDIN
 Author-email: fgardin.pro@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/MusicLang/musiclang/
@@ -114,15 +114,15 @@
         	piano__0=s2.ed.mp + r.s, 
         	piano__2=s4.ed.mp + r.s, 
         	piano__4=s6.ed.o(-1).mp + r.s, 
         	piano__5=s0.ed.o(-1).mp + r.s, 
         	piano__6=s4.ed.o(-1).mp + r.s))
         
         # Predict a continuation of the score using hugginface musiclang model
-        predicted_score = score.predict_score()
+        predicted_score = score.predict_score(temperature=0.5)
         # Save it to midi
         predicted_score.to_midi('test.mid')
         ```
         
         Please note that this feature is still experimental, it will only work with
         piano music for now and the model is not yet trained on a large corpus of music.
         If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
```

### Comparing `musiclang-0.8.2/README.md` & `musiclang-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 	piano__0=s2.ed.mp + r.s, 
 	piano__2=s4.ed.mp + r.s, 
 	piano__4=s6.ed.o(-1).mp + r.s, 
 	piano__5=s0.ed.o(-1).mp + r.s, 
 	piano__6=s4.ed.o(-1).mp + r.s))
 
 # Predict a continuation of the score using hugginface musiclang model
-predicted_score = score.predict_score()
+predicted_score = score.predict_score(temperature=0.5)
 # Save it to midi
 predicted_score.to_midi('test.mid')
 ```
 
 Please note that this feature is still experimental, it will only work with
 piano music for now and the model is not yet trained on a large corpus of music.
 If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
```

### Comparing `musiclang-0.8.2/musiclang/__init__.py` & `musiclang-0.8.3/musiclang/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/cache.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/cache.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/chord_vocabulary.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/chord_vocabulary.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/feature_representation.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/feature_representation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/inference.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/inference.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/input_representations.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/input_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/keydistance.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/keydistance.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/models.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/models.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/output_representations.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/output_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/score_parser.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/score_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/augmented_net/utils.py` & `musiclang-0.8.3/musiclang/analyze/augmented_net/utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/constants.py` & `musiclang-0.8.3/musiclang/analyze/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/item.py` & `musiclang-0.8.3/musiclang/analyze/item.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/midi_parser.py` & `musiclang-0.8.3/musiclang/analyze/midi_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/parser.py` & `musiclang-0.8.3/musiclang/analyze/parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/pattern_analyzer.py` & `musiclang-0.8.3/musiclang/analyze/pattern_analyzer.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,15 +111,51 @@
         instruments = instruments[:-nb]
     parts = [i[0] for i in instruments]
     new_chord = chord(**{instr: item for instr, item in chord.score.items() if instr in parts})
 
     return new_chord, parts
 
 
+def inverse_recursive_correct_octave(chord):
+    """
+    Transform a chord to a chord with bass pitch between -6 and 6
+    Parameters
+    ----------
+    chord
+
+    Returns
+    -------
+
+    """
+    bass_pitch = chord.bass_pitch
+    if bass_pitch > 6:
+        chord = chord.o(-1)
+        for voice, melody in chord.score.items():
+            chord.score[voice] = melody.o(1)
+        return inverse_recursive_correct_octave(chord)
+    elif bass_pitch <= -6:
+        chord = chord.o(1)
+        for voice, melody in chord.score.items():
+            chord.score[voice] = melody.o(-1)
+        return inverse_recursive_correct_octave(chord)
+    else:
+        new_chord = chord.copy()
+        return new_chord
+
 def recursive_correct_octave(chord):
+    """
+    Transform chord and melodies to normalize chord octaves
+    Parameters
+    ----------
+    chord
+
+    Returns
+    -------
+
+    """
     bass_pitch = chord.bass_pitch
     if bass_pitch > 6:
         chord = chord.o(-1)
         for voice, melody in chord.score.items():
             chord.score[voice] = melody.o(1)
         return recursive_correct_octave(chord)
     elif bass_pitch <= -6:
```

### Comparing `musiclang-0.8.2/musiclang/analyze/pattern_sampler.py` & `musiclang-0.8.3/musiclang/analyze/pattern_sampler.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/roman_parser.py` & `musiclang-0.8.3/musiclang/analyze/roman_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/score_formatter.py` & `musiclang-0.8.3/musiclang/analyze/score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/score_formatter_elements.py` & `musiclang-0.8.3/musiclang/analyze/score_formatter_elements.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/to_musiclang.py` & `musiclang-0.8.3/musiclang/analyze/to_musiclang.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/analyze/voice_separation.py` & `musiclang-0.8.3/musiclang/analyze/voice_separation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/__init__.py` & `musiclang-0.8.3/musiclang/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/arranger/arranger.py` & `musiclang-0.8.3/musiclang/predict/arranger/arranger.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/arranger/arranger_trainer.py` & `musiclang-0.8.3/musiclang/predict/arranger/arranger_trainer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/composer/auto_composer.py` & `musiclang-0.8.3/musiclang/predict/composer/auto_composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/composer/composer.py` & `musiclang-0.8.3/musiclang/predict/composer/composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/composer/harmony.py` & `musiclang-0.8.3/musiclang/predict/composer/harmony.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,21 @@
 
 
 def auto_enrich_melody(melody, proba_enrich=1.0):
     new_melody = None
     for note in melody.notes:
         random_number = np.random.random()
         if random_number < proba_enrich:
-            if np.random.random() < 0.2:
+            second_random_number = np.random.random()
+            if second_random_number < 0.2:
                 new_note = note.add_tag(np.random.choice(ORNEMENTATIONS))
-            else:
+            elif note.duration >= 0.5:
                 new_note = note.add_tag(np.random.choice(INTERPOLATE))
+            else:
+                new_note = note.copy()
         else:
             new_note = note.copy()
 
         new_melody += new_note
 
     return new_melody
 
@@ -78,15 +81,16 @@
         return float((beat) * ratio) + 1
 
     from fractions import Fraction as frac
     melody_arranger = [[(note, 1)] for note in melody.notes]
     chord_progression = arranger.arrange(melody_arranger, tonality, temperature=temperature)
     # Convert to harmony grid
     bar_duration = 4 * frac(time_signature[0], time_signature[1])
-    text = [f"Time Signature : {time_signature[0]}/{time_signature[1]}"]
+    text = [f"Time Signature : {time_signature[0]}/{time_signature[1]}",
+            f"Tonality : {tonality}"]
     current_bar_idx = 0
     current_beat = 0
     time = 0
     current_text = f"m{current_bar_idx}"
     for note, chord in zip(melody.notes, chord_progression):
         bar_idx = time // bar_duration
         if bar_idx != current_bar_idx:
```

### Comparing `musiclang-0.8.2/musiclang/predict/predictors/huggin.py` & `musiclang-0.8.3/musiclang/predict/predictors/huggin.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Returns
     -------
 
     """
     return prompt.replace(' ', '').replace('\t', '').replace('\r', '').replace('\n', '')
 
-def predict_score_from_hugginface(prompt):
+def predict_score_from_hugginface(prompt, temperature=1.0, top_k=20):
     """
 
     Parameters
     ----------
     prompt
 
     Returns
@@ -41,16 +41,18 @@
     max_iter = 5
     i = 0
 
     # We need to keep the first half of the prompt to be able to reconstruct the score
     end_prompt = prompt[-block_size//2:]
     start_prompt = prompt[:-block_size//2]
     prompt = end_prompt
+    # Predict until we find ')+(' sequence or we reach the maximum number of iterations
+
     while not eos in text and (i < max_iter):
-        res = predictor(prompt, max_length=block_size, temperature=0.75, do_sample=True, top_k=10)[0]['generated_text']
+        res = predictor(prompt, max_length=block_size, temperature=temperature, do_sample=True, top_k=top_k)[0]['generated_text']
         remaining = block_size//2
         text += res[:remaining]
         prompt = res[remaining:]
         i+= 1
 
     if i < max_iter:
         return start_prompt + text.split(eos)[0]
```

### Comparing `musiclang-0.8.2/musiclang/predict/predictors/windowed.py` & `musiclang-0.8.3/musiclang/predict/predictors/windowed.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/predict/tokenizers/chord_tokenizer.py` & `musiclang-0.8.3/musiclang/predict/tokenizers/chord_tokenizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/__init__.py` & `musiclang-0.8.3/musiclang/transform/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from .mask import Mask
 from .transformer import Transformer, ChordTransformer, ScoreTransformer, MelodyTransformer, NoteTransformer
 from .transformer import ChordFilter, ChordFilterTransform, MelodyFilterTransform, MelodyFilter
 from .transformer import NoteFilter, NoteFilterTransform, FeatureExtractor
 from .transformer import MaskFilter, NoteMaskFilter, ChordMaskFilter, MelodyMaskFilter
 from .merger import ScoreMerger
 from .graph import TransformGraph
-from .composing import VoiceLeading, PartComposer
+from .composing import VoiceLeading, PartComposer, create_counterpoint_on_score
 from .dynamics import PitchDynamizer
 from .melody import ContinuationWhenSameNote
 from .composing import Patternator, OrchestralLayer, MelodicLayer, GlobalLayer
 from .orchestrations import get_epic_orchestration, get_nocturne_orchestration
 
 __all__ = ['TransformPipeline', 'ConcatPipeline', 'Mask',
            'Transformer', 'ChordTransformer', 'ScoreTransformer', 'MelodyTransformer',
            'NoteTransformer',
            'ChordFilter', 'ChordFilterTransform', 'MelodyFilterTransform', 'MelodyFilter',
            'NoteFilter', 'NoteFilterTransform', 'FeatureExtractor', 'MaskFilter', 'NoteMaskFilter',
            'ChordMaskFilter', 'MelodyMaskFilter', 'ScoreMerger', 'TransformGraph',
            'VoiceLeading', 'PitchDynamizer', 'ContinuationWhenSameNote', 'Patternator',
            'get_epic_orchestration', 'get_nocturne_orchestration', 'PartComposer','OrchestralLayer',
-              'MelodicLayer', 'GlobalLayer'
+              'MelodicLayer', 'GlobalLayer', 'create_counterpoint_on_score'
            ]
```

### Comparing `musiclang-0.8.2/musiclang/transform/base_transformer.py` & `musiclang-0.8.3/musiclang/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/chord/basics.py` & `musiclang-0.8.3/musiclang/transform/chord/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/arrange.py` & `musiclang-0.8.3/musiclang/transform/composing/arrange.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/counterpoint.py` & `musiclang-0.8.3/musiclang/transform/composing/counterpoint.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/layer.py` & `musiclang-0.8.3/musiclang/transform/composing/layer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/pattern.py` & `musiclang-0.8.3/musiclang/transform/composing/pattern.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/patternator.py` & `musiclang-0.8.3/musiclang/transform/composing/patternator.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/project.py` & `musiclang-0.8.3/musiclang/transform/composing/project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/composing/voice_leading.py` & `musiclang-0.8.3/musiclang/transform/composing/voice_leading.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         for it in range(max_iter):
             pitches = self.get_pitch_solution(dvals)
             mov = self.get_movement(pitches).astype(np.float32)  # Find movements
             mov *= self.dvalsmask[:, :-1]
             sgn_mov = np.sign(mov)
             # Find probabilities of moving an index
             proba = np.exp(mov/temperature)/np.sum(np.exp(mov/temperature))
-            assert np.max(proba) < 1
+            assert np.max(proba) <= 1
             # Sample index given proba
             delta1 = sgn_mov * (self.rg.random(mov.shape) < proba)
             delta1 = (np.c_[delta1, np.zeros(len(delta1))])
             delta2 = - sgn_mov * (self.rg.random(mov.shape) < proba)
             delta2 = (np.c_[np.zeros(len(delta2)), delta2])
             mov = (delta1 + delta2).astype(int)
             proposed_sol = (dvals + mov).clip(-max_norm, max_norm)
```

### Comparing `musiclang-0.8.2/musiclang/transform/dynamics/dynamizer.py` & `musiclang-0.8.3/musiclang/transform/dynamics/dynamizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/features/basics.py` & `musiclang-0.8.3/musiclang/transform/features/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/graph.py` & `musiclang-0.8.3/musiclang/transform/graph.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/library.py` & `musiclang-0.8.3/musiclang/transform/library.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/mask.py` & `musiclang-0.8.3/musiclang/transform/mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/melody/basics.py` & `musiclang-0.8.3/musiclang/transform/melody/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/melody/continuation.py` & `musiclang-0.8.3/musiclang/transform/melody/continuation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/note/basics.py` & `musiclang-0.8.3/musiclang/transform/note/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/orchestrations/epic.py` & `musiclang-0.8.3/musiclang/transform/orchestrations/epic.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/orchestrations/nocturne.py` & `musiclang-0.8.3/musiclang/transform/orchestrations/nocturne.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/pipeline.py` & `musiclang-0.8.3/musiclang/transform/pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/score_merger/basics.py` & `musiclang-0.8.3/musiclang/transform/score_merger/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/structure_graphs/forms.py` & `musiclang-0.8.3/musiclang/transform/structure_graphs/forms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/transformer.py` & `musiclang-0.8.3/musiclang/transform/transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/transform/utils_random.py` & `musiclang-0.8.3/musiclang/transform/utils_random.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/arrange_utils/arrange_utils.py` & `musiclang-0.8.3/musiclang/write/arrange_utils/arrange_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/arrange_utils/skyline_algorithm.py` & `musiclang-0.8.3/musiclang/write/arrange_utils/skyline_algorithm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/chord.py` & `musiclang-0.8.3/musiclang/write/chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,62 @@
             return note.val
         elif note.type in ['l', 'r']:
             return (None, None)
         elif note.type == 'h':
             pass
 
 
+    def realize_tags(self, last_note=None, final_note=None):
+        new_chord_dict = {}
+        last_note = last_note or {}
+        final_note = final_note or {}
+        for key, melody in self.score.items():
+            new_chord_dict[key] = melody.realize_tags(last_note.get(key, None), final_note.get(key, None))
+        return self(**new_chord_dict)
+
+
+    def correct_chord_octave(self):
+        """
+        Correct chord octaves to minimize distance with central C
+
+        Returns
+        -------
+        score: Score
+        """
+        from musiclang.analyze import inverse_recursive_correct_octave
+        return inverse_recursive_correct_octave(self)
+
+    def split(self, max_length):
+        """
+        Split the chords that are too long into smaller chords
+        Parameters
+        ----------
+        max_length: fraction
+           The maximum length of a chord
+
+        Returns
+        -------
+        score: Score
+           The score with shorter chords
+
+        """
+        score = None
+        if self.duration <= max_length:
+            return self
+        nb_chords = 1 + (self.duration // max_length)
+        remaining_duration = self.duration % max_length
+        from musiclang.library import s0
+        chords = [self(s0.augment(max_length)) for i in range(nb_chords)]
+        if remaining_duration > 0:
+            chords[-1].score['piano__0'] = chords[-1].score['piano__0'].set_duration(remaining_duration)
+        else:
+            chords = chords[:-1]
+        chords = sum(chords, None)
+        return self.project_on_score(chords)
+
 
     @property
     def mode(self):
         return self.tonality.mode
 
     def change_mode(self, mode):
         """
```

### Comparing `musiclang-0.8.2/musiclang/write/constants.py` & `musiclang-0.8.3/musiclang/write/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/element.py` & `musiclang-0.8.3/musiclang/write/element.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/elements/chord.py` & `musiclang-0.8.3/musiclang/write/elements/chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/library.py` & `musiclang-0.8.3/musiclang/write/library.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/melody.py` & `musiclang-0.8.3/musiclang/write/melody.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 
         Returns
         -------
         melody: Melody
         """
         cp = self.copy()
         cp.tags = set()
+
         return cp
 
     def set_amp(self, amp):
         return Melody([n.set_amp(amp) for n in self.notes], nb_bars=self.nb_bars, tags=set(self.tags))
 
 
     def set_duration(self, duration):
```

### Comparing `musiclang-0.8.2/musiclang/write/note.py` & `musiclang-0.8.3/musiclang/write/note.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 
         Returns
         -------
 
         """
         if isinstance(value, float):
             value = frac(value).limit_denominator(8)
+        elif isinstance(value, int):
+            value = frac(value, 1)
         result = self.copy()
         result.duration = value
         return result
 
     def augment(self, value):
         """
         Returns a copy with augmented duration (multiply current duration by the value)
@@ -501,15 +503,16 @@
         >>> from fractions import Fraction
         >>> s0.augment(Fraction(8, 7))
         s0.augment(frac(8, 7))
 
         """
         if isinstance(value, float):
             value = frac(value).limit_denominator(8)
-
+        if isinstance(value, int):
+            value = frac(value, 1)
         result = self.copy()
         result.duration *= value
         return result
 
     def change_type(self, new_type):
         """
 
@@ -886,15 +889,15 @@
             new_note = self.copy()
             base_note = chord.parse(chord.to_pitch(self))
             new_note.type = base_note.type
             new_note.val = base_note.val
             new_note.octave = base_note.octave
             return new_note
         else:
-            return self
+            return self.add_tags(self.tags)
 
     def to_absolute_note(self, chord):
         if not self.is_note:
             return self.copy()
         pitch = chord.to_pitch(self)
         new_note = self.copy()
         new_note.type = 'a'
```

### Comparing `musiclang-0.8.2/musiclang/write/note_pitch.py` & `musiclang-0.8.3/musiclang/write/note_pitch.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/ornementation.py` & `musiclang-0.8.3/musiclang/write/ornementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,23 +216,24 @@
     Returns
     -------
 
     """
     from musiclang import Note
     if next_note is None or not next_note.is_note or not new_note.is_note:
         return new_note
-
+    
     first_val = new_note.val if new_note.type == 's' else int(7 * new_note.val/12)
     first_val += 7 * new_note.octave
     second_val = next_note.val if next_note.type == 's' else int(7 * next_note.val / 12)
     second_val += 7 * next_note.octave
     delta_scale = second_val - first_val
     if delta_scale == 0:
         return new_note
-    duration = frac(new_note.duration, abs(delta_scale))
+    duration = frac(new_note.duration, int(abs(delta_scale)))
+
     up = delta_scale > 0
     temp_note = L.su1.set_duration(duration) if up else L.sd1.set_duration(duration)
     melody = None
     for i in range(first_val, second_val, 1 if up else -1):
         if i == first_val:
             melody += new_note.set_duration(duration)
         else:
```

### Comparing `musiclang-0.8.2/musiclang/write/out/constants.py` & `musiclang-0.8.3/musiclang/write/out/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/out/midi_utils.py` & `musiclang-0.8.3/musiclang/write/out/midi_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/out/to_code.py` & `musiclang-0.8.3/musiclang/write/out/to_code.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/out/to_midi.py` & `musiclang-0.8.3/musiclang/write/out/to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/out/to_mxl.py` & `musiclang-0.8.3/musiclang/write/out/to_mxl.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/pitches/pitches_utils.py` & `musiclang-0.8.3/musiclang/write/pitches/pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/properties/note_properties.py` & `musiclang-0.8.3/musiclang/write/properties/note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/rhythm/metric.py` & `musiclang-0.8.3/musiclang/write/rhythm/metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/rhythm/score_rythm.py` & `musiclang-0.8.3/musiclang/write/rhythm/score_rythm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/rhythm/utils_metric.py` & `musiclang-0.8.3/musiclang/write/rhythm/utils_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/score.py` & `musiclang-0.8.3/musiclang/write/score.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Copyright (c) 2023, Florian GARDIN
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 from musiclang.library import *
-
+import re
 
 class Score:
     """Represents a score in musiclang
 
 
     """
     def __init__(self, chords=None, config=None, tags=None):
@@ -252,26 +252,26 @@
         Inverse operation of :func:`~Score.normalize_instruments`
         For each chord remove all instruments that are silenced
         Returns
         -------
         score: Score
         """
 
-        score = None
+        chords = []
         for chord_raw in self.chords:
             chord = chord_raw.copy()
             chord_score = chord.score
 
             for instrument in list(chord_score.keys()):
                 if all([n.type == 'r' for n in chord_score[instrument]]):
                     del chord_score[instrument]
 
-            score += chord(**chord_score)
+            chords.append(chord(**chord_score))
 
-        return score
+        return sum(chords, None)
 
     def replace_instruments(self, **instruments_dict):
         """
         Replace any instrument with another (use full part name (eg: piano__0)
 
         Parameters
         ----------
@@ -387,14 +387,40 @@
             insts = list(chord.score.keys())
             result += insts
             result = list(set(result))
 
         return list(sorted(result, key=lambda x: (x.split('__')[0], int(x.split('__')[1]))))
 
 
+    def normalize(self):
+        """
+        Normalize the score to be standardized for the language model
+        - Normalize instruments in each chord
+        - Convert relative notes to real notes
+        - Correct chord octaves to minimize distance with central C
+        FIXME : Relative notes should be converted first
+
+        Returns
+        -------
+        score: Score
+        """
+        score = self.to_standard_note()
+        score = score.correct_chord_octave()
+        score = score.split_too_long_chords(8)
+        return score
+
+    def correct_chord_octave(self):
+        """
+        Correct chord octaves to minimize distance with central C
+        Returns
+        -------
+        score: Score
+        """
+        return sum([c.correct_chord_octave() for c in self.chords], None)
+
     def octaver(self, **instruments_octaves):
         """
         Transpose down octave per instrument
 
 
         Parameters
         ----------
@@ -591,31 +617,63 @@
         import os
         directory = os.path.dirname(filepath)
         if create_dir and not os.path.exists(directory):
             os.makedirs(directory)
         with open(filepath, 'wb') as f:
             pickle.dump(self, f)
 
-    def predict_score(self):
+    def predict_score(self, temperature=0.5, top_k=10):
         """
         Predict the continuation of the score given the current score
-        Currently it takes no argument.
+
         Please note that this method is still very experimental as we are
         currently improving our musiclang language model.
 
         Returns
         -------
         predicted_score: Score
             The predicted score
 
+        temperature: float
+            The temperature of the prediction. The higher the more random
+            To avoid syntax errors set lower than 0.75
+        top_k: int
+            The number of tokens to consider for the prediction.
+            The higher the more random
+            To avoid syntax errors set lower than 20
+
         """
         from musiclang.predict.predictors import predict_score_from_hugginface
-        score_str = predict_score_from_hugginface(str(self))
+        score_str = predict_score_from_hugginface(str(self.normalize()), temperature=temperature, top_k=top_k)
         return Score.from_str(score_str)
 
+
+    def split_too_long_chords(self, max_length):
+        """
+        Split the chords that are too long into smaller chords
+        Parameters
+        ----------
+        max_length: fraction
+            The maximum length of a chord
+
+        Returns
+        -------
+        score: Score
+            The score with shorter chords
+
+        """
+
+        new_score = None
+        for chord in self:
+            if chord.duration > max_length:
+                new_score += chord.split(max_length)
+            else:
+                new_score += chord
+        return new_score
+
     def to_text_file(self, filepath, create_dir=False):
         """
         Save as a musiclang txt file
         Parameters
         ----------
         filepath
         create_dir: bool (Default value = False)
@@ -884,15 +942,17 @@
         -------
         score: Score
                The loaded score
 
         """
         from musiclang.analyze import parse_to_musiclang
         score, config = parse_to_musiclang(filename)
-        score.config = config
+        real_config = {**score.config, **config}
+        score = score.normalize()
+        score.config = real_config
         return score
 
     def to_extension_note(self):
         return Score([chord.to_extension_note() for chord in self.chords], tags=set(self.tags))
 
     def to_chord_note(self):
         return Score([chord.to_chord_note() for chord in self.chords], tags=set(self.tags))
@@ -940,16 +1000,23 @@
             return self
         else:
             return self.copy()
 
 
     @classmethod
     def from_str(cls, s):
-
-        return eval(str(s).replace('\n', ''))
+        try:
+            from musiclang import Chord
+            pattern = re.compile(r'(?<=\))\s*\+\s*(?=\()')
+            data = re.split(pattern, str(s))
+            chords = [eval(str(d).replace('\n', '')) for d in data]
+            assert isinstance(chords[0], Chord)
+            return Score(chords)
+        except:
+            return eval(str(s).replace('\n', ''))
 
     @classmethod
     def from_sequence(cls, sequence, **kwargs):
         """
 
         Parameters
         ----------
@@ -1068,14 +1135,29 @@
 
         """
         from .out.to_code import chord_serie_to_code
 
         code = chord_serie_to_code(self, **kwargs)
         return code
 
+
+    def realize_tags(self):
+        new_score = None
+        last_notes = {}
+        final_notes = {}
+        for idx, chord in enumerate(self.chords):
+            if idx > 0:
+                last_notes = {instrument: self.chords[idx-1].score[instrument].notes[-1] for instrument in self.chords[idx-1].score.keys()}
+            if idx < len(self.chords)-1:
+                final_notes = {instrument: self.chords[idx+1].score[instrument].notes[0] for instrument in self.chords[idx+1].score.keys()}
+
+            new_score += chord.realize_tags(last_note=last_notes, final_note=final_notes)
+
+        return new_score
+
     def to_code_file(self, filepath, **kwargs):
         """Export the chord serie as a file representing valid python code that recreates the score
 
         Parameters
         ----------
         filepath :
             return:
```

### Comparing `musiclang-0.8.2/musiclang/write/sequence/sequence.py` & `musiclang-0.8.3/musiclang/write/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/sequence/sequence_utils.py` & `musiclang-0.8.3/musiclang/write/sequence/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/time_utils/time_utils.py` & `musiclang-0.8.3/musiclang/write/time_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang/write/tonality.py` & `musiclang-0.8.3/musiclang/write/tonality.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/musiclang.egg-info/PKG-INFO` & `musiclang-0.8.3/musiclang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.2
+Version: 0.8.3
 Summary: A python package for music notation and generation
 Home-page: UNKNOWN
 Author: Florian GARDIN
 Author-email: fgardin.pro@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/MusicLang/musiclang/
@@ -114,15 +114,15 @@
         	piano__0=s2.ed.mp + r.s, 
         	piano__2=s4.ed.mp + r.s, 
         	piano__4=s6.ed.o(-1).mp + r.s, 
         	piano__5=s0.ed.o(-1).mp + r.s, 
         	piano__6=s4.ed.o(-1).mp + r.s))
         
         # Predict a continuation of the score using hugginface musiclang model
-        predicted_score = score.predict_score()
+        predicted_score = score.predict_score(temperature=0.5)
         # Save it to midi
         predicted_score.to_midi('test.mid')
         ```
         
         Please note that this feature is still experimental, it will only work with
         piano music for now and the model is not yet trained on a large corpus of music.
         If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
```

### Comparing `musiclang-0.8.2/musiclang.egg-info/SOURCES.txt` & `musiclang-0.8.3/musiclang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 musiclang/analyze/augmented_net/output_representations.py
 musiclang/analyze/augmented_net/score_parser.py
 musiclang/analyze/augmented_net/utils.py
 musiclang/predict/__init__.py
 musiclang/predict/arranger/__init__.py
 musiclang/predict/arranger/arranger.py
 musiclang/predict/arranger/arranger_trainer.py
+musiclang/predict/arranger/melody_arranger.py
+musiclang/predict/arranger/melody_arranger_trainer.py
 musiclang/predict/composer/__init__.py
 musiclang/predict/composer/auto_composer.py
 musiclang/predict/composer/composer.py
 musiclang/predict/composer/harmony.py
 musiclang/predict/predictors/__init__.py
 musiclang/predict/predictors/huggin.py
 musiclang/predict/predictors/windowed.py
```

### Comparing `musiclang-0.8.2/pyproject.toml` & `musiclang-0.8.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "musiclang"
-version = "0.8.2"
+version = "0.8.3"
 description = "A python package for music notation and generation"
 readme = "README.md"
 authors = [{ name = "Florian GARDIN", email = "fgardin.pro@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `musiclang-0.8.2/setup.py` & `musiclang-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="musiclang",
-    version="0.8.2",
+    version="0.8.3",
     author="Florian GARDIN",
     author_email="fgardin.pro@gmail.com",
     description=("A python package for music notation and generation"
                 ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
```

### Comparing `musiclang-0.8.2/tests/analyze/test_score_formatter.py` & `musiclang-0.8.3/tests/analyze/test_score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/composing/test_project.py` & `musiclang-0.8.3/tests/composing/test_project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/composing/test_voice_leading.py` & `musiclang-0.8.3/tests/composing/test_voice_leading.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/predict/test_auto_composer.py` & `musiclang-0.8.3/tests/predict/test_auto_composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/transform/test_mask.py` & `musiclang-0.8.3/tests/transform/test_mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/transform/test_pipeline.py` & `musiclang-0.8.3/tests/transform/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/transform/test_transforms.py` & `musiclang-0.8.3/tests/transform/test_transforms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/out/test_to_midi.py` & `musiclang-0.8.3/tests/write/out/test_to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/pitches/test_pitches_utils.py` & `musiclang-0.8.3/tests/write/pitches/test_pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/properties/test_note_properties.py` & `musiclang-0.8.3/tests/write/properties/test_note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/rythm/test_metric.py` & `musiclang-0.8.3/tests/write/rythm/test_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_bass_notes.py` & `musiclang-0.8.3/tests/write/test_bass_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_chord.py` & `musiclang-0.8.3/tests/write/test_chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_chord_notes.py` & `musiclang-0.8.3/tests/write/test_chord_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_drum_notes.py` & `musiclang-0.8.3/tests/write/test_drum_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_extensions.py` & `musiclang-0.8.3/tests/write/test_extensions.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_note.py` & `musiclang-0.8.3/tests/write/test_note.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.2/tests/write/test_score.py` & `musiclang-0.8.3/tests/write/test_score.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,8 +137,27 @@
     expected_result = ((I % II.M)(
 	piano__0=b0 + su1 + b0 + su1,
 	piano__1=b1.e + bu1.e + bd1 + b1.e + bu1.e + bd1))
 
     score_voicing = (I % II.M)(b0.w, b1.w)
 
     result_score = pattern.project_pattern(score_voicing, restart_each_chord=False)
-    assert expected_result == result_score
+    assert expected_result == result_score
+
+from musiclang.library import *
+
+def test_split_too_long_chords():
+    score = None + (I %V.M)(s0.augment(7) + s1.augment(2), s4.augment(9))
+
+    splitted_score = score.split_too_long_chords(8)
+
+    print(splitted_score)
+
+    expected_score = (
+    (I % V.M)(
+        piano__0=s0.augment(frac(7, 1)) + s1,
+        piano__1=s4.augment(frac(8, 1)))+
+    (I % V.M)(
+        piano__0=l,
+        piano__1=l)
+    )
+    assert splitted_score == expected_score
```

### Comparing `musiclang-0.8.2/tests/write/test_tonality.py` & `musiclang-0.8.3/tests/write/test_tonality.py`

 * *Files identical despite different names*

