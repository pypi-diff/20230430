# Comparing `tmp/toml_tools-1.0.0.tar.gz` & `tmp/toml_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_tools-1.0.0.tar", last modified: Sat Apr 29 22:36:10 2023, max compression
+gzip compressed data, was "toml_tools-1.1.0.tar", last modified: Sun Apr 30 21:22:52 2023, max compression
```

## Comparing `toml_tools-1.0.0.tar` & `toml_tools-1.1.0.tar`

### file list

```diff
@@ -1,1085 +1,31 @@
--rw-r--r--   0        0        0     1973 2023-04-29 19:23:43.119770 toml_tools-1.0.0/.gitignore
--rw-r--r--   0        0        0     1093 2023-04-29 19:23:43.119770 toml_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0      124 2023-04-29 19:23:43.119770 toml_tools-1.0.0/LICENSE-HEADER
--rw-r--r--   0        0        0    13663 2023-04-29 22:35:27.820113 toml_tools-1.0.0/README.md
--rw-r--r--   0        0        0     1145 2023-04-29 18:26:02.632538 toml_tools-1.0.0/benchmark/LICENSE
--rw-r--r--   0        0        0      499 2023-04-29 21:48:45.395219 toml_tools-1.0.0/benchmark/README.md
--rw-r--r--   0        0        0     4021 2023-04-29 18:26:02.632538 toml_tools-1.0.0/benchmark/data.toml
--rw-r--r--   0        0        0      200 2023-04-29 18:26:02.648159 toml_tools-1.0.0/benchmark/requirements.txt
--rw-r--r--   0        0        0     2343 2023-04-29 21:46:20.074116 toml_tools-1.0.0/benchmark/run.py
--rw-r--r--   0        0        0      962 2023-04-29 20:33:06.670966 toml_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      421 2023-04-29 20:44:41.018432 toml_tools-1.0.0/src/toml_tools/__init__.py
--rw-r--r--   0        0        0      444 2023-04-29 21:12:30.876917 toml_tools-1.0.0/src/toml_tools/_helpers.py
--rw-r--r--   0        0        0    23697 2023-04-29 21:41:46.370600 toml_tools-1.0.0/src/toml_tools/_parser.py
--rw-r--r--   0        0        0     2990 2023-04-29 21:02:43.422755 toml_tools-1.0.0/src/toml_tools/_re.py
--rw-r--r--   0        0        0     7829 2023-04-29 21:12:00.651302 toml_tools-1.0.0/src/toml_tools/_writer.py
--rw-r--r--   0        0        0      300 2023-04-29 20:46:08.005110 toml_tools-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4169 2023-04-29 20:46:16.800553 toml_tools-1.0.0/tests/burntsushi.py
--rw-r--r--   0        0        0       71 2023-04-29 20:23:21.975482 toml_tools-1.0.0/tests/data/extras/valid/apostrophes-in-literal-string.toml
--rw-r--r--   0        0        0       62 2023-04-29 20:23:21.976488 toml_tools-1.0.0/tests/data/extras/valid/array/array-subtables.toml
--rw-r--r--   0        0        0       51 2023-04-29 20:23:21.977487 toml_tools-1.0.0/tests/data/extras/valid/array/open-parent-table.toml
--rw-r--r--   0        0        0       22 2023-04-29 20:23:21.978489 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-empty.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:21.979490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-hetergeneous.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:21.980490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-nested-inline-table.toml
--rw-r--r--   0        0        0       23 2023-04-29 20:23:21.981484 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-nested.toml
--rw-r--r--   0        0        0       16 2023-04-29 20:23:21.982486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-nospaces.toml
--rw-r--r--   0        0        0       21 2023-04-29 20:23:21.982486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-string-quote-comma-2.toml
--rw-r--r--   0        0        0       60 2023-04-29 20:23:21.983486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-string-quote-comma.toml
--rw-r--r--   0        0        0       56 2023-04-29 20:23:21.984490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-string-with-comma.toml
--rw-r--r--   0        0        0       32 2023-04-29 20:23:21.984490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array-table-array-string-backslash.toml
--rw-r--r--   0        0        0      215 2023-04-29 20:23:21.985487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/array.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:21.985487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/arrays-hetergeneous.toml
--rw-r--r--   0        0        0       23 2023-04-29 20:23:21.986486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/arrays-nested.toml
--rw-r--r--   0        0        0      215 2023-04-29 20:23:21.987486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/arrays.toml
--rw-r--r--   0        0        0       21 2023-04-29 20:23:21.987486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/bool.toml
--rw-r--r--   0        0        0       87 2023-04-29 20:23:21.988487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comment-at-eof.toml
--rw-r--r--   0        0        0       87 2023-04-29 20:23:21.988487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comment-at-eof2.toml
--rw-r--r--   0        0        0      480 2023-04-29 20:23:21.989485 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comment-everywhere.toml
--rw-r--r--   0        0        0      416 2023-04-29 20:23:21.989485 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comment-tricky.toml
--rw-r--r--   0        0        0       87 2023-04-29 20:23:21.990487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comments-at-eof.toml
--rw-r--r--   0        0        0       85 2023-04-29 20:23:21.990487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comments-at-eof2.toml
--rw-r--r--   0        0        0      480 2023-04-29 20:23:21.991485 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/comments-everywhere.toml
--rw-r--r--   0        0        0       26 2023-04-29 20:23:21.992489 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/datetime-local-date.toml
--rw-r--r--   0        0        0       56 2023-04-29 20:23:21.992489 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/datetime-local-time.toml
--rw-r--r--   0        0        0      121 2023-04-29 20:23:21.993489 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/datetime-local.toml
--rw-r--r--   0        0        0       41 2023-04-29 20:23:21.993489 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/datetime-timezone.toml
--rw-r--r--   0        0        0      168 2023-04-29 20:23:21.994486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/datetime.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:21.996485 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/double-quote-escape.toml
--rw-r--r--   0        0        0        0 2023-04-29 20:23:21.996485 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/empty-file.toml
--rw-r--r--   0        0        0        0 2023-04-29 20:23:21.997484 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/empty.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:21.998490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/escaped-escape.toml
--rw-r--r--   0        0        0       96 2023-04-29 20:23:21.998490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/example.toml
--rw-r--r--   0        0        0       51 2023-04-29 20:23:21.999487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/exponent-part-float.toml
--rw-r--r--   0        0        0      122 2023-04-29 20:23:22.000483 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/float-exponent.toml
--rw-r--r--   0        0        0      240 2023-04-29 20:23:22.001487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/float-inf-and-nan.toml
--rw-r--r--   0        0        0       60 2023-04-29 20:23:22.001487 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/float-long.toml
--rw-r--r--   0        0        0       59 2023-04-29 20:23:22.002484 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/float-underscore.toml
--rw-r--r--   0        0        0       63 2023-04-29 20:23:22.003486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/float.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:22.004488 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/implicit-and-explicit-after.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:22.005494 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/implicit-and-explicit-before.toml
--rw-r--r--   0        0        0       22 2023-04-29 20:23:22.005494 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/implicit-groups.toml
--rw-r--r--   0        0        0      173 2023-04-29 20:23:22.006491 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table-array.toml
--rw-r--r--   0        0        0      163 2023-04-29 20:23:22.007488 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table-empty.toml
--rw-r--r--   0        0        0       71 2023-04-29 20:23:22.008490 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table-end-in-bool.toml
--rw-r--r--   0        0        0       92 2023-04-29 20:23:22.009491 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table-multiline.toml
--rw-r--r--   0        0        0      382 2023-04-29 20:23:22.010486 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table-nest.toml
--rw-r--r--   0        0        0      162 2023-04-29 20:23:22.011736 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/inline-table.toml
--rw-r--r--   0        0        0      110 2023-04-29 20:23:22.012741 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/integer-literals.toml
--rw-r--r--   0        0        0       64 2023-04-29 20:23:22.012741 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/integer-long.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.013743 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/integer-underscore.toml
--rw-r--r--   0        0        0       57 2023-04-29 20:23:22.014739 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/integer.toml
--rw-r--r--   0        0        0      187 2023-04-29 20:23:22.015738 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-alphanum.toml
--rw-r--r--   0        0        0      216 2023-04-29 20:23:22.016755 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-case-sensitive.toml
--rw-r--r--   0        0        0      105 2023-04-29 20:23:22.017745 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-dotted.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.018742 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-empty.toml
--rw-r--r--   0        0        0       11 2023-04-29 20:23:22.019739 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-equals-nospace.toml
--rw-r--r--   0        0        0      159 2023-04-29 20:23:22.020742 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-escapes.toml
--rw-r--r--   0        0        0        7 2023-04-29 20:23:22.021746 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-numeric.toml
--rw-r--r--   0        0        0      122 2023-04-29 20:23:22.022747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-quoted-dots.toml
--rw-r--r--   0        0        0       11 2023-04-29 20:23:22.023748 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-space.toml
--rw-r--r--   0        0        0       43 2023-04-29 20:23:22.024757 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-special-chars.toml
--rw-r--r--   0        0        0       78 2023-04-29 20:23:22.025744 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/key-special-word.toml
--rw-r--r--   0        0        0      120 2023-04-29 20:23:22.026740 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/keys-with-dots.toml
--rw-r--r--   0        0        0       60 2023-04-29 20:23:22.027747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/long-float.toml
--rw-r--r--   0        0        0       64 2023-04-29 20:23:22.028743 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/long-integer.toml
--rw-r--r--   0        0        0      109 2023-04-29 20:23:22.029747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/multiline-string-accidental-whitespace.toml
--rw-r--r--   0        0        0      318 2023-04-29 20:23:22.030746 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/multiline-string-quotes.toml
--rw-r--r--   0        0        0      417 2023-04-29 20:23:22.031746 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/multiline-string.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:22.032738 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/nested-inline-table-array.toml
--rw-r--r--   0        0        0       30 2023-04-29 20:23:22.033747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/newline-crlf.toml
--rw-r--r--   0        0        0       29 2023-04-29 20:23:22.034747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/newline-lf.toml
--rw-r--r--   0        0        0      204 2023-04-29 20:23:22.034747 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/raw-multiline-string.toml
--rw-r--r--   0        0        0      380 2023-04-29 20:23:22.035740 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/raw-string.toml
--rw-r--r--   0        0        0       71 2023-04-29 20:23:22.036738 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/right-curly-brace-after-boolean.toml
--rw-r--r--   0        0        0      399 2023-04-29 20:23:22.037736 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/spec-example-1-compact.toml
--rw-r--r--   0        0        0      592 2023-04-29 20:23:22.038751 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/spec-example-1.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.038751 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-double-quote-escape.toml
--rw-r--r--   0        0        0       13 2023-04-29 20:23:22.039746 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-empty.toml
--rw-r--r--   0        0        0      343 2023-04-29 20:23:22.041751 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-escape-tricky.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.041751 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-escaped-escape.toml
--rw-r--r--   0        0        0      784 2023-04-29 20:23:22.042742 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-escapes.toml
--rw-r--r--   0        0        0      121 2023-04-29 20:23:22.043746 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-nl.toml
--rw-r--r--   0        0        0       48 2023-04-29 20:23:22.045040 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-simple.toml
--rw-r--r--   0        0        0       44 2023-04-29 20:23:22.046046 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-unicode-escape.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.046046 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-unicode-literal.toml
--rw-r--r--   0        0        0      115 2023-04-29 20:23:22.047043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/string-with-pound.toml
--rw-r--r--   0        0        0       39 2023-04-29 20:23:22.048042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-array-implicit.toml
--rw-r--r--   0        0        0      174 2023-04-29 20:23:22.049044 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-array-many.toml
--rw-r--r--   0        0        0      279 2023-04-29 20:23:22.050044 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-array-nest.toml
--rw-r--r--   0        0        0       61 2023-04-29 20:23:22.051043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-array-one.toml
--rw-r--r--   0        0        0      115 2023-04-29 20:23:22.052044 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-array-table-array.toml
--rw-r--r--   0        0        0        5 2023-04-29 20:23:22.053045 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-empty.toml
--rw-r--r--   0        0        0        9 2023-04-29 20:23:22.054042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-no-eol.toml
--rw-r--r--   0        0        0       12 2023-04-29 20:23:22.054042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-sub-empty.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.055042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-whitespace.toml
--rw-r--r--   0        0        0       45 2023-04-29 20:23:22.056044 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-with-literal-string.toml
--rw-r--r--   0        0        0       28 2023-04-29 20:23:22.057043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-with-pound.toml
--rw-r--r--   0        0        0       41 2023-04-29 20:23:22.057043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-with-single-quotes.toml
--rw-r--r--   0        0        0      125 2023-04-29 20:23:22.058042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/table-without-super.toml
--rw-r--r--   0        0        0       36 2023-04-29 20:23:22.059043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/underscored-float.toml
--rw-r--r--   0        0        0       21 2023-04-29 20:23:22.059043 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/underscored-integer.toml
--rw-r--r--   0        0        0       44 2023-04-29 20:23:22.060042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/unicode-escape.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.061042 toml_tools-1.0.0/tests/data/extras/valid/burntsushi-repo/unicode-literal.toml
--rw-r--r--   0        0        0       36 2023-04-29 20:23:22.062045 toml_tools-1.0.0/tests/data/extras/valid/empty-inline-table.toml
--rw-r--r--   0        0        0       52 2023-04-29 20:23:22.062045 toml_tools-1.0.0/tests/data/extras/valid/five-quotes.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:22.064041 toml_tools-1.0.0/tests/data/extras/valid/multiline-basic-str/ends-in-whitespace-escape.toml
--rw-r--r--   0        0        0       24 2023-04-29 20:23:22.064041 toml_tools-1.0.0/tests/data/extras/valid/no-newlines.toml
--rw-r--r--   0        0        0     1100 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/COPYING
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/missing-separator.toml
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/no-close-2.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/no-close-table-2.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/no-close-table.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/no-close.toml
--rw-r--r--   0        0        0       59 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/tables-1.toml
--rw-r--r--   0        0        0      198 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/tables-2.toml
--rw-r--r--   0        0        0       74 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/text-after-array-entries.toml
--rw-r--r--   0        0        0       75 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/text-before-array-separator.toml
--rw-r--r--   0        0        0       61 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/array/text-in-array.toml
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/bool/mixed-case.toml
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.130286 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/bool/wrong-case-false.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/bool/wrong-case-true.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/bare-null.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/comment-cr.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/comment-del.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/comment-lf.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/comment-null.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/comment-us.toml
--rw-r--r--   0        0        0      645 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/control.multi
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/multi-del.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/multi-lf.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/multi-null.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/multi-us.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawmulti-del.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawmulti-lf.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawmulti-null.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawmulti-us.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawstring-del.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawstring-lf.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawstring-null.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/rawstring-us.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/string-bs.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/string-del.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/string-lf.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/string-null.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/control/string-us.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/hour-over.toml
--rw-r--r--   0        0        0      140 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/mday-over.toml
--rw-r--r--   0        0        0      140 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/mday-under.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/minute-over.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/month-over.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.145927 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/month-under.toml
--rw-r--r--   0        0        0       95 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/no-leads-with-milli.toml
--rw-r--r--   0        0        0       92 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/no-leads.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/no-secs.toml
--rw-r--r--   0        0        0       72 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/no-t.toml
--rw-r--r--   0        0        0      140 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/second-over.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/time-no-leads-2.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/time-no-leads.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/datetime/trailing-t.toml
--rw-r--r--   0        0        0      246 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/bad-utf8-at-end.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/bad-utf8-in-comment.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/bad-utf8-in-string.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/bom-not-at-start-1.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/bom-not-at-start-2.toml
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/utf16-bom.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/encoding/utf16.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/double-point-1.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/double-point-2.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-double-e-1.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-double-e-2.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-double-us.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-leading-us.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-point-1.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-point-2.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/exp-trailing-us.toml
--rw-r--r--   0        0        0      737 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/float.multi
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/inf-incomplete-1.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/inf-incomplete-2.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/inf-incomplete-3.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/inf_underscore.toml
--rw-r--r--   0        0        0       29 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-point-neg.toml
--rw-r--r--   0        0        0       30 2023-04-29 19:23:43.161554 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-point-plus.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-point.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-us.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-zero-neg.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-zero-plus.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/leading-zero.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/nan-incomplete-1.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/nan-incomplete-2.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/nan-incomplete-3.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/nan_underscore.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/trailing-point-min.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/trailing-point-plus.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/trailing-point.toml
--rw-r--r--   0        0        0      157 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/trailing-us-exp.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/trailing-us.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/us-after-point.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/float/us-before-point.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/double-comma.toml
--rw-r--r--   0        0        0       67 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/duplicate-key.toml
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/empty.toml
--rw-r--r--   0        0        0      115 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/linebreak-1.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/linebreak-2.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/linebreak-3.toml
--rw-r--r--   0        0        0       79 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/linebreak-4.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/no-comma.toml
--rw-r--r--   0        0        0       93 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/overwrite.toml
--rw-r--r--   0        0        0      143 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/inline-table/trailing-comma.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/capital-bin.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/capital-hex.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.177179 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/capital-oct.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/double-sign-nex.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/double-sign-plus.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/double-us.toml
--rw-r--r--   0        0        0      741 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/integer.multi
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/invalid-bin.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/invalid-hex.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/invalid-oct.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-us-bin.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-us-hex.toml
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-us-oct.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-us.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-1.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-2.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-3.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-sign-1.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-sign-2.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/leading-zero-sign-3.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/negative-bin.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/negative-hex.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/negative-oct.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/positive-bin.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/positive-hex.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/positive-oct.toml
--rw-r--r--   0        0        0       34 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/text-after-integer.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/trailing-us-bin.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/trailing-us-hex.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.192803 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/trailing-us-oct.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/trailing-us.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/us-after-bin.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/us-after-hex.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/integer/us-after-oct.toml
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/after-array.toml
--rw-r--r--   0        0        0       37 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/after-table.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/after-value.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/bare-invalid-character.toml
--rw-r--r--   0        0        0       80 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/dotted-redefine-table.toml
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/duplicate-keys.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/duplicate.toml
--rw-r--r--   0        0        0        6 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/empty.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/escape.toml
--rw-r--r--   0        0        0        8 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/hash.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/multiline.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/newline.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/no-eol.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/open-bracket.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/partial-quoted.toml
--rw-r--r--   0        0        0        3 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/single-open-bracket.toml
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/space.toml
--rw-r--r--   0        0        0       30 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/special-character.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/start-bracket.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/two-equals.toml
--rw-r--r--   0        0        0        6 2023-04-29 19:23:43.208428 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/two-equals2.toml
--rw-r--r--   0        0        0        7 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/two-equals3.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/without-value-1.toml
--rw-r--r--   0        0        0        8 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/key/without-value-2.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-byte-escape.toml
--rw-r--r--   0        0        0       82 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-codepoint.toml
--rw-r--r--   0        0        0       30 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-concat.toml
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-escape-1.toml
--rw-r--r--   0        0        0       65 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-escape-2.toml
--rw-r--r--   0        0        0       35 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-multiline.toml
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-slash-escape.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/bad-uni-esc.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.224054 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-byte-escapes.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-multiline-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-multiline-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-multiline-quotes.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-multiline-unknown-escape.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/basic-unknown-escape.toml
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/literal-multiline-quotes-1.toml
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/literal-multiline-quotes-2.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/missing-quotes.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-bad-escape-1.toml
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-bad-escape-2.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-bad-escape-3.toml
--rw-r--r--   0        0        0       31 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-escape-space.toml
--rw-r--r--   0        0        0        7 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-no-close-2.toml
--rw-r--r--   0        0        0       35 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-no-close.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-quotes-1.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/multiline-quotes-2.toml
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/no-close.toml
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/text-after-string.toml
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/string/wrong-close.toml
--rw-r--r--   0        0        0      508 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/append-with-dotted-keys-1.toml
--rw-r--r--   0        0        0      270 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/append-with-dotted-keys-2.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/array-empty.toml
--rw-r--r--   0        0        0      636 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/array-implicit.toml
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/array-missing-bracket.toml
--rw-r--r--   0        0        0       57 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate-key-dotted-table.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate-key-dotted-table2.toml
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.230570 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate-key-table.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate-table-array.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate-table-array2.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/duplicate.toml
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/empty-implicit-table.toml
--rw-r--r--   0        0        0        4 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/empty.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/equals-sign.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/llbrace.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/nested-brackets-close.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/nested-brackets-open.toml
--rw-r--r--   0        0        0       36 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/quoted-no-close.toml
--rw-r--r--   0        0        0       84 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/redefine.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/rrbrace.toml
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/text-after-table.toml
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/whitespace.toml
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/burntsushi/invalid/table/with-pound.toml
--rw-r--r--   0        0        0     1183 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/LICENSE
--rw-r--r--   0        0        0      316 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/README.md
--rw-r--r--   0        0        0       59 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/array/array-of-tables-1.toml
--rw-r--r--   0        0        0      198 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/array/array-of-tables-2.toml
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/comment/comment-control-1.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/comment/comment-control-2.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/comment/comment-control-3.toml
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/comment/comment-control-4.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/integer/int-0-padded.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.246215 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/integer/int-signed-bin.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/integer/int-signed-hex.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/integer/int-signed-oct.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/bare-key-1.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/bare-key-2.toml
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/bare-key-3.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/key-value-pair-1.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/key-value-pair-2.toml
--rw-r--r--   0        0        0      233 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/multiple-dot-key.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/multiple-key.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/key-value/no-key-name.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-control-1.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-control-2.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-control-3.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-control-4.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-control-1.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-control-2.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-control-3.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-control-4.toml
--rw-r--r--   0        0        0       31 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-invalid-backslash.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.261840 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-quotes.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-multiline-unknown-escape.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-basic-unknown-escape.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-control-1.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-control-2.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-control-3.toml
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-control-4.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-multiline-control-1.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-multiline-control-2.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-multiline-control-4.toml
--rw-r--r--   0        0        0       73 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/string/string-literal-multiline-quotes.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/inline-table-immutable-1.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/inline-table-immutable-2.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/inline-table-trailing-comma.toml
--rw-r--r--   0        0        0       74 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-1.toml
--rw-r--r--   0        0        0       88 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-2.toml
--rw-r--r--   0        0        0       84 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-3.toml
--rw-r--r--   0        0        0       90 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-4.toml
--rw-r--r--   0        0        0      250 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-invalid-1.toml
--rw-r--r--   0        0        0       59 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-invalid-2.toml
--rw-r--r--   0        0        0      279 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-invalid-3.toml
--rw-r--r--   0        0        0      276 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/_external/toml-lang-compliance/invalid/table/table-invalid-4.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.277466 toml_tools-1.0.0/tests/data/invalid/array-missing-comma.toml
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/array-of-tables/overwrite-array-in-parent.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/array-of-tables/overwrite-bool-with-aot.toml
--rw-r--r--   0        0        0        4 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/array/file-end-after-val.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/array/unclosed-after-item.toml
--rw-r--r--   0        0        0        3 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/array/unclosed-empty.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/basic-str-ends-in-escape.toml
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/boolean/invalid-false-casing.toml
--rw-r--r--   0        0        0        8 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/boolean/invalid-true-casing.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/dates-and-times/invalid-day.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/dotted-keys/access-non-table.toml
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/dotted-keys/extend-defined-aot.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/dotted-keys/extend-defined-table-with-subtable.toml
--rw-r--r--   0        0        0       36 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/dotted-keys/extend-defined-table.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table-missing-comma.toml
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/define-twice-in-subtable.toml
--rw-r--r--   0        0        0       30 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/define-twice.toml
--rw-r--r--   0        0        0        6 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/file-end-after-key-val.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/mutate.toml
--rw-r--r--   0        0        0       75 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/override-val-in-table.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/override-val-with-array.toml
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.293089 toml_tools-1.0.0/tests/data/invalid/inline-table/override-val-with-table.toml
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/inline-table/overwrite-implicitly.toml
--rw-r--r--   0        0        0       53 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/inline-table/overwrite-value-in-inner-array.toml
--rw-r--r--   0        0        0       55 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/inline-table/overwrite-value-in-inner-table.toml
--rw-r--r--   0        0        0        3 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/inline-table/unclosed-empty.toml
--rw-r--r--   0        0        0       39 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/invalid-comment-char.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/invalid-escaped-unicode.toml
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/invalid-hex.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/keys-and-vals/ends-early-table-def.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/keys-and-vals/ends-early.toml
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/keys-and-vals/no-value.toml
--rw-r--r--   0        0        0        3 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/keys-and-vals/only-ws-after-dot.toml
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/keys-and-vals/overwrite-with-deep-table.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/literal-str/unclosed.toml
--rw-r--r--   0        0        0       36 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/missing-closing-double-square-bracket.toml
--rw-r--r--   0        0        0       36 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/missing-closing-square-bracket.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-basic-str/carriage-return.toml
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-basic-str/escape-only.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-basic-str/file-ends-after-opening.toml
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-basic-str/last-line-escape.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-basic-str/unclosed-ends-in-whitespace-escape.toml
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-literal-str/file-ends-after-opening.toml
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/multiline-literal-str/unclosed.toml
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/non-scalar-escaped.toml
--rw-r--r--   0        0        0        1 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/table/eof-after-opening.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.308716 toml_tools-1.0.0/tests/data/invalid/table/redefine-1.toml
--rw-r--r--   0        0        0       31 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/invalid/table/redefine-2.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/invalid/unclosed-multiline-string.toml
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/invalid/unclosed-string.toml
--rw-r--r--   0        0        0     1183 2023-04-29 20:23:22.066046 toml_tools-1.0.0/tests/data/toml-lang-compliance/LICENSE
--rw-r--r--   0        0        0      316 2023-04-29 20:23:22.067042 toml_tools-1.0.0/tests/data/toml-lang-compliance/README.md
--rw-r--r--   0        0        0       24 2023-04-29 20:23:22.068042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-1.toml
--rw-r--r--   0        0        0       39 2023-04-29 20:23:22.069042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-2.toml
--rw-r--r--   0        0        0       47 2023-04-29 20:23:22.069042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-3.toml
--rw-r--r--   0        0        0       68 2023-04-29 20:23:22.070042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-4.toml
--rw-r--r--   0        0        0       52 2023-04-29 20:23:22.071042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-5.toml
--rw-r--r--   0        0        0       29 2023-04-29 20:23:22.072041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-7.toml
--rw-r--r--   0        0        0       43 2023-04-29 20:23:22.072041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-8.toml
--rw-r--r--   0        0        0       38 2023-04-29 20:23:22.073048 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-mixed-number-types.toml
--rw-r--r--   0        0        0      143 2023-04-29 20:23:22.074043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-more-mixed-types.toml
--rw-r--r--   0        0        0      128 2023-04-29 20:23:22.074043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-of-tables-1.toml
--rw-r--r--   0        0        0      270 2023-04-29 20:23:22.075043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-of-tables-2.toml
--rw-r--r--   0        0        0      112 2023-04-29 20:23:22.076042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/array/spec-array-of-tables-3.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.076042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/boolean/spec-boolean-1.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.077042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/boolean/spec-boolean-2.toml
--rw-r--r--   0        0        0      126 2023-04-29 20:23:22.079044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/comment/spec-comment-mid-array.toml
--rw-r--r--   0        0        0       37 2023-04-29 20:23:22.079044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/comment/spec-comment-mid-string.toml
--rw-r--r--   0        0        0      136 2023-04-29 20:23:22.080045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/comment/spec-comment-tab.toml
--rw-r--r--   0        0        0       87 2023-04-29 20:23:22.081052 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/comment/spec-comment.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.082046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-local-1.toml
--rw-r--r--   0        0        0       29 2023-04-29 20:23:22.082046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-1.toml
--rw-r--r--   0        0        0       34 2023-04-29 20:23:22.083044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-2.toml
--rw-r--r--   0        0        0       41 2023-04-29 20:23:22.083044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-3.toml
--rw-r--r--   0        0        0       29 2023-04-29 20:23:22.084045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-4.toml
--rw-r--r--   0        0        0       33 2023-04-29 20:23:22.085044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-5.toml
--rw-r--r--   0        0        0       34 2023-04-29 20:23:22.085044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-6.toml
--rw-r--r--   0        0        0       28 2023-04-29 20:23:22.086046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-local-1.toml
--rw-r--r--   0        0        0       35 2023-04-29 20:23:22.086046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-date-time-local-2.toml
--rw-r--r--   0        0        0       16 2023-04-29 20:23:22.087042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-time-1.toml
--rw-r--r--   0        0        0       23 2023-04-29 20:23:22.087042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/date-time/spec-time-2.toml
--rw-r--r--   0        0        0       13 2023-04-29 20:23:22.089045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-1.toml
--rw-r--r--   0        0        0       32 2023-04-29 20:23:22.089045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-10.toml
--rw-r--r--   0        0        0       32 2023-04-29 20:23:22.090043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-11.toml
--rw-r--r--   0        0        0       32 2023-04-29 20:23:22.091041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-12.toml
--rw-r--r--   0        0        0       67 2023-04-29 20:23:22.092041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-13.toml
--rw-r--r--   0        0        0       28 2023-04-29 20:23:22.092041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-14.toml
--rw-r--r--   0        0        0       64 2023-04-29 20:23:22.093041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-15.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.093041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-2.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.094041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-3.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.095045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-4.toml
--rw-r--r--   0        0        0       13 2023-04-29 20:23:22.096046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-5.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.096046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-6.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.097043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-7.toml
--rw-r--r--   0        0        0       28 2023-04-29 20:23:22.097043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-8.toml
--rw-r--r--   0        0        0       13 2023-04-29 20:23:22.098044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/float/spec-float-9.toml
--rw-r--r--   0        0        0       12 2023-04-29 20:23:22.099041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-1.toml
--rw-r--r--   0        0        0       11 2023-04-29 20:23:22.100042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-2.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.100042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-3.toml
--rw-r--r--   0        0        0       12 2023-04-29 20:23:22.101042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-3a.toml
--rw-r--r--   0        0        0       12 2023-04-29 20:23:22.102041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-3b.toml
--rw-r--r--   0        0        0       12 2023-04-29 20:23:22.102041 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-4.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.103042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-5.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.103042 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-6.toml
--rw-r--r--   0        0        0       46 2023-04-29 20:23:22.104043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-7.toml
--rw-r--r--   0        0        0       19 2023-04-29 20:23:22.105045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-bin1.toml
--rw-r--r--   0        0        0       19 2023-04-29 20:23:22.105045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-hex1.toml
--rw-r--r--   0        0        0       19 2023-04-29 20:23:22.106045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-hex2.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:22.106045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-hex3.toml
--rw-r--r--   0        0        0       31 2023-04-29 20:23:22.107047 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-max.toml
--rw-r--r--   0        0        0       32 2023-04-29 20:23:22.107047 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-min.toml
--rw-r--r--   0        0        0       19 2023-04-29 20:23:22.108045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-oct1.toml
--rw-r--r--   0        0        0       49 2023-04-29 20:23:22.108045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/integer/spec-int-oct2.toml
--rw-r--r--   0        0        0       49 2023-04-29 20:23:22.109049 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-case-sensitive.toml
--rw-r--r--   0        0        0       96 2023-04-29 20:23:22.110043 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-dotted-keys-1.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.111044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-dotted-keys-2.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.111044 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-dotted-keys-3.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:22.112046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-empty-key-name-1.toml
--rw-r--r--   0        0        0       42 2023-04-29 20:23:22.113050 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-empty-key-name-2.toml
--rw-r--r--   0        0        0       15 2023-04-29 20:23:22.114052 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-1.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:22.115049 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-2.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:22.115049 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-3.toml
--rw-r--r--   0        0        0       16 2023-04-29 20:23:22.116047 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-4.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.117050 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-5.toml
--rw-r--r--   0        0        0        5 2023-04-29 20:23:22.117050 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-6.toml
--rw-r--r--   0        0        0        5 2023-04-29 20:23:22.118047 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-7.toml
--rw-r--r--   0        0        0       13 2023-04-29 20:23:22.119045 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-8.toml
--rw-r--r--   0        0        0       16 2023-04-29 20:23:22.120046 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-key-value-pair-9.toml
--rw-r--r--   0        0        0       22 2023-04-29 20:23:22.121051 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-newline-1.toml
--rw-r--r--   0        0        0       22 2023-04-29 20:23:22.122056 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-newline-2.toml
--rw-r--r--   0        0        0       33 2023-04-29 20:23:22.123053 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-newline-3.toml
--rw-r--r--   0        0        0       20 2023-04-29 20:23:22.124055 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-quoted-basic-keys-1.toml
--rw-r--r--   0        0        0       28 2023-04-29 20:23:22.125053 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/key-value/spec-quoted-literal-keys-1.toml
--rw-r--r--   0        0        0    14021 2023-04-29 20:23:22.126052 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-array-inline-1000.toml
--rw-r--r--   0        0        0     2011 2023-04-29 20:23:22.127051 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-array-inline-nested-1000.toml
--rw-r--r--   0        0        0    40016 2023-04-29 20:23:22.128490 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-key-literal-40kb.toml
--rw-r--r--   0        0        0    40016 2023-04-29 20:23:22.129491 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-key-string-40kb.toml
--rw-r--r--   0        0        0    40014 2023-04-29 20:23:22.131495 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-scalar-literal-40kb.toml
--rw-r--r--   0        0        0    40116 2023-04-29 20:23:22.132509 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-scalar-literal-multiline-40kb.toml
--rw-r--r--   0        0        0    40014 2023-04-29 20:23:22.133497 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-scalar-string-40kb.toml
--rw-r--r--   0        0        0    40116 2023-04-29 20:23:22.134496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-scalar-string-multiline-40kb.toml
--rw-r--r--   0        0        0    19914 2023-04-29 20:23:22.135493 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-table-inline-1000.toml
--rw-r--r--   0        0        0     8011 2023-04-29 20:23:22.135493 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/qa/qa-table-inline-nested-1000.toml
--rw-r--r--   0        0        0      578 2023-04-29 20:23:22.136496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/spec-readme-example.toml
--rw-r--r--   0        0        0       48 2023-04-29 20:23:22.137491 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-1.toml
--rw-r--r--   0        0        0       76 2023-04-29 20:23:22.138492 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-2.toml
--rw-r--r--   0        0        0       94 2023-04-29 20:23:22.139493 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-3.toml
--rw-r--r--   0        0        0       24 2023-04-29 20:23:22.140488 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-4.toml
--rw-r--r--   0        0        0       62 2023-04-29 20:23:22.140488 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-5.toml
--rw-r--r--   0        0        0       63 2023-04-29 20:23:22.141490 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-6.toml
--rw-r--r--   0        0        0       52 2023-04-29 20:23:22.142488 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-7.toml
--rw-r--r--   0        0        0       70 2023-04-29 20:23:22.142488 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-8.toml
--rw-r--r--   0        0        0       65 2023-04-29 20:23:22.143490 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-multiline-9.toml
--rw-r--r--   0        0        0       27 2023-04-29 20:23:22.143490 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-tab-multiline.toml
--rw-r--r--   0        0        0       23 2023-04-29 20:23:22.145493 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic-tab.toml
--rw-r--r--   0        0        0       76 2023-04-29 20:23:22.145493 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-basic.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.146497 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-1.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.147499 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-2.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.147499 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-3.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.148490 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-4.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.149498 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-5.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.150497 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-6.toml
--rw-r--r--   0        0        0       10 2023-04-29 20:23:22.151496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-7.toml
--rw-r--r--   0        0        0       14 2023-04-29 20:23:22.151496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-8.toml
--rw-r--r--   0        0        0       18 2023-04-29 20:23:22.152499 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-escape-9.toml
--rw-r--r--   0        0        0       40 2023-04-29 20:23:22.152499 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-1.toml
--rw-r--r--   0        0        0       41 2023-04-29 20:23:22.153491 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-2.toml
--rw-r--r--   0        0        0       40 2023-04-29 20:23:22.154497 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-3.toml
--rw-r--r--   0        0        0       25 2023-04-29 20:23:22.154497 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-4.toml
--rw-r--r--   0        0        0       45 2023-04-29 20:23:22.155496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-multiline-1.toml
--rw-r--r--   0        0        0      109 2023-04-29 20:23:22.156498 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-multiline-2.toml
--rw-r--r--   0        0        0       66 2023-04-29 20:23:22.156498 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-multiline-3.toml
--rw-r--r--   0        0        0       53 2023-04-29 20:23:22.157498 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/string/spec-string-literal-multiline-4.toml
--rw-r--r--   0        0        0      144 2023-04-29 20:23:22.158496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-extend-dotted-object-1.toml
--rw-r--r--   0        0        0      166 2023-04-29 20:23:22.159496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-extend-dotted-object-2.toml
--rw-r--r--   0        0        0      154 2023-04-29 20:23:22.159496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-extend-dotted-object-3.toml
--rw-r--r--   0        0        0       95 2023-04-29 20:23:22.160492 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-1.toml
--rw-r--r--   0        0        0       38 2023-04-29 20:23:22.161496 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-2.toml
--rw-r--r--   0        0        0        9 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-3.toml
--rw-r--r--   0        0        0       38 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-4.toml
--rw-r--r--   0        0        0       38 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-5.toml
--rw-r--r--   0        0        0       44 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-6.toml
--rw-r--r--   0        0        0      125 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-7.toml
--rw-r--r--   0        0        0      122 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-8.toml
--rw-r--r--   0        0        0       51 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-inline-1.toml
--rw-r--r--   0        0        0       26 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-inline-2.toml
--rw-r--r--   0        0        0       33 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table-inline-3.toml
--rw-r--r--   0        0        0        9 2023-04-29 20:23:22.161673 toml_tools-1.0.0/tests/data/toml-lang-compliance/valid/table/spec-table.toml
--rw-r--r--   0        0        0     1100 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/COPYING
--rw-r--r--   0        0        0     1016 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/array.json
--rw-r--r--   0        0        0      217 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/array.toml
--rw-r--r--   0        0        0      143 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/bool.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.324340 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/bool.toml
--rw-r--r--   0        0        0       95 2023-04-29 19:23:43.330889 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/empty.json
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.330889 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/empty.toml
--rw-r--r--   0        0        0      478 2023-04-29 19:23:43.330889 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/hetergeneous.json
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/hetergeneous.toml
--rw-r--r--   0        0        0      200 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-array.json
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-array.toml
--rw-r--r--   0        0        0      156 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-float.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-float.toml
--rw-r--r--   0        0        0      158 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-string.json
--rw-r--r--   0        0        0       31 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-int-string.toml
--rw-r--r--   0        0        0      415 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-string-table.json
--rw-r--r--   0        0        0      143 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/mixed-string-table.toml
--rw-r--r--   0        0        0      410 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested-double.json
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested-double.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested-inline-table.json
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested-inline-table.toml
--rw-r--r--   0        0        0      187 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested.json
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.332933 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nested.toml
--rw-r--r--   0        0        0      206 2023-04-29 19:23:43.341002 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nospaces.json
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.341002 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/nospaces.toml
--rw-r--r--   0        0        0       88 2023-04-29 19:23:43.341002 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-quote-comma-2.json
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.341002 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-quote-comma-2.toml
--rw-r--r--   0        0        0      179 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-quote-comma.json
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-quote-comma.toml
--rw-r--r--   0        0        0      175 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-with-comma.json
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/string-with-comma.toml
--rw-r--r--   0        0        0      293 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/strings.json
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/strings.toml
--rw-r--r--   0        0        0      121 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/table-array-string-backslash.json
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/array/table-array-string-backslash.toml
--rw-r--r--   0        0        0      122 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/bool/bool.json
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/bool/bool.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/at-eof.json
--rw-r--r--   0        0        0       87 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/at-eof.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/at-eof2.json
--rw-r--r--   0        0        0       87 2023-04-29 19:23:43.343049 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/at-eof2.toml
--rw-r--r--   0        0        0      428 2023-04-29 19:23:43.351091 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/everywhere.json
--rw-r--r--   0        0        0      610 2023-04-29 19:23:43.351091 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/everywhere.toml
--rw-r--r--   0        0        0        4 2023-04-29 19:23:43.351091 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/noeol.json
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.351091 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/noeol.toml
--rw-r--r--   0        0        0     1627 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/tricky.json
--rw-r--r--   0        0        0      416 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/comment/tricky.toml
--rw-r--r--   0        0        0      169 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/datetime.json
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/datetime.toml
--rw-r--r--   0        0        0       85 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local-date.json
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local-date.toml
--rw-r--r--   0        0        0      167 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local-time.json
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local-time.toml
--rw-r--r--   0        0        0      270 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local.json
--rw-r--r--   0        0        0       91 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/local.toml
--rw-r--r--   0        0        0      361 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/milliseconds.json
--rw-r--r--   0        0        0      144 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/milliseconds.toml
--rw-r--r--   0        0        0      342 2023-04-29 19:23:43.353135 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/timezone.json
--rw-r--r--   0        0        0      138 2023-04-29 19:23:43.361210 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/datetime/timezone.toml
--rw-r--r--   0        0        0        4 2023-04-29 19:23:43.361210 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/empty-file.json
--rw-r--r--   0        0        0        0 2023-04-29 19:23:43.361210 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/empty-file.toml
--rw-r--r--   0        0        0      428 2023-04-29 19:23:43.361210 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/example.json
--rw-r--r--   0        0        0       96 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/example.toml
--rw-r--r--   0        0        0      523 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/exponent.json
--rw-r--r--   0        0        0      122 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/exponent.toml
--rw-r--r--   0        0        0      263 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/float.json
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/float.toml
--rw-r--r--   0        0        0      400 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/inf-and-nan.json
--rw-r--r--   0        0        0      240 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/inf-and-nan.toml
--rw-r--r--   0        0        0      163 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/long.json
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/long.toml
--rw-r--r--   0        0        0      210 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/underscore.json
--rw-r--r--   0        0        0       59 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/underscore.toml
--rw-r--r--   0        0        0      474 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/zero.json
--rw-r--r--   0        0        0      145 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/float/zero.toml
--rw-r--r--   0        0        0      222 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-and-explicit-after.json
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.363259 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-and-explicit-after.toml
--rw-r--r--   0        0        0      222 2023-04-29 19:23:43.371321 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-and-explicit-before.json
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.371321 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-and-explicit-before.toml
--rw-r--r--   0        0        0      150 2023-04-29 19:23:43.371321 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-groups.json
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.371321 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/implicit-groups.toml
--rw-r--r--   0        0        0      585 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/array.json
--rw-r--r--   0        0        0      173 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/array.toml
--rw-r--r--   0        0        0      153 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/bool.json
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/bool.toml
--rw-r--r--   0        0        0      401 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/empty.json
--rw-r--r--   0        0        0      163 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/empty.toml
--rw-r--r--   0        0        0      267 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/end-in-bool.json
--rw-r--r--   0        0        0       71 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/end-in-bool.toml
--rw-r--r--   0        0        0      700 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/inline-table.json
--rw-r--r--   0        0        0      162 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/inline-table.toml
--rw-r--r--   0        0        0     2211 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/key-dotted.json
--rw-r--r--   0        0        0      331 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/key-dotted.toml
--rw-r--r--   0        0        0      324 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/multiline.json
--rw-r--r--   0        0        0       92 2023-04-29 19:23:43.373365 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/multiline.toml
--rw-r--r--   0        0        0      919 2023-04-29 19:23:43.381435 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/nest.json
--rw-r--r--   0        0        0      382 2023-04-29 19:23:43.381435 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/inline-table/nest.toml
--rw-r--r--   0        0        0      265 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/integer.json
--rw-r--r--   0        0        0       57 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/integer.toml
--rw-r--r--   0        0        0      595 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/literals.json
--rw-r--r--   0        0        0      162 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/literals.toml
--rw-r--r--   0        0        0      178 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/long.json
--rw-r--r--   0        0        0       71 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/long.toml
--rw-r--r--   0        0        0      130 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/underscore.json
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/underscore.toml
--rw-r--r--   0        0        0      713 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/zero.json
--rw-r--r--   0        0        0      137 2023-04-29 19:23:43.383477 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/integer/zero.toml
--rw-r--r--   0        0        0      710 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/alphanum.json
--rw-r--r--   0        0        0      187 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/alphanum.toml
--rw-r--r--   0        0        0      671 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/case-sensitive.json
--rw-r--r--   0        0        0      216 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/case-sensitive.toml
--rw-r--r--   0        0        0     2149 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/dotted.json
--rw-r--r--   0        0        0      570 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/dotted.toml
--rw-r--r--   0        0        0       65 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/empty.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/empty.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/equals-nospace.json
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/equals-nospace.toml
--rw-r--r--   0        0        0      383 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/escapes.json
--rw-r--r--   0        0        0      159 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/escapes.toml
--rw-r--r--   0        0        0       86 2023-04-29 19:23:43.391531 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/numeric-dotted.json
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.401587 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/numeric-dotted.toml
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.401587 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/numeric.json
--rw-r--r--   0        0        0        7 2023-04-29 19:23:43.401587 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/numeric.toml
--rw-r--r--   0        0        0      508 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/quoted-dots.json
--rw-r--r--   0        0        0      122 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/quoted-dots.toml
--rw-r--r--   0        0        0       65 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/space.json
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/space.toml
--rw-r--r--   0        0        0      112 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/special-chars.json
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/special-chars.toml
--rw-r--r--   0        0        0      279 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/special-word.json
--rw-r--r--   0        0        0       78 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/key/special-word.toml
--rw-r--r--   0        0        0      131 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/newline-crlf.json
--rw-r--r--   0        0        0       30 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/newline-crlf.toml
--rw-r--r--   0        0        0      130 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/newline-lf.json
--rw-r--r--   0        0        0       29 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/newline-lf.toml
--rw-r--r--   0        0        0     1711 2023-04-29 19:23:43.403632 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/spec-example-1-compact.json
--rw-r--r--   0        0        0      399 2023-04-29 19:23:43.411682 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/spec-example-1-compact.toml
--rw-r--r--   0        0        0     1711 2023-04-29 19:23:43.411682 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/spec-example-1.json
--rw-r--r--   0        0        0      592 2023-04-29 19:23:43.411682 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/spec-example-1.toml
--rw-r--r--   0        0        0       71 2023-04-29 19:23:43.411682 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/double-quote-escape.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/double-quote-escape.toml
--rw-r--r--   0        0        0       66 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/empty.json
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/empty.toml
--rw-r--r--   0        0        0      651 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escape-tricky.json
--rw-r--r--   0        0        0      343 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escape-tricky.toml
--rw-r--r--   0        0        0       71 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escaped-escape.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escaped-escape.toml
--rw-r--r--   0        0        0     1407 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escapes.json
--rw-r--r--   0        0        0      784 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/escapes.toml
--rw-r--r--   0        0        0      778 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/multiline-quotes.json
--rw-r--r--   0        0        0      463 2023-04-29 19:23:43.413719 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/multiline-quotes.toml
--rw-r--r--   0        0        0     1125 2023-04-29 19:23:43.421779 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/multiline.json
--rw-r--r--   0        0        0      979 2023-04-29 19:23:43.421779 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/multiline.toml
--rw-r--r--   0        0        0      359 2023-04-29 19:23:43.421779 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/nl.json
--rw-r--r--   0        0        0      121 2023-04-29 19:23:43.421779 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/nl.toml
--rw-r--r--   0        0        0      337 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/raw-multiline.json
--rw-r--r--   0        0        0      375 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/raw-multiline.toml
--rw-r--r--   0        0        0      729 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/raw.json
--rw-r--r--   0        0        0      380 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/raw.toml
--rw-r--r--   0        0        0      101 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/simple.json
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/simple.toml
--rw-r--r--   0        0        0      133 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/unicode-escape.json
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/unicode-escape.toml
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/unicode-literal.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/unicode-literal.toml
--rw-r--r--   0        0        0      193 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/with-pound.json
--rw-r--r--   0        0        0      115 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/string/with-pound.toml
--rw-r--r--   0        0        0      159 2023-04-29 19:23:43.423827 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-implicit.json
--rw-r--r--   0        0        0       39 2023-04-29 19:23:43.431876 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-implicit.toml
--rw-r--r--   0        0        0      585 2023-04-29 19:23:43.431876 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-many.json
--rw-r--r--   0        0        0      174 2023-04-29 19:23:43.431876 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-many.toml
--rw-r--r--   0        0        0      798 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-nest.json
--rw-r--r--   0        0        0      279 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-nest.toml
--rw-r--r--   0        0        0      216 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-one.json
--rw-r--r--   0        0        0       61 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-one.toml
--rw-r--r--   0        0        0      363 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-table-array.json
--rw-r--r--   0        0        0      115 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/array-table-array.toml
--rw-r--r--   0        0        0       17 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/empty.json
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/empty.toml
--rw-r--r--   0        0        0       64 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/keyword.json
--rw-r--r--   0        0        0       41 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/keyword.toml
--rw-r--r--   0        0        0      304 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/names.json
--rw-r--r--   0        0        0       99 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/names.toml
--rw-r--r--   0        0        0       21 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/no-eol.json
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.433920 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/no-eol.toml
--rw-r--r--   0        0        0       34 2023-04-29 19:23:43.441973 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/sub-empty.json
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.441973 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/sub-empty.toml
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.441973 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/whitespace.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/whitespace.toml
--rw-r--r--   0        0        0      154 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-literal-string.json
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-literal-string.toml
--rw-r--r--   0        0        0      100 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-pound.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-pound.toml
--rw-r--r--   0        0        0      150 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-single-quotes.json
--rw-r--r--   0        0        0       41 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/with-single-quotes.toml
--rw-r--r--   0        0        0       80 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/without-super.json
--rw-r--r--   0        0        0      125 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/burntsushi/valid/table/without-super.toml
--rw-r--r--   0        0        0     1183 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/LICENSE
--rw-r--r--   0        0        0      316 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/README.md
--rw-r--r--   0        0        0      156 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-1.json
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.444020 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-1.toml
--rw-r--r--   0        0        0      162 2023-04-29 19:23:43.452098 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-2.json
--rw-r--r--   0        0        0       39 2023-04-29 19:23:43.452098 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-2.toml
--rw-r--r--   0        0        0      317 2023-04-29 19:23:43.452098 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-3.json
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-3.toml
--rw-r--r--   0        0        0      215 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-4.json
--rw-r--r--   0        0        0       68 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-4.toml
--rw-r--r--   0        0        0      313 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-5.json
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-5.toml
--rw-r--r--   0        0        0      157 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-7.json
--rw-r--r--   0        0        0       29 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-7.toml
--rw-r--r--   0        0        0      120 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-8.json
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-8.toml
--rw-r--r--   0        0        0      266 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-mixed-number-types.json
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-mixed-number-types.toml
--rw-r--r--   0        0        0      315 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-more-mixed-types.json
--rw-r--r--   0        0        0      143 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-more-mixed-types.toml
--rw-r--r--   0        0        0      344 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-1.json
--rw-r--r--   0        0        0      128 2023-04-29 19:23:43.454142 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-1.toml
--rw-r--r--   0        0        0      618 2023-04-29 19:23:43.462202 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-2.json
--rw-r--r--   0        0        0      270 2023-04-29 19:23:43.462202 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-2.toml
--rw-r--r--   0        0        0      496 2023-04-29 19:23:43.462202 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-3.json
--rw-r--r--   0        0        0      112 2023-04-29 19:23:43.462202 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/array/spec-array-of-tables-3.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/boolean/spec-boolean-1.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/boolean/spec-boolean-1.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/boolean/spec-boolean-2.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/boolean/spec-boolean-2.toml
--rw-r--r--   0        0        0      118 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-mid-array.json
--rw-r--r--   0        0        0      126 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-mid-array.toml
--rw-r--r--   0        0        0       69 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-mid-string.json
--rw-r--r--   0        0        0       37 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-mid-string.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-tab.json
--rw-r--r--   0        0        0      136 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment-tab.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.464244 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment.json
--rw-r--r--   0        0        0       87 2023-04-29 19:23:43.472296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/comment/spec-comment.toml
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.472296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-local-1.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.472296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-local-1.toml
--rw-r--r--   0        0        0       72 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-1.json
--rw-r--r--   0        0        0       29 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-1.toml
--rw-r--r--   0        0        0       77 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-2.json
--rw-r--r--   0        0        0       34 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-2.toml
--rw-r--r--   0        0        0       84 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-3.json
--rw-r--r--   0        0        0       41 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-3.toml
--rw-r--r--   0        0        0       72 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-4.json
--rw-r--r--   0        0        0       29 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-4.toml
--rw-r--r--   0        0        0       76 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-5.json
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-5.toml
--rw-r--r--   0        0        0       77 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-6.json
--rw-r--r--   0        0        0       34 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-6.toml
--rw-r--r--   0        0        0       70 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-local-1.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.474339 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-local-1.toml
--rw-r--r--   0        0        0       77 2023-04-29 19:23:43.482389 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-local-2.json
--rw-r--r--   0        0        0       35 2023-04-29 19:23:43.482389 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-date-time-local-2.toml
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.482389 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-time-1.json
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.482389 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-time-1.toml
--rw-r--r--   0        0        0       61 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-time-2.json
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/date-time/spec-time-2.toml
--rw-r--r--   0        0        0       43 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-1.json
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-1.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-10.json
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-10.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-11.json
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-11.toml
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-12.json
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-12.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-13.json
--rw-r--r--   0        0        0       67 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-13.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-14.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.484438 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-14.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.492482 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-15.json
--rw-r--r--   0        0        0       64 2023-04-29 19:23:43.492482 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-15.toml
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.492482 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-2.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.492482 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-2.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-3.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-3.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-4.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-4.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-5.json
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-5.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-6.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-6.toml
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-7.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-7.toml
--rw-r--r--   0        0        0       58 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-8.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-8.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-9.json
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.494530 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/float/spec-float-9.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.502590 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-1.json
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.502590 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-1.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.502590 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-2.json
--rw-r--r--   0        0        0       11 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-2.toml
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3a.json
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3a.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3b.json
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-3b.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-4.json
--rw-r--r--   0        0        0       12 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-4.toml
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-5.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-5.toml
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-6.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-6.toml
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.504640 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-7.json
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.512683 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-7.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.512683 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-bin1.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.512683 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-bin1.toml
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.512683 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex1.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex1.toml
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex2.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex2.toml
--rw-r--r--   0        0        0       54 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex3.json
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-hex3.toml
--rw-r--r--   0        0        0       62 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-max.json
--rw-r--r--   0        0        0       31 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-max.toml
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-min.json
--rw-r--r--   0        0        0       32 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-min.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-oct1.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-oct1.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-oct2.json
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/integer/spec-int-oct2.toml
--rw-r--r--   0        0        0       92 2023-04-29 19:23:43.514725 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-case-sensitive.json
--rw-r--r--   0        0        0       49 2023-04-29 19:23:43.522779 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-case-sensitive.toml
--rw-r--r--   0        0        0      240 2023-04-29 19:23:43.522779 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-1.json
--rw-r--r--   0        0        0       96 2023-04-29 19:23:43.522779 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-1.toml
--rw-r--r--   0        0        0       55 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-2.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-2.toml
--rw-r--r--   0        0        0       55 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-3.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-dotted-keys-3.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-empty-key-name-1.json
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-empty-key-name-1.toml
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-empty-key-name-2.json
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-empty-key-name-2.toml
--rw-r--r--   0        0        0       47 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-1.json
--rw-r--r--   0        0        0       15 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-1.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-2.json
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-2.toml
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-3.json
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-3.toml
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.524818 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-4.json
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.532864 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-4.toml
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.532864 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-5.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.532864 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-5.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.532864 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-6.json
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-6.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-7.json
--rw-r--r--   0        0        0        5 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-7.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-8.json
--rw-r--r--   0        0        0       13 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-8.toml
--rw-r--r--   0        0        0       58 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-9.json
--rw-r--r--   0        0        0       16 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-key-value-pair-9.toml
--rw-r--r--   0        0        0       92 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-1.json
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-1.toml
--rw-r--r--   0        0        0       92 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-2.json
--rw-r--r--   0        0        0       22 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-2.toml
--rw-r--r--   0        0        0      138 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-3.json
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.534903 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-newline-3.toml
--rw-r--r--   0        0        0       50 2023-04-29 19:23:43.542971 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-quoted-basic-keys-1.json
--rw-r--r--   0        0        0       20 2023-04-29 19:23:43.542971 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-quoted-basic-keys-1.toml
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.542971 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-quoted-literal-keys-1.json
--rw-r--r--   0        0        0       28 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/key-value/spec-quoted-literal-keys-1.toml
--rw-r--r--   0        0        0    42078 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-array-inline-1000.json
--rw-r--r--   0        0        0    14021 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-array-inline-1000.toml
--rw-r--r--   0        0        0     2011 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-array-inline-nested-1000.toml
--rw-r--r--   0        0        0    40046 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-key-literal-40kb.json
--rw-r--r--   0        0        0    40016 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-key-literal-40kb.toml
--rw-r--r--   0        0        0    40046 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-key-string-40kb.json
--rw-r--r--   0        0        0    40016 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-key-string-40kb.toml
--rw-r--r--   0        0        0    40046 2023-04-29 19:23:43.545017 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-literal-40kb.json
--rw-r--r--   0        0        0    40014 2023-04-29 19:23:43.553070 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-literal-40kb.toml
--rw-r--r--   0        0        0    40144 2023-04-29 19:23:43.553070 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-literal-multiline-40kb.json
--rw-r--r--   0        0        0    40116 2023-04-29 19:23:43.553070 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-literal-multiline-40kb.toml
--rw-r--r--   0        0        0    40046 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-string-40kb.json
--rw-r--r--   0        0        0    40014 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-string-40kb.toml
--rw-r--r--   0        0        0    40144 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-string-multiline-40kb.json
--rw-r--r--   0        0        0    40116 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-scalar-string-multiline-40kb.toml
--rw-r--r--   0        0        0    45948 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-table-inline-1000.json
--rw-r--r--   0        0        0    19914 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-table-inline-1000.toml
--rw-r--r--   0        0        0     8011 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/qa/qa-table-inline-nested-1000.toml
--rw-r--r--   0        0        0     1310 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/spec-readme-example.json
--rw-r--r--   0        0        0      578 2023-04-29 19:23:43.555117 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/spec-readme-example.toml
--rw-r--r--   0        0        0       74 2023-04-29 19:23:43.563159 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-1.json
--rw-r--r--   0        0        0       48 2023-04-29 19:23:43.563159 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-1.toml
--rw-r--r--   0        0        0       86 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-2.json
--rw-r--r--   0        0        0       76 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-2.toml
--rw-r--r--   0        0        0       86 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-3.json
--rw-r--r--   0        0        0       94 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-3.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-4.json
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-4.toml
--rw-r--r--   0        0        0       78 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-5.json
--rw-r--r--   0        0        0       62 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-5.toml
--rw-r--r--   0        0        0       93 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-6.json
--rw-r--r--   0        0        0       63 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-6.toml
--rw-r--r--   0        0        0       82 2023-04-29 19:23:43.565204 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-7.json
--rw-r--r--   0        0        0       52 2023-04-29 19:23:43.573256 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-7.toml
--rw-r--r--   0        0        0      108 2023-04-29 19:23:43.573256 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-8.json
--rw-r--r--   0        0        0       70 2023-04-29 19:23:43.573256 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-8.toml
--rw-r--r--   0        0        0       97 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-9.json
--rw-r--r--   0        0        0       65 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-multiline-9.toml
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-tab-multiline.json
--rw-r--r--   0        0        0       27 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-tab-multiline.toml
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-tab.json
--rw-r--r--   0        0        0       23 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic-tab.toml
--rw-r--r--   0        0        0      108 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic.json
--rw-r--r--   0        0        0       76 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-basic.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-1.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.575296 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-1.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.583356 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-2.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.583356 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-2.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-3.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-3.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-4.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-4.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-5.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-5.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-6.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-6.toml
--rw-r--r--   0        0        0       42 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-7.json
--rw-r--r--   0        0        0       10 2023-04-29 19:23:43.585390 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-7.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-8.json
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-8.toml
--rw-r--r--   0        0        0       46 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-9.json
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-escape-9.toml
--rw-r--r--   0        0        0       74 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-1.json
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-1.toml
--rw-r--r--   0        0        0       78 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-2.json
--rw-r--r--   0        0        0       41 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-2.toml
--rw-r--r--   0        0        0       72 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-3.json
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-3.toml
--rw-r--r--   0        0        0       57 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-4.json
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-4.toml
--rw-r--r--   0        0        0       74 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-1.json
--rw-r--r--   0        0        0       45 2023-04-29 19:23:43.593430 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-1.toml
--rw-r--r--   0        0        0      134 2023-04-29 19:23:43.603493 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-2.json
--rw-r--r--   0        0        0      109 2023-04-29 19:23:43.603493 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-2.toml
--rw-r--r--   0        0        0      109 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-3.json
--rw-r--r--   0        0        0       66 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-3.toml
--rw-r--r--   0        0        0       81 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-4.json
--rw-r--r--   0        0        0       53 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/string/spec-string-literal-multiline-4.toml
--rw-r--r--   0        0        0      135 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-1.json
--rw-r--r--   0        0        0      144 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-1.toml
--rw-r--r--   0        0        0      337 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-2.json
--rw-r--r--   0        0        0      166 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-2.toml
--rw-r--r--   0        0        0      337 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-3.json
--rw-r--r--   0        0        0      154 2023-04-29 19:23:43.605537 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-extend-dotted-object-3.toml
--rw-r--r--   0        0        0      249 2023-04-29 19:23:43.613583 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-1.json
--rw-r--r--   0        0        0       95 2023-04-29 19:23:43.613583 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-1.toml
--rw-r--r--   0        0        0      101 2023-04-29 19:23:43.613583 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-2.json
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-2.toml
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-3.json
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-3.toml
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-4.json
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-4.toml
--rw-r--r--   0        0        0       40 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-5.json
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-5.toml
--rw-r--r--   0        0        0       41 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-6.json
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-6.toml
--rw-r--r--   0        0        0       56 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-7.json
--rw-r--r--   0        0        0      125 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-7.toml
--rw-r--r--   0        0        0      238 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-8.json
--rw-r--r--   0        0        0      122 2023-04-29 19:23:43.615630 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-8.toml
--rw-r--r--   0        0        0      123 2023-04-29 19:23:43.623707 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-1.json
--rw-r--r--   0        0        0       51 2023-04-29 19:23:43.623707 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-1.toml
--rw-r--r--   0        0        0      104 2023-04-29 19:23:43.623707 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-2.json
--rw-r--r--   0        0        0       26 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-2.toml
--rw-r--r--   0        0        0       80 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-3.json
--rw-r--r--   0        0        0       33 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table-inline-3.toml
--rw-r--r--   0        0        0       18 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table.json
--rw-r--r--   0        0        0        9 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/_external/toml-lang-compliance/valid/table/spec-table.toml
--rw-r--r--   0        0        0      101 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/apostrophes-in-literal-string.json
--rw-r--r--   0        0        0       71 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/apostrophes-in-literal-string.toml
--rw-r--r--   0        0        0      205 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/array/array-subtables.json
--rw-r--r--   0        0        0       62 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/array/array-subtables.toml
--rw-r--r--   0        0        0      125 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/array/open-parent-table.json
--rw-r--r--   0        0        0       73 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/array/open-parent-table.toml
--rw-r--r--   0        0        0       86 2023-04-29 19:23:43.625749 toml_tools-1.0.0/tests/data/valid/boolean.json
--rw-r--r--   0        0        0       19 2023-04-29 19:23:43.633796 toml_tools-1.0.0/tests/data/valid/boolean.toml
--rw-r--r--   0        0        0      143 2023-04-29 19:23:43.633796 toml_tools-1.0.0/tests/data/valid/dates-and-times/datetimes.json
--rw-r--r--   0        0        0       60 2023-04-29 19:23:43.635806 toml_tools-1.0.0/tests/data/valid/dates-and-times/datetimes.toml
--rw-r--r--   0        0        0       59 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/dates-and-times/localtime.json
--rw-r--r--   0        0        0       25 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/dates-and-times/localtime.toml
--rw-r--r--   0        0        0       14 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/empty-inline-table.json
--rw-r--r--   0        0        0       36 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/empty-inline-table.toml
--rw-r--r--   0        0        0      159 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/five-quotes.json
--rw-r--r--   0        0        0      103 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/five-quotes.toml
--rw-r--r--   0        0        0      122 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/hex-char.json
--rw-r--r--   0        0        0       38 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/hex-char.toml
--rw-r--r--   0        0        0       55 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/multiline-basic-str/ends-in-whitespace-escape.json
--rw-r--r--   0        0        0       44 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/multiline-basic-str/ends-in-whitespace-escape.toml
--rw-r--r--   0        0        0        4 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/no-newlines.json
--rw-r--r--   0        0        0       24 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/no-newlines.toml
--rw-r--r--   0        0        0       97 2023-04-29 19:23:43.635836 toml_tools-1.0.0/tests/data/valid/trailing-comma.json
--rw-r--r--   0        0        0        8 2023-04-29 19:23:43.643895 toml_tools-1.0.0/tests/data/valid/trailing-comma.toml
--rw-r--r--   0        0        0       58 2023-04-29 20:33:59.186339 toml_tools-1.0.0/tests/requirements.txt
--rw-r--r--   0        0        0     2321 2023-04-29 20:46:21.775322 toml_tools-1.0.0/tests/test_data.py
--rw-r--r--   0        0        0     2204 2023-04-29 20:46:25.387446 toml_tools-1.0.0/tests/test_error.py
--rw-r--r--   0        0        0      873 2023-04-29 20:46:31.020119 toml_tools-1.0.0/tests/test_for_profiler.py
--rw-r--r--   0        0        0      405 2023-04-29 20:46:35.408766 toml_tools-1.0.0/tests/test_invalid.py
--rw-r--r--   0        0        0     3381 2023-04-29 20:46:39.792588 toml_tools-1.0.0/tests/test_misc.py
--rw-r--r--   0        0        0     5621 2023-04-29 20:46:51.625979 toml_tools-1.0.0/tests/test_style.py
--rw-r--r--   0        0        0      750 2023-04-29 20:46:57.524011 toml_tools-1.0.0/tests/test_types.py
--rw-r--r--   0        0        0     1863 2023-04-29 20:47:06.364333 toml_tools-1.0.0/tests/test_valid.py
--rw-r--r--   0        0        0      294 2023-04-29 20:47:14.411870 toml_tools-1.0.0/tests/test_write_file.py
--rw-r--r--   0        0        0    14086 1970-01-01 00:00:00.000000 toml_tools-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.692536 toml_tools-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-04-29 19:23:43.000000 toml_tools-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-04-30 11:09:23.000000 toml_tools-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14622 2023-04-30 21:22:52.693535 toml_tools-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13663 2023-04-29 22:35:27.000000 toml_tools-1.1.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-30 21:22:52.696540 toml_tools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-04-30 21:22:49.000000 toml_tools-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.647349 toml_tools-1.1.0/tests/
+-rw-rw-rw-   0        0        0      425 2023-04-30 13:19:52.000000 toml_tools-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4292 2023-04-30 21:03:53.000000 toml_tools-1.1.0/tests/burntsushi.py
+-rw-rw-rw-   0        0        0     2750 2023-04-30 14:27:16.000000 toml_tools-1.1.0/tests/test_data.py
+-rw-rw-rw-   0        0        0     2290 2023-04-30 13:05:45.000000 toml_tools-1.1.0/tests/test_error.py
+-rw-rw-rw-   0        0        0      910 2023-04-30 13:43:35.000000 toml_tools-1.1.0/tests/test_for_profiler.py
+-rw-rw-rw-   0        0        0      439 2023-04-30 13:09:48.000000 toml_tools-1.1.0/tests/test_invalid.py
+-rw-rw-rw-   0        0        0     3971 2023-04-30 15:41:55.000000 toml_tools-1.1.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5612 2023-04-30 13:11:25.000000 toml_tools-1.1.0/tests/test_style.py
+-rw-rw-rw-   0        0        0      757 2023-04-30 09:56:38.000000 toml_tools-1.1.0/tests/test_types.py
+-rw-rw-rw-   0        0        0     2075 2023-04-30 21:09:47.000000 toml_tools-1.1.0/tests/test_valid.py
+-rw-rw-rw-   0        0        0      301 2023-04-30 09:56:56.000000 toml_tools-1.1.0/tests/test_write_file.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.659540 toml_tools-1.1.0/toml_tools/
+-rw-rw-rw-   0        0        0      421 2023-04-30 21:19:11.000000 toml_tools-1.1.0/toml_tools/__init__.py
+-rw-rw-rw-   0        0        0      444 2023-04-29 21:12:30.000000 toml_tools-1.1.0/toml_tools/_helpers.py
+-rw-rw-rw-   0        0        0    23870 2023-04-30 15:19:52.000000 toml_tools-1.1.0/toml_tools/_parser.py
+-rw-rw-rw-   0        0        0     4285 2023-04-30 14:29:54.000000 toml_tools-1.1.0/toml_tools/_re.py
+-rw-rw-rw-   0        0        0     6509 2023-04-30 11:54:56.000000 toml_tools-1.1.0/toml_tools/_writer.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.690541 toml_tools-1.1.0/toml_tools.egg-info/
+-rw-rw-rw-   0        0        0    14622 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1271 2023-04-30 21:11:20.000000 toml_tools-1.1.0/tox.ini
```

### Comparing `toml_tools-1.0.0/LICENSE` & `toml_tools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_tools-1.0.0/README.md` & `toml_tools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `toml_tools-1.0.0/src/toml_tools/_parser.py` & `toml_tools-1.1.0/toml_tools/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
+import sys
 from collections import namedtuple
 import string
+import struct
 
 from ._re import (
     RE_DATETIME,
     RE_LOCALTIME,
     RE_NUMBER,
     match_to_datetime,
     match_to_localtime,
     match_to_number,
 )
 
 from ._helpers import ReadOnlyDict
 
+if sys.version_info < (3,):
+    def unichar(i):
+        """https://stackoverflow.com/a/28326717/20785734
+        """
+        try:
+            return unichr(i)
+        except ValueError:
+            return struct.pack('i', i).decode('utf-32')
+        
+    chr = unichar
+
 ASCII_CTRL = frozenset(chr(i) for i in range(32)) | frozenset(chr(127))
 
 # Neither of these sets include quotation mark or backslash. They are
 # currently handled as separate cases in the parser functions.
 ILLEGAL_BASIC_STR_CHARS = ASCII_CTRL - frozenset("\t")
 ILLEGAL_MULTILINE_BASIC_STR_CHARS = ASCII_CTRL - frozenset("\t\n")
 
@@ -55,17 +68,17 @@
 def load(__fp, parse_float = float):
     #type(IO[bytes], Callable[[str], type(any)])) -> dict[str, Any]
     """Parse TOML from a binary file object."""
     b = __fp.read()
     try:
         s = b.decode()
     except AttributeError:
-        raise TypeError(
-            "File must be opened in binary mode, e.g. use `open('foo.toml', 'rb')`"
-        ) from None
+        raise TypeError("File must be opened in binary mode"
+                        ", e.g. use `open('foo.toml', 'rb')`"
+                       )
     return loads(s, parse_float=parse_float)
 
 
 def loads(__s, parse_float = float):
     #type(str, Callable[[str], type(any)])) -> dict[str, Any]
     """Parse TOML from a string."""
 
@@ -99,15 +112,15 @@
             pos += 1
             continue
         if char in KEY_INITIAL_CHARS:
             pos = key_value_rule(src, pos, out, header, parse_float)
             pos = skip_chars(src, pos, TOML_WS)
         elif char == "[":
             try:
-                second_char: str | None = src[pos + 1]
+                second_char = src[pos + 1]
             except IndexError:
                 second_char = None
             out.flags.finalize_pending()
             if second_char == "[":
                 pos, header = create_list_rule(src, pos, out)
             else:
                 pos, header = create_dict_rule(src, pos, out)
@@ -137,28 +150,29 @@
 
     # Marks an immutable namespace (inline array or inline table).
     FROZEN = 0
     # Marks a nest that has been explicitly created and can no longer
     # be opened using the "[table]" syntax.
     EXPLICIT_NEST = 1
 
-    def __init__(self) -> None:
+    def __init__(self):
         self._flags = {} # : dict[str, dict]
         self._pending_flags = set() # set[tuple[Key, int]]
 
-    def add_pending(self, key, flag) -> None:
+    def add_pending(self, key, flag):
         #type(Tuple[str, ...], Pos) -> None
         self._pending_flags.add((key, flag))
 
-    def finalize_pending(self) -> None:
+    def finalize_pending(self):
+        #type() -> None
         for key, flag in self._pending_flags:
             self.set(key, flag, recursive=False)
         self._pending_flags.clear()
 
-    def unset_all(self, key) -> None:
+    def unset_all(self, key):
         # type(Tuple[str, ...]) -> None
         cont = self._flags
         for k in key[:-1]:
             if k not in cont:
                 return
             cont = cont[k]["nested"]
         cont.pop(key[-1], None)
@@ -241,27 +255,27 @@
 def skip_until(src, pos, expect, error_on, error_on_eof):
     #type(str, int, str, frozenset[str], bool) -> int
     try:
         new_pos = src.index(expect, pos)
     except ValueError:
         new_pos = len(src)
         if error_on_eof:
-            raise suffixed_err(src, new_pos, f"Expected {expect!r}") from None
+            raise suffixed_err(src, new_pos, "Expected %s" % (expect,))
 
     if not error_on.isdisjoint(src[pos:new_pos]):
         while src[pos] not in error_on:
             pos += 1
-        raise suffixed_err(src, pos, f"Found invalid character {src[pos]!r}")
+        raise suffixed_err(src, pos, "Found invalid character %s" % repr(src[pos]))
     return new_pos
 
 
 def skip_comment(src, pos):
     #type(str, int) -> int
     try:
-        char: str | None = src[pos]
+        char = src[pos]
     except IndexError:
         char = None
     if char == "#":
         return skip_until(
             src, pos + 1, "\n", error_on=ILLEGAL_COMMENT_CHARS, error_on_eof=False
         )
     return pos
@@ -273,93 +287,93 @@
         pos_before_skip = pos
         pos = skip_chars(src, pos, TOML_WS_AND_NEWLINE)
         pos = skip_comment(src, pos)
         if pos == pos_before_skip:
             return pos
 
 
-def create_dict_rule(src: str, pos: int, out: Output):
+def create_dict_rule(src, pos, out):
     #type(str, int, Output) -> tuple[Pos, Key]:
     pos += 1  # Skip "["
     pos = skip_chars(src, pos, TOML_WS)
     pos, key = parse_key(src, pos)
 
     if out.flags.is_(key, Flags.EXPLICIT_NEST) or out.flags.is_(key, Flags.FROZEN):
-        raise suffixed_err(src, pos, f"Cannot declare {key} twice")
+        raise suffixed_err(src, pos, "Cannot declare %s twice" % (key,))
     out.flags.set(key, Flags.EXPLICIT_NEST, recursive=False)
     try:
         out.data.get_or_create_nest(key)
     except KeyError:
-        raise suffixed_err(src, pos, "Cannot overwrite a value") from None
+        raise suffixed_err(src, pos, "Cannot overwrite a value") 
 
     if not src.startswith("]", pos):
         raise suffixed_err(src, pos, "Expected ']' at the end of a table declaration")
     return pos + 1, key
 
 
-def create_list_rule(src: str, pos: int, out: Output):
+def create_list_rule(src, pos, out):
     #type(str, int, Output) -> tuple[Pos, Key]:
     pos += 2  # Skip "[["
     pos = skip_chars(src, pos, TOML_WS)
     pos, key = parse_key(src, pos)
 
     if out.flags.is_(key, Flags.FROZEN):
-        raise suffixed_err(src, pos, f"Cannot mutate immutable namespace {key}")
+        raise suffixed_err(src, pos, "Cannot mutate immutable namespace %s" % (key,))
     # Free the namespace now that it points to another empty list item...
     out.flags.unset_all(key)
     # ...but this key precisely is still prohibited from table declaration
     out.flags.set(key, Flags.EXPLICIT_NEST, recursive=False)
     try:
         out.data.append_nest_to_list(key)
     except KeyError:
-        raise suffixed_err(src, pos, "Cannot overwrite a value") from None
+        raise suffixed_err(src, pos, "Cannot overwrite a value")
 
     if not src.startswith("]]", pos):
         raise suffixed_err(src, pos, "Expected ']]' at the end of an array declaration")
     return pos + 2, key
 
 
-def key_value_rule(src: str, pos, out, header, parse_float):
+def key_value_rule(src, pos, out, header, parse_float):
     #type(str, int, Output, Key, Callable[[str], type(any)])) -> Pos
     pos, key, value = parse_key_value_pair(src, pos, parse_float)
     key_parent, key_stem = key[:-1], key[-1]
     abs_key_parent = header + key_parent
 
     relative_path_cont_keys = (header + key[:i] for i in range(1, len(key)))
     for cont_key in relative_path_cont_keys:
         # Check that dotted key syntax does not redefine an existing table
         if out.flags.is_(cont_key, Flags.EXPLICIT_NEST):
-            raise suffixed_err(src, pos, f"Cannot redefine namespace {cont_key}")
+            raise suffixed_err(src, pos, "Cannot redefine namespace %s" % (cont_key,))
         # Containers in the relative path can't be opened with the table syntax or
         # dotted key/value syntax in following table sections.
         out.flags.add_pending(cont_key, Flags.EXPLICIT_NEST)
 
     if out.flags.is_(abs_key_parent, Flags.FROZEN):
         raise suffixed_err(
-            src, pos, f"Cannot mutate immutable namespace {abs_key_parent}"
+            src, pos, "Cannot mutate immutable namespace %s" % (abs_key_parent,)
         )
 
     try:
         nest = out.data.get_or_create_nest(abs_key_parent)
     except KeyError:
-        raise suffixed_err(src, pos, "Cannot overwrite a value") from None
+        raise suffixed_err(src, pos, "Cannot overwrite a value")
     if key_stem in nest:
         raise suffixed_err(src, pos, "Cannot overwrite a value")
     # Mark inline table and array namespaces recursively immutable
     if isinstance(value, (dict, list)):
         out.flags.set(header + key, Flags.FROZEN, recursive=True)
     nest[key_stem] = value
     return pos
 
 
 def parse_key_value_pair(src, pos, parse_float):
     #type(str, int, Callable[[str], type(any)])) -> tuple[Pos, Key, Any]:
     pos, key = parse_key(src, pos)
     try:
-        char: str | None = src[pos]
+        char = src[pos]
     except IndexError:
         char = None
     if char != "=":
         raise suffixed_err(src, pos, "Expected '=' after a key in a key/value pair")
     pos += 1
     pos = skip_chars(src, pos, TOML_WS)
     pos, value = parse_value(src, pos, parse_float)
@@ -369,30 +383,30 @@
 def parse_key(src, pos):
     #type(str, int) -> tuple[int, Tuple[str, ...]]
     pos, key_part = parse_key_part(src, pos)
     key = (key_part,)
     pos = skip_chars(src, pos, TOML_WS)
     while True:
         try:
-            char: str | None = src[pos]
+            char = src[pos]
         except IndexError:
             char = None
         if char != ".":
             return pos, key
         pos += 1
         pos = skip_chars(src, pos, TOML_WS)
         pos, key_part = parse_key_part(src, pos)
         key += (key_part,)
         pos = skip_chars(src, pos, TOML_WS)
 
 
 def parse_key_part(src, pos):
     #type(str, int) -> tuple[int, str]
     try:
-        char: str | None = src[pos]
+        char = src[pos]
     except IndexError:
         char = None
     if char in BARE_KEY_CHARS:
         start_pos = pos
         pos = skip_chars(src, pos, BARE_KEY_CHARS)
         return pos, src[start_pos:pos]
     if char == "'":
@@ -407,15 +421,15 @@
     pos += 1
     return parse_basic_str(src, pos, multiline=False)
 
 
 def parse_array(src, pos, parse_float):
     #type(str, int, Callable[[str], type(any)])) -> tuple[Pos, list]:
     pos += 1
-    array: list = []
+    array = []
 
     pos = skip_comments_and_array_ws(src, pos)
     if src.startswith("]", pos):
         return pos + 1, array
     while True:
         pos, val = parse_value(src, pos, parse_float)
         array.append(val)
@@ -442,21 +456,21 @@
     pos = skip_chars(src, pos, TOML_WS)
     if src.startswith("}", pos):
         return pos + 1, nested_dict.dict
     while True:
         pos, key, value = parse_key_value_pair(src, pos, parse_float)
         key_parent, key_stem = key[:-1], key[-1]
         if flags.is_(key, Flags.FROZEN):
-            raise suffixed_err(src, pos, f"Cannot mutate immutable namespace {key}")
+            raise suffixed_err(src, pos, "Cannot mutate immutable namespace %s" % (key,))
         try:
             nest = nested_dict.get_or_create_nest(key_parent, access_lists=False)
         except KeyError:
-            raise suffixed_err(src, pos, "Cannot overwrite a value") from None
+            raise suffixed_err(src, pos, "Cannot overwrite a value")
         if key_stem in nest:
-            raise suffixed_err(src, pos, f"Duplicate inline table key {key_stem!r}")
+            raise suffixed_err(src, pos, "Duplicate inline table key  %s" % repr(key_stem))
         nest[key_stem] = value
         pos = skip_chars(src, pos, TOML_WS)
         c = src[pos : pos + 1]
         if c == "}":
             return pos + 1, nested_dict.dict
         if c != ",":
             raise suffixed_err(src, pos, "Unclosed inline table")
@@ -487,23 +501,23 @@
     if escape_id == "\\u":
         return parse_hex_char(src, pos, 4)
     if escape_id == "\\U":
         return parse_hex_char(src, pos, 8)
     try:
         return pos, BASIC_STR_ESCAPE_REPLACEMENTS[escape_id]
     except KeyError:
-        raise suffixed_err(src, pos, "Unescaped '\\' in a string") from None
+        raise suffixed_err(src, pos, "Unescaped '\\' in a string")
 
 
 def parse_basic_str_escape_multiline(src, pos):
     #type(str, int) -> tuple[int, str]:
     return parse_basic_str_escape(src, pos, multiline=True)
 
 
-def parse_hex_char(src: str, pos: int, hex_len: int):
+def parse_hex_char(src, pos, hex_len):
     #type(str, int, int) -> tuple[int, str]:
     hex_str = src[pos : pos + hex_len]
     if len(hex_str) != hex_len or not HEXDIGIT_CHARS.issuperset(hex_str):
         raise suffixed_err(src, pos, "Invalid hex value")
     pos += hex_len
     hex_int = int(hex_str, 16)
     if not is_unicode_scalar_value(hex_int):
@@ -563,37 +577,37 @@
         parse_escapes = parse_basic_str_escape
     result = ""
     start_pos = pos
     while True:
         try:
             char = src[pos]
         except IndexError:
-            raise suffixed_err(src, pos, "Unterminated string") from None
+            raise suffixed_err(src, pos, "Unterminated string")
         if char == '"':
             if not multiline:
                 return pos + 1, result + src[start_pos:pos]
             if src.startswith('"""', pos):
                 return pos + 3, result + src[start_pos:pos]
             pos += 1
             continue
         if char == "\\":
             result += src[start_pos:pos]
             pos, parsed_escape = parse_escapes(src, pos)
             result += parsed_escape
             start_pos = pos
             continue
         if char in error_on:
-            raise suffixed_err(src, pos, f"Illegal character {char!r}")
+            raise suffixed_err(src, pos, "Illegal character %s" % repr(char))
         pos += 1
 
 
 def parse_value(src, pos, parse_float):
     #type(str, int, Callable[[str], type(any)]) -> tuple[Pos, Any]:
     try:
-        char: str | None = src[pos]
+        char = src[pos]
     except IndexError:
         char = None
 
     # IMPORTANT: order conditions based on speed of checking and likelihood
 
     # Basic strings
     if char == '"':
@@ -625,15 +639,15 @@
 
     # Dates and times
     datetime_match = RE_DATETIME.match(src, pos)
     if datetime_match:
         try:
             datetime_obj = match_to_datetime(datetime_match)
         except ValueError as e:
-            raise suffixed_err(src, pos, "Invalid date or datetime") from e
+            raise suffixed_err(src, pos, "Invalid date or datetime")
         return datetime_match.end(), datetime_obj
     localtime_match = RE_LOCALTIME.match(src, pos)
     if localtime_match:
         return localtime_match.end(), match_to_localtime(localtime_match)
 
     # Integers and "normal" floats.
     # The regex will greedily match any type starting with a decimal
@@ -649,30 +663,31 @@
     first_four = src[pos : pos + 4]
     if first_four in {"-inf", "+inf", "-nan", "+nan"}:
         return pos + 4, parse_float(first_four)
 
     raise suffixed_err(src, pos, "Invalid value")
 
 
-def suffixed_err(src: str, pos: int, msg: str) -> TOMLDecodeError:
+def suffixed_err(src, pos, msg):
+    #type(str, int, str) -> TOMLDecodeError
     """Return a `TOMLDecodeError` where error message is suffixed with
     coordinates in source."""
 
-    def coord_repr(src, pos) -> str:
+    def coord_repr(src, pos):
         #type(str, int) -> str
         if pos >= len(src):
             return "end of document"
         line = src.count("\n", 0, pos) + 1
         if line == 1:
             column = pos + 1
         else:
             column = pos - src.rindex("\n", 0, pos)
-        return f"line {line}, column {column}"
+        return "line %s, column %s" % (line, column)
 
-    return TOMLDecodeError(f"{msg} (at {coord_repr(src, pos)})")
+    return TOMLDecodeError("%s (at %s)" % (msg, coord_repr(src, pos)))
 
 
 def is_unicode_scalar_value(codepoint):
     #type(int) -> bool
     return (0 <= codepoint <= 55295) or (57344 <= codepoint <= 1114111)
```

