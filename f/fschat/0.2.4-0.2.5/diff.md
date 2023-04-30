# Comparing `tmp/fschat-0.2.4.tar.gz` & `tmp/fschat-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.4.tar", last modified: Fri Apr 28 16:37:51 2023, max compression
+gzip compressed data, was "fschat-0.2.5.tar", last modified: Sun Apr 30 01:50:56 2023, max compression
```

## Comparing `fschat-0.2.4.tar` & `fschat-0.2.5.tar`

### file list

```diff
@@ -1,205 +1,212 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14167 2023-04-28 16:37:51.441497 fschat-0.2.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13673 2023-04-28 16:37:35.000000 fschat-0.2.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/fastchat/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10534 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3166 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5998 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/model/apply_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1688 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/protocol/chat_completion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6637 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11251 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6177 2023-04-27 21:49:08.000000 fschat-0.2.4/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6921 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13979 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_block_arena_anony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13609 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/gradio_block_arena_named.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5205 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11425 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8045 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2480 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8627 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14871 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5407 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14167 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-28 16:37:35.000000 fschat-0.2.4/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-28 16:37:51.441497 fschat-0.2.4/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/wandb/latest-run/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.4/wandb/latest-run/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8305 2023-04-23 12:16:11.000000 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8235 2023-04-23 12:33:09.000000 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8252 2023-04-23 12:33:55.000000 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8026 2023-04-23 12:44:12.000000 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8027 2023-04-23 12:45:40.000000 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8050 2023-04-23 12:47:12.000000 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-04-23 12:48:16.000000 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2023-04-23 12:49:50.000000 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8172 2023-04-23 12:50:49.000000 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8177 2023-04-23 12:51:43.000000 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8217 2023-04-23 12:53:11.000000 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:15:57.000000 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:17:37.000000 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:22:26.000000 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:28:07.000000 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:28:26.000000 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:29:26.000000 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8722 2023-04-25 09:30:15.000000 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:31:04.000000 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:32:09.000000 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.209236 fschat-0.2.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15090 2023-04-30 01:50:56.205236 fschat-0.2.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14596 2023-04-30 01:50:41.000000 fschat-0.2.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-30 01:50:41.000000 fschat-0.2.5/fastchat/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/client/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/client/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10621 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3036 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.5/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1849 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/protocol/chat_completion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.201236 fschat-0.2.5/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6165 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11455 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5330 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6921 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13439 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13063 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17943 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5205 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13703 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7474 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/serve/rwkv_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2430 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.201236 fschat-0.2.5/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8637 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14838 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5407 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15090 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3424 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-30 01:50:41.000000 fschat-0.2.5/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-30 01:50:56.209236 fschat-0.2.5/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/latest-run/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8667 2023-04-29 11:02:46.000000 fschat-0.2.5/wandb/latest-run/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8305 2023-04-23 12:16:11.000000 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8235 2023-04-23 12:33:09.000000 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8252 2023-04-23 12:33:55.000000 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8026 2023-04-23 12:44:12.000000 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8027 2023-04-23 12:45:40.000000 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8050 2023-04-23 12:47:12.000000 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-04-23 12:48:16.000000 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2023-04-23 12:49:50.000000 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8172 2023-04-23 12:50:49.000000 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8177 2023-04-23 12:51:43.000000 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8217 2023-04-23 12:53:11.000000 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:15:57.000000 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:17:37.000000 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:22:26.000000 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:28:07.000000 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:28:26.000000 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:29:26.000000 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8722 2023-04-25 09:30:15.000000 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:31:04.000000 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:32:09.000000 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8667 2023-04-29 11:02:46.000000 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/train/train.py
```

### Comparing `fschat-0.2.4/LICENSE` & `fschat-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/PKG-INFO` & `fschat-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.4
+Version: 0.2.5
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastChat
-| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
 
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
@@ -25,15 +25,15 @@
 
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
-- [Vicuna Weights](#vicuna-weights)
+- [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
 - [Fine-tuning](#fine-tuning)
 
 ## Install
@@ -59,106 +59,117 @@
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
-## Vicuna Weights
+## Model Weights
+### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
-### Vicuna-7B
+#### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
     --target-model-path /output/path/to/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-13B
+#### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
     --target-model-path /output/path/to/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
-### Fastchat-T5
-This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
-```bash
-python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
-```
+#### Old weights
+See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
-### Old weights
-See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
-
-
-### Low CPU Memory Conversion
+#### Low CPU Memory Conversion
 You can try these methods to reduce the CPU RAM requirement of weight conversion.
 1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
 2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
 
+### FastChat-T5
+Simply run the line below to start chatting.
+It will automatically download the weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). 
+
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
+```
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
+#### Supported Models
+The following models are tested:
+- Vicuna, Alpaca, LLaMA, Koala
+- [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
+- [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
+- [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
+- [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
 Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 
-#### No Enough Memory or Other Platforms
+#### No Enough Memory
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
 This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
-
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
-Besides, we are actively exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome.
+In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
@@ -167,22 +178,23 @@
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
 #### Launch the model worker
 ```bash
-python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
 Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
-python3 -m fastchat.serve.test_message --model-name vicuna-13b
+python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
+You will see a short output.
 
 #### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
```

#### html2text {}

```diff
@@ -1,132 +1,144 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.4 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.5 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat | [Discord](https://discord.gg/h6kCZb72G7)
-| [Twitter](https://twitter.com/lmsysorg) | An open platform for training,
+dev License-File: LICENSE # FastChat | [Demo](https://chat.lmsys.org/) |
+[Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) |
+[Twitter](https://twitter.com/lmsysorg) | An open platform for training,
 serving, and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
 [weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
 Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
 vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+## Contents - [Install](#install) - [Model Weights](#model-weights) -
 [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
 (#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
 ```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
 repository and navigate to the FastChat folder ```bash git clone https://
 github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
 ```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
-release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
-with the LLaMA model license. You can add our delta to the original LLaMA
-weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
-weights in the huggingface format by following the instructions [here](https://
-huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
-scripts to get Vicuna weights by applying our delta. They will automatically
-download delta weights from our Hugging Face [account](https://huggingface.co/
-lmsys). **NOTE**: Weights v1.1 are only compatible with
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
 ```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
 packages accordingly. If you follow the above commands to do a fresh install,
-then you should get all the correct versions. ### Vicuna-7B This conversion
+then you should get all the correct versions. #### Vicuna-7B This conversion
 command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
 section below if you do not have enough memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
 model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
-``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
 the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
 llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
-lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
-Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
-run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
-model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
-weights_version.md](docs/weights_version.md) for all versions of weights and
-their differences. ### Low CPU Memory Conversion You can try these methods to
-reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
-to the commands above, which will split large weight files into smaller ones
-and use the disk as temporary storage. This can keep the peak memory at less
-than 16GB. 2. Create a large swap file and rely on the operating system to
-automatically utilize the disk as virtual memory. ## Inference with Command
-Line Interface (Experimental Feature: You can specify `--style rich` to enable
-rich text output and better text streaming quality for some non-ASCII content.
-This may not work properly on certain terminals.) [assets/screenshot_cli.png]
-#### Single GPU The command below requires around 28GB of GPU memory for
-Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
-section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
-GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
-on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
-does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
-around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
-Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
-acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
-turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
-path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
-M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
-If you do not have enough memory, you can enable 8-bit compression by adding `-
--load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
-to make the model easier to run on more platforms. Contributions and pull
-requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
-serve using the web UI, you need three main components: web servers that
-interface with users, model workers that host one or more models, and a
-controller to coordinate the webserver and model workers. Here are the commands
-to follow in your terminal: #### Launch the controller ```bash python3 -
-m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker ```bash python3 -
-m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
+vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
+weights and their differences. #### Low CPU Memory Conversion You can try these
+methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
+low-cpu-mem` to the commands above, which will split large weight files into
+smaller ones and use the disk as temporary storage. This can keep the peak
+memory at less than 16GB. 2. Create a large swap file and rely on the operating
+system to automatically utilize the disk as virtual memory. ### FastChat-T5
+Simply run the line below to start chatting. It will automatically download the
+weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
+v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
+v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
+can specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Supported Models The following
+models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
+(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
+12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
+baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
+[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
+[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
+stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
+chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
+memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
+Memory" section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the
+same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
+require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
+30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
+with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
+on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
+compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
+with 1 - 2 words / second. #### No Enough Memory If you do not have enough
+memory, you can enable 8-bit compression by adding `--load-8bit` to commands
+above. This can reduce memory usage by around half with slightly degraded model
+quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
+8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
+``` In addition to that, you can add `--cpu-offloading` to commands above to
+offload weights that don't fit on your GPU onto the CPU memory. This requires
+8-bit compression to be enabled and the bitsandbytes package to be installed,
+which is only available on linux operating systems. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+Here are the commands to follow in your terminal: #### Launch the controller
+```bash python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
-Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
-is the user interface that users will interact with. By following these steps,
-you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## API ### Huggingface Generation APIs See
-[fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
-API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
-api-reference/chat/create Some features/compatibilities to be implemented: -
-[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found) - [ ] the return value in
-the client SDK could be used like a dict **RESTful API Server** First, launch
-the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
-the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
-'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
-RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
-21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
-API server ```bash curl http://localhost:8000/v1/chat/completions \ -
-H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
-(e.g., `http://localhost:8000`), you can use the following code to send a
-request to the API server: ```python import os from fastchat import client
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
-client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
-"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
+output. #### Launch the Gradio web server ```bash python3 -
+m fastchat.serve.gradio_web_server ``` This is the user interface that users
+will interact with. By following these steps, you will be able to serve your
+models using the web UI. You can open your browser and chat with a model now.
+## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
+(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
+(Experimental. We will keep improving the API and SDK.) #### Chat Completion
+Reference: https://platform.openai.com/docs/api-reference/chat/create Some
+features/compatibilities to be implemented: - [ ] streaming - [ ] support of
+some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
+(e.g. model not found) - [ ] the return value in the client SDK could be used
+like a dict **RESTful API Server** First, launch the controller ```bash python3
+-m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
+path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
+m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
+```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
+application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
+variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
+localhost:8000`), you can use the following code to send a request to the API
+server: ```python import os from fastchat import client client.set_baseurl
+(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
+( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
+print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
+evaluation pipeline is based on GPT-4. This section provides a high-level
+summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.4/README.md` & `fschat-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # FastChat
-| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
 
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
@@ -12,15 +12,15 @@
 
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
-- [Vicuna Weights](#vicuna-weights)
+- [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
 - [Fine-tuning](#fine-tuning)
 
 ## Install
@@ -46,106 +46,117 @@
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
-## Vicuna Weights
+## Model Weights
+### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
-### Vicuna-7B
+#### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
     --target-model-path /output/path/to/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-13B
+#### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
     --target-model-path /output/path/to/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
-### Fastchat-T5
-This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
-```bash
-python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
-```
+#### Old weights
+See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
-### Old weights
-See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
-
-
-### Low CPU Memory Conversion
+#### Low CPU Memory Conversion
 You can try these methods to reduce the CPU RAM requirement of weight conversion.
 1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
 2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
 
+### FastChat-T5
+Simply run the line below to start chatting.
+It will automatically download the weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). 
+
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
+```
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
+#### Supported Models
+The following models are tested:
+- Vicuna, Alpaca, LLaMA, Koala
+- [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
+- [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
+- [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
+- [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
 Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 
-#### No Enough Memory or Other Platforms
+#### No Enough Memory
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
 This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
-
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
-Besides, we are actively exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome.
+In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
@@ -154,22 +165,23 @@
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
 #### Launch the model worker
 ```bash
-python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
 Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
-python3 -m fastchat.serve.test_message --model-name vicuna-13b
+python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
+You will see a short output.
 
 #### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
```

#### html2text {}

```diff
@@ -1,126 +1,138 @@
-# FastChat | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://
-twitter.com/lmsysorg) | An open platform for training, serving, and evaluating
-large language model based chatbots. ## Release
+# FastChat | [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org)
+| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/
+lmsysorg) | An open platform for training, serving, and evaluating large
+language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
 [weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
 Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
 vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+## Contents - [Install](#install) - [Model Weights](#model-weights) -
 [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
 (#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
 ```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
 repository and navigate to the FastChat folder ```bash git clone https://
 github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
 ```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
-release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
-with the LLaMA model license. You can add our delta to the original LLaMA
-weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
-weights in the huggingface format by following the instructions [here](https://
-huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
-scripts to get Vicuna weights by applying our delta. They will automatically
-download delta weights from our Hugging Face [account](https://huggingface.co/
-lmsys). **NOTE**: Weights v1.1 are only compatible with
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
 ```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
 packages accordingly. If you follow the above commands to do a fresh install,
-then you should get all the correct versions. ### Vicuna-7B This conversion
+then you should get all the correct versions. #### Vicuna-7B This conversion
 command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
 section below if you do not have enough memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
 model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
-``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
 the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
 llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
-lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
-Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
-run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
-model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
-weights_version.md](docs/weights_version.md) for all versions of weights and
-their differences. ### Low CPU Memory Conversion You can try these methods to
-reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
-to the commands above, which will split large weight files into smaller ones
-and use the disk as temporary storage. This can keep the peak memory at less
-than 16GB. 2. Create a large swap file and rely on the operating system to
-automatically utilize the disk as virtual memory. ## Inference with Command
-Line Interface (Experimental Feature: You can specify `--style rich` to enable
-rich text output and better text streaming quality for some non-ASCII content.
-This may not work properly on certain terminals.) [assets/screenshot_cli.png]
-#### Single GPU The command below requires around 28GB of GPU memory for
-Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
-section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
-GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
-on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
-does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
-around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
-Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
-acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
-turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
-path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
-M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
-If you do not have enough memory, you can enable 8-bit compression by adding `-
--load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
-to make the model easier to run on more platforms. Contributions and pull
-requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
-serve using the web UI, you need three main components: web servers that
-interface with users, model workers that host one or more models, and a
-controller to coordinate the webserver and model workers. Here are the commands
-to follow in your terminal: #### Launch the controller ```bash python3 -
-m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker ```bash python3 -
-m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
+vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
+weights and their differences. #### Low CPU Memory Conversion You can try these
+methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
+low-cpu-mem` to the commands above, which will split large weight files into
+smaller ones and use the disk as temporary storage. This can keep the peak
+memory at less than 16GB. 2. Create a large swap file and rely on the operating
+system to automatically utilize the disk as virtual memory. ### FastChat-T5
+Simply run the line below to start chatting. It will automatically download the
+weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
+v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
+v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
+can specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Supported Models The following
+models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
+(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
+12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
+baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
+[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
+[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
+stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
+chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
+memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
+Memory" section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the
+same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
+require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
+30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
+with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
+on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
+compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
+with 1 - 2 words / second. #### No Enough Memory If you do not have enough
+memory, you can enable 8-bit compression by adding `--load-8bit` to commands
+above. This can reduce memory usage by around half with slightly degraded model
+quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
+8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
+``` In addition to that, you can add `--cpu-offloading` to commands above to
+offload weights that don't fit on your GPU onto the CPU memory. This requires
+8-bit compression to be enabled and the bitsandbytes package to be installed,
+which is only available on linux operating systems. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+Here are the commands to follow in your terminal: #### Launch the controller
+```bash python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
-Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
-is the user interface that users will interact with. By following these steps,
-you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## API ### Huggingface Generation APIs See
-[fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
-API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
-api-reference/chat/create Some features/compatibilities to be implemented: -
-[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found) - [ ] the return value in
-the client SDK could be used like a dict **RESTful API Server** First, launch
-the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
-the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
-'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
-RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
-21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
-API server ```bash curl http://localhost:8000/v1/chat/completions \ -
-H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
-(e.g., `http://localhost:8000`), you can use the following code to send a
-request to the API server: ```python import os from fastchat import client
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
-client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
-"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
+output. #### Launch the Gradio web server ```bash python3 -
+m fastchat.serve.gradio_web_server ``` This is the user interface that users
+will interact with. By following these steps, you will be able to serve your
+models using the web UI. You can open your browser and chat with a model now.
+## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
+(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
+(Experimental. We will keep improving the API and SDK.) #### Chat Completion
+Reference: https://platform.openai.com/docs/api-reference/chat/create Some
+features/compatibilities to be implemented: - [ ] streaming - [ ] support of
+some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
+(e.g. model not found) - [ ] the return value in the client SDK could be used
+like a dict **RESTful API Server** First, launch the controller ```bash python3
+-m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
+path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
+m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
+```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
+application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
+variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
+localhost:8000`), you can use the following code to send a request to the API
+server: ```python import os from fastchat import client client.set_baseurl
+(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
+( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
+print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
+evaluation pipeline is based on GPT-4. This section provides a high-level
+summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.4/fastchat/client/api.py` & `fschat-0.2.5/fastchat/client/api.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/client/test_client.py` & `fschat-0.2.5/fastchat/client/test_client.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/conversation.py` & `fschat-0.2.5/fastchat/conversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,103 @@
 """
-Conversation prompt template.
-
-Now we support
-- Vicuna
-- Koala
-- OpenAssistant/oasst-sft-1-pythia-12b
-- StabilityAI/stablelm-tuned-alpha-7b
-- databricks/dolly-v2-12b
-- THUDM/chatglm-6b
-- project-baize/baize-lora-7B
-- Alpaca/LLaMa
+Conversation prompt templates.
 """
 
 import dataclasses
 from enum import auto, Enum
 from typing import List, Tuple, Any
 
 
 class SeparatorStyle(Enum):
     """Different separator style."""
 
-    SINGLE = auto()
-    TWO = auto()
-    DOLLY = auto()
-    OASST_PYTHIA = auto()
+    ADD_COLON_SINGLE = auto()
+    ADD_COLON_TWO = auto()
+    NO_COLON_SINGLE = auto()
     BAIZE = auto()
+    DOLLY = auto()
+    RWKV = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
 
     system: str
     roles: List[str]
     messages: List[List[str]]
+    # Offset of few shot examples
     offset: int
-    sep_style: SeparatorStyle = SeparatorStyle.SINGLE
-    sep: str = "###"
+    # Separator
+    sep_style: SeparatorStyle
+    sep: str
     sep2: str = None
+    # Stop criteria (the default one is EOS token)
+    stop_str: str = None
+    stop_token_ids: List[int] = None
 
     # Used for the state in the gradio servers.
     # TODO(lmzheng): refactor this
     conv_id: Any = None
     skip_next: bool = False
     model_name: str = None
 
     def get_prompt(self):
-        if self.sep_style == SeparatorStyle.SINGLE:
-            ret = self.system
+        if self.sep_style == SeparatorStyle.ADD_COLON_SINGLE:
+            ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
-                    ret += self.sep + " " + role + ": " + message
+                    ret += role + ": " + message + self.sep
                 else:
-                    ret += self.sep + " " + role + ":"
+                    ret += role + ":"
             return ret
-        elif self.sep_style == SeparatorStyle.TWO:
+        elif self.sep_style == SeparatorStyle.ADD_COLON_TWO:
             seps = [self.sep, self.sep2]
             ret = self.system + seps[0]
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ": " + message + seps[i % 2]
                 else:
                     ret += role + ":"
             return ret
+        elif self.sep_style == SeparatorStyle.NO_COLON_SINGLE:
+            ret = self.system
+            for role, message in self.messages:
+                if message:
+                    ret += role + message + self.sep
+                else:
+                    ret += role
+            return ret
+        elif self.sep_style == SeparatorStyle.BAIZE:
+            ret = self.system + "\n"
+            for role, message in self.messages:
+                if message:
+                    ret += role + message + "\n"
+                else:
+                    ret += role
+            return ret
         elif self.sep_style == SeparatorStyle.DOLLY:
             seps = [self.sep, self.sep2]
             ret = self.system
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ":\n" + message + seps[i % 2]
                     if i % 2 == 1:
                         ret += "\n\n"
                 else:
                     ret += role + ":\n"
             return ret
-        elif self.sep_style == SeparatorStyle.OASST_PYTHIA:
-            ret = self.system
-            for role, message in self.messages:
-                if message:
-                    ret += role + message + self.sep
-                else:
-                    ret += role
-            return ret
-        elif self.sep_style == SeparatorStyle.BAIZE:
+        elif self.sep_style == SeparatorStyle.RWKV:
             ret = self.system
-            for role, message in self.messages:
+            for i, (role, message) in enumerate(self.messages):
                 if message:
-                    ret += "\n" + role + message
+                    ret += role + ": " + message.replace('\r\n','\n').replace('\n\n','\n')
+                    ret += "\n\n"
                 else:
-                    ret += "\n" + role
+                    ret += role + ":"
             return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role, message):
         self.messages.append([role, message])
 
@@ -110,31 +115,32 @@
             system=self.system,
             roles=self.roles,
             messages=[[x, y] for x, y in self.messages],
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
+            stop_str=self.stop_str,
+            stop_token_ids=self.stop_token_ids,
             conv_id=self.conv_id,
             model_name=self.model_name,
         )
 
     def dict(self):
         return {
             "system": self.system,
             "roles": self.roles,
             "messages": self.messages,
             "offset": self.offset,
-            "sep": self.sep,
-            "sep2": self.sep2,
             "conv_id": self.conv_id,
             "model_name": self.model_name,
         }
 
 
+# A template with one conversation example
 conv_one_shot = Conversation(
     system="A chat between a curious human and an artificial intelligence assistant. "
     "The assistant gives helpful, detailed, and polite answers to the human's questions.",
     roles=("Human", "Assistant"),
     messages=(
         (
             "Human",
@@ -159,94 +165,114 @@
             "5. Flexibility: Renewable energy sources are often more flexible and can be adapted to different "
             "situations and needs, while non-renewable sources are more rigid and inflexible.\n"
             "6. Sustainability: Renewable energy sources are more sustainable over the long term, while "
             "non-renewable sources are not, and their depletion can lead to economic and social instability.",
         ),
     ),
     offset=2,
-    sep_style=SeparatorStyle.SINGLE,
-    sep="###",
+    sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+    sep="\n### ",
+    stop_str="###",
 )
 
 
+# Vicuna v1.1 template
 conv_vicuna_v1_1 = Conversation(
     system="A chat between a curious user and an artificial intelligence assistant. "
     "The assistant gives helpful, detailed, and polite answers to the user's questions.",
     roles=("USER", "ASSISTANT"),
     messages=(),
     offset=0,
-    sep_style=SeparatorStyle.TWO,
+    sep_style=SeparatorStyle.ADD_COLON_TWO,
     sep=" ",
     sep2="</s>",
 )
 
-
+# Koala default template
 conv_koala_v1 = Conversation(
     system="BEGINNING OF CONVERSATION:",
     roles=("USER", "GPT"),
     messages=(),
     offset=0,
-    sep_style=SeparatorStyle.TWO,
+    sep_style=SeparatorStyle.ADD_COLON_TWO,
     sep=" ",
     sep2="</s>",
 )
 
+# Dolly V2 default template
 conv_dolly = Conversation(
     system="Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
     roles=("### Instruction", "### Response"),
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.DOLLY,
     sep="\n\n",
     sep2="### End",
 )
 
+# OpenAssistant Pythia default template
 conv_oasst = Conversation(
     system="",
     roles=("<|prompter|>", "<|assistant|>"),
     messages=(),
     offset=0,
-    sep_style=SeparatorStyle.OASST_PYTHIA,
+    sep_style=SeparatorStyle.NO_COLON_SINGLE,
     sep="<|endoftext|>",
 )
 
+# StableLM Alpha default template
 conv_stablelm = Conversation(
     system="""<|SYSTEM|># StableLM Tuned (Alpha version)
 - StableLM is a helpful and harmless open-source AI language model developed by StabilityAI.
 - StableLM is excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
 - StableLM is more than just an information source, StableLM is also able to write poetry, short stories, and make jokes.
 - StableLM will refuse to participate in anything that could harm a human.
 """,
     roles=("<|USER|>", "<|ASSISTANT|>"),
     messages=(),
     offset=0,
-    sep_style=SeparatorStyle.OASST_PYTHIA,
+    sep_style=SeparatorStyle.NO_COLON_SINGLE,
     sep="",
+    stop_token_ids=[50278, 50279, 50277, 1, 0],
 )
 
+# Baize default template
 conv_baize = Conversation(
     system="The following is a conversation between a human and an AI assistant named Baize (named after a mythical creature in Chinese folklore). Baize is an open-source AI assistant developed by UCSD and Sun Yat-Sen University. The human and the AI assistant take turns chatting. Human statements start with [|Human|] and AI assistant statements start with [|AI|]. The AI assistant always provides responses in as much detail as possible, and in Markdown format. The AI assistant always declines to engage with topics, questions and instructions related to unethical, controversial, or sensitive issues. Complete the transcript in exactly that format.",
     roles=("[|Human|]", "[|AI|]"),
     messages=(
         ("[|Human|]", "Hello!"),
         ("[|AI|]", "Hi!"),
     ),
     offset=2,
     sep_style=SeparatorStyle.BAIZE,
     sep="[|Human|]",
+    stop_str="[|Human|]",
 )
 
+# RWKV-4-Raven default template
+conv_rwkv = Conversation(
+    system="",
+    roles=("Bob", "Alice"),
+    messages=(),
+    offset=0,
+    sep_style=SeparatorStyle.RWKV,
+    sep="",
+    stop_str="\n\n",
+)
 
 conv_templates = {
+    "baize": conv_baize,
     "conv_one_shot": conv_one_shot,
-    "vicuna_v1.1": conv_vicuna_v1_1,
-    "koala_v1": conv_koala_v1,
     "dolly": conv_dolly,
+    "koala_v1": conv_koala_v1,
     "oasst": conv_oasst,
-    "baize": conv_baize,
+    "stablelm": conv_stablelm,
+    "vicuna_v1.1": conv_vicuna_v1_1,
+    "rwkv": conv_rwkv
 }
 
 
 def get_default_conv_template(model_name):
     model_name = model_name.lower()
     if "vicuna" in model_name or "output" in model_name:
         return conv_vicuna_v1_1
@@ -256,41 +282,19 @@
         return conv_dolly
     elif "oasst" in model_name and "pythia" in model_name:
         return conv_oasst
     elif "baize" in model_name:
         return conv_baize
     elif "stablelm" in model_name:
         return conv_stablelm
+    elif "rwkv-4" in model_name:
+        return conv_rwkv
     return conv_one_shot
 
 
-def compute_skip_echo_len(model_name, conv, prompt):
-    model_name = model_name.lower()
-    if "chatglm" in model_name:
-        skip_echo_len = len(conv.messages[-2][1]) + 1
-    elif "dolly-v2" in model_name:
-        special_toks = ["### Instruction:", "### Response:", "### End"]
-        skip_echo_len = len(prompt)
-        for tok in special_toks:
-            skip_echo_len -= prompt.count(tok) * len(tok)
-    elif "t5" in model_name:
-         skip_echo_len = len(prompt)
-    elif "oasst" in model_name and "pythia" in model_name:
-        special_toks = ["<|prompter|>", "<|assistant|>", "<|endoftext|>"]
-        skip_echo_len = len(prompt)
-        for tok in special_toks:
-            skip_echo_len -= prompt.count(tok) * len(tok)
-    elif "stablelm" in model_name:
-        special_toks = ["<|SYSTEM|>", "<|USER|>", "<|ASSISTANT|>"]
-        skip_echo_len = len(prompt)
-        for tok in special_toks:
-            skip_echo_len -= prompt.count(tok) * len(tok)
-    elif "baize" in model_name:
-        skip_echo_len = len(prompt)
-    else:
-        skip_echo_len = len(prompt) + 1 - prompt.count("</s>") * 3
-    return skip_echo_len
-
-
 if __name__ == "__main__":
-    default_conversation = conv_templates["vicuna_v1.1"]
-    print(default_conversation.get_prompt())
+    conv = conv_templates["vicuna_v1.1"].copy()
+    conv.append_message(conv.roles[0], "Hello!")
+    conv.append_message(conv.roles[1], "Hi!")
+    conv.append_message(conv.roles[0], "How are you?")
+    conv.append_message(conv.roles[1], None)
+    print(conv.get_prompt())
```

### Comparing `fschat-0.2.4/fastchat/data/alpaca-converter.py` & `fschat-0.2.5/fastchat/data/alpaca-converter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/clean_sharegpt.py` & `fschat-0.2.5/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/hardcoded_questions.py` & `fschat-0.2.5/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/inspect.py` & `fschat-0.2.5/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/merge.py` & `fschat-0.2.5/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/optional_clean.py` & `fschat-0.2.5/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/sample.py` & `fschat-0.2.5/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/data/split_long_conversation.py` & `fschat-0.2.5/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.5/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.5/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/eval/get_model_answer.py` & `fschat-0.2.5/fastchat/eval/get_model_answer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
-from fastchat.conversation import get_default_conv_template, compute_skip_echo_len
-from fastchat.utils import disable_torch_init
+from fastchat.conversation import get_default_conv_template
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
         for line in ques_file:
@@ -35,41 +34,39 @@
         for line in ans_jsons:
             ans_file.write(json.dumps(line) + "\n")
 
 
 @ray.remote(num_gpus=1)
 @torch.inference_mode()
 def get_model_answers(model_path, model_id, question_jsons):
-    disable_torch_init()
     model_path = os.path.expanduser(model_path)
     tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
     model = AutoModelForCausalLM.from_pretrained(
-        model_path, torch_dtype=torch.float16
+        model_path, low_cpu_mem_usage=True, torch_dtype=torch.float16
     ).cuda()
 
     ans_jsons = []
     for i, line in enumerate(tqdm(question_jsons)):
         ques_json = json.loads(line)
         idx = ques_json["question_id"]
         qs = ques_json["text"]
         conv = get_default_conv_template(model_id).copy()
         conv.append_message(conv.roles[0], qs)
         conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
-        inputs = tokenizer([prompt])
+        input_ids = tokenizer([prompt]).input_ids
         output_ids = model.generate(
-            torch.as_tensor(inputs.input_ids).cuda(),
+            torch.as_tensor(input_ids).cuda(),
             do_sample=True,
             temperature=0.7,
             max_new_tokens=1024,
         )
-        outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
-        skip_echo_len = compute_skip_echo_len(model_id, conv, prompt)
+        output_ids = output_ids[0][len(input_ids[0]):]
+        outputs = tokenizer.decode(output_ids, skip_special_tokens=True).strip()
 
-        outputs = outputs[skip_echo_len:].strip()
         ans_id = shortuuid.uuid()
         ans_jsons.append(
             {
                 "question_id": idx,
                 "text": outputs,
                 "answer_id": ans_id,
                 "model_id": model_id,
```

### Comparing `fschat-0.2.4/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.5/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/model/apply_delta.py` & `fschat-0.2.5/fastchat/model/apply_delta.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,27 +64,27 @@
     except Exception as e:
         print(f"An error occurred during split_files: {e}")
         shutil.rmtree(tmp_path)
         raise
 
 
 def apply_delta_low_cpu_mem(base_model_path, target_model_path, delta_path):
-    base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
-    base_config = AutoConfig.from_pretrained(base_model_path)
+    delta_tokenizer = AutoTokenizer.from_pretrained(delta_path, use_fast=False)
+    delta_config = AutoConfig.from_pretrained(delta_path)
 
     if os.path.exists(target_model_path):
         shutil.rmtree(target_model_path)
     os.makedirs(target_model_path)
 
     split_size = 4 * GB
 
     with tempfile.TemporaryDirectory() as tmp_base_path, tempfile.TemporaryDirectory() as tmp_delta_path:
         print(f"Split files for the base model to {tmp_base_path}")
         split_files(base_model_path, tmp_base_path, split_size)
-        print(f"Split files for the delta model to {tmp_delta_path}")
+        print(f"Split files for the delta weights to {tmp_delta_path}")
         split_files(delta_path, tmp_delta_path, split_size)
 
         base_pattern = os.path.join(tmp_base_path, "pytorch_model-*.bin")
         base_files = glob.glob(base_pattern)
         delta_pattern = os.path.join(tmp_delta_path, "pytorch_model-*.bin")
         delta_files = glob.glob(delta_pattern)
         delta_state_dict = torch.load(delta_files[0])
@@ -114,38 +114,38 @@
             os.path.join(target_model_path, "pytorch_model.bin.index.json"), "w"
         ) as f:
             json.dump(
                 {"weight_map": weight_map, "metadata": {"total_size": total_size}}, f
             )
 
     print(f"Saving the target model to {target_model_path}")
-    base_tokenizer.save_pretrained(target_model_path)
-    base_config.save_pretrained(target_model_path)
+    delta_tokenizer.save_pretrained(target_model_path)
+    delta_config.save_pretrained(target_model_path)
 
 
 def apply_delta(base_model_path, target_model_path, delta_path):
+    print(f"Loading the delta weights from {delta_path}")
+    delta_tokenizer = AutoTokenizer.from_pretrained(delta_path, use_fast=False)
+    delta = AutoModelForCausalLM.from_pretrained(
+        delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
+
     print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
     )
-    base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
-
-    print(f"Loading the delta from {delta_path}")
-    delta = AutoModelForCausalLM.from_pretrained(
-        delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
-    )
 
     print("Applying the delta")
     for name, param in tqdm(base.state_dict().items(), desc="Applying delta"):
         assert name in delta.state_dict()
         param.data += delta.state_dict()[name]
 
     print(f"Saving the target model to {target_model_path}")
     base.save_pretrained(target_model_path)
-    base_tokenizer.save_pretrained(target_model_path)
+    delta_tokenizer.save_pretrained(target_model_path)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--base-model-path", type=str, required=True)
     parser.add_argument("--target-model-path", type=str, required=True)
     parser.add_argument("--delta-path", type=str, required=True)
```

### Comparing `fschat-0.2.4/fastchat/model/apply_lora.py` & `fschat-0.2.5/fastchat/model/apply_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/model/convert_fp16.py` & `fschat-0.2.5/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/model/make_delta.py` & `fschat-0.2.5/fastchat/model/make_delta.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,30 @@
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
     )
 
     print(f"Loading the target model from {target_model_path}")
     target = AutoModelForCausalLM.from_pretrained(
         target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
     )
+    target_tokenizer = AutoTokenizer.from_pretrained(
+        target_model_path, use_fast=False
+    )
 
     print("Calculating the delta")
     for name, param in tqdm(target.state_dict().items(), desc="Calculating delta"):
         assert name in base.state_dict()
         param.data -= base.state_dict()[name]
 
     print(f"Saving the delta to {delta_path}")
     if args.hub_repo_id:
         kwargs = {"push_to_hub": True, "repo_id": args.hub_repo_id}
     else:
         kwargs = {}
     target.save_pretrained(delta_path, **kwargs)
+    target_tokenizer.save_pretrained(delta_path, **kwargs)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--base-model-path", type=str, required=True)
     parser.add_argument("--target-model-path", type=str, required=True)
     parser.add_argument("--delta-path", type=str, required=True)
```

### Comparing `fschat-0.2.4/fastchat/protocol/chat_completion.py` & `fschat-0.2.5/fastchat/protocol/chat_completion.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/api.py` & `fschat-0.2.5/fastchat/serve/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from fastchat.protocol.chat_completion import (
     ChatCompletionRequest,
     ChatCompletionResponse,
     ChatMessage,
     ChatCompletionResponseChoice,
 )
 from fastchat.conversation import get_default_conv_template, SeparatorStyle
-from fastchat.serve.inference import compute_skip_echo_len
 
 logger = logging.getLogger(__name__)
 
 
 class AppSettings(BaseSettings):
     # The address of the model controller.
     FASTCHAT_CONTROLLER_URL: str = "http://localhost:21001"
@@ -51,27 +50,28 @@
     models.sort()
     return {"data": [{"id": m} for m in models], "object": "list"}
 
 
 @app.post("/v1/chat/completions")
 async def create_chat_completion(request: ChatCompletionRequest):
     """Creates a completion for the chat message"""
-    payload, skip_echo_len = generate_payload(
+    gen_params = get_gen_params(
         request.model,
         request.messages,
         temperature=request.temperature,
         max_tokens=request.max_tokens,
+        echo=False,
         stop=request.stop,
     )
 
     choices = []
     # TODO: batch the requests. maybe not necessary if using CacheFlow worker
     chat_completions = []
     for i in range(request.n):
-        content = asyncio.create_task(chat_completion(request.model, payload, skip_echo_len))
+        content = asyncio.create_task(chat_completion(request.model, gen_params))
         chat_completions.append(content)
 
     for i, content_task in enumerate(chat_completions):
         content = await content_task
         choices.append(
             ChatCompletionResponseChoice(
                 index=i,
@@ -86,31 +86,27 @@
     #     "prompt_tokens": 9,
     #     "completion_tokens": 12,
     #     "total_tokens": 21
     # }
     return ChatCompletionResponse(choices=choices)
 
 
-def generate_payload(
+def get_gen_params(
     model_name: str,
     messages: List[Dict[str, str]],
     *,
     temperature: float,
     max_tokens: int,
+    echo: bool,
     stop: Union[str, None],
 ):
     is_chatglm = "chatglm" in model_name.lower()
     # TODO(suquark): The template is currently a reference. Here we have to make a copy.
-    # We use create a template factory to avoid this.
     conv = get_default_conv_template(model_name).copy()
 
-    # TODO(suquark): Conv.messages should be a list. But it is a tuple now.
-    #  We should change it to a list.
-    conv.messages = list(conv.messages)
-
     for message in messages:
         msg_role = message["role"]
         if msg_role == "system":
             conv.system = message["content"]
         elif msg_role == "user":
             conv.append_message(conv.roles[0], message["content"])
         elif msg_role == "assistant":
@@ -121,36 +117,32 @@
     # Add a blank message for the assistant.
     conv.append_message(conv.roles[1], None)
 
     if is_chatglm:
         prompt = conv.messages[conv.offset :]
     else:
         prompt = conv.get_prompt()
-    skip_echo_len = compute_skip_echo_len(model_name, conv, prompt)
-
-    if stop is None:
-        stop = conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2
 
-    # TODO(suquark): We should get the default `max_new_tokens`` from the model.
     if max_tokens is None:
         max_tokens = 512
 
-    payload = {
+    gen_params = {
         "model": model_name,
         "prompt": prompt,
         "temperature": temperature,
         "max_new_tokens": max_tokens,
-        "stop": stop,
+        "echo": echo,
+        "stop": conv.stop_str,
+        "stop_token_ids": conv.stop_token_ids,
     }
-
-    logger.debug(f"==== request ====\n{payload}")
-    return payload, skip_echo_len
+    logger.debug(f"==== request ====\n{gen_params}")
+    return gen_params
 
 
-async def chat_completion(model_name: str, payload: Dict[str, Any], skip_echo_len: int):
+async def chat_completion(model_name: str, gen_params: Dict[str, Any]):
     controller_url = app_settings.FASTCHAT_CONTROLLER_URL
     async with httpx.AsyncClient() as client:
         ret = await client.post(
             controller_url + "/get_worker_address", json={"model": model_name}
         )
         worker_addr = ret.json()["address"]
         # No available worker
@@ -161,25 +153,25 @@
 
         output = ""
         delimiter = b"\0"
         async with client.stream(
             "POST",
             worker_addr + "/worker_generate_stream",
             headers=headers,
-            json=payload,
+            json=gen_params,
             timeout=20,
         ) as response:
             content = await response.aread()
 
         for chunk in content.split(delimiter):
             if not chunk:
                 continue
             data = json.loads(chunk.decode())
             if data["error_code"] == 0:
-                output = data["text"][skip_echo_len:].strip()
+                output = data["text"].strip()
 
         return output
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="FastChat ChatGPT-compatible Restful API server."
```

### Comparing `fschat-0.2.4/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.5/fastchat/serve/cacheflow_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,16 @@
 
     async def generate_stream(self, params):
         tokenizer = self.tokenizer
         context = params["prompt"]
         temperature = float(params.get("temperature", 1.0))
         max_new_tokens = min(int(params.get("max_new_tokens", 256)), 1024)
         stop_str = params.get("stop", None)
+        echo = params.get("echo", True)
+        params["stop_token_ids"] = params.get("stop_token_ids", None) or []
 
         input_ids = tokenizer(context).input_ids
         max_src_len = self.context_len - max_new_tokens - 8
         input_ids = input_ids[-max_src_len:]
 
         # make sampling params in cacheflow
         sampling_params = SamplingParams.from_dict(params)
@@ -225,14 +227,16 @@
             except:
                 pass
             group_event.clear()
             seq_group = self.running_seq_groups[group_id]
             all_outputs = []
             for seq in seq_group.seqs:
                 token_ids = seq.get_token_ids()
+                if not echo:
+                    token_ids = token_ids[len(input_ids):]
                 output = self.tokenizer.decode(token_ids, skip_special_tokens=True)
                 if stop_str is not None:
                     if output.endswith(stop_str):
                         output = output[: -len(stop_str)]
                 all_outputs.append(output)
             assert len(seq_group.seqs) == 1
             ret = {
```

### Comparing `fschat-0.2.4/fastchat/serve/cli.py` & `fschat-0.2.5/fastchat/serve/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,28 @@
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.live import Live
 
-from fastchat.serve.inference import chat_loop, ChatIO
+from fastchat.serve.inference import chat_loop, ChatIO, add_model_args
 
 
 class SimpleChatIO(ChatIO):
     def prompt_for_input(self, role) -> str:
         return input(f"{role}: ")
 
     def prompt_for_output(self, role: str):
         print(f"{role}: ", end="", flush=True)
 
-    def stream_output(self, output_stream, skip_echo_len: int):
+    def stream_output(self, output_stream):
         pre = 0
         for outputs in output_stream:
-            outputs = outputs[skip_echo_len:].strip()
-            outputs = outputs.split(" ")
+            outputs = outputs.strip().split(" ")
             now = len(outputs) - 1
             if now > pre:
                 print(" ".join(outputs[pre:now]), end=" ", flush=True)
                 pre = now
         print(" ".join(outputs[pre:]), flush=True)
         return " ".join(outputs)
 
@@ -58,107 +57,85 @@
         )
         self._console.print()
         return prompt_input
 
     def prompt_for_output(self, role: str):
         self._console.print(f"[bold]{role}:")
 
-    def stream_output(self, output_stream, skip_echo_len: int):
+    def stream_output(self, output_stream):
         """Stream output from a role."""
         # TODO(suquark): the console flickers when there is a code block
         #  above it. We need to cut off "live" when a code block is done.
 
         # Create a Live context for updating the console output
         with Live(console=self._console, refresh_per_second=4) as live:
             # Read lines from the stream
             for outputs in output_stream:
-                accumulated_text = outputs[skip_echo_len:]
-                if not accumulated_text:
+                if not outputs:
                     continue
                 # Render the accumulated text as Markdown
                 # NOTE: this is a workaround for the rendering "unstandard markdown"
                 #  in rich. The chatbots output treat "\n" as a new line for
                 #  better compatibility with real-world text. However, rendering
                 #  in markdown would break the format. It is because standard markdown
                 #  treat a single "\n" in normal text as a space.
                 #  Our workaround is adding two spaces at the end of each line.
                 #  This is not a perfect solution, as it would
                 #  introduce trailing spaces (only) in code block, but it works well
                 #  especially for console output, because in general the console does not
                 #  care about trailing spaces.
                 lines = []
-                for line in accumulated_text.splitlines():
+                for line in outputs.splitlines():
                     lines.append(line)
                     if line.startswith("```"):
                         # Code block marker - do not add trailing spaces, as it would
                         #  break the syntax highlighting
                         lines.append("\n")
                     else:
                         lines.append("  \n")
                 markdown = Markdown("".join(lines))
                 # Update the Live console output
                 live.update(markdown)
         self._console.print()
-        return outputs[skip_echo_len:]
+        return outputs
 
 
 def main(args):
     if args.gpus:
-        if args.num_gpus and len(args.gpus.split(",")) < int(args.num_gpus):
+        if len(args.gpus.split(",")) < args.num_gpus:
             raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
+
     if args.style == "simple":
         chatio = SimpleChatIO()
     elif args.style == "rich":
         chatio = RichChatIO()
     else:
         raise ValueError(f"Invalid style for console: {args.style}")
     try:
         chat_loop(
             args.model_path,
             args.device,
             args.num_gpus,
             args.max_gpu_memory,
             args.load_8bit,
+            args.cpu_offloading,
             args.conv_template,
             args.temperature,
             args.max_new_tokens,
             chatio,
             args.debug,
         )
     except KeyboardInterrupt:
         print("exit...")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--model-path",
-        type=str,
-        default="facebook/opt-350m",
-        help="The path to the weights",
-    )
-    parser.add_argument(
-        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
-    )
-    parser.add_argument(
-        "--gpus",
-        type=str,
-        default=None,
-        help="A single GPU like 1 or multiple GPUs like 0,2"
-    )
-    parser.add_argument("--num-gpus", type=str, default="1")
-    parser.add_argument(
-        "--max-gpu-memory",
-        type=str,
-        help="The maximum memory per gpu. Use a string like '13Gib'",
-    )
-    parser.add_argument(
-        "--load-8bit", action="store_true", help="Use 8-bit quantization."
-    )
+    add_model_args(parser)
     parser.add_argument(
         "--conv-template", type=str, default=None, help="Conversation prompt template."
     )
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument(
         "--style",
```

### Comparing `fschat-0.2.4/fastchat/serve/compression.py` & `fschat-0.2.5/fastchat/serve/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/controller.py` & `fschat-0.2.5/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/gradio_block_arena_anony.py` & `fschat-0.2.5/fastchat/serve/gradio_block_arena_anony.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     http_bot,
     get_conv_log_filename,
     no_change_btn,
     enable_btn,
     disable_btn,
+    model_description_md,
+    learn_more_md,
 )
 
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 num_models = 2
 enable_moderation = False
@@ -66,19 +68,19 @@
             "ip": request.client.host,
         }
         fout.write(json.dumps(data) + "\n")
 
     if ":" not in model_selectors[0]:
         for i in range(15):
             names = ("### Model A: " + states[0].model_name, "### Model B: " + states[1].model_name)
-            yield names + ("",) + (disable_btn,) * 3
+            yield names + ("",) + (disable_btn,) * 4
             time.sleep(0.2)
     else:
         names = ("### Model A: " + states[0].model_name, "### Model B: " + states[1].model_name)
-        yield names + ("",) + (disable_btn,) * 3
+        yield names + ("",) + (disable_btn,) * 4
 
 
 def leftvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
     logger.info(f"leftvote (anony). ip: {request.client.host}")
     for x in vote_last_response(
@@ -103,26 +105,36 @@
     logger.info(f"tievote (anony). ip: {request.client.host}")
     for x in vote_last_response(
         [state0, state1], "tievote", [model_selector0, model_selector1], request
     ):
         yield x
 
 
+def bothbad_vote_last_response(
+    state0, state1, model_selector0, model_selector1, request: gr.Request
+):
+    logger.info(f"bothbad_vote (anony). ip: {request.client.host}")
+    for x in vote_last_response(
+        [state0, state1], "bothbad_vote", [model_selector0, model_selector1], request
+    ):
+        yield x
+
+
 def regenerate(state0, state1, request: gr.Request):
     logger.info(f"regenerate (anony). ip: {request.client.host}")
     states = [state0, state1]
     for i in range(num_models):
         states[i].messages[-1][-1] = None
         states[i].skip_next = False
-    return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 5
+    return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 6
 
 
 def clear_history(request: gr.Request):
     logger.info(f"clear_history (anony). ip: {request.client.host}")
-    return [None] * num_models + [None] * num_models + anony_names + [""] + [disable_btn] * 5
+    return [None] * num_models + [None] * num_models + anony_names + [""] + [disable_btn] * 6
 
 
 def share_click(state0, state1, model_selector0, model_selector1,
                 request: gr.Request):
     logger.info(f"share (anony). ip: {request.client.host}")
     if state0 is not None and state1 is not None:
         vote_last_response(
@@ -132,15 +144,15 @@
 
 def add_text(state0, state1, text, request: gr.Request):
     logger.info(f"add_text (anony). ip: {request.client.host}. len: {len(text)}")
     states = [state0, state1]
 
     if states[0] is None:
         assert states[1] is None
-        weights = ([8, 4, 2, 1] + [1] * 32)[:len(models)]
+        weights = ([1, 1, 1, 1] + [1] * 32)[:len(models)]
         if len(models) > 1:
             weights = weights / np.sum(weights)
             model_left, model_right = np.random.choice(
                 models, size=(2,), p=weights, replace=False)
         else:
             model_left = model_right = models[0]
 
@@ -157,15 +169,15 @@
         return (
             states
             + [x.to_gradio_chatbot() for x in states]
             + [""]
             + [
                 no_change_btn,
             ]
-            * 5
+            * 6
         )
 
     if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
             logger.info(f"violate moderation (anony). ip: {request.client.host}. text: {text}")
             for i in range(num_models):
@@ -173,15 +185,15 @@
             return (
                 states
                 + [x.to_gradio_chatbot() for x in states]
                 + [moderation_msg]
                 + [
                     no_change_btn,
                 ]
-                * 5
+                * 6
             )
 
     text = text[:1536]  # Hard cut-off
     for i in range(num_models):
         states[i].append_message(states[i].roles[0], text)
         states[i].append_message(states[i].roles[1], None)
         states[i].skip_next = False
@@ -189,28 +201,35 @@
     return (
         states
         + [x.to_gradio_chatbot() for x in states]
         + [""]
         + [
             disable_btn,
         ]
-        * 5
+        * 6
     )
 
 
 def http_bot_all(
     state0,
     state1,
     model_selector0,
     model_selector1,
     temperature,
     max_new_tokens,
     request: gr.Request,
 ):
     logger.info(f"http_bot_all (anony). ip: {request.client.host}")
+
+    if state0.skip_next:
+        # This generate call is skipped due to invalid inputs
+        yield (state0, state1, state0.to_gradio_chatbot(),
+            state1.to_gradio_chatbot()) + (no_change_btn,) * 6
+        return
+
     states = [state0, state1]
     model_selector = [state0.model_name, state1.model_name]
     gen = []
     for i in range(num_models):
         gen.append(
             http_bot(states[i], model_selector[i], temperature, max_new_tokens, request)
         )
@@ -218,65 +237,53 @@
     chatbots = [None] * num_models
     while True:
         stop = True
         for i in range(num_models):
             try:
                 ret = next(gen[i])
                 states[i], chatbots[i] = ret[0], ret[1]
-                buttons = ret[2:]
                 stop = False
             except StopIteration:
                 pass
-        yield states + chatbots + list(buttons)
+        yield states + chatbots + [disable_btn] * 6
         if stop:
             break
 
     for i in range(10):
         if i % 2 == 0:
-            yield states + chatbots + [disable_btn] * 3 + list(buttons)[3:]
+            yield states + chatbots + [disable_btn] * 4 + [enable_btn] * 2
         else:
-            yield states + chatbots + list(buttons)
+            yield states + chatbots + [enable_btn] * 6
         time.sleep(0.2)
 
 
 def build_side_by_side_ui_anony(models):
-    notice_markdown = """
+    notice_markdown = ("""
 # ⚔️  Chatbot Arena ⚔️ 
 Rules:
 - Chat with two anonymous models side-by-side and vote for which one is better!
 - The names of the models will be revealed after your vote.
 - You can continue chating and voting or click "Clear history" to start a new round.
 - A leaderboard will be available soon.
 - [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
 The demo works better on desktop devices with a wide screen.
 
 ### The participated models
-| | |
-| ---- | ---- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
-| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
-"""
-
-    learn_more_markdown = """
-### License
-The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
-"""
+""" + model_description_md)
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
     notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
-    with gr.Box(elem_id="share-region"):
+    with gr.Box(elem_id="share-region-anony"):
         with gr.Row():
             for i in range(num_models):
                 with gr.Column():
                     model_selectors[i] = gr.Markdown(anony_names[i])
 
         with gr.Row():
             for i in range(num_models):
@@ -284,16 +291,17 @@
                 with gr.Column():
                     chatbots[i] = grChatbot(label=label, elem_id=f"chatbot{i}",
                         visible=False).style(height=550)
 
         with gr.Box() as button_row:
             with gr.Row():
                 leftvote_btn = gr.Button(value="👈  A is better", interactive=False)
-                tie_btn = gr.Button(value="🤝  Tie", interactive=False)
                 rightvote_btn = gr.Button(value="👉  B is better", interactive=False)
+                tie_btn = gr.Button(value="🤝  Tie", interactive=False)
+                bothbad_btn = gr.Button(value="👎  Both are bad", interactive=False)
 
     with gr.Row():
         with gr.Column(scale=20):
             textbox = gr.Textbox(
                 show_label=False,
                 placeholder="Enter text and press ENTER",
                 visible=False,
@@ -320,46 +328,52 @@
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
         )
 
-    gr.Markdown(learn_more_markdown)
+    gr.Markdown(learn_more_md)
 
     # Register listeners
-    btn_list = [leftvote_btn, rightvote_btn, tie_btn, regenerate_btn, clear_btn]
+    btn_list = [leftvote_btn, rightvote_btn, tie_btn, bothbad_btn,
+                regenerate_btn, clear_btn]
     leftvote_btn.click(
         leftvote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     rightvote_btn.click(
         rightvote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     tie_btn.click(
         tievote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+    )
+    bothbad_btn.click(
+        bothbad_vote_last_response,
+        states + model_selectors,
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     regenerate_btn.click(
         regenerate, states, states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
         states + model_selectors + [temperature, max_output_tokens],
         states + chatbots + btn_list,
     )
     clear_btn.click(clear_history, None, states + chatbots + model_selectors + [
         textbox] + btn_list)
 
     share_js="""
 function (a, b, c, d) {
-    const captureElement = document.querySelector('#share-region');
+    const captureElement = document.querySelector('#share-region-anony');
     html2canvas(captureElement)
         .then(canvas => {
             canvas.style.display = 'none'
             document.body.appendChild(canvas)
             return canvas
         })
         .then(canvas => {
```

### Comparing `fschat-0.2.4/fastchat/serve/gradio_block_arena_named.py` & `fschat-0.2.5/fastchat/serve/gradio_block_arena_named.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     http_bot,
     get_conv_log_filename,
     no_change_btn,
     enable_btn,
     disable_btn,
+    model_description_md,
+    learn_more_md,
 )
 
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 num_models = 2
 enable_moderation = False
@@ -32,15 +34,15 @@
 
 
 def load_demo_side_by_side_named(models, url_params):
     states = (None,) * num_models
 
     model_left = models[0]
     if len(models) > 1:
-        weights = ([8, 4, 2, 1] + [1] * 32)[:len(models) - 1]
+        weights = ([1, 1, 1, 1] + [1] * 32)[:len(models) - 1]
         weights = weights / np.sum(weights)
         model_right = np.random.choice(models[1:], p=weights)
     else:
         model_right = model_left
 
     selector_updates = (
         gr.Dropdown.update(model_left, visible=True),
@@ -76,49 +78,59 @@
 def leftvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
     logger.info(f"leftvote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "leftvote", [model_selector0, model_selector1], request
     )
-    return ("",) + (disable_btn,) * 3
+    return ("",) + (disable_btn,) * 4
 
 
 def rightvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
     logger.info(f"rightvote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "rightvote", [model_selector0, model_selector1], request
     )
-    return ("",) + (disable_btn,) * 3
+    return ("",) + (disable_btn,) * 4
 
 
 def tievote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
     logger.info(f"tievote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "tievote", [model_selector0, model_selector1], request
     )
-    return ("",) + (disable_btn,) * 3
+    return ("",) + (disable_btn,) * 4
+
+
+def bothbad_vote_last_response(
+    state0, state1, model_selector0, model_selector1, request: gr.Request
+):
+    logger.info(f"bothbad_vote (named). ip: {request.client.host}")
+    vote_last_response(
+        [state0, state1], "bothbad_vote", [model_selector0, model_selector1], request
+    )
+    return ("",) + (disable_btn,) * 4
 
 
 def regenerate(state0, state1, request: gr.Request):
     logger.info(f"regenerate (named). ip: {request.client.host}")
     states = [state0, state1]
     for i in range(num_models):
         states[i].messages[-1][-1] = None
         states[i].skip_next = False
-    return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 5
+    return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 6
 
 
 def clear_history(request: gr.Request):
     logger.info(f"clear_history (named). ip: {request.client.host}")
-    return [None] * num_models + [None] * num_models + [""] + [disable_btn] * 5
+    return [None] * num_models + [None] * num_models + [""] + [disable_btn] * 6
 
 
 def share_click(state0, state1, model_selector0, model_selector1,
                 request: gr.Request):
     logger.info(f"share (named). ip: {request.client.host}")
     if state0 is not None and state1 is not None:
         vote_last_response(
@@ -140,15 +152,15 @@
         return (
             states
             + [x.to_gradio_chatbot() for x in states]
             + [""]
             + [
                 no_change_btn,
             ]
-            * 5
+            * 6
         )
 
     if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
             logger.info(f"violate moderation (named). ip: {request.client.host}. text: {text}")
             for i in range(num_models):
@@ -156,15 +168,15 @@
             return (
                 states
                 + [x.to_gradio_chatbot() for x in states]
                 + [moderation_msg]
                 + [
                     no_change_btn,
                 ]
-                * 5
+                * 6
             )
 
     text = text[:1536]  # Hard cut-off
     for i in range(num_models):
         states[i].append_message(states[i].roles[0], text)
         states[i].append_message(states[i].roles[1], None)
         states[i].skip_next = False
@@ -172,28 +184,35 @@
     return (
         states
         + [x.to_gradio_chatbot() for x in states]
         + [""]
         + [
             disable_btn,
         ]
-        * 5
+        * 6
     )
 
 
 def http_bot_all(
     state0,
     state1,
     model_selector0,
     model_selector1,
     temperature,
     max_new_tokens,
     request: gr.Request,
 ):
     logger.info(f"http_bot_all (named). ip: {request.client.host}")
+
+    if state0.skip_next:
+        # This generate call is skipped due to invalid inputs
+        yield (state0, state1, state0.to_gradio_chatbot(),
+            state1.to_gradio_chatbot()) + (no_change_btn,) * 6
+        return
+
     states = [state0, state1]
     model_selector = [model_selector0, model_selector1]
     gen = []
     for i in range(num_models):
         gen.append(
             http_bot(states[i], model_selector[i], temperature, max_new_tokens, request)
         )
@@ -201,65 +220,53 @@
     chatbots = [None] * num_models
     while True:
         stop = True
         for i in range(num_models):
             try:
                 ret = next(gen[i])
                 states[i], chatbots[i] = ret[0], ret[1]
-                buttons = ret[2:]
                 stop = False
             except StopIteration:
                 pass
-        yield states + chatbots + list(buttons)
+        yield states + chatbots + [disable_btn] * 6
         if stop:
             break
 
     for i in range(10):
         if i % 2 == 0:
-            yield states + chatbots + [disable_btn] * 3 + list(buttons)[3:]
+            yield states + chatbots + [disable_btn] * 4 + [enable_btn] * 2
         else:
-            yield states + chatbots + list(buttons)
+            yield states + chatbots + [enable_btn] * 6
         time.sleep(0.2)
 
 
 def build_side_by_side_ui_named(models):
-    notice_markdown = """
+    notice_markdown = ("""
 # ⚔️  Chatbot Arena ⚔️ 
 Rules:
 - Chat with two models side-by-side and vote for which one is better!
 - You pick the models you want to chat with.
 - You can continue chating and voting or click "Clear history" to start a new round.
 - A leaderboard will be available soon.
 - [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
 The demo works better on desktop devices with a wide screen.
 
 ### Choose two models to chat with
-| | |
-| ---- | ---- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
-| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
-"""
-
-    learn_more_markdown = """
-### License
-The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
-"""
+""" + model_description_md)
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
     notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
-    with gr.Box(elem_id="share-region"):
+    with gr.Box(elem_id="share-region-named"):
         with gr.Row():
             for i in range(num_models):
                 with gr.Column():
                     model_selectors[i] = gr.Dropdown(
                         choices=models,
                         value=models[i] if len(models) > i else "",
                         interactive=True,
@@ -272,16 +279,17 @@
                 with gr.Column():
                     chatbots[i] = grChatbot(label=label, elem_id=f"chatbot{i}",
                         visible=False).style(height=550)
 
         with gr.Box() as button_row:
             with gr.Row():
                 leftvote_btn = gr.Button(value="👈  A is better", interactive=False)
-                tie_btn = gr.Button(value="🤝  Tie", interactive=False)
                 rightvote_btn = gr.Button(value="👉  B is better", interactive=False)
+                tie_btn = gr.Button(value="🤝  Tie", interactive=False)
+                bothbad_btn = gr.Button(value="👎  Both are bad", interactive=False)
 
     with gr.Row():
         with gr.Column(scale=20):
             textbox = gr.Textbox(
                 show_label=False,
                 placeholder="Enter text and press ENTER",
                 visible=False,
@@ -308,45 +316,51 @@
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
         )
 
-    gr.Markdown(learn_more_markdown)
+    gr.Markdown(learn_more_md)
 
     # Register listeners
-    btn_list = [leftvote_btn, rightvote_btn, tie_btn, regenerate_btn, clear_btn]
+    btn_list = [leftvote_btn, rightvote_btn, tie_btn, bothbad_btn,
+                regenerate_btn, clear_btn]
     leftvote_btn.click(
         leftvote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     rightvote_btn.click(
         rightvote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     tie_btn.click(
         tievote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+    )
+    bothbad_btn.click(
+        bothbad_vote_last_response,
+        states + model_selectors,
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     regenerate_btn.click(
         regenerate, states, states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
         states + model_selectors + [temperature, max_output_tokens],
         states + chatbots + btn_list,
     )
     clear_btn.click(clear_history, None, states + chatbots + [textbox] + btn_list)
 
     share_js="""
 function (a, b, c, d) {
-    const captureElement = document.querySelector('#share-region');
+    const captureElement = document.querySelector('#share-region-named');
     html2canvas(captureElement)
         .then(canvas => {
             canvas.style.display = 'none'
             document.body.appendChild(canvas)
             return canvas
         })
         .then(canvas => {
```

### Comparing `fschat-0.2.4/fastchat/serve/gradio_css.py` & `fschat-0.2.5/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/gradio_patch.py` & `fschat-0.2.5/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/gradio_web_server.py` & `fschat-0.2.5/fastchat/serve/gradio_web_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import uuid
 
 import gradio as gr
 import requests
 
 from fastchat.conversation import (
     get_default_conv_template,
-    compute_skip_echo_len,
     SeparatorStyle,
 )
 from fastchat.constants import LOGDIR
 from fastchat.utils import (
     build_logger,
     server_error_msg,
     violates_moderation,
@@ -36,20 +35,38 @@
 controller_url = None
 enable_moderation = False
 
 
 priority = {
     "vicuna-13b": "aaa",
     "koala-13b": "aab",
-    "oasst-pythia-12b": "aac",
-    "dolly-v2-12b": "aad",
+    "fastchat-t5-3b": "aac",
+    "oasst-pythia-12b": "aad",
     "chatglm-6b": "aae",
     "stablelm-tuned-alpha-7b": "aaf",
+    "alpaca-13b": "aag",
+    "llama-13b": "aah",
+    "dolly-v2-12b": "aai",
 }
 
+model_description_md = """
+| | |
+| ---- | ---- |
+| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
+| [FastChat-T5](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0): a chat assistant fine-tuned from FLAN-T5 by LMSYS. | [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. |
+| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
+| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
+| [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. | |
+"""
+
+learn_more_md = """
+### License
+The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
+"""
+
 
 def set_global_vars(controller_url_, enable_moderation_):
     global controller_url, enable_moderation
     controller_url = controller_url_
     enable_moderation = enable_moderation_
 
 
@@ -221,47 +238,49 @@
             disable_btn,
             enable_btn,
             enable_btn,
         )
         return
 
     # Construct prompt
+    conv = state
     if "chatglm" in model_name:
-        prompt = state.messages[state.offset :]
+        prompt = conv.messages[conv.offset :]
     else:
-        prompt = state.get_prompt()
-    skip_echo_len = compute_skip_echo_len(model_name, state, prompt)
+        prompt = conv.get_prompt()
 
     # Make requests
-    pload = {
+    gen_params = {
         "model": model_name,
         "prompt": prompt,
         "temperature": temperature,
         "max_new_tokens": max_new_tokens,
-        "stop": state.sep if state.sep_style == SeparatorStyle.SINGLE else None,
+        "stop": conv.stop_str,
+        "stop_token_ids": conv.stop_token_ids,
+        "echo": False,
     }
-    logger.info(f"==== request ====\n{pload}")
+    logger.info(f"==== request ====\n{gen_params}")
 
     state.messages[-1][-1] = "▌"
     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
 
     try:
         # Stream output
         response = requests.post(
             worker_addr + "/worker_generate_stream",
             headers=headers,
-            json=pload,
+            json=gen_params,
             stream=True,
             timeout=20,
         )
         for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
             if chunk:
                 data = json.loads(chunk.decode())
                 if data["error_code"] == 0:
-                    output = data["text"][skip_echo_len:].strip()
+                    output = data["text"].strip()
                     output = post_process_code(output)
                     state.messages[-1][-1] = output + "▌"
                     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
                 else:
                     output = data["text"] + f" (error_code: {data['error_code']})"
                     state.messages[-1][-1] = output
                     yield (state, state.to_gradio_chatbot()) + (
@@ -321,36 +340,25 @@
     display: none;
 }
 """
 )
 
 
 def build_single_model_ui(models):
-    notice_markdown = """
+    notice_markdown = ("""
 # 🏔️ Chat with Open Large Language Models
 - Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[Evaluation]](https://vicuna.lmsys.org/eval/)
 - Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/)
 - [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
 
 ### Choose a model to chat with
-| | |
-| ---- | ---- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
-| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
-"""
-
-    learn_more_markdown = """
-### License
-The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
-"""
+""" + model_description_md)
 
     state = gr.State()
     notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
     with gr.Row(elem_id="model_selector_row"):
         model_selector = gr.Dropdown(
             choices=models,
@@ -392,15 +400,15 @@
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
         )
 
-    gr.Markdown(learn_more_markdown)
+    gr.Markdown(learn_more_md)
 
     # Register listeners
     btn_list = [upvote_btn, downvote_btn, flag_btn, regenerate_btn, clear_btn]
     upvote_btn.click(
         upvote_last_response,
         [state, model_selector],
         [textbox, upvote_btn, downvote_btn, flag_btn],
```

### Comparing `fschat-0.2.4/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.5/fastchat/serve/gradio_web_server_multi.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/huggingface_api.py` & `fschat-0.2.5/fastchat/serve/huggingface_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,71 +4,58 @@
 """
 import argparse
 import json
 
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
-from fastchat.conversation import get_default_conv_template, compute_skip_echo_len
-from fastchat.serve.inference import load_model
+from fastchat.conversation import get_default_conv_template
+from fastchat.serve.inference import load_model, add_model_args
 
 
 @torch.inference_mode()
 def main(args):
     model, tokenizer = load_model(
         args.model_path,
         args.device,
         args.num_gpus,
         args.max_gpu_memory,
         args.load_8bit,
+        args.cpu_offloading,
         debug=args.debug,
     )
 
     msg = args.message
 
     conv = get_default_conv_template(args.model_path).copy()
     conv.append_message(conv.roles[0], msg)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
-    inputs = tokenizer([prompt])
+    input_ids = tokenizer([prompt]).input_ids
     output_ids = model.generate(
-        torch.as_tensor(inputs.input_ids).cuda(),
+        torch.as_tensor(input_ids).cuda(),
         do_sample=True,
         temperature=0.7,
         max_new_tokens=1024,
     )
-    outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
-    skip_echo_len = compute_skip_echo_len(args.model_path, conv, prompt)
-    outputs = outputs[skip_echo_len:]
+    if model.config.is_encoder_decoder:
+        output_ids = output_ids[0]
+    else:
+        output_ids = output_ids[0][len(input_ids[0]):]
+    outputs = tokenizer.decode(output_ids, skip_special_tokens=True,
+                               spaces_between_special_tokens=False)
 
     print(f"{conv.roles[0]}: {msg}")
     print(f"{conv.roles[1]}: {outputs}")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--model-path",
-        type=str,
-        default="facebook/opt-350m",
-        help="The path to the weights",
-    )
-    parser.add_argument(
-        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
-    )
-    parser.add_argument("--num-gpus", type=str, default="1")
-    parser.add_argument(
-        "--max-gpu-memory",
-        type=str,
-        help="The maximum memory per gpu. Use a string like '13Gib'",
-    )
-    parser.add_argument(
-        "--load-8bit", action="store_true", help="Use 8-bit quantization."
-    )
+    add_model_args(parser)
     parser.add_argument(
         "--conv-template", type=str, default=None, help="Conversation prompt template."
     )
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--debug", action="store_true")
     parser.add_argument("--message", type=str, default="Hello! Who are you?")
```

### Comparing `fschat-0.2.4/fastchat/serve/inference.py` & `fschat-0.2.5/fastchat/serve/inference.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 """Inference for FastChat models."""
 import abc
+import gc
+import math
 from typing import Optional
+import sys
 import warnings
 
+import psutil
 import torch
-
-try:
-    from transformers import (
-        AutoTokenizer,
-        AutoModelForCausalLM,
-        LlamaTokenizer,
-        LlamaForCausalLM,
-        AutoModel,
-        AutoModelForSeq2SeqLM,
-        T5Tokenizer,
-        AutoConfig,
-    )
-except ImportError:
-    from transformers import (
-        AutoTokenizer,
-        AutoModelForCausalLM,
-        LLaMATokenizer,
-        LLamaForCausalLM,
-        AutoModel,
-        AutoModelForSeq2SeqLM,
-        T5Tokenizer,
-        AutoConfig,
-    )
+from transformers import (
+    AutoTokenizer,
+    AutoModelForCausalLM,
+    LlamaTokenizer,
+    LlamaForCausalLM,
+    AutoModel,
+    AutoModelForSeq2SeqLM,
+    T5Tokenizer,
+    AutoConfig,
+)
 
 from fastchat.conversation import (
     conv_templates,
     get_default_conv_template,
-    compute_skip_echo_len,
     SeparatorStyle,
 )
 from fastchat.serve.compression import load_compress_model
 from fastchat.serve.monkey_patch_non_inplace import (
     replace_llama_attn_with_non_inplace_operations,
 )
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 
-
-def raise_warning_for_old_weights(model_path, model):
-    if "vicuna" in model_path.lower():
-        try:
-            is_vicuna = isinstance(model, LlamaForCausalLM)
-        except Exception:
-            is_vicuna = isinstance(model, LLamaForCausalLM)
-        if is_vicuna and model.model.vocab_size > 32000:
-            warnings.warn(
-                "\nYou are probably using the old Vicuna-v0 model, "
-                "which will generate unexpected results with the "
-                "current fschat.\nYou can try one of the following methods:\n"
-                "1. Upgrade your weights to the new Vicuna-v1.1: https://github.com/lm-sys/FastChat#vicuna-weights.\n"
-                "2. Use the old conversation template by `python3 -m fastchat.serve.cli --model-path /path/to/vicuna-v0 --conv-template conv_one_shot`\n"
-                "3. Downgrade fschat to fschat==0.1.10 (Not recommonded).\n"
-            )
-
+def raise_warning_for_incompatible_cpu_offloading_configuration(device: str, load_8bit: bool, cpu_offloading: bool):
+    if cpu_offloading:
+        if not load_8bit:
+            warnings.warn("The cpu-offloading feature can only be used while also using 8-bit-quantization.\n"
+                          "Use '--load-8bit' to enable 8-bit-quantization\n"
+                          "Continuing without cpu-offloading enabled\n")
+            return False
+        if not "linux" in sys.platform:
+            warnings.warn("CPU-offloading is only supported on linux-systems due to the limited compatability with the bitsandbytes-package\n"
+                          "Continuing without cpu-offloading enabled\n")
+            return False
+        if device != "cuda":
+            warnings.warn("CPU-offloading is only enabled when using CUDA-devices\n"
+                          "Continuing without cpu-offloading enabled\n")
+            return False
+    return cpu_offloading
 
 def get_gpu_memory(max_gpus=None):
     gpu_memory = []
     num_gpus = (
         torch.cuda.device_count()
         if max_gpus is None
         else min(max_gpus, torch.cuda.device_count())
@@ -73,102 +62,123 @@
             total_memory = gpu_properties.total_memory / (1024**3)
             allocated_memory = torch.cuda.memory_allocated() / (1024**3)
             available_memory = total_memory - allocated_memory
             gpu_memory.append(available_memory)
     return gpu_memory
 
 
+def raise_warning_for_old_weights(model_path, model):
+    if "vicuna" in model_path.lower() and isinstance(model, LlamaForCausalLM):
+        if model.model.vocab_size > 32000:
+            warnings.warn(
+                "\nYou are probably using the old Vicuna-v0 model, "
+                "which will generate unexpected results with the "
+                "current fastchat.\nYou can try one of the following methods:\n"
+                "1. Upgrade your weights to the new Vicuna-v1.1: https://github.com/lm-sys/FastChat#vicuna-weights.\n"
+                "2. Use the old conversation template by `python3 -m fastchat.serve.cli --model-path /path/to/vicuna-v0 --conv-template conv_one_shot`\n"
+                "3. Downgrade fschat to fschat==0.1.10 (Not recommonded).\n"
+            )
+
 def load_model(
-    model_path, device, num_gpus, max_gpu_memory=None, load_8bit=False, debug=False
+    model_path, device, num_gpus, max_gpu_memory=None, load_8bit=False, cpu_offloading=False, debug=False
 ):
+    cpu_offloading = raise_warning_for_incompatible_cpu_offloading_configuration(device, load_8bit, cpu_offloading)
     if device == "cpu":
         kwargs = {"torch_dtype": torch.float32}
     elif device == "cuda":
         kwargs = {"torch_dtype": torch.float16}
-        if num_gpus == "auto":
+        if num_gpus != 1:
             kwargs["device_map"] = "auto"
-        else:
-            num_gpus = int(num_gpus)
-            if num_gpus != 1:
-                kwargs["device_map"] = "auto"
-                if max_gpu_memory is None:
-                    kwargs[
-                        "device_map"
-                    ] = "sequential"  # This is important for not the same VRAM sizes
-                    available_gpu_memory = get_gpu_memory(num_gpus)
-                    kwargs["max_memory"] = {
-                        i: str(int(available_gpu_memory[i] * 0.85)) + "GiB"
-                        for i in range(num_gpus)
-                    }
-                else:
-                    kwargs["max_memory"] = {i: max_gpu_memory for i in range(num_gpus)}
+            if max_gpu_memory is None:
+                kwargs[
+                    "device_map"
+                ] = "sequential"  # This is important for not the same VRAM sizes
+                available_gpu_memory = get_gpu_memory(num_gpus)
+                kwargs["max_memory"] = {
+                    i: str(int(available_gpu_memory[i] * 0.85)) + "GiB"
+                    for i in range(num_gpus)
+                }
+            else:
+                kwargs["max_memory"] = {i: max_gpu_memory for i in range(num_gpus)}
         print("init_kwargs", kwargs)
     elif device == "mps":
         kwargs = {"torch_dtype": torch.float16}
         # Avoid bugs in mps backend by not using in-place operations.
         replace_llama_attn_with_non_inplace_operations()
     else:
         raise ValueError(f"Invalid device: {device}")
-    
-    if load_8bit:
-        if num_gpus != 1 and num_gpus != "1":
+
+    if cpu_offloading:
+        # raises an error on incompatible platforms
+        from transformers import BitsAndBytesConfig
+        if "max_memory" in kwargs:
+            kwargs["max_memory"]["cpu"] = str(math.floor(psutil.virtual_memory().available / 2**20)) + 'Mib'
+        kwargs["quantization_config"] = BitsAndBytesConfig(load_in_8bit_fp32_cpu_offload=cpu_offloading)
+        kwargs["load_in_8bit"] = load_8bit
+    elif load_8bit:
+        if num_gpus != 1:
             warnings.warn("8-bit quantization is not supported for multi-gpu inference.")
         else:
-            return load_compress_model(model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"])
+            return load_compress_model(model_path=model_path,
+                device=device, torch_dtype=kwargs["torch_dtype"])
 
     if "chatglm" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, trust_remote_code=True)
-        model = AutoModel.from_pretrained(
-            model_path, trust_remote_code=True, **kwargs
-        ).cuda()
-    elif "t5" in model_path:
-         model = AutoModelForSeq2SeqLM.from_pretrained(model_path,
-                                                       low_cpu_mem_usage=True, **kwargs)
-         tokenizer = T5Tokenizer.from_pretrained(model_path, use_fast=False)
+        model = AutoModel.from_pretrained(model_path, trust_remote_code=True, **kwargs)
     elif "dolly" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
         model = AutoModelForCausalLM.from_pretrained(
             model_path, low_cpu_mem_usage=True, **kwargs
         )
         # 50277 means "### End"
         tokenizer.eos_token_id = 50277
     elif "pythia" in model_path or "stablelm" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
         model = AutoModelForCausalLM.from_pretrained(
             model_path, low_cpu_mem_usage=True, **kwargs
         )
+    elif "t5" in model_path:
+        model = AutoModelForSeq2SeqLM.from_pretrained(model_path,
+                                                      low_cpu_mem_usage=True, **kwargs)
+        tokenizer = T5Tokenizer.from_pretrained(model_path, use_fast=False)
+    elif "RWKV-4" in model_path:
+        from fastchat.serve.rwkv_model import RwkvModel
+        model = RwkvModel(model_path)
+        tokenizer = AutoTokenizer.from_pretrained('EleutherAI/pythia-160m', use_fast=True)
     else:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
         model = AutoModelForCausalLM.from_pretrained(
             model_path, low_cpu_mem_usage=True, **kwargs
         )
         raise_warning_for_old_weights(model_path, model)
 
-
-    if (device == "cuda" and num_gpus == 1) or device == "mps":
+    if (device == "cuda" and num_gpus == 1 and not cpu_offloading) or device == "mps":
         model.to(device)
 
     if debug:
         print(model)
 
     return model, tokenizer
 
 
 @torch.inference_mode()
 def generate_stream(
     model, tokenizer, params, device, context_len=2048, stream_interval=2
 ):
     prompt = params["prompt"]
-    l_prompt = len(prompt)
+    len_prompt = len(prompt)
     temperature = float(params.get("temperature", 1.0))
     max_new_tokens = int(params.get("max_new_tokens", 256))
     stop_str = params.get("stop", None)
-    stop_token_ids = params.get("stop_ids", [tokenizer.eos_token_id])
+    echo = params.get("echo", True)
+    stop_token_ids = params.get("stop_token_ids", None) or []
+    stop_token_ids.append(tokenizer.eos_token_id)
 
     input_ids = tokenizer(prompt).input_ids
+    input_echo_len = len(input_ids)
     output_ids = list(input_ids)
 
     if model.config.is_encoder_decoder:
          max_src_len = context_len
     else:
          max_src_len = context_len - max_new_tokens - 8
 
@@ -224,61 +234,68 @@
 
         if token in stop_token_ids:
             stopped = True
         else:
             stopped = False
 
         if i % stream_interval == 0 or i == max_new_tokens - 1 or stopped:
-            if "t5" in model.config._name_or_path:
-                output = tokenizer.decode(output_ids, skip_special_tokens=True, 
-                                          spaces_between_special_tokens=False)
+            if echo:
+                tmp_output_ids = output_ids
+                rfind_start = len_prompt
             else:
-                output = tokenizer.decode(output_ids, skip_special_tokens=True)
+                tmp_output_ids = output_ids[input_echo_len:]
+                rfind_start = 0
+
+            output = tokenizer.decode(tmp_output_ids, skip_special_tokens=True, 
+                                      spaces_between_special_tokens=False)
             if stop_str:
-                pos = output.rfind(stop_str, l_prompt)
+                pos = output.rfind(stop_str, rfind_start)
                 if pos != -1:
                     output = output[:pos]
                     stopped = True
             yield output
 
         if stopped:
             break
 
-    del past_key_values
+    del past_key_values, out
+    gc.collect()
+    torch.cuda.empty_cache()
 
 
 class ChatIO(abc.ABC):
     @abc.abstractmethod
     def prompt_for_input(self, role: str) -> str:
         """Prompt for input from a role."""
 
     @abc.abstractmethod
     def prompt_for_output(self, role: str):
         """Prompt for output from a role."""
 
     @abc.abstractmethod
-    def stream_output(self, output_stream, skip_echo_len: int):
+    def stream_output(self, output_stream):
         """Stream output."""
 
 
 def chat_loop(
     model_path: str,
     device: str,
-    num_gpus: str,
+    num_gpus: int,
     max_gpu_memory: str,
     load_8bit: bool,
+    cpu_offloading: bool,
     conv_template: Optional[str],
     temperature: float,
     max_new_tokens: int,
     chatio: ChatIO,
     debug: bool,
 ):
     # Model
     model, tokenizer = load_model(
-        model_path, device, num_gpus, max_gpu_memory, load_8bit, debug
+        model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading, debug
     )
     is_chatglm = "chatglm" in str(type(model)).lower()
 
     # Chat
     if conv_template:
         conv = conv_templates[conv_template].copy()
     else:
@@ -293,36 +310,62 @@
             print("exit...")
             break
 
         conv.append_message(conv.roles[0], inp)
         conv.append_message(conv.roles[1], None)
 
         if is_chatglm:
-            prompt = conv.messages[conv.offset :]
             generate_stream_func = chatglm_generate_stream
+            prompt = conv.messages[conv.offset:]
         else:
             generate_stream_func = generate_stream
             prompt = conv.get_prompt()
 
-        skip_echo_len = compute_skip_echo_len(model_path, conv, prompt)
-        stop_str = (
-            conv.sep
-            if conv.sep_style in [SeparatorStyle.SINGLE, SeparatorStyle.BAIZE]
-            else None
-        )
-
-        params = {
+        gen_params = {
             "model": model_path,
             "prompt": prompt,
             "temperature": temperature,
             "max_new_tokens": max_new_tokens,
-            "stop": stop_str,
+            "stop": conv.stop_str,
+            "stop_token_ids": conv.stop_token_ids,
+            "echo": False,
         }
 
         chatio.prompt_for_output(conv.roles[1])
-        output_stream = generate_stream_func(model, tokenizer, params, device)
-        outputs = chatio.stream_output(output_stream, skip_echo_len)
+        output_stream = generate_stream_func(model, tokenizer, gen_params, device)
+        outputs = chatio.stream_output(output_stream)
         # NOTE: strip is important to align with the training data.
         conv.messages[-1][-1] = outputs.strip()
 
         if debug:
             print("\n", {"prompt": prompt, "outputs": outputs}, "\n")
+
+
+def add_model_args(parser):
+    parser.add_argument(
+        "--model-path",
+        type=str,
+        default="lmsys/fastchat-t5-3b-v1.0",
+        help="The path to the weights. This can be a local folder or a Hugging Face repo ID.",
+    )
+    parser.add_argument(
+        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda",
+        help="The device type"
+    )
+    parser.add_argument(
+        "--gpus",
+        type=str,
+        default=None,
+        help="A single GPU like 1 or multiple GPUs like 0,2"
+    )
+    parser.add_argument("--num-gpus", type=int, default=1)
+    parser.add_argument(
+        "--max-gpu-memory",
+        type=str,
+        help="The maximum memory per gpu. Use a string like '13Gib'",
+    )
+    parser.add_argument(
+        "--load-8bit", action="store_true", help="Use 8-bit quantization"
+    )
+    parser.add_argument(
+        "--cpu-offloading", action="store_true", help="Only when using 8-bit quantization: Offload excess weights to the CPU that don't fit on the GPU"
+    )
```

### Comparing `fschat-0.2.4/fastchat/serve/model_worker.py` & `fschat-0.2.5/fastchat/serve/model_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         LLaMATokenizer,
         AutoModel,
     )
 import torch
 import uvicorn
 
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
-from fastchat.serve.inference import load_model, generate_stream
+from fastchat.serve.inference import load_model, generate_stream, add_model_args
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 from fastchat.utils import build_logger, server_error_msg, pretty_print_semaphore
 
 GB = 1 << 30
 
 worker_id = str(uuid.uuid4())[:6]
 logger = build_logger("model_worker", f"model_worker_{worker_id}.log")
@@ -62,26 +62,27 @@
         no_register,
         model_path,
         model_name,
         device,
         num_gpus,
         max_gpu_memory,
         load_8bit=False,
+        cpu_offloading=False,
     ):
         self.controller_addr = controller_addr
         self.worker_addr = worker_addr
         self.worker_id = worker_id
         if model_path.endswith("/"):
             model_path = model_path[:-1]
         self.model_name = model_name or model_path.split("/")[-1]
         self.device = device
 
         logger.info(f"Loading the model {self.model_name} on worker {worker_id} ...")
         self.model, self.tokenizer = load_model(
-            model_path, device, num_gpus, max_gpu_memory, load_8bit
+            model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading
         )
 
         if hasattr(self.model.config, "max_sequence_length"):
             self.context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self.context_len = self.model.config.max_position_embeddings
         else:
@@ -215,54 +216,34 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
     parser.add_argument("--worker-address", type=str, default="http://localhost:21002")
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
     )
-    parser.add_argument(
-        "--model-path",
-        type=str,
-        default="facebook/opt-350m",
-        help="The path to the weights",
-    )
-    parser.add_argument("--model-name", type=str, help="Optional name")
-    parser.add_argument(
-        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
-    )
-    parser.add_argument("--num-gpus", type=int, default=1)
-    parser.add_argument(
-        "--gpus",
-        type=str,
-        default=None,
-        help="A single GPU like 1 or multiple GPUs like 0,2"
-    )
-    parser.add_argument(
-        "--max-gpu-memory",
-        type=str,
-        help="The maximum memory per gpu. Use a string like '13Gib'",
-    )
-    parser.add_argument("--load-8bit", action="store_true")
+    add_model_args(parser)
+    parser.add_argument("--model-name", type=str, help="Optional display name")
     parser.add_argument("--limit-model-concurrency", type=int, default=5)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     if args.gpus:
-        if args.num_gpus and len(args.gpus.split(",")) < int(args.num_gpus):
+        if len(args.gpus.split(",")) < args.num_gpus:
             raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
     
     worker = ModelWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
         args.no_register,
         args.model_path,
         args.model_name,
         args.device,
         args.num_gpus,
         args.max_gpu_memory,
         args.load_8bit,
+        args.cpu_offloading,
     )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `fschat-0.2.4/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.5/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/register_worker.py` & `fschat-0.2.5/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/serve/serve_chatglm.py` & `fschat-0.2.5/fastchat/serve/serve_chatglm.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     model, tokenizer, params, device, context_len=2048, stream_interval=2
 ):
     """Generate text using model's chat api"""
     messages = params["prompt"]
     max_new_tokens = int(params.get("max_new_tokens", 256))
     temperature = float(params.get("temperature", 1.0))
     top_p = float(params.get("top_p", 0.7))
+    echo = params.get("echo", True)
 
     gen_kwargs = {
         "max_new_tokens": max_new_tokens,
         "do_sample": True,
         "top_p": top_p,
         "temperature": temperature,
         "logits_processor": None,
@@ -22,9 +23,13 @@
 
     hist = []
     for i in range(0, len(messages) - 2, 2):
         hist.append((messages[i][1], messages[i + 1][1]))
     query = messages[-2][1]
 
     for response, new_hist in model.stream_chat(tokenizer, query, hist):
-        output = query + " " + response
+        if echo:
+            output = query + " " + response
+        else:
+            output = response
+
         yield output
```

### Comparing `fschat-0.2.4/fastchat/serve/test_message.py` & `fschat-0.2.5/fastchat/serve/test_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import json
 
 import requests
 
 from fastchat.conversation import (
     get_default_conv_template,
-    compute_skip_echo_len,
     SeparatorStyle,
 )
 
 
 def main():
     model_name = args.model_name
 
@@ -26,55 +25,57 @@
         ret = requests.post(
             controller_addr + "/get_worker_address", json={"model": model_name}
         )
         worker_addr = ret.json()["address"]
         print(f"worker_addr: {worker_addr}")
 
     if worker_addr == "":
+        print(f"No available workers for {model_name}")
         return
 
     conv = get_default_conv_template(model_name).copy()
     conv.append_message(conv.roles[0], args.message)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
-    headers = {"User-Agent": "fastchat Client"}
-    pload = {
+    headers = {"User-Agent": "FastChat Client"}
+    gen_params = {
         "model": model_name,
         "prompt": prompt,
-        "max_new_tokens": args.max_new_tokens,
         "temperature": args.temperature,
-        "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
+        "max_new_tokens": args.max_new_tokens,
+        "stop": conv.stop_str,
+        "stop_token_ids": conv.stop_token_ids,
+        "echo": False,
     }
     response = requests.post(
         worker_addr + "/worker_generate_stream",
         headers=headers,
-        json=pload,
+        json=gen_params,
         stream=True,
     )
 
     print(f"{conv.roles[0]}: {args.message}")
     for chunk in response.iter_lines(
         chunk_size=8192, decode_unicode=False, delimiter=b"\0"
     ):
         if chunk:
             data = json.loads(chunk.decode("utf-8"))
-            skip_echo_len = compute_skip_echo_len(model_name, conv, prompt)
-            output = data["text"][skip_echo_len:].strip()
+            output = data["text"].strip()
             print(f"{conv.roles[1]}: {output}", end="\r")
     print("")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
     )
     parser.add_argument("--worker-address", type=str)
-    parser.add_argument("--model-name", type=str, default="facebook/opt-350m")
+    parser.add_argument("--model-name", type=str, required=True)
     parser.add_argument("--temperature", type=float, default=0.0)
     parser.add_argument("--max-new-tokens", type=int, default=32)
     parser.add_argument(
         "--message", type=str, default="Tell me a story with more than 1000 words."
     )
     args = parser.parse_args()
```

### Comparing `fschat-0.2.4/fastchat/serve/test_throughput.py` & `fschat-0.2.5/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.5/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/train/train.py` & `fschat-0.2.5/fastchat/train/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return_tensors="pt",
         padding="max_length",
         max_length=tokenizer.model_max_length,
         truncation=True,
     ).input_ids
     targets = input_ids.clone()
 
-    assert conv.sep_style == SeparatorStyle.TWO
+    assert conv.sep_style == SeparatorStyle.ADD_COLON_TWO
 
     # Mask targets
     sep = conv.sep + conv.roles[1] + ": "
     for conversation, target in zip(conversations, targets):
         total_len = int(target.ne(tokenizer.pad_token_id).sum())
 
         rounds = conversation.split(conv.sep2)
```

### Comparing `fschat-0.2.4/fastchat/train/train_flant5.py` & `fschat-0.2.5/fastchat/train/train_flant5.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import torch
 
 import transformers
 from torch.utils.data import Dataset
 from transformers import Trainer, AddedToken
 
-from fastchat import conversation as conversation_lib
+from fastchat.conversation import conv_one_shot as default_conversation
 
 # TODO: import and use code from ../data/dataset.py
 
 IGNORE_INDEX = -100
 DEFAULT_PAD_TOKEN = "[PAD]"
 DEFAULT_EOS_TOKEN = "</s>"
 DEFAULT_BOS_TOKEN = "</s>"
@@ -169,16 +169,16 @@
     """Add speaker and start/end signal on each round."""
     BEGIN_SIGNAL = "### "
     END_SIGNAL = "\n"
     conversation = header
     
     unknown_role = "unknown"  # use default unknown role
     roles = {
-        "human": conversation_lib.default_conversation.roles[0],  # human role
-        "gpt": conversation_lib.default_conversation.roles[1],  # gpt role
+        "human": default_conversation.roles[0],  # human role
+        "gpt": default_conversation.roles[1],  # gpt role
     }
 
     for i in range(len(source)):
         sentence = source[i]
         sentence_from = sentence["from"].lower()
   
         # TODO(Dacheng): verify this is a good way to split sentences
@@ -219,15 +219,15 @@
     1. Add signal '### ' at the beginning each sentence, with end signal '\n';
     2. Concatenate conversations together;
     3. Tokenize the concatenated conversation;
     4. Make a deepcopy as the target. Mask human words with IGNORE_INDEX.
     """
     # add end signal and concatenate together
     conversations = []
-    header = f"{conversation_lib.default_conversation.system}\n\n"
+    header = f"{default_conversation.system}\n\n"
     for source in sources:
         conversation = _add_speaker_and_signal(header, source, tokenizer)
         conversations.append(conversation)
     # TODO(Dacheng): This is related to whether the dataset has been truncated..
     # Assume we get long conversations, don't pad, don't return tensor
     tokenized_conversations = tokenizer(conversations, max_length=None)["input_ids"]
     q_list = []
```

### Comparing `fschat-0.2.4/fastchat/train/train_lora.py` & `fschat-0.2.5/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fastchat/utils.py` & `fschat-0.2.5/fastchat/utils.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/fschat.egg-info/PKG-INFO` & `fschat-0.2.5/fschat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.4
+Version: 0.2.5
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastChat
-| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
 
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
@@ -25,15 +25,15 @@
 
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
-- [Vicuna Weights](#vicuna-weights)
+- [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
 - [Fine-tuning](#fine-tuning)
 
 ## Install
@@ -59,106 +59,117 @@
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
-## Vicuna Weights
+## Model Weights
+### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
-### Vicuna-7B
+#### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
     --target-model-path /output/path/to/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-13B
+#### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
     --target-model-path /output/path/to/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
-### Fastchat-T5
-This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
-```bash
-python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
-```
+#### Old weights
+See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
-### Old weights
-See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
-
-
-### Low CPU Memory Conversion
+#### Low CPU Memory Conversion
 You can try these methods to reduce the CPU RAM requirement of weight conversion.
 1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
 2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
 
+### FastChat-T5
+Simply run the line below to start chatting.
+It will automatically download the weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). 
+
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
+```
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
+#### Supported Models
+The following models are tested:
+- Vicuna, Alpaca, LLaMA, Koala
+- [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
+- [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
+- [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
+- [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
 Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 
-#### No Enough Memory or Other Platforms
+#### No Enough Memory
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
 This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
-
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
-Besides, we are actively exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome.
+In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
@@ -167,22 +178,23 @@
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
 #### Launch the model worker
 ```bash
-python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
+python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
 Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
-python3 -m fastchat.serve.test_message --model-name vicuna-13b
+python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
+You will see a short output.
 
 #### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
```

#### html2text {}

```diff
@@ -1,132 +1,144 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.4 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.5 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat | [Discord](https://discord.gg/h6kCZb72G7)
-| [Twitter](https://twitter.com/lmsysorg) | An open platform for training,
+dev License-File: LICENSE # FastChat | [Demo](https://chat.lmsys.org/) |
+[Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) |
+[Twitter](https://twitter.com/lmsysorg) | An open platform for training,
 serving, and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
 [weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
 Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
 vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+## Contents - [Install](#install) - [Model Weights](#model-weights) -
 [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
 (#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
 ```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
 repository and navigate to the FastChat folder ```bash git clone https://
 github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
 ```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
-release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
-with the LLaMA model license. You can add our delta to the original LLaMA
-weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
-weights in the huggingface format by following the instructions [here](https://
-huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
-scripts to get Vicuna weights by applying our delta. They will automatically
-download delta weights from our Hugging Face [account](https://huggingface.co/
-lmsys). **NOTE**: Weights v1.1 are only compatible with
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
 ```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
 packages accordingly. If you follow the above commands to do a fresh install,
-then you should get all the correct versions. ### Vicuna-7B This conversion
+then you should get all the correct versions. #### Vicuna-7B This conversion
 command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
 section below if you do not have enough memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
 model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
-``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
 the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
 llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
-lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
-Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
-run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
-model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
-weights_version.md](docs/weights_version.md) for all versions of weights and
-their differences. ### Low CPU Memory Conversion You can try these methods to
-reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
-to the commands above, which will split large weight files into smaller ones
-and use the disk as temporary storage. This can keep the peak memory at less
-than 16GB. 2. Create a large swap file and rely on the operating system to
-automatically utilize the disk as virtual memory. ## Inference with Command
-Line Interface (Experimental Feature: You can specify `--style rich` to enable
-rich text output and better text streaming quality for some non-ASCII content.
-This may not work properly on certain terminals.) [assets/screenshot_cli.png]
-#### Single GPU The command below requires around 28GB of GPU memory for
-Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
-section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
-GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
-on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
-does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
-around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
-Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
-acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
-turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
-path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
-M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
-If you do not have enough memory, you can enable 8-bit compression by adding `-
--load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
-to make the model easier to run on more platforms. Contributions and pull
-requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
-serve using the web UI, you need three main components: web servers that
-interface with users, model workers that host one or more models, and a
-controller to coordinate the webserver and model workers. Here are the commands
-to follow in your terminal: #### Launch the controller ```bash python3 -
-m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker ```bash python3 -
-m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
+vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
+weights and their differences. #### Low CPU Memory Conversion You can try these
+methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
+low-cpu-mem` to the commands above, which will split large weight files into
+smaller ones and use the disk as temporary storage. This can keep the peak
+memory at less than 16GB. 2. Create a large swap file and rely on the operating
+system to automatically utilize the disk as virtual memory. ### FastChat-T5
+Simply run the line below to start chatting. It will automatically download the
+weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
+v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
+v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
+can specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Supported Models The following
+models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
+(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
+12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
+baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
+[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
+[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
+stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
+chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
+memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
+Memory" section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the
+same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
+require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
+30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
+with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
+on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
+compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
+weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
+with 1 - 2 words / second. #### No Enough Memory If you do not have enough
+memory, you can enable 8-bit compression by adding `--load-8bit` to commands
+above. This can reduce memory usage by around half with slightly degraded model
+quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
+8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
+python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
+``` In addition to that, you can add `--cpu-offloading` to commands above to
+offload weights that don't fit on your GPU onto the CPU memory. This requires
+8-bit compression to be enabled and the bitsandbytes package to be installed,
+which is only available on linux operating systems. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+Here are the commands to follow in your terminal: #### Launch the controller
+```bash python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
-Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
-is the user interface that users will interact with. By following these steps,
-you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## API ### Huggingface Generation APIs See
-[fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
-API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
-api-reference/chat/create Some features/compatibilities to be implemented: -
-[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found) - [ ] the return value in
-the client SDK could be used like a dict **RESTful API Server** First, launch
-the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
-the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
-'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
-RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
-21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
-API server ```bash curl http://localhost:8000/v1/chat/completions \ -
-H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
-(e.g., `http://localhost:8000`), you can use the following code to send a
-request to the API server: ```python import os from fastchat import client
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
-client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
-"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
+output. #### Launch the Gradio web server ```bash python3 -
+m fastchat.serve.gradio_web_server ``` This is the user interface that users
+will interact with. By following these steps, you will be able to serve your
+models using the web UI. You can open your browser and chat with a model now.
+## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
+(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
+(Experimental. We will keep improving the API and SDK.) #### Chat Completion
+Reference: https://platform.openai.com/docs/api-reference/chat/create Some
+features/compatibilities to be implemented: - [ ] streaming - [ ] support of
+some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
+(e.g. model not found) - [ ] the return value in the client SDK could be used
+like a dict **RESTful API Server** First, launch the controller ```bash python3
+-m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
+path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
+m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
+```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
+application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
+variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
+localhost:8000`), you can use the following code to send a request to the API
+server: ```python import os from fastchat import client client.set_baseurl
+(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
+( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
+print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
+evaluation pipeline is based on GPT-4. This section provides a high-level
+summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.4/fschat.egg-info/SOURCES.txt` & `fschat-0.2.5/fschat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 fastchat/serve/gradio_web_server.py
 fastchat/serve/gradio_web_server_multi.py
 fastchat/serve/huggingface_api.py
 fastchat/serve/inference.py
 fastchat/serve/model_worker.py
 fastchat/serve/monkey_patch_non_inplace.py
 fastchat/serve/register_worker.py
+fastchat/serve/rwkv_model.py
 fastchat/serve/serve_chatglm.py
 fastchat/serve/test_message.py
 fastchat/serve/test_throughput.py
 fastchat/train/llama_flash_attn_monkey_patch.py
 fastchat/train/train.py
 fastchat/train/train_flant5.py
 fastchat/train/train_lora.py
@@ -75,8 +76,9 @@
 wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py
 wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py
 wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py
 wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py
 wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py
 wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py
 wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py
-wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
+wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
+wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/train/train.py
```

### Comparing `fschat-0.2.4/pyproject.toml` & `fschat-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.4"
+version = "0.2.5"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

### Comparing `fschat-0.2.4/wandb/latest-run/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py` & `fschat-0.2.5/wandb/latest-run/files/code/fastchat/train/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return_tensors="pt",
         padding="max_length",
         max_length=tokenizer.model_max_length,
         truncation=True,
     ).input_ids
     targets = input_ids.clone()
 
-    assert conv.sep_style == SeparatorStyle.TWO
+    assert conv.sep_style == SeparatorStyle.ADD_COLON_TWO
 
     # Mask targets
     sep = conv.sep + conv.roles[1] + ": "
     for conversation, target in zip(conversations, targets):
         total_len = int(target.ne(tokenizer.pad_token_id).sum())
 
         rounds = conversation.split(conv.sep2)
@@ -235,15 +235,15 @@
     parser = transformers.HfArgumentParser(
         (ModelArguments, DataArguments, TrainingArguments)
     )
     model_args, data_args, training_args = parser.parse_args_into_dataclasses()
     local_rank = training_args.local_rank
     model = transformers.AutoModelForCausalLM.from_pretrained(
         #model_args.model_name_or_path,
-        "facebook/opt-125m",
+        "facebook/opt-350m",
         cache_dir=training_args.cache_dir,
     )
     model.config.use_cache = False
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
         model_max_length=training_args.model_max_length,
```