### Comparing `toml_tools-1.0.0/src/toml_tools/_writer.py` & `toml_tools-1.1.0/toml_tools/_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,89 +24,67 @@
                                 "\u000D": "\\r",  # carriage return
                                 "\u0022": '\\"',  # quote
                                 "\u005C": "\\\\",  # backslash
                                }
                               )
 
 
-def dump(
-    # __obj: dict[str, Any], __fp: BinaryIO, *, multiline_strings: bool = False
-    __obj, __fp, multiline_strings = False
-# ) -> None:
-):
+def dump(__obj, __fp, multiline_strings = False):
+    #type(dict, BinaryIO, bool) -> None
     ctx = Context(multiline_strings, {})
     for chunk in gen_table_chunks(__obj, ctx, name=""):
         __fp.write(chunk.encode(encoding = 'utf8'))
 
 
-# def dumps(__obj: dict[str, Any], *, multiline_strings: bool = False) -> str:
 def dumps(__obj,  multiline_strings = False):
+    #type(dict, bool) -> str
     ctx = Context(multiline_strings, {})
     return "".join(gen_table_chunks(__obj, ctx, name=""))
 
 
-# class Context(NamedTuple):
-#     allow_multiline: bool
-#     # cache rendered inline tables (mapping from object id to rendered inline table)
-#     inline_table_cache: dict[int, str]
+
 
 Context = namedtuple('Context', ('allow_multiline', 'inline_table_cache'))
 
-# def gen_table_chunks(
-#     table: Mapping[str, Any],
-#     ctx: Context,
-#     *,
-#     name: str,
-#     inside_aot: bool = False,
-# ) -> Generator[str, None, None]:
-
-def gen_table_chunks(
-    table,
-    ctx,
-    name,
-    inside_aot = False,
-):
+
+def gen_table_chunks(table, ctx, name, inside_aot = False):
+    #type(Mapping, Context, str bool) -> Iterator[str]
     yielded = False
     literals = []
-    # tables: list[tuple[str, Any, bool]] = []  # => [(key, value, inside_aot)]
-    tables = []  # => [(key, value, inside_aot)]
+    tables = []  
     for k, v in table.items():
         if isinstance(v, dict):
             tables.append((k, v, False))
         elif is_aot(v) and not all(is_suitable_inline_table(t, ctx) for t in v):
             tables.extend((k, t, True) for t in v)
         else:
             literals.append((k, v))
 
     if inside_aot or name and (literals or not tables):
         yielded = True
-        # yield f"[[{name}]]\n" if inside_aot else f"[{name}]\n"
         yield ("[[%s]]\n" if inside_aot else "[%s]\n") % name
 
     if literals:
         yielded = True
         for k, v in literals:
-            # yield f"{format_key_part(k)} = {format_literal(v, ctx)}\n"
             yield "%s = %s\n" % (format_key_part(k), format_literal(v, ctx))
 
     for k, v, in_aot in tables:
         if yielded:
             yield "\n"
         else:
             yielded = True
         key_part = format_key_part(k)
-        # display_name = f"{name}.{key_part}" if name else key_part
         display_name = ("%s.%s" % (name, key_part)) if name else key_part
-        # yield from gen_table_chunks(v, ctx, name=display_name, inside_aot=in_aot)
         for chunk in gen_table_chunks(v, ctx, name=display_name, inside_aot=in_aot):
             yield chunk
 
 
-# def format_literal(obj: object, ctx: Context, *, nest_level: int = 0) -> str:
 def format_literal(obj, ctx, nest_level= 0):
+    #type(type[any], Context, int) -> str
     if isinstance(obj, bool):
         return "true" if obj else "false"
     if isinstance(obj, (int, float, date, datetime)):
         return str(obj)
     if isinstance(obj, Decimal):
         return format_decimal(obj)
     if isinstance(obj, time):
@@ -115,78 +93,76 @@
         return str(obj)
     if isinstance(obj, str):
         return format_string(obj, allow_multiline=ctx.allow_multiline)
     if isinstance(obj, ARRAY_TYPES):
         return format_inline_array(obj, ctx, nest_level)
     if isinstance(obj, dict):
         return format_inline_table(obj, ctx)
-    # raise TypeError(f"Object of type {type(obj)} is not TOML serializable")
     raise TypeError("Object of type %s is not TOML serializable" % type(obj))
 
 
-# def format_decimal(obj: Decimal) -> str:
 def format_decimal(obj):
+    #type(Decimal) -> str
     if obj.is_nan():
         return "nan"
     if obj == Decimal("inf"):
         return "inf"
     if obj == Decimal("-inf"):
         return "-inf"
     return str(obj)
 
 
-# def format_inline_table(obj: dict, ctx: Context) -> str:
 def format_inline_table(obj, ctx):
+    #type(type[any], Context) -> str
+
     # check cache first
     obj_id = id(obj)
     if obj_id in ctx.inline_table_cache:
         return ctx.inline_table_cache[obj_id]
 
     if not obj:
         rendered = "{}"
     else:
         rendered = (
             "{ "
             + ", ".join(
-                # f"{format_key_part(k)} = {format_literal(v, ctx)}"
                 ("%s = %s" % (format_key_part(k), format_literal(v, ctx)))
                 for k, v in obj.items()
             )
             + " }"
         )
     ctx.inline_table_cache[obj_id] = rendered
     return rendered
 
 
-# def format_inline_array(obj: tuple | list, ctx: Context, nest_level: int) -> str:
 def format_inline_array(obj, ctx, nest_level):
+    #type(tuple | list, Context, int) -> str
     if not obj:
         return "[]"
     item_indent = ARRAY_INDENT * (1 + nest_level)
     closing_bracket_indent = ARRAY_INDENT * nest_level
     return (
         "[\n"
         + ",\n".join(
             item_indent + format_literal(item, ctx, nest_level=nest_level + 1)
             for item in obj
         )
-        # + f",\n{closing_bracket_indent}]"
         + ",\n%s]" % closing_bracket_indent
     )
 
 
-# def format_key_part(part: str) -> str:
 def format_key_part(part):
+    #type(str) -> str
     if part and BARE_KEY_CHARS.issuperset(part):
         return part
     return format_string(part, allow_multiline=False)
 
 
-# def format_string(s: str, *, allow_multiline: bool) -> str:
 def format_string(s, allow_multiline):
+    #type(str, bool) -> str
     do_multiline = allow_multiline and "\n" in s
     if do_multiline:
         result = '"""\n'
         s = s.replace("\r\n", "\n")
     else:
         result = '"'
 
@@ -208,23 +184,22 @@
                     result += COMPACT_ESCAPES[char]
             else:
                 result += "\\u" + hex(ord(char))[2:].rjust(4, "0")
             seq_start = pos + 1
         pos += 1
 
 
-# def is_aot(obj: Any) -> bool:
 def is_aot(obj):
+    #type(type[Any]) -> bool
     """Decides if an object behaves as an array of tables (i.e. a nonempty list
     of dicts)."""
     return bool(
         isinstance(obj, ARRAY_TYPES) and obj and all(isinstance(v, dict) for v in obj)
     )
 
 
-# def is_suitable_inline_table(obj: dict, ctx: Context) -> bool:
 def is_suitable_inline_table(obj, ctx):
+    #type(dict, Context) -> bool
     """Use heuristics to decide if the inline-style representation is a good
     choice for a given table."""
-    # rendered_inline = f"{ARRAY_INDENT}{format_inline_table(obj, ctx)},"
     rendered_inline = "%s%s," % (ARRAY_INDENT, format_inline_table(obj, ctx))
     return len(rendered_inline) <= MAX_LINE_LENGTH and "\n" not in rendered_inline
```

### Comparing `toml_tools-1.0.0/tests/burntsushi.py` & `toml_tools-1.1.0/tests/burntsushi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
 """Utilities for tests that are in the "burntsushi" format."""
 
+import sys
 import datetime
-from typing import Any
+
+try:
+    basestring #type: ignore
+except NameError:
+    basestring = str
 
 # Aliases for converting TOML compliance format [1] to BurntSushi format [2]
 # [1] https://github.com/toml-lang/compliance/blob/db7c3211fda30ff9ddb10292f4aeda7e2e10abc4/docs/json-encoding.md  # noqa: E501
 # [2] https://github.com/BurntSushi/toml-test/blob/4634fdf3a6ecd6aaea5f4cdcd98b2733c2694993/README.md  # noqa: E501
 _aliases = {
     "boolean": "bool",
     "offset datetime": "datetime",
     "local datetime": "datetime-local",
     "local date": "date-local",
     "local time": "time-local",
 }
 
 
 def convert(obj):  # noqa: C901
-    if isinstance(obj, str):
+    if isinstance(obj, basestring):
         return {"type": "string", "value": obj}
     elif isinstance(obj, bool):
         return {"type": "bool", "value": str(obj).lower()}
     elif isinstance(obj, int):
         return {"type": "integer", "value": str(obj)}
     elif isinstance(obj, float):
         return {"type": "float", "value": _normalize_float_str(str(obj))}
@@ -44,18 +49,18 @@
             "type": "date-local",
             "value": str(obj),
         }
     elif isinstance(obj, list):
         return [convert(i) for i in obj]
     elif isinstance(obj, dict):
         return {k: convert(v) for k, v in obj.items()}
-    raise Exception("unsupported type")
+    raise Exception("unsupported type: %s, %s" % (obj, type(obj)) )
 
 
-def normalize(obj: Any) -> Any:
+def normalize(obj):
     """Normalize test objects.
 
     This normalizes primitive values (e.g. floats), and also converts from
     TOML compliance format [1] to BurntSushi format [2].
 
     [1] https://github.com/toml-lang/compliance/blob/db7c3211fda30ff9ddb10292f4aeda7e2e10abc4/docs/json-encoding.md  # noqa: E501
     [2] https://github.com/BurntSushi/toml-test/blob/4634fdf3a6ecd6aaea5f4cdcd98b2733c2694993/README.md  # noqa: E501
@@ -79,15 +84,16 @@
             if norm_type == "array":
                 return [normalize(item) for item in value]
             return {"type": norm_type, "value": norm_value}
         return {k: normalize(v) for k, v in obj.items()}
     raise AssertionError("Burntsushi fixtures should be dicts/lists only")
 
 
-def _normalize_datetime_str(dt_str: str) -> str:
+def _normalize_datetime_str(dt_str):
+    #type(str) -> str
     if dt_str[-1].lower() == "z":
         dt_str = dt_str[:-1] + "+00:00"
 
     date = dt_str[:10]
     rest = dt_str[11:]
 
     if "+" in rest:
@@ -103,19 +109,21 @@
         time = rest
         offset = ""
 
     time = time.rstrip("0") if "." in time else time
     return date + "T" + time + sign + offset
 
 
-def _normalize_localtime_str(lt_str: str) -> str:
+def _normalize_localtime_str(lt_str):
+    #type(str) -> str
     return lt_str.rstrip("0") if "." in lt_str else lt_str
 
 
-def _normalize_float_str(float_str: str) -> str:
+def _normalize_float_str(float_str):
+    #type(str) -> str
     as_float = float(float_str)
 
     # Normalize "-0.0" and "+0.0"
     if as_float == 0:
         return "0"
 
     return str(as_float)
```

### Comparing `toml_tools-1.0.0/tests/test_data.py` & `toml_tools-1.1.0/tests/test_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
+import os
 import json
-from pathlib import Path
+import glob 
 import unittest
 
-from . import burntsushi, tomllib
+from . import burntsushi, toml_tools, stem
 
 
 class MissingFile:
-    def __init__(self, path: Path):
+    def __init__(self, path):
         self.path = path
 
 
-DATA_DIR = Path(__file__).parent / "data"
+DATA_DIR = os.path.join(os.path.dirname(__file__), "data")
 
-VALID_FILES = tuple((DATA_DIR / "valid").glob("**/*.toml"))
+VALID_FILES = glob.glob(os.path.join(DATA_DIR, "valid", "**/*.toml"))
 assert VALID_FILES, "Valid TOML test files not found"
 
 _expected_files = []
 for p in VALID_FILES:
-    json_path = p.with_suffix(".json")
+    json_path = os.path.splitext(p)[0] + ".json"
     try:
-        text = json.loads(json_path.read_bytes().decode())
+        with open(json_path, 'rb') as f:
+            text = json.loads(f.read().decode())
     except FileNotFoundError:
         text = MissingFile(json_path)
     _expected_files.append(text)
 VALID_FILES_EXPECTED = tuple(_expected_files)
 
-INVALID_FILES = tuple((DATA_DIR / "invalid").glob("**/*.toml"))
+INVALID_FILES = glob.glob(os.path.join(DATA_DIR, "invalid", "**/*.toml"))
 assert INVALID_FILES, "Invalid TOML test files not found"
 
 
 class TestData(unittest.TestCase):
-    def test_invalid(self):
-        for invalid in INVALID_FILES:
-            with self.subTest(msg=invalid.stem):
-                toml_bytes = invalid.read_bytes()
-                try:
-                    toml_str = toml_bytes.decode()
-                except UnicodeDecodeError:
-                    # Some BurntSushi tests are not valid UTF-8. Skip those.
-                    continue
-                with self.assertRaises(tomllib.TOMLDecodeError):
-                    tomllib.loads(toml_str)
-
-    def test_valid(self):
-        for valid, expected in zip(VALID_FILES, VALID_FILES_EXPECTED):
-            with self.subTest(msg=valid.stem):
-                if isinstance(expected, MissingFile):
-                    # For a poor man's xfail, assert that this is one of the
-                    # test cases where expected data is known to be missing.
-                    assert valid.stem in {
-                        "qa-array-inline-nested-1000",
-                        "qa-table-inline-nested-1000",
-                    }
-                    continue
-                toml_str = valid.read_bytes().decode()
-                actual = tomllib.loads(toml_str)
-                actual = burntsushi.convert(actual)
-                expected = burntsushi.normalize(expected)
-                self.assertEqual(actual, expected)
+    pass
+
+def make_valid_test(valid, expected):
+    def test_valid(self, valid = valid, expected  = expected):
+
+        if isinstance(expected, MissingFile):
+            # For a poor man's xfail, assert that this is one of the
+            # test cases where expected data is known to be missing.
+            assert stem(valid) in {
+                "qa-array-inline-nested-1000",
+                "qa-table-inline-nested-1000",
+            }
+            return
+        
+
+        with open(valid, 'rb') as f:
+            toml_str = f.read().decode()
+        actual = toml_tools.loads(toml_str)
+        actual = burntsushi.convert(actual)
+        expected = burntsushi.normalize(expected)
+        self.assertEqual(actual, expected)
+    return test_valid
+
+for valid, expected in zip(VALID_FILES, VALID_FILES_EXPECTED):
+    setattr(TestData, 
+            'test_valid_%s' % stem(valid).replace('-','_'), 
+            make_valid_test(valid, expected))
+
+
+
+def make_invalid_test(invalid):
+    def test_invalid(self, invalid = invalid):
+        with open(invalid,'rb') as f:
+            toml_bytes = f.read()
+            try:
+                toml_str = toml_bytes.decode('utf8')
+            except UnicodeDecodeError:
+                # Some BurntSushi tests are not valid UTF-8. Skip those.
+
+                assert True # a poorer man's xfail
+                return
+            with self.assertRaises(toml_tools.TOMLDecodeError):
+                toml_tools.loads(toml_str)
+    return test_invalid
+
+for invalid in INVALID_FILES:
+    setattr(TestData,
+            'test_invalid_%s' % stem(invalid).replace('-','_'), 
+            make_invalid_test(invalid))
```

### Comparing `toml_tools-1.0.0/tests/test_for_profiler.py` & `toml_tools-1.1.0/tests/test_for_profiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 This test can be useful for profiling, as most of the execution time
 will be spent writing TOML instead of managing pytest execution
 environment. To get and read profiler results:
   - `tox -e profile`
   - `firefox .tox/prof/combined.svg`
 """
 import os
-from pathlib import Path
 
-import toml_tools
+from . import toml_tools
 
 
-path = Path(__file__).parent.parent / "benchmark" / "data.toml"
-benchmark_toml = path.read_bytes().decode()
+path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "benchmark", "data.toml")
+with open(path, 'rb') as f:
+    benchmark_toml = f.read().decode('utf8')
 data = toml_tools.loads(benchmark_toml)
 
 
 def test_for_profiler():
     # increase the count here to reduce the impact of
     # setting up pytest execution environment. Let's keep
     # the count low by default because this is part of the
```

### Comparing `toml_tools-1.0.0/tests/test_misc.py` & `toml_tools-1.1.0/tests/test_misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
+import os
 import copy
 import datetime
 from decimal import Decimal as D
-from pathlib import Path
 import tempfile
 import unittest
+import io
 
-from . import tomllib
+from . import toml_tools
 
+from toml_tools._re import timezone
 
 class TestMiscellaneous(unittest.TestCase):
     def test_load(self):
         content = "one=1 \n two='two' \n arr=[]"
         expected = {"one": 1, "two": "two", "arr": []}
-        with tempfile.TemporaryDirectory() as tmp_dir_path:
-            file_path = Path(tmp_dir_path) / "test.toml"
-            file_path.write_text(content)
+        tmp_dir_path = os.path.join(tempfile.gettempdir(), 'toml_tools_test_incorrect_load')
 
-            with open(file_path, "rb") as bin_f:
-                actual = tomllib.load(bin_f)
+        if not os.path.isdir(tmp_dir_path):
+            os.mkdir(tmp_dir_path)
+        
+        file_path = os.path.join(tmp_dir_path, "test.toml")
+        with open(file_path, 'wt') as f:
+            f.write(content)
+
+        with open(file_path, "rb") as bin_f:
+            actual = toml_tools.load(bin_f)
         self.assertEqual(actual, expected)
 
+        os.unlink(file_path)
+        os.rmdir(tmp_dir_path)
+
+    @unittest.skipIf(hasattr(str, 'decode'), reason = "str can be decoded, so won't trip error (Python 2 or Iron Python 2)")
     def test_incorrect_load(self):
+
         content = "one=1"
-        with tempfile.TemporaryDirectory() as tmp_dir_path:
-            file_path = Path(tmp_dir_path) / "test.toml"
-            file_path.write_text(content)
-
-            with open(file_path, "r") as txt_f:
-                with self.assertRaises(TypeError):
-                    tomllib.load(txt_f)  # type: ignore[arg-type]
+        tmp_dir_path = os.path.join(tempfile.gettempdir(), 'toml_tools_test_incorrect_load')
+
+        if not os.path.isdir(tmp_dir_path):
+            os.mkdir(tmp_dir_path)
+
+        file_path = os.path.join(tmp_dir_path, "test.toml")
+        with open(file_path, 'wt') as f:
+            f.write(content)
+
+        with open(file_path, "rt") as txt_f:
+            with self.assertRaises(TypeError):
+                toml_tools.load(txt_f)  # type: ignore[arg-type]
+
+        os.unlink(file_path)
+        os.rmdir(tmp_dir_path)
 
     def test_parse_float(self):
         doc = """
               val=0.1
               biggest1=inf
               biggest2=+inf
               smallest=-inf
               notnum1=nan
               notnum2=-nan
               notnum3=+nan
               """
-        obj = tomllib.loads(doc, parse_float=D)
+        obj = toml_tools.loads(doc, parse_float=D)
         expected = {
             "val": D("0.1"),
             "biggest1": D("inf"),
             "biggest2": D("inf"),
             "smallest": D("-inf"),
             "notnum1": D("nan"),
             "notnum2": D("-nan"),
@@ -64,39 +84,39 @@
                 self.assertEqual(actual_val, expected_val)
 
     def test_deepcopy(self):
         doc = """
               [bliibaa.diibaa]
               offsettime=[1979-05-27T00:32:00.999999-07:00]
               """
-        obj = tomllib.loads(doc)
+        obj = toml_tools.loads(doc)
         obj_copy = copy.deepcopy(obj)
         self.assertEqual(obj_copy, obj)
         expected_obj = {
             "bliibaa": {
                 "diibaa": {
                     "offsettime": [
                         datetime.datetime(
                             1979,
                             5,
                             27,
                             0,
                             32,
                             0,
                             999999,
-                            tzinfo=datetime.timezone(datetime.timedelta(hours=-7)),
+                            tzinfo=timezone(datetime.timedelta(hours=-7)),
                         )
                     ]
                 }
             }
         }
         self.assertEqual(obj_copy, expected_obj)
 
     def test_inline_array_recursion_limit(self):
         nest_count = 470
         recursive_array_toml = "arr = " + nest_count * "[" + nest_count * "]"
-        tomllib.loads(recursive_array_toml)
+        toml_tools.loads(recursive_array_toml)
 
     def test_inline_table_recursion_limit(self):
         nest_count = 310
         recursive_table_toml = nest_count * "key = {" + nest_count * "}"
-        tomllib.loads(recursive_table_toml)
+        toml_tools.loads(recursive_table_toml)
```

### Comparing `toml_tools-1.0.0/tests/test_style.py` & `toml_tools-1.1.0/tests/test_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-import toml_tools
+from . import toml_tools
 
 
 
 def test_newline_before_table():
     actual = toml_tools.dumps({"table": {}})
     expected = "[table]\n"
     assert actual == expected
@@ -91,15 +91,15 @@
 
 [a.b.c.d.e2.f2]
 """
     assert actual == expected
 
 
 def test_array_of_tables_containing_lists():
-    example: dict = {"aot": [{"a": [0, 1, 2, 3]}]}
+    example = {"aot": [{"a": [0, 1, 2, 3]}]}
     expected = """\
 [[aot]]
 a = [
     0,
     1,
     2,
     3,
@@ -143,22 +143,22 @@
     assert actual == expected
     assert toml_tools.loads(actual) == example
 
 
 def test_array_of_short_tables():
     long_name = "a" * 87
     example = {"table": {"nested-array": [{long_name: 0}, {"b": 1}, {"c": 2}]}}
-    expected = f"""\
+    expected = """\
 [table]
 nested-array = [
-    {{ {long_name} = 0 }},
-    {{ b = 1 }},
-    {{ c = 2 }},
+    { %s = 0 },
+    { b = 1 },
+    { c = 2 },
 ]
-"""
+""" % long_name
     actual = toml_tools.dumps(example)
     assert actual == expected
 
 
 def test_example_issue_12():
     example = {
         "table": {
@@ -189,15 +189,15 @@
     actual = toml_tools.dumps(example)
     assert actual == expected
     assert toml_tools.loads(actual) == example
 
 
 def test_table_with_empty_array():
     # Empty arrays should never be AoTs
-    example: dict = {"table": {"array": []}}
+    example = {"table": {"array": []}}
     expected = """\
 [table]
 array = []
 """
     actual = toml_tools.dumps(example)
     assert actual == expected
     assert toml_tools.loads(actual) == example
```

### Comparing `toml_tools-1.0.0/tests/test_types.py` & `toml_tools-1.1.0/tests/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from decimal import Decimal
 
-import toml_tools
+from . import toml_tools
 
 
 def test_decimal():
     obj = {
         "decimal-0": Decimal(0),
         "decimal-pi": Decimal("3.14159"),
         "decimal-inf": Decimal("inf"),
```

### Comparing `toml_tools-1.0.0/tests/test_valid.py` & `toml_tools-1.1.0/tests/test_valid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # -*- coding: utf-8 -*-
 
+import os
+import glob
 from decimal import Decimal
 from math import isnan
-from pathlib import Path
-from typing import Union
 
 import pytest
-import toml_tools
+from . import toml_tools, stem
 
 
-COMPLIANCE_DIR = Path(__file__).parent / "data" / "toml-lang-compliance" / "valid"
-EXTRAS_DIR = Path(__file__).parent / "data" / "extras" / "valid"
+PARENT_DIR = os.path.dirname(__file__)
+COMPLIANCE_DIR = os.path.join(PARENT_DIR, "data", "toml-lang-compliance", "valid")
+EXTRAS_DIR = os.path.join(PARENT_DIR, "data", "extras", "valid")
 
-VALID_FILES = tuple(COMPLIANCE_DIR.glob("**/*.toml")) + tuple(
-    EXTRAS_DIR.glob("**/*.toml")
-)
+VALID_FILES = (glob.glob(os.path.join(COMPLIANCE_DIR,"**/*.toml")) + 
+               glob.glob(os.path.join(EXTRAS_DIR, "**/*.toml")))
 
 
 @pytest.mark.parametrize(
     "valid",
-    VALID_FILES,
-    ids=[p.stem for p in VALID_FILES],
+    VALID_FILES#),
+    #ids=[os.path.splitext(p)[0] for p in VALID_FILES],
+    # ids=[stem(p) for p in VALID_FILES],
 )
 def test_valid(valid):
-    if valid.stem in {"qa-array-inline-nested-1000", "qa-table-inline-nested-1000"}:
+    if stem(valid) in {"qa-array-inline-nested-1000", "qa-table-inline-nested-1000"}:
         pytest.xfail("This much recursion is not supported")
-    original_str = valid.read_bytes().decode()
+    with open(valid,'rb') as f:
+        original_str = f.read().decode()
+    # original_str = valid.read_bytes().decode()
     original_data = toml_tools.loads(original_str)
     dump_str = toml_tools.dumps(original_data)
     after_dump_data = toml_tools.loads(dump_str)
     assert replace_nans(after_dump_data) == replace_nans(original_data)
 
 
 NAN = object()
 
 
-def replace_nans(cont: Union[dict, list]) -> Union[dict, list]:
+def replace_nans(cont):
+    #type(Union[dict, list] -> Union[dict, list])
     """Replace NaNs with a sentinel object to fix the problem that NaN is not
     equal to another NaN."""
     for k, v in cont.items() if isinstance(cont, dict) else enumerate(cont):
         if isinstance(v, (float, Decimal)) and isnan(v):
             cont[k] = NAN
         elif isinstance(v, dict) or isinstance(v, list):
             cont[k] = replace_nans(cont[k])
```

### Comparing `toml_tools-1.0.0/PKG-INFO` & `toml_tools-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,375 +1,379 @@
-Metadata-Version: 2.1
-Name: toml_tools
-Version: 1.0.0
-Summary: Tomli and Tomli-W for Python 2 and Iron Python
-Keywords: toml
-Author-email: Taneli Hukkinen <hukkin@users.noreply.github.com>, James Parrott <james.parrott@proton.me>
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Project-URL: Homepage, https://github.com/JamesParrott/toml_tools
-
-# toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
-
-v1.0.0 is a complete overhaul.  toml_tools is now based on tomli and tomli-w.
-
-# Parent Project number (1/2)'s Readme File (Tomli)
-
-> A lil' TOML parser
-
-**Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
-
-<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->
-
-- [Intro](#intro)
-- [Installation](#installation)
-- [Usage](#usage)
-  - [Parse a TOML string](#parse-a-toml-string)
-  - [Parse a TOML file](#parse-a-toml-file)
-  - [Handle invalid TOML](#handle-invalid-toml)
-  - [Construct `decimal.Decimal`s from TOML floats](#construct-decimaldecimals-from-toml-floats)
-  - [Building a `tomli`/`tomllib` compatibility layer](#building-a-tomlitomllib-compatibility-layer)
-- [FAQ](#faq)
-  - [Why this parser?](#why-this-parser)
-  - [Is comment preserving round-trip parsing supported?](#is-comment-preserving-round-trip-parsing-supported)
-  - [Is there a `dumps`, `write` or `encode` function?](#is-there-a-dumps-write-or-encode-function)
-  - [How do TOML types map into Python types?](#how-do-toml-types-map-into-python-types)
-- [Performance](#performance)
-
-<!-- mdformat-toc end -->
-
-## Intro<a name="intro"></a>
-
-Tomli is a Python library for parsing [TOML](https://toml.io).
-It is fully compatible with [TOML v1.0.0](https://toml.io/en/v1.0.0).
-
-A version of Tomli, the `tomllib` module,
-was added to the standard library in Python 3.11
-via [PEP 680](https://www.python.org/dev/peps/pep-0680/).
-Tomli continues to provide a backport on PyPI for Python versions
-where the standard library module is not available
-and that have not yet reached their end-of-life.
-
-## Installation<a name="installation"></a>
-
-```bash
-pip install tomli
-```
-
-## Usage<a name="usage"></a>
-
-### Parse a TOML string<a name="parse-a-toml-string"></a>
-
-```python
-import tomli
-
-toml_str = """
-[[players]]
-name = "Lehtinen"
-number = 26
-
-[[players]]
-name = "Numminen"
-number = 27
-"""
-
-toml_dict = tomli.loads(toml_str)
-assert toml_dict == {
-    "players": [{"name": "Lehtinen", "number": 26}, {"name": "Numminen", "number": 27}]
-}
-```
-
-### Parse a TOML file<a name="parse-a-toml-file"></a>
-
-```python
-import tomli
-
-with open("path_to_file/conf.toml", "rb") as f:
-    toml_dict = tomli.load(f)
-```
-
-The file must be opened in binary mode (with the `"rb"` flag).
-Binary mode will enforce decoding the file as UTF-8 with universal newlines disabled,
-both of which are required to correctly parse TOML.
-
-### Handle invalid TOML<a name="handle-invalid-toml"></a>
-
-```python
-import tomli
-
-try:
-    toml_dict = tomli.loads("]] this is invalid TOML [[")
-except tomli.TOMLDecodeError:
-    print("Yep, definitely not valid.")
-```
-
-Note that error messages are considered informational only.
-They should not be assumed to stay constant across Tomli versions.
-
-### Construct `decimal.Decimal`s from TOML floats<a name="construct-decimaldecimals-from-toml-floats"></a>
-
-```python
-from decimal import Decimal
-import tomli
-
-toml_dict = tomli.loads("precision-matters = 0.982492", parse_float=Decimal)
-assert isinstance(toml_dict["precision-matters"], Decimal)
-assert toml_dict["precision-matters"] == Decimal("0.982492")
-```
-
-Note that `decimal.Decimal` can be replaced with another callable that converts a TOML float from string to a Python type.
-The `decimal.Decimal` is, however, a practical choice for use cases where float inaccuracies can not be tolerated.
-
-Illegal types are `dict` and `list`, and their subtypes.
-A `ValueError` will be raised if `parse_float` produces illegal types.
-
-### Building a `tomli`/`tomllib` compatibility layer<a name="building-a-tomlitomllib-compatibility-layer"></a>
-
-Python versions 3.11+ ship with a version of Tomli:
-the `tomllib` standard library module.
-To build code that uses the standard library if available,
-but still works seamlessly with Python 3.6+,
-do the following.
-
-Instead of a hard Tomli dependency, use the following
-[dependency specifier](https://packaging.python.org/en/latest/specifications/dependency-specifiers/)
-to only require Tomli when the standard library module is not available:
-
-```
-tomli >= 1.1.0 ; python_version < "3.11"
-```
-
-Then, in your code, import a TOML parser using the following fallback mechanism:
-
-```python
-try:
-    import tomllib
-except ModuleNotFoundError:
-    import tomli as tomllib
-
-tomllib.loads("['This parses fine with Python 3.6+']")
-```
-
-## FAQ<a name="faq"></a>
-
-### Why this parser?<a name="why-this-parser"></a>
-
-- it's lil'
-- pure Python with zero dependencies
-- the fastest pure Python parser [\*](#performance):
-  16x as fast as [tomlkit](https://pypi.org/project/tomlkit/),
-  2.3x as fast as [toml](https://pypi.org/project/toml/)
-- outputs [basic data types](#how-do-toml-types-map-into-python-types) only
-- 100% spec compliant: passes all tests in
-  [BurntSushi/toml-test](https://github.com/BurntSushi/toml-test)
-  test suite
-- thoroughly tested: 100% branch coverage
-
-### Is comment preserving round-trip parsing supported?<a name="is-comment-preserving-round-trip-parsing-supported"></a>
-
-No.
-
-The `tomli.loads` function returns a plain `dict` that is populated with builtin types and types from the standard library only.
-Preserving comments requires a custom type to be returned so will not be supported,
-at least not by the `tomli.loads` and `tomli.load` functions.
-
-Look into [TOML Kit](https://github.com/sdispater/tomlkit) if preservation of style is what you need.
-
-### Is there a `dumps`, `write` or `encode` function?<a name="is-there-a-dumps-write-or-encode-function"></a>
-
-[Tomli-W](https://github.com/hukkin/tomli-w) is the write-only counterpart of Tomli, providing `dump` and `dumps` functions.
-
-The core library does not include write capability, as most TOML use cases are read-only, and Tomli intends to be minimal.
-
-### How do TOML types map into Python types?<a name="how-do-toml-types-map-into-python-types"></a>
-
-| TOML type        | Python type         | Details                                                      |
-| ---------------- | ------------------- | ------------------------------------------------------------ |
-| Document Root    | `dict`              |                                                              |
-| Key              | `str`               |                                                              |
-| String           | `str`               |                                                              |
-| Integer          | `int`               |                                                              |
-| Float            | `float`             |                                                              |
-| Boolean          | `bool`              |                                                              |
-| Offset Date-Time | `datetime.datetime` | `tzinfo` attribute set to an instance of `datetime.timezone` |
-| Local Date-Time  | `datetime.datetime` | `tzinfo` attribute set to `None`                             |
-| Local Date       | `datetime.date`     |                                                              |
-| Local Time       | `datetime.time`     |                                                              |
-| Array            | `list`              |                                                              |
-| Table            | `dict`              |                                                              |
-| Inline Table     | `dict`              |                                                              |
-
-## Performance<a name="performance"></a>
-
-The `benchmark/` folder in this repository contains a performance benchmark for comparing the various Python TOML parsers.
-The benchmark can be run with `tox -e benchmark-pypi`.
-Running the benchmark on my personal computer output the following:
-
-```console
-foo@bar:~/dev/tomli$ tox -e benchmark-pypi
-benchmark-pypi installed: attrs==21.4.0,click==8.0.3,pytomlpp==1.0.10,qtoml==0.3.1,rtoml==0.7.1,toml==0.10.2,tomli==2.0.1,tomlkit==0.9.2
-benchmark-pypi run-test-pre: PYTHONHASHSEED='3088452573'
-benchmark-pypi run-test: commands[0] | python -c 'import datetime; print(datetime.date.today())'
-2022-02-09
-benchmark-pypi run-test: commands[1] | python --version
-Python 3.8.10
-benchmark-pypi run-test: commands[2] | python benchmark/run.py
-Parsing data.toml 5000 times:
-------------------------------------------------------
-    parser |  exec time | performance (more is better)
------------+------------+-----------------------------
-     rtoml |    0.891 s | baseline (100%)
-  pytomlpp |    0.969 s | 91.90%
-     tomli |        4 s | 22.25%
-      toml |     9.01 s | 9.88%
-     qtoml |     11.1 s | 8.05%
-   tomlkit |       63 s | 1.41%
-```
-
-The parsers are ordered from fastest to slowest, using the fastest parser as baseline.
-Tomli performed the best out of all pure Python TOML parsers,
-losing only to pytomlpp (wraps C++) and rtoml (wraps Rust).
-
-# Iron-Tomli-W
-
-A fork of Tomli-W for Iron Python 2
-
-- **Reluctant Iron Python 2 user**: [James Parrott](https://github.com/JamesParrott)
-- **Version**: 1.0.0
-- **Date**: 25 April, 2023
- - **License**: [MIT](https://github.com/GeospatialPython/pyshp/blob/master/LICENSE.TXT)
- - 
-## Installation<a name="installation"></a>
-
-For the time being, manually copy `_write.py` and `__init__.py` into a folder called `iron-tomli-w` into a path (and append that to sys.path if it's not already there)
-
-# Parent Project number (2/2)'s Readme File (Iron-Tomli-W)
-
-A fork of Tomli-W for Iron Python 2
-
-- **Reluctant Iron Python 2 user**: [James Parrott](https://github.com/JamesParrott)
-- **Version**: 1.0.0
-- **Date**: 25 April, 2023
- - **License**: [MIT](https://github.com/GeospatialPython/pyshp/blob/master/LICENSE.TXT)
- - 
-## Installation<a name="installation"></a>
-
-For the time being, manually copy `_write.py` and `__init__.py` into a folder called `iron-tomli-w` into a path (and append that to sys.path if it's not already there)
-
-# Tomli-W
-
-> A lil' TOML writer
-
-**Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
-
-<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->
-
-- [Intro](#intro)
-- [Installation](#installation)
-- [Usage](#usage)
-  - [Write to string](#write-to-string)
-  - [Write to file](#write-to-file)
-- [FAQ](#faq)
-  - [Does Tomli-W sort the document?](#does-tomli-w-sort-the-document)
-  - [Does Tomli-W support writing documents with comments or custom whitespace?](#does-tomli-w-support-writing-documents-with-comments-or-custom-whitespace)
-  - [Why does Tomli-W not write a multi-line string if the string value contains newlines?](#why-does-tomli-w-not-write-a-multi-line-string-if-the-string-value-contains-newlines)
-  - [Is Tomli-W output guaranteed to be valid TOML?](#is-tomli-w-output-guaranteed-to-be-valid-toml)
-
-<!-- mdformat-toc end -->
-
-## Intro<a name="intro"></a>
-
-Tomli-W is a Python library for writing [TOML](https://toml.io).
-It is a write-only counterpart to [Tomli](https://github.com/hukkin/tomli),
-which is a read-only TOML parser.
-Tomli-W is fully compatible with [TOML v1.0.0](https://toml.io/en/v1.0.0).
-
-## Usage<a name="usage"></a>
-
-### Write to string<a name="write-to-string"></a>
-
-```python
-import tomli_w
-
-doc = {"table": {"nested": {}, "val3": 3}, "val2": 2, "val1": 1}
-expected_toml = """\
-val2 = 2
-val1 = 1
-
-[table]
-val3 = 3
-
-[table.nested]
-"""
-assert tomli_w.dumps(doc) == expected_toml
-```
-
-### Write to file<a name="write-to-file"></a>
-
-```python
-import tomli_w
-
-doc = {"one": 1, "two": 2, "pi": 3}
-with open("path_to_file/conf.toml", "wb") as f:
-    tomli_w.dump(doc, f)
-```
-
-## FAQ<a name="faq"></a>
-
-### Does Tomli-W sort the document?<a name="does-tomli-w-sort-the-document"></a>
-
-No, but it respects sort order of the input data,
-so one could sort the content of the `dict` (recursively) before calling `tomli_w.dumps`.
-
-### Does Tomli-W support writing documents with comments or custom whitespace?<a name="does-tomli-w-support-writing-documents-with-comments-or-custom-whitespace"></a>
-
-No.
-
-### Why does Tomli-W not write a multi-line string if the string value contains newlines?<a name="why-does-tomli-w-not-write-a-multi-line-string-if-the-string-value-contains-newlines"></a>
-
-This default was chosen to achieve lossless parse/write round-trips.
-
-TOML strings can contain newlines where exact bytes matter, e.g.
-
-```toml
-s = "here's a newline\r\n"
-```
-
-TOML strings also can contain newlines where exact byte representation is not relevant, e.g.
-
-```toml
-s = """here's a newline
-"""
-```
-
-A parse/write round-trip that converts the former example to the latter does not preserve the original newline byte sequence.
-This is why Tomli-W avoids writing multi-line strings.
-
-A keyword argument is provided for users who do not need newline bytes to be preserved:
-
-```python
-import tomli_w
-
-doc = {"s": "here's a newline\r\n"}
-expected_toml = '''\
-s = """
-here's a newline
-"""
-'''
-assert tomli_w.dumps(doc, multiline_strings=True) == expected_toml
-```
-
-### Is Tomli-W output guaranteed to be valid TOML?<a name="is-tomli-w-output-guaranteed-to-be-valid-toml"></a>
-
-No.
-If there's a chance that your input data is bad and you need output validation,
-parse the output string once with `tomli.loads`.
-If the parse is successful (does not raise `tomli.TOMLDecodeError`) then the string is valid TOML.
-
+Metadata-Version: 2.1
+Name: toml_tools
+Version: 1.1.0
+Summary: Tomli and Tomli-W for Python 2 and Iron Python
+Home-page: https://github.com/JamesParrott/toml_tools
+Author: Taneli Hukkinen
+Author-email: hukkin@users.noreply.github.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: IronPython
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
+
+v1.0.0 is a complete overhaul.  toml_tools is now based on tomli and tomli-w.
+
+# Parent Project number (1/2)'s Readme File (Tomli)
+
+> A lil' TOML parser
+
+**Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
+
+<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->
+
+- [Intro](#intro)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Parse a TOML string](#parse-a-toml-string)
+  - [Parse a TOML file](#parse-a-toml-file)
+  - [Handle invalid TOML](#handle-invalid-toml)
+  - [Construct `decimal.Decimal`s from TOML floats](#construct-decimaldecimals-from-toml-floats)
+  - [Building a `tomli`/`tomllib` compatibility layer](#building-a-tomlitomllib-compatibility-layer)
+- [FAQ](#faq)
+  - [Why this parser?](#why-this-parser)
+  - [Is comment preserving round-trip parsing supported?](#is-comment-preserving-round-trip-parsing-supported)
+  - [Is there a `dumps`, `write` or `encode` function?](#is-there-a-dumps-write-or-encode-function)
+  - [How do TOML types map into Python types?](#how-do-toml-types-map-into-python-types)
+- [Performance](#performance)
+
+<!-- mdformat-toc end -->
+
+## Intro<a name="intro"></a>
+
+Tomli is a Python library for parsing [TOML](https://toml.io).
+It is fully compatible with [TOML v1.0.0](https://toml.io/en/v1.0.0).
+
+A version of Tomli, the `tomllib` module,
+was added to the standard library in Python 3.11
+via [PEP 680](https://www.python.org/dev/peps/pep-0680/).
+Tomli continues to provide a backport on PyPI for Python versions
+where the standard library module is not available
+and that have not yet reached their end-of-life.
+
+## Installation<a name="installation"></a>
+
+```bash
+pip install tomli
+```
+
+## Usage<a name="usage"></a>
+
+### Parse a TOML string<a name="parse-a-toml-string"></a>
+
+```python
+import tomli
+
+toml_str = """
+[[players]]
+name = "Lehtinen"
+number = 26
+
+[[players]]
+name = "Numminen"
+number = 27
+"""
+
+toml_dict = tomli.loads(toml_str)
+assert toml_dict == {
+    "players": [{"name": "Lehtinen", "number": 26}, {"name": "Numminen", "number": 27}]
+}
+```
+
+### Parse a TOML file<a name="parse-a-toml-file"></a>
+
+```python
+import tomli
+
+with open("path_to_file/conf.toml", "rb") as f:
+    toml_dict = tomli.load(f)
+```
+
+The file must be opened in binary mode (with the `"rb"` flag).
+Binary mode will enforce decoding the file as UTF-8 with universal newlines disabled,
+both of which are required to correctly parse TOML.
+
+### Handle invalid TOML<a name="handle-invalid-toml"></a>
+
+```python
+import tomli
+
+try:
+    toml_dict = tomli.loads("]] this is invalid TOML [[")
+except tomli.TOMLDecodeError:
+    print("Yep, definitely not valid.")
+```
+
+Note that error messages are considered informational only.
+They should not be assumed to stay constant across Tomli versions.
+
+### Construct `decimal.Decimal`s from TOML floats<a name="construct-decimaldecimals-from-toml-floats"></a>
+
+```python
+from decimal import Decimal
+import tomli
+
+toml_dict = tomli.loads("precision-matters = 0.982492", parse_float=Decimal)
+assert isinstance(toml_dict["precision-matters"], Decimal)
+assert toml_dict["precision-matters"] == Decimal("0.982492")
+```
+
+Note that `decimal.Decimal` can be replaced with another callable that converts a TOML float from string to a Python type.
+The `decimal.Decimal` is, however, a practical choice for use cases where float inaccuracies can not be tolerated.
+
+Illegal types are `dict` and `list`, and their subtypes.
+A `ValueError` will be raised if `parse_float` produces illegal types.
+
+### Building a `tomli`/`tomllib` compatibility layer<a name="building-a-tomlitomllib-compatibility-layer"></a>
+
+Python versions 3.11+ ship with a version of Tomli:
+the `tomllib` standard library module.
+To build code that uses the standard library if available,
+but still works seamlessly with Python 3.6+,
+do the following.
+
+Instead of a hard Tomli dependency, use the following
+[dependency specifier](https://packaging.python.org/en/latest/specifications/dependency-specifiers/)
+to only require Tomli when the standard library module is not available:
+
+```
+tomli >= 1.1.0 ; python_version < "3.11"
+```
+
+Then, in your code, import a TOML parser using the following fallback mechanism:
+
+```python
+try:
+    import tomllib
+except ModuleNotFoundError:
+    import tomli as tomllib
+
+tomllib.loads("['This parses fine with Python 3.6+']")
+```
+
+## FAQ<a name="faq"></a>
+
+### Why this parser?<a name="why-this-parser"></a>
+
+- it's lil'
+- pure Python with zero dependencies
+- the fastest pure Python parser [\*](#performance):
+  16x as fast as [tomlkit](https://pypi.org/project/tomlkit/),
+  2.3x as fast as [toml](https://pypi.org/project/toml/)
+- outputs [basic data types](#how-do-toml-types-map-into-python-types) only
+- 100% spec compliant: passes all tests in
+  [BurntSushi/toml-test](https://github.com/BurntSushi/toml-test)
+  test suite
+- thoroughly tested: 100% branch coverage
+
+### Is comment preserving round-trip parsing supported?<a name="is-comment-preserving-round-trip-parsing-supported"></a>
+
+No.
+
+The `tomli.loads` function returns a plain `dict` that is populated with builtin types and types from the standard library only.
+Preserving comments requires a custom type to be returned so will not be supported,
+at least not by the `tomli.loads` and `tomli.load` functions.
+
+Look into [TOML Kit](https://github.com/sdispater/tomlkit) if preservation of style is what you need.
+
+### Is there a `dumps`, `write` or `encode` function?<a name="is-there-a-dumps-write-or-encode-function"></a>
+
+[Tomli-W](https://github.com/hukkin/tomli-w) is the write-only counterpart of Tomli, providing `dump` and `dumps` functions.
+
+The core library does not include write capability, as most TOML use cases are read-only, and Tomli intends to be minimal.
+
+### How do TOML types map into Python types?<a name="how-do-toml-types-map-into-python-types"></a>
+
+| TOML type        | Python type         | Details                                                      |
+| ---------------- | ------------------- | ------------------------------------------------------------ |
+| Document Root    | `dict`              |                                                              |
+| Key              | `str`               |                                                              |
+| String           | `str`               |                                                              |
+| Integer          | `int`               |                                                              |
+| Float            | `float`             |                                                              |
+| Boolean          | `bool`              |                                                              |
+| Offset Date-Time | `datetime.datetime` | `tzinfo` attribute set to an instance of `datetime.timezone` |
+| Local Date-Time  | `datetime.datetime` | `tzinfo` attribute set to `None`                             |
+| Local Date       | `datetime.date`     |                                                              |
+| Local Time       | `datetime.time`     |                                                              |
+| Array            | `list`              |                                                              |
+| Table            | `dict`              |                                                              |
+| Inline Table     | `dict`              |                                                              |
+
+## Performance<a name="performance"></a>
+
+The `benchmark/` folder in this repository contains a performance benchmark for comparing the various Python TOML parsers.
+The benchmark can be run with `tox -e benchmark-pypi`.
+Running the benchmark on my personal computer output the following:
+
+```console
+foo@bar:~/dev/tomli$ tox -e benchmark-pypi
+benchmark-pypi installed: attrs==21.4.0,click==8.0.3,pytomlpp==1.0.10,qtoml==0.3.1,rtoml==0.7.1,toml==0.10.2,tomli==2.0.1,tomlkit==0.9.2
+benchmark-pypi run-test-pre: PYTHONHASHSEED='3088452573'
+benchmark-pypi run-test: commands[0] | python -c 'import datetime; print(datetime.date.today())'
+2022-02-09
+benchmark-pypi run-test: commands[1] | python --version
+Python 3.8.10
+benchmark-pypi run-test: commands[2] | python benchmark/run.py
+Parsing data.toml 5000 times:
+------------------------------------------------------
+    parser |  exec time | performance (more is better)
+-----------+------------+-----------------------------
+     rtoml |    0.891 s | baseline (100%)
+  pytomlpp |    0.969 s | 91.90%
+     tomli |        4 s | 22.25%
+      toml |     9.01 s | 9.88%
+     qtoml |     11.1 s | 8.05%
+   tomlkit |       63 s | 1.41%
+```
+
+The parsers are ordered from fastest to slowest, using the fastest parser as baseline.
+Tomli performed the best out of all pure Python TOML parsers,
+losing only to pytomlpp (wraps C++) and rtoml (wraps Rust).
+
+# Iron-Tomli-W
+
+A fork of Tomli-W for Iron Python 2
+
+- **Reluctant Iron Python 2 user**: [James Parrott](https://github.com/JamesParrott)
+- **Version**: 1.0.0
+- **Date**: 25 April, 2023
+ - **License**: [MIT](https://github.com/GeospatialPython/pyshp/blob/master/LICENSE.TXT)
+ - 
+## Installation<a name="installation"></a>
+
+For the time being, manually copy `_write.py` and `__init__.py` into a folder called `iron-tomli-w` into a path (and append that to sys.path if it's not already there)
+
+# Parent Project number (2/2)'s Readme File (Iron-Tomli-W)
+
+A fork of Tomli-W for Iron Python 2
+
+- **Reluctant Iron Python 2 user**: [James Parrott](https://github.com/JamesParrott)
+- **Version**: 1.0.0
+- **Date**: 25 April, 2023
+ - **License**: [MIT](https://github.com/GeospatialPython/pyshp/blob/master/LICENSE.TXT)
+ - 
+## Installation<a name="installation"></a>
+
+For the time being, manually copy `_write.py` and `__init__.py` into a folder called `iron-tomli-w` into a path (and append that to sys.path if it's not already there)
+
+# Tomli-W
+
+> A lil' TOML writer
+
+**Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
+
+<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->
+
+- [Intro](#intro)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Write to string](#write-to-string)
+  - [Write to file](#write-to-file)
+- [FAQ](#faq)
+  - [Does Tomli-W sort the document?](#does-tomli-w-sort-the-document)
+  - [Does Tomli-W support writing documents with comments or custom whitespace?](#does-tomli-w-support-writing-documents-with-comments-or-custom-whitespace)
+  - [Why does Tomli-W not write a multi-line string if the string value contains newlines?](#why-does-tomli-w-not-write-a-multi-line-string-if-the-string-value-contains-newlines)
+  - [Is Tomli-W output guaranteed to be valid TOML?](#is-tomli-w-output-guaranteed-to-be-valid-toml)
+
+<!-- mdformat-toc end -->
+
+## Intro<a name="intro"></a>
+
+Tomli-W is a Python library for writing [TOML](https://toml.io).
+It is a write-only counterpart to [Tomli](https://github.com/hukkin/tomli),
+which is a read-only TOML parser.
+Tomli-W is fully compatible with [TOML v1.0.0](https://toml.io/en/v1.0.0).
+
+## Usage<a name="usage"></a>
+
+### Write to string<a name="write-to-string"></a>
+
+```python
+import tomli_w
+
+doc = {"table": {"nested": {}, "val3": 3}, "val2": 2, "val1": 1}
+expected_toml = """\
+val2 = 2
+val1 = 1
+
+[table]
+val3 = 3
+
+[table.nested]
+"""
+assert tomli_w.dumps(doc) == expected_toml
+```
+
+### Write to file<a name="write-to-file"></a>
+
+```python
+import tomli_w
+
+doc = {"one": 1, "two": 2, "pi": 3}
+with open("path_to_file/conf.toml", "wb") as f:
+    tomli_w.dump(doc, f)
+```
+
+## FAQ<a name="faq"></a>
+
+### Does Tomli-W sort the document?<a name="does-tomli-w-sort-the-document"></a>
+
+No, but it respects sort order of the input data,
+so one could sort the content of the `dict` (recursively) before calling `tomli_w.dumps`.
+
+### Does Tomli-W support writing documents with comments or custom whitespace?<a name="does-tomli-w-support-writing-documents-with-comments-or-custom-whitespace"></a>
+
+No.
+
+### Why does Tomli-W not write a multi-line string if the string value contains newlines?<a name="why-does-tomli-w-not-write-a-multi-line-string-if-the-string-value-contains-newlines"></a>
+
+This default was chosen to achieve lossless parse/write round-trips.
+
+TOML strings can contain newlines where exact bytes matter, e.g.
+
+```toml
+s = "here's a newline\r\n"
+```
+
+TOML strings also can contain newlines where exact byte representation is not relevant, e.g.
+
+```toml
+s = """here's a newline
+"""
+```
+
+A parse/write round-trip that converts the former example to the latter does not preserve the original newline byte sequence.
+This is why Tomli-W avoids writing multi-line strings.
+
+A keyword argument is provided for users who do not need newline bytes to be preserved:
+
+```python
+import tomli_w
+
+doc = {"s": "here's a newline\r\n"}
+expected_toml = '''\
+s = """
+here's a newline
+"""
+'''
+assert tomli_w.dumps(doc, multiline_strings=True) == expected_toml
+```
+
+### Is Tomli-W output guaranteed to be valid TOML?<a name="is-tomli-w-output-guaranteed-to-be-valid-toml"></a>
+
+No.
+If there's a chance that your input data is bad and you need output validation,
+parse the output string once with `tomli.loads`.
+If the parse is successful (does not raise `tomli.TOMLDecodeError`) then the string is valid TOML.
```

