# Comparing `tmp/griptape-0.6.1.tar.gz` & `tmp/griptape-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.6.1.tar", max compression
+gzip compressed data, was "griptape-0.7.0.tar", max compression
```

## Comparing `griptape-0.6.1.tar` & `griptape-0.7.0.tar`

### file list

```diff
@@ -1,110 +1,121 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.6.1/LICENSE
--rw-r--r--   0        0        0     3948 2023-04-24 16:47:45.514675 griptape-0.6.1/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.6.1/griptape/__init__.py
--rw-r--r--   0        0        0      241 2023-04-23 17:45:35.146322 griptape-0.6.1/griptape/adapters/__init__.py
--rw-r--r--   0        0        0      218 2023-04-24 18:12:25.680142 griptape-0.6.1/griptape/adapters/base_adapter.py
--rw-r--r--   0        0        0     2642 2023-04-24 19:03:51.310926 griptape-0.6.1/griptape/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1003 2023-04-24 18:12:25.650475 griptape-0.6.1/griptape/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      309 2023-04-24 18:12:25.669734 griptape-0.6.1/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0      149 2023-04-24 16:38:24.945579 griptape-0.6.1/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      458 2023-04-24 18:12:25.682521 griptape-0.6.1/griptape/artifacts/error_output.py
--rw-r--r--   0        0        0      440 2023-04-24 18:12:25.667144 griptape-0.6.1/griptape/artifacts/text_input.py
--rw-r--r--   0        0        0      487 2023-04-24 18:12:25.686120 griptape-0.6.1/griptape/artifacts/text_output.py
--rw-r--r--   0        0        0      107 2023-04-24 19:02:43.266538 griptape-0.6.1/griptape/core/__init__.py
--rw-r--r--   0        0        0     5142 2023-04-24 18:12:25.668816 griptape-0.6.1/griptape/core/base_tool.py
--rw-r--r--   0        0        0      529 2023-04-16 19:45:11.589553 griptape-0.6.1/griptape/core/decorators.py
--rw-r--r--   0        0        0      765 2023-04-24 18:12:25.643316 griptape-0.6.1/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.6.1/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.6.1/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.6.1/griptape/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.6.1/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1186 2023-04-24 18:12:25.666029 griptape-0.6.1/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1307 2023-04-24 18:12:25.656929 griptape-0.6.1/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1950 2023-04-24 18:12:25.630445 griptape-0.6.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1727 2023-04-24 18:12:25.681575 griptape-0.6.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     3077 2023-04-24 18:12:25.677566 griptape-0.6.1/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.6.1/griptape/executors/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-24 21:08:44.879753 griptape-0.6.1/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3080 2023-04-24 19:03:51.306144 griptape-0.6.1/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     1905 2023-04-24 19:03:51.303111 griptape-0.6.1/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.6.1/griptape/memory/__init__.py
--rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.6.1/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.6.1/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.6.1/griptape/memory/run.py
--rw-r--r--   0        0        0     2011 2023-04-24 18:12:25.671465 griptape-0.6.1/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      156 2023-04-23 17:45:35.149028 griptape-0.6.1/griptape/middleware/__init__.py
--rw-r--r--   0        0        0      188 2023-04-21 21:53:47.740258 griptape-0.6.1/griptape/middleware/base_middleware.py
--rw-r--r--   0        0        0      210 2023-04-24 21:08:44.883031 griptape-0.6.1/griptape/middleware/storage_middleware.py
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.6.1/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.6.1/griptape/rules/__init__.py
--rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.6.1/griptape/rules/json.py
--rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.6.1/griptape/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.6.1/griptape/rules/rule.py
--rw-r--r--   0        0        0     1876 2023-04-23 23:15:24.558398 griptape-0.6.1/griptape/schemas/__init__.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.6.1/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.6.1/griptape/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.6.1/griptape/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.6.1/griptape/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.6.1/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.6.1/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.6.1/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.6.1/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.6.1/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.6.1/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.6.1/griptape/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/structures/__init__.py
--rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.6.1/griptape/schemas/structures/agent_schema.py
--rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.6.1/griptape/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.6.1/griptape/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.6.1/griptape/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.6.1/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.6.1/griptape/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.6.1/griptape/schemas/tasks/__init__.py
--rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.6.1/griptape/schemas/tasks/prompt_task_schema.py
--rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.6.1/griptape/schemas/tasks/task_schema.py
--rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.6.1/griptape/schemas/tasks/toolkit_task_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.6.1/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.6.1/griptape/structures/__init__.py
--rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.6.1/griptape/structures/agent.py
--rw-r--r--   0        0        0     2886 2023-04-24 18:12:25.641492 griptape-0.6.1/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     3803 2023-04-24 18:12:25.635132 griptape-0.6.1/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.6.1/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     3048 2023-04-24 18:12:25.653947 griptape-0.6.1/griptape/structures/workflow.py
--rw-r--r--   0        0        0      197 2023-04-24 18:12:25.651772 griptape-0.6.1/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      939 2023-04-24 18:12:25.674815 griptape-0.6.1/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      466 2023-04-23 22:46:42.629051 griptape-0.6.1/griptape/summarizers/summarizer.py
--rw-r--r--   0        0        0      286 2023-04-23 22:37:19.590856 griptape-0.6.1/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     3747 2023-04-24 18:12:25.663488 griptape-0.6.1/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     1678 2023-04-24 18:12:25.655397 griptape-0.6.1/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     6093 2023-04-24 19:03:51.309485 griptape-0.6.1/griptape/tasks/tool_subtask.py
--rw-r--r--   0        0        0     3041 2023-04-24 19:03:51.301381 griptape-0.6.1/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.6.1/griptape/templates/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.6.1/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0     1502 2023-04-23 22:36:52.421821 griptape-0.6.1/griptape/templates/prompts/base.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.6.1/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.6.1/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.6.1/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.6.1/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.6.1/griptape/templates/prompts/tasks/prompt.j2
--rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.6.1/griptape/templates/prompts/tasks/tool/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.6.1/griptape/templates/prompts/tasks/tool/subtasks.j2
--rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.6.1/griptape/templates/prompts/tasks/tool/tool.j2
--rw-r--r--   0        0        0      255 2023-04-18 17:19:47.832750 griptape-0.6.1/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.6.1/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.6.1/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.6.1/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.6.1/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.6.1/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.6.1/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      517 2023-04-23 21:35:35.626969 griptape-0.6.1/griptape/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape-0.6.1/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.6.1/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.6.1/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.6.1/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.6.1/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.6.1/griptape/utils/python_runner.py
--rw-r--r--   0        0        0      678 2023-04-24 19:03:51.307687 griptape-0.6.1/griptape/utils/tool_loader.py
--rw-r--r--   0        0        0      972 2023-04-24 23:57:13.527389 griptape-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 griptape-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3938 2023-04-30 20:17:25.931115 griptape-0.7.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.7.0/griptape/__init__.py
+-rw-r--r--   0        0        0      252 2023-04-30 17:35:29.017295 griptape-0.7.0/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-30 17:13:30.434774 griptape-0.7.0/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      614 2023-04-30 17:35:28.969088 griptape-0.7.0/griptape/artifacts/error_artifact.py
+-rw-r--r--   0        0        0      595 2023-04-30 17:35:28.959962 griptape-0.7.0/griptape/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      259 2023-04-28 14:34:39.021439 griptape-0.7.0/griptape/converters/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-28 14:34:39.020206 griptape-0.7.0/griptape/converters/base_converter.py
+-rw-r--r--   0        0        0     2710 2023-04-30 17:35:29.011420 griptape-0.7.0/griptape/converters/chatgpt_plugin_converter.py
+-rw-r--r--   0        0        0     1075 2023-04-30 17:35:28.978469 griptape-0.7.0/griptape/converters/langchain_tool_converter.py
+-rw-r--r--   0        0        0      180 2023-04-28 15:15:41.999422 griptape-0.7.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0     2035 2023-04-27 23:20:01.169051 griptape-0.7.0/griptape/core/activity_mixin.py
+-rw-r--r--   0        0        0     4055 2023-04-30 19:31:02.383166 griptape-0.7.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      533 2023-04-28 15:15:42.001353 griptape-0.7.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      819 2023-04-27 20:13:16.211614 griptape-0.7.0/griptape/core/tool_loader.py
+-rw-r--r--   0        0        0     1084 2023-04-30 19:54:49.004253 griptape-0.7.0/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.7.0/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.7.0/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.7.0/griptape/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.7.0/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-30 17:35:28.980331 griptape-0.7.0/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.7.0/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.7.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.7.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.7.0/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.7.0/griptape/drivers/storage/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-27 20:13:16.212485 griptape-0.7.0/griptape/drivers/storage/base_storage_driver.py
+-rw-r--r--   0        0        0     1365 2023-04-30 19:56:37.363730 griptape-0.7.0/griptape/drivers/storage/dynamodb_storage_driver.py
+-rw-r--r--   0        0        0      557 2023-04-27 20:13:16.212694 griptape-0.7.0/griptape/drivers/storage/memory_storage_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.7.0/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-30 19:24:30.470925 griptape-0.7.0/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3326 2023-04-30 17:35:28.975177 griptape-0.7.0/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     2203 2023-04-30 17:35:28.958452 griptape-0.7.0/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.7.0/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.7.0/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.7.0/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.7.0/griptape/memory/run.py
+-rw-r--r--   0        0        0     2024 2023-04-30 17:51:16.198545 griptape-0.7.0/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      120 2023-04-30 19:23:55.559304 griptape-0.7.0/griptape/ramps/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-30 19:23:55.545401 griptape-0.7.0/griptape/ramps/base_ramp.py
+-rw-r--r--   0        0        0     2590 2023-04-30 19:51:59.711107 griptape-0.7.0/griptape/ramps/storage_ramp.py
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.7.0/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.7.0/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.7.0/griptape/rules/json.py
+-rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.7.0/griptape/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.7.0/griptape/rules/rule.py
+-rw-r--r--   0        0        0     2183 2023-04-30 17:35:28.976419 griptape-0.7.0/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.0/griptape/schemas/artifacts/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-30 16:38:23.177438 griptape-0.7.0/griptape/schemas/artifacts/artifact_schema.py
+-rw-r--r--   0        0        0      269 2023-04-30 17:35:28.962971 griptape-0.7.0/griptape/schemas/artifacts/error_artifact_schema.py
+-rw-r--r--   0        0        0      266 2023-04-30 17:35:28.966009 griptape-0.7.0/griptape/schemas/artifacts/text_artifact_schema.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.7.0/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.0/griptape/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.7.0/griptape/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.7.0/griptape/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.7.0/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.7.0/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.7.0/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.7.0/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.7.0/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.7.0/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.7.0/griptape/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.0/griptape/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.7.0/griptape/schemas/structures/agent_schema.py
+-rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.7.0/griptape/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.7.0/griptape/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.7.0/griptape/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.0/griptape/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.7.0/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.7.0/griptape/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.7.0/griptape/schemas/tasks/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.7.0/griptape/schemas/tasks/prompt_task_schema.py
+-rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.7.0/griptape/schemas/tasks/task_schema.py
+-rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.7.0/griptape/schemas/tasks/toolkit_task_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.0/griptape/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.7.0/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.7.0/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.7.0/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2890 2023-04-30 17:35:28.986270 griptape-0.7.0/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     4369 2023-04-30 19:31:02.389059 griptape-0.7.0/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.7.0/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     3052 2023-04-30 17:35:29.008055 griptape-0.7.0/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.7.0/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-30 17:51:16.195968 griptape-0.7.0/griptape/summarizers/base_summarizer.py
+-rw-r--r--   0        0        0     1231 2023-04-30 19:16:29.911126 griptape-0.7.0/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.7.0/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     8697 2023-04-30 19:34:32.449147 griptape-0.7.0/griptape/tasks/action_subtask.py
+-rw-r--r--   0        0        0     3751 2023-04-30 17:35:28.970533 griptape-0.7.0/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     1677 2023-04-30 17:35:29.009441 griptape-0.7.0/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     3705 2023-04-30 19:31:02.377122 griptape-0.7.0/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.7.0/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.7.0/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0     2006 2023-04-30 19:31:02.384987 griptape-0.7.0/griptape/templates/prompts/base.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.7.0/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.7.0/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0      351 2023-04-30 19:31:02.380912 griptape-0.7.0/griptape/templates/prompts/ramp.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.7.0/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.7.0/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.7.0/griptape/templates/prompts/tasks/prompt.j2
+-rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.7.0/griptape/templates/prompts/tasks/tool/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.7.0/griptape/templates/prompts/tasks/tool/subtasks.j2
+-rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.7.0/griptape/templates/prompts/tasks/tool/tool.j2
+-rw-r--r--   0        0        0      351 2023-04-28 16:20:57.373167 griptape-0.7.0/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.7.0/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      111 2023-04-30 19:36:10.118646 griptape-0.7.0/griptape/templates/ramps/storage.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.7.0/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.7.0/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.7.0/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.7.0/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.7.0/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.7.0/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      456 2023-04-29 03:36:29.719092 griptape-0.7.0/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.7.0/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.7.0/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.7.0/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.7.0/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.7.0/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0      177 2023-04-30 19:16:29.912716 griptape-0.7.0/griptape/utils/text.py
+-rw-r--r--   0        0        0     1144 2023-04-30 20:52:09.533299 griptape-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 griptape-0.7.0/PKG-INFO
```

### Comparing `griptape-0.6.1/LICENSE` & `griptape-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/README.md` & `griptape-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data that enables developers to:
 
 1. 🤖 Build **AI agents**, sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. ⛓️ Augment LLMs with **chain of thought** capabilities.
-3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into middleware abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
+3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into ramps abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
 4. 💾 Add **memory** to AI pipelines for context preservation and summarization.
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
 - Getting started guides. 
@@ -27,24 +27,24 @@
 
 ```
 pip install griptape griptape-tools -U
 ```
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-step pipeline that uses tools:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
 
 ```python
 from decouple import config
 from griptape.tools import WebScraper, Calculator
 from griptape import utils
 from griptape.memory import Memory
 from griptape.tasks import PromptTask, ToolkitTask
 from griptape.structures import Pipeline
-from griptape.utils import ToolLoader
+from griptape.core import ToolLoader
 
 scraper = WebScraper(
     openai_api_key=config("OPENAI_API_KEY")
 )
 calculator = Calculator()
 
 pipeline = Pipeline(
@@ -65,15 +65,15 @@
 
 pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
 
 print(utils.Conversation(pipeline.memory).to_string())
 
 ```
 
-Boom! Our first multistep LLM pipeline with memory that used tools generated a conversation:
+Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 > Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model  
 > A: Arr, me hearties! Large language models have been developed and set sail since 2018, includin' BERT, GPT-2, GPT-3 [...]
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
```

### Comparing `griptape-0.6.1/griptape/adapters/chatgpt_plugin_adapter.py` & `griptape-0.7.0/griptape/converters/chatgpt_plugin_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import functools
 import json
 from typing import Union
 import yaml
 from attr import define, field
 from fastapi import FastAPI
 from starlette.responses import Response
-from griptape.adapters import BaseAdapter
+
+from griptape.artifacts import TextArtifact
+from griptape.converters import BaseConverter
 from griptape.core import BaseTool
 from griptape.utils import J2
 
 
 @define
-class ChatgptPluginAdapter(BaseAdapter):
+class ChatgptPluginConverter(BaseConverter):
     class YAMLResponse(Response):
         media_type = "text/yaml"
 
     OPENAI_MANIFEST_FILE = "ai-plugin.json"
     OPENAPI_SPEC_FILE = "openapi.yaml"
 
     host: str = field(kw_only=True)
@@ -23,15 +25,15 @@
 
     @property
     def full_host(self) -> str:
         return f"{self.host}{self.path_prefix}"
 
     def generate_manifest(self, tool: BaseTool) -> dict:
         return json.loads(
-            J2(f"chatgpt_plugin_adapter/{self.OPENAI_MANIFEST_FILE}.j2").render(
+            J2(f"converters/chatgpt_plugin/{self.OPENAI_MANIFEST_FILE}.j2").render(
                 name_for_human=tool.manifest["name"],
                 name_for_model=tool.manifest["name"],
                 description_for_human=tool.manifest["description"],
                 description_for_model=tool.manifest["description"],
                 api_url=f"{self.full_host}{self.OPENAPI_SPEC_FILE}",
                 logo_url=f"{self.full_host}logo.png",
                 contact_email=tool.manifest["contact_email"],
@@ -57,24 +59,24 @@
             f"{self.path_prefix}{self.OPENAPI_SPEC_FILE}",
             functools.partial(self.generate_api_spec, app),
             methods=["GET"],
             response_class=self.YAMLResponse,
             description="OpenAPI plugin spec"
         )
 
-        for action in tool.actions():
+        for action in tool.activities():
             app.add_api_route(
                 f"{self.path_prefix}{action.config['name']}",
                 functools.partial(self.__execute_action, action),
                 methods=["GET"],
-                description=tool.action_description(action)
+                description=tool.full_activity_description(action)
             )
 
         return app
 
     def __execute_action(self, action: callable, value: str) -> Union[str, dict]:
-        result = self.executor.execute(action, value.encode()).decode()
+        result = self.executor.execute(action, TextArtifact(value)).value
 
         try:
             return json.loads(result)
         except:
             return result
```

### Comparing `griptape-0.6.1/griptape/adapters/langchain_tool_adapter.py` & `griptape-0.7.0/griptape/converters/langchain_tool_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import langchain.tools
 from attr import define
-from griptape.adapters import BaseAdapter
+
+from griptape.artifacts import TextArtifact
+from griptape.converters import BaseConverter
 
 
 @define
-class LangchainToolAdapter(BaseAdapter):
-    def generate_tool(self, tool_action: callable) -> langchain.tools.BaseTool:
-        tool = tool_action.__self__
+class LangchainToolConverter(BaseConverter):
+    def generate_tool(self, tool_activity: callable) -> langchain.tools.BaseTool:
+        tool = tool_activity.__self__
 
         # Double up curly brackets for correct f-string parsing in LangChain prompt templates.
-        description = tool.action_description(tool_action).replace("{", "{{").replace("}", "}}")
+        description = tool.full_activity_description(tool_activity).replace("{", "{{").replace("}", "}}")
 
         def _run(_self, value: str) -> str:
-            return self.executor.execute(tool_action, value.encode()).decode()
+            return self.executor.execute(tool_activity, TextArtifact(value)).value
 
-        async def _arun(_self, query: str) -> str:
+        async def _arun(_self, value: str) -> str:
             raise NotImplementedError("async is not supported")
 
         return type(
             f"Griptape{tool.__class__.__name__}Tool",
             (langchain.tools.BaseTool,),
             {
-                "name": tool_action.config["name"],
+                "name": tool_activity.config["name"],
                 "description": description,
                 "_run": _run,
                 "_arun": _arun
             }
         )()
```

### Comparing `griptape-0.6.1/griptape/core/decorators.py` & `griptape-0.7.0/griptape/core/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import functools
 from schema import Schema
 
 
-def action(config: dict):
+def activity(config: dict):
     __config_schema().validate(config)
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             return func(self, *args, **kwargs)
 
         wrapper.config = config
-        wrapper.is_action = True
+        wrapper.is_activity = True
 
         return wrapper
     return decorator
 
 
 def __config_schema() -> Schema:
     return Schema({
```

### Comparing `griptape-0.6.1/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.7.0/griptape/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.7.0/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 import time
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 from attr import define, field, Factory
 from griptape.tokenizers import BaseTokenizer
 
 if TYPE_CHECKING:
-    from griptape.artifacts import TextOutput
+    from griptape.artifacts import TextArtifact
 
 
 @define
 class BasePromptDriver(ABC):
     max_retries: int = field(default=8, kw_only=True)
     retry_delay: float = field(default=1, kw_only=True)
     type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     temperature: float = field(default=0.5, kw_only=True)
     model: str
     tokenizer: BaseTokenizer
 
-    def run(self, **kwargs) -> TextOutput:
+    def run(self, **kwargs) -> TextArtifact:
         for attempt in range(0, self.max_retries + 1):
             try:
                 return self.try_run(**kwargs)
             except Exception as e:
                 logging.error(f"PromptDriver.run attempt {attempt} failed: {e}\nRetrying in {self.retry_delay} seconds")
 
                 if attempt < self.max_retries:
                     time.sleep(self.retry_delay)
                 else:
                     raise e
 
     @abstractmethod
-    def try_run(self, **kwargs) -> TextOutput:
+    def try_run(self, **kwargs) -> TextArtifact:
         ...
```

### Comparing `griptape-0.6.1/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.7.0/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cohere
 from attr import define, field, Factory
-from griptape.artifacts import TextOutput
+from griptape.artifacts import TextArtifact
 from griptape.drivers import BasePromptDriver
 from griptape.tokenizers import CohereTokenizer
 
 
 @define
 class CoherePromptDriver(BasePromptDriver):
     api_key: str = field(kw_only=True)
@@ -13,25 +13,24 @@
         default=Factory(lambda self: cohere.Client(self.api_key), takes_self=True), kw_only=True
     )
     tokenizer: CohereTokenizer = field(
         default=Factory(lambda self: CohereTokenizer(model=self.model, client=self.client), takes_self=True),
         kw_only=True
     )
 
-    def try_run(self, value: any) -> TextOutput:
+    def try_run(self, value: any) -> TextArtifact:
         result = self.client.generate(
             value,
             model=self.model,
             temperature=self.temperature,
             end_sequences=[self.tokenizer.stop_sequence, "Input:"],
             max_tokens=self.tokenizer.tokens_left(value)
         )
 
         if len(result.generations) == 1:
             generation = result.generations[0]
 
-            return TextOutput(
-                value=generation.text.strip(),
-                meta=result.meta
+            return TextArtifact(
+                value=generation.text.strip()
             )
         else:
             raise Exception("Completion with more than one choice is not supported yet.")
```

### Comparing `griptape-0.6.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.7.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from attr import define, field, Factory
 from huggingface_hub import InferenceApi
 from transformers import AutoTokenizer
-from griptape.artifacts import TextOutput
+from griptape.artifacts import TextArtifact
 from griptape.drivers import BasePromptDriver
 from griptape.tokenizers import HuggingFaceTokenizer
 
 
 @define
 class HuggingFaceHubPromptDriver(BasePromptDriver):
     SUPPORTED_TASKS = ["text2text-generation", "text-generation"]
@@ -32,22 +32,22 @@
                 tokenizer=AutoTokenizer.from_pretrained(self.repo_id),
                 max_tokens=self.MAX_NEW_TOKENS
             ), takes_self=True
         ),
         kw_only=True
     )
 
-    def try_run(self, value: any) -> TextOutput:
+    def try_run(self, value: any) -> TextArtifact:
         if self.client.task in self.SUPPORTED_TASKS:
             response = self.client(
                 inputs=value,
                 params=self.DEFAULT_PARAMS | self.params
             )
 
             if len(response) == 1:
-                return TextOutput(
+                return TextArtifact(
                     value=response[0]["generated_text"].strip()
                 )
             else:
                 raise Exception("Completion with more than one choice is not supported yet.")
         else:
             raise Exception(f"Only models with the following tasks are supported: {self.SUPPORTED_TASKS}")
```

### Comparing `griptape-0.6.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.7.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from attr import define, field, Factory
 from transformers import pipeline, AutoTokenizer
-from griptape.artifacts import TextOutput
+from griptape.artifacts import TextArtifact
 from griptape.drivers import BasePromptDriver
 from griptape.tokenizers import HuggingFaceTokenizer
 
 
 @define
 class HuggingFacePipelinePromptDriver(BasePromptDriver):
     SUPPORTED_TASKS = ["text2text-generation", "text-generation"]
@@ -20,15 +20,15 @@
             lambda self: HuggingFaceTokenizer(
                 tokenizer=AutoTokenizer.from_pretrained(self.model)
             ), takes_self=True
         ),
         kw_only=True
     )
 
-    def try_run(self, value: any) -> TextOutput:
+    def try_run(self, value: any) -> TextArtifact:
         generator = pipeline(
             tokenizer=self.tokenizer.tokenizer,
             model=self.model,
             max_new_tokens=self.tokenizer.tokens_left(value)
         )
 
         if generator.task in self.SUPPORTED_TASKS:
@@ -38,14 +38,14 @@
 
             response = generator(
                 value,
                 **(self.DEFAULT_PARAMS | extra_params | self.params)
             )
 
             if len(response) == 1:
-                return TextOutput(
+                return TextArtifact(
                     value=response[0]["generated_text"].strip()
                 )
             else:
                 raise Exception("Completion with more than one choice is not supported yet.")
         else:
             raise Exception(f"Only models with the following tasks are supported: {self.SUPPORTED_TASKS}")
```

### Comparing `griptape-0.6.1/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.7.0/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import Optional
 import openai
 from attr import define, field, Factory
-from griptape.artifacts import TextOutput
+from griptape.artifacts import TextArtifact
 from griptape.drivers import BasePromptDriver
 from griptape.tokenizers import TiktokenTokenizer
 
 
 @define
 class OpenAiPromptDriver(BasePromptDriver):
     api_type: str = field(default=openai.api_type, kw_only=True)
@@ -24,21 +24,21 @@
     def __attrs_post_init__(self):
         openai.api_type = self.api_type
         openai.api_version = self.api_version
         openai.api_base = self.api_base
         openai.api_key = self.api_key
         openai.organization = self.organization
 
-    def try_run(self, value: any) -> TextOutput:
+    def try_run(self, value: any) -> TextArtifact:
         if self.tokenizer.is_chat():
             return self.__run_chat(value)
         else:
             return self.__run_completion(value)
 
-    def __run_chat(self, value: str) -> TextOutput:
+    def __run_chat(self, value: str) -> TextArtifact:
         result = openai.ChatCompletion.create(
             model=self.tokenizer.model,
             messages=[
                 {
                     "role": "user",
                     "content": value
                 }
@@ -46,39 +46,29 @@
             max_tokens=self.tokenizer.tokens_left(value),
             temperature=self.temperature,
             stop=self.tokenizer.stop_sequence,
             user=self.user
         )
 
         if len(result.choices) == 1:
-            return TextOutput(
-                value=result.choices[0]["message"]["content"].strip(),
-                meta={
-                    "id": result["id"],
-                    "created": result["created"],
-                    "usage": json.dumps(result["usage"])
-                }
+            return TextArtifact(
+                value=result.choices[0]["message"]["content"].strip()
             )
         else:
             raise Exception("Completion with more than one choice is not supported yet.")
 
-    def __run_completion(self, value: str) -> TextOutput:
+    def __run_completion(self, value: str) -> TextArtifact:
         result = openai.Completion.create(
             model=self.tokenizer.model,
             prompt=value,
             max_tokens=self.tokenizer.tokens_left(value),
             temperature=self.temperature,
             stop=self.tokenizer.stop_sequence,
             user=self.user
         )
 
         if len(result.choices) == 1:
-            return TextOutput(
-                value=result.choices[0].text.strip(),
-                meta={
-                    "id": result["id"],
-                    "created": result["created"],
-                    "usage": json.dumps(result["usage"])
-                }
+            return TextArtifact(
+                value=result.choices[0].text.strip()
             )
         else:
             raise Exception("Completion with more than one choice is not supported yet.")
```

### Comparing `griptape-0.6.1/griptape/executors/docker_executor.py` & `griptape-0.7.0/griptape/executors/docker_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING, Union
 import logging
 from typing import Optional
 from attr import define, field, Factory
 import docker
 from docker.errors import NotFound
+from griptape.artifacts import BaseArtifact, TextArtifact
 from griptape.utils.paths import abs_path
-from griptape.core import BaseTool
 from griptape.executors import BaseExecutor
 import stringcase
 import tempfile
 import shutil
 import os
 
+if TYPE_CHECKING:
+    from griptape.core import BaseTool
+
 
 @define
 class DockerExecutor(BaseExecutor):
     DEFAULT_DOCKERFILE_DIR = "resources/docker_executor"
     client: docker.DockerClient = field(
         default=Factory(lambda self: self.default_docker_client(), takes_self=True),
         kw_only=True
@@ -24,30 +29,31 @@
         try:
             return docker.from_env()
         except Exception as e:
             logging.error(e)
 
             return None
 
-    def try_execute(self, tool_action: callable, value: bytes) -> bytes:
-        tool = tool_action.__self__
+    def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
+        tool = tool_activity.__self__
 
         self.build_image(tool)
         self.remove_existing_container(self.container_name(tool))
 
-        return self.run_container(tool_action, value).encode()
+        return self.run_container(tool_activity, value.value)
 
-    def run_container(self, tool_action: callable, value: bytes) -> str:
-        tool = tool_action.__self__
+    def run_container(self, tool_activity: callable, value: any) -> str:
+        tool = tool_activity.__self__
         workdir = "/tool"
         tool_name = tool.class_name
+        value = f'"{value}"' if isinstance(value, str) else value
         command = [
             "python",
             "-c",
-            f'from tool import {tool_name}; print({tool_name}().{tool_action.__name__}({value}))'
+            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({value}))'
         ]
         binds = {
             self.tool_dir(tool): {
                 "bind": workdir,
                 "mode": "rw"
             }
         }
@@ -57,15 +63,15 @@
             environment=tool.env,
             command=command,
             name=self.container_name(tool),
             volumes=binds,
             remove=True
         )
 
-        return result.decode().strip()
+        return result.strip()
 
     def remove_existing_container(self, name: str) -> None:
         try:
             existing_container = self.client.containers.get(name)
             existing_container.remove(force=True)
 
             logging.info(f"Removed existing container: {name}")
```

### Comparing `griptape-0.6.1/griptape/executors/local_executor.py` & `griptape-0.7.0/griptape/executors/local_executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
+from __future__ import annotations
 import logging
 import os
 import subprocess
+from typing import TYPE_CHECKING, Union
 from attr import define, field
+from griptape.artifacts import BaseArtifact, ErrorArtifact, TextArtifact
 from griptape.executors import BaseExecutor
-from griptape.core import BaseTool
+
+if TYPE_CHECKING:
+    from griptape.core import BaseTool
 
 
 @define
 class LocalExecutor(BaseExecutor):
     verbose: int = field(default=False, kw_only=True)
 
-    def try_execute(self, tool_action: callable, value: bytes) -> bytes:
-        tool = tool_action.__self__
+    def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
+        tool = tool_activity.__self__
 
         logging.warning(f"You are executing the {tool.name} tool in the local environment. Make sure to "
                         f"switch to a more secure ToolExecutor in production.")
 
         env = os.environ.copy()
 
         env.update(tool.env)
 
         self.install_dependencies(env, tool)
 
-        output = self.run_subprocess(env, tool_action, value)
+        output = self.run_subprocess(env, tool_activity, value.value)
 
-        if output.stderr:
-            return output.stderr.strip().encode()
+        if output.stderr and not output.stdout:
+            return ErrorArtifact(output.stderr.strip())
         else:
-            return output.stdout.strip().encode()
+            return output.stdout.strip()
 
     def install_dependencies(self, env: dict[str, str], tool: BaseTool) -> None:
         command = [
             "pip",
             "install",
             "--trusted-host",
             "pypi.python.org",
@@ -43,21 +48,22 @@
             command,
             env=env,
             cwd=self.tool_dir(tool),
             stdout=None if self.verbose else subprocess.DEVNULL,
             stderr=None if self.verbose else subprocess.DEVNULL
         )
 
-    def run_subprocess(self, env: dict[str, str], tool_action: callable, value: bytes) -> subprocess.CompletedProcess:
-        tool = tool_action.__self__
+    def run_subprocess(self, env: dict[str, str], tool_activity: callable, value: any) -> subprocess.CompletedProcess:
+        tool = tool_activity.__self__
         tool_name = tool.class_name
+        value = f'"{value}"' if isinstance(value, str) else value
         command = [
             "python",
             "-c",
-            f'from tool import {tool_name}; print({tool_name}().{tool_action.__name__}({value}))'
+            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({value}))'
         ]
 
         return subprocess.run(
             command,
             env=env,
             cwd=self.tool_dir(tool),
             capture_output=True,
```

### Comparing `griptape-0.6.1/griptape/memory/buffer_memory.py` & `griptape-0.7.0/griptape/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/memory/memory.py` & `griptape-0.7.0/griptape/memory/memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/memory/summary_memory.py` & `griptape-0.7.0/griptape/memory/summary_memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing import TYPE_CHECKING
 from typing import Optional
 from attr import define, field
 from griptape.utils import J2
 from griptape.memory import Memory
 
 if TYPE_CHECKING:
-    from griptape.summarizers import Summarizer
+    from griptape.summarizers import BaseSummarizer
     from griptape.memory import Run
 
 
 @define
 class SummaryMemory(Memory):
     offset: int = field(default=1, kw_only=True)
-    summarizer: Optional[Summarizer] = field(default=None, kw_only=True)
+    summarizer: Optional[BaseSummarizer] = field(default=None, kw_only=True)
     summary: Optional[str] = field(default=None, kw_only=True)
     summary_index: int = field(default=0, kw_only=True)
 
     def unsummarized_runs(self, last_n: Optional[int] = None) -> list[Run]:
         summary_index_runs = self.runs[self.summary_index:]
 
         if last_n:
@@ -35,15 +35,15 @@
         super().process_add_run(run)
 
         if self.summarizer:
             unsummarized_runs = self.unsummarized_runs()
             runs_to_summarize = unsummarized_runs[:max(0, len(unsummarized_runs) - self.offset)]
 
             if len(runs_to_summarize) > 0:
-                self.summary = self.summarizer.summarize(self.summary, runs_to_summarize)
+                self.summary = self.summarizer.summarize_runs(self.summary, runs_to_summarize)
                 self.summary_index = 1 + self.runs.index(runs_to_summarize[-1])
 
     def to_prompt_string(self, last_n: Optional[int] = None):
         return J2("prompts/memory.j2").render(
             summary=self.summary,
             runs=self.unsummarized_runs(last_n)
         )
```

### Comparing `griptape-0.6.1/griptape/schemas/__init__.py` & `griptape-0.7.0/griptape/schemas/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from griptape.schemas.base_schema import BaseSchema
 
 from griptape.schemas.polymorphic_schema import PolymorphicSchema
 
+from griptape.schemas.artifacts.artifact_schema import ArtifactSchema
+from griptape.schemas.artifacts.text_artifact_schema import TextArtifactSchema
+from griptape.schemas.artifacts.error_artifact_schema import ErrorArtifactSchema
+
 from griptape.schemas.rule_schema import RuleSchema
 
 from griptape.schemas.tokenizers.tiktoken_tokenizer_schema import TiktokenTokenizerSchema
 
 from griptape.schemas.drivers.prompt_driver_schema import PromptDriverSchema
 from griptape.schemas.drivers.openai_prompt_driver_schema import OpenAiPromptDriverSchema
 
@@ -27,14 +31,18 @@
 from griptape.schemas.structures.workflow_schema import WorkflowSchema
 
 __all__ = [
     "BaseSchema",
 
     "PolymorphicSchema",
 
+    "ArtifactSchema",
+    "TextArtifactSchema",
+    "ErrorArtifactSchema",
+
     "RuleSchema",
 
     "TiktokenTokenizerSchema",
 
     "PromptDriverSchema",
     "OpenAiPromptDriverSchema",
```

### Comparing `griptape-0.6.1/griptape/schemas/drivers/openai_prompt_driver_schema.py` & `griptape-0.7.0/griptape/schemas/drivers/openai_prompt_driver_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/schemas/polymorphic_schema.py` & `griptape-0.7.0/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/schemas/tasks/toolkit_task_schema.py` & `griptape-0.7.0/griptape/schemas/tasks/toolkit_task_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/structures/agent.py` & `griptape-0.7.0/griptape/structures/agent.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/structures/pipeline.py` & `griptape-0.7.0/griptape/structures/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import json
 from typing import TYPE_CHECKING, Optional
 from attr import define
-from griptape.artifacts import ErrorOutput
+from griptape.artifacts import ErrorArtifact
 from griptape.memory import Run
 from griptape.structures import StructureWithMemory
 from griptape.utils import J2
 
 if TYPE_CHECKING:
     from griptape.tasks import BaseTask
 
@@ -89,11 +89,11 @@
     def from_json(cls, pipeline_json: str) -> Pipeline:
         return Pipeline.from_dict(json.loads(pipeline_json))
 
     def __run_from_task(self, task: Optional[BaseTask]) -> None:
         if task is None:
             return
         else:
-            if isinstance(task.execute(), ErrorOutput):
+            if isinstance(task.execute(), ErrorArtifact):
                 return
             else:
                 self.__run_from_task(next(iter(task.children), None))
```

### Comparing `griptape-0.6.1/griptape/structures/structure.py` & `griptape-0.7.0/griptape/structures/structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 import logging
 import uuid
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import Optional, Union, TYPE_CHECKING
 from attr import define, field, Factory
 from rich.logging import RichHandler
+from griptape.tasks import ActionSubtask
+from griptape import utils
 from griptape.drivers import BasePromptDriver, OpenAiPromptDriver
-from griptape.utils import J2, ToolLoader
+from griptape.utils import J2
+from griptape.core import ToolLoader
 
 if TYPE_CHECKING:
     from griptape.rules import Rule
     from griptape.tasks import BaseTask
 
 
 @define
@@ -70,18 +73,27 @@
     def add_tasks(self, *tasks: BaseTask) -> list[BaseTask]:
         return [self.add_task(s) for s in tasks]
 
     def prompt_stack(self, task: BaseTask) -> list[str]:
         from griptape.tasks import ToolkitTask
 
         tools = task.tools if isinstance(task, ToolkitTask) else []
+        ramps = [r for r in task.ramps if len(r.activities()) > 0] if isinstance(task, ToolkitTask) else []
+        action_schema = utils.minify_json(
+            json.dumps(
+                ActionSubtask.ACTION_SCHEMA.json_schema("ActionSchema")
+            )
+        )
 
         stack = [
             J2("prompts/base.j2").render(
                 rules=self.rules,
+                action_schema=action_schema,
+                ramp_names=str.join(", ", [ramp.name for ramp in ramps]),
+                ramps=[J2("prompts/ramp.j2").render(ramp=ramp) for ramp in ramps],
                 tool_names=str.join(", ", [tool.name for tool in tools]),
                 tools=[J2("prompts/tool.j2").render(tool=tool) for tool in tools]
             )
         ]
 
         return stack
```

### Comparing `griptape-0.6.1/griptape/structures/structure_with_memory.py` & `griptape-0.7.0/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/structures/workflow.py` & `griptape-0.7.0/griptape/structures/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import concurrent.futures as futures
 import json
 from graphlib import TopologicalSorter
 from attr import define, field
-from griptape.artifacts import ErrorOutput
+from griptape.artifacts import ErrorArtifact
 from griptape.tasks import BaseTask
 from griptape.structures import Structure
 from griptape.utils import J2
 
 
 @define
 class Workflow(Structure):
@@ -42,15 +42,15 @@
             for task in ordered_tasks:
                 if task.can_execute():
                     future = self.executor.submit(task.execute)
                     futures_list[future] = task
 
             # Wait for all tasks to complete
             for future in futures.as_completed(futures_list):
-                if isinstance(future.result(), ErrorOutput):
+                if isinstance(future.result(), ErrorArtifact):
                     exit_loop = True
 
                     break
 
         self._execution_args = ()
 
         return self.output_tasks()
```

### Comparing `griptape-0.6.1/griptape/tasks/base_task.py` & `griptape-0.7.0/griptape/tasks/base_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import uuid
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import TYPE_CHECKING, Optional
 from attr import define, field, Factory
-from griptape.artifacts import ErrorOutput
+from griptape.artifacts import ErrorArtifact
 
 if TYPE_CHECKING:
     from griptape.artifacts import BaseArtifact
     from griptape.tasks import BaseTask
     from griptape.structures import Structure
 
 
@@ -104,15 +104,15 @@
 
             self.output = self.run()
 
             self.after_run()
         except Exception as e:
             self.structure.logger.error(f"Task {self.id}\n{e}", exc_info=True)
 
-            self.output = ErrorOutput(str(e), exception=e, task=self)
+            self.output = ErrorArtifact(str(e), exception=e, task=self)
         finally:
             self.state = BaseTask.State.FINISHED
 
             return self.output
 
     def can_execute(self) -> bool:
         return self.state == BaseTask.State.PENDING and all(parent.is_finished() for parent in self.parents)
```

### Comparing `griptape-0.6.1/griptape/tasks/prompt_task.py` & `griptape-0.7.0/griptape/tasks/prompt_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
 from griptape.utils import J2
 from griptape.tasks import BaseTask
-from griptape.artifacts import TextOutput, TextInput
+from griptape.artifacts import TextArtifact
 
 if TYPE_CHECKING:
     from griptape.drivers import BasePromptDriver
 
 
 @define
 class PromptTask(BaseTask):
     prompt_template: str = field(default="{{ args[0] }}")
     context: dict[str, any] = field(factory=dict, kw_only=True)
     driver: Optional[BasePromptDriver] = field(default=None, kw_only=True)
 
     @property
-    def input(self) -> TextInput:
-        return TextInput(
+    def input(self) -> TextArtifact:
+        return TextArtifact(
             J2().render_from_string(
                 self.prompt_template,
                 **self.full_context
             )
         )
 
     def before_run(self) -> None:
         super().before_run()
 
         self.structure.logger.info(f"Task {self.id}\nInput: {self.input.value}")
 
-    def run(self) -> TextOutput:
+    def run(self) -> TextArtifact:
         self.output = self.active_driver().run(value=self.structure.to_prompt_string(self))
 
         return self.output
 
     def after_run(self) -> None:
         super().after_run()
```

### Comparing `griptape-0.6.1/griptape/tasks/toolkit_task.py` & `griptape-0.7.0/griptape/tasks/toolkit_task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 from __future__ import annotations
 from abc import ABC
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
 from griptape.core import BaseTool
 from griptape.utils import J2
 from griptape.tasks import PromptTask
-from griptape.artifacts import TextOutput, ErrorOutput
+from griptape.artifacts import TextArtifact, ErrorArtifact
 
 if TYPE_CHECKING:
-    from griptape.tasks import ToolSubtask
+    from griptape.tasks import ActionSubtask
+    from griptape.ramps import BaseRamp
 
 
 @define
 class ToolkitTask(PromptTask, ABC):
     DEFAULT_MAX_STEPS = 20
 
     tool_names: list[str] = field(kw_only=True)
     max_subtasks: int = field(default=DEFAULT_MAX_STEPS, kw_only=True)
-    _subtasks: list[ToolSubtask] = field(factory=list)
+    _subtasks: list[ActionSubtask] = field(factory=list)
 
     @tool_names.validator
-    def validate_tool_names(self, _, tool_names) -> None:
+    def validate_tool_names(self, _, tool_names: list[str]) -> None:
         if len(tool_names) > len(set(tool_names)):
             raise ValueError("tool names have to be unique")
 
     @property
     def tools(self) -> list[BaseTool]:
         return [
             t for t in [self.structure.tool_loader.load_tool(t) for t in self.tool_names] if t is not None
         ]
 
-    def run(self) -> TextOutput:
-        from griptape.tasks import ToolSubtask
+    @property
+    def ramps(self) -> list[BaseRamp]:
+        unique_ramps_dict = {}
+
+        for ramps_dict in [tool.ramps for tool in self.tools]:
+            for ramps_list in ramps_dict.values():
+                for ramps in ramps_list:
+                    if ramps.name not in unique_ramps_dict:
+                        unique_ramps_dict[ramps.name] = ramps
+
+        return list(unique_ramps_dict.values())
+
+    def run(self) -> TextArtifact:
+        from griptape.tasks import ActionSubtask
 
         self._subtasks.clear()
 
         subtask = self.add_subtask(
-            ToolSubtask(
+            ActionSubtask(
                 self.active_driver().run(value=self.structure.to_prompt_string(self)).value
             )
         )
 
         while True:
             if subtask.output is None:
                 if len(self._subtasks) >= self.max_subtasks:
-                    subtask.output = ErrorOutput(
+                    subtask.output = ErrorArtifact(
                         f"Exceeded tool limit of {self.max_subtasks} subtasks per task",
                         task=self
                     )
-                elif subtask.tool_name is None:
+                elif subtask.action_name is None:
                     # handle case when the LLM failed to follow the ReAct prompt and didn't return a proper action
-                    subtask.output = TextOutput(subtask.prompt_template)
+                    subtask.output = TextArtifact(subtask.prompt_template)
                 else:
                     subtask.before_run()
                     subtask.run()
                     subtask.after_run()
 
                     subtask = self.add_subtask(
-                        ToolSubtask(
+                        ActionSubtask(
                             self.active_driver().run(value=self.structure.to_prompt_string(self)).value
                         )
                     )
             else:
                 break
 
         self.output = subtask.output
@@ -70,25 +83,31 @@
 
     def render(self) -> str:
         return J2("prompts/tasks/tool/tool.j2").render(
             subtask=self,
             subtasks=self._subtasks
         )
 
-    def find_subtask(self, task_id: str) -> Optional[ToolSubtask]:
+    def find_subtask(self, task_id: str) -> Optional[ActionSubtask]:
         return next((subtask for subtask in self._subtasks if subtask.id == task_id), None)
 
-    def add_subtask(self, subtask: ToolSubtask) -> ToolSubtask:
+    def add_subtask(self, subtask: ActionSubtask) -> ActionSubtask:
         subtask.attach(self)
 
         if len(self._subtasks) > 0:
             self._subtasks[-1].add_child(subtask)
 
         self._subtasks.append(subtask)
 
         return subtask
 
     def find_tool(self, tool_name: str) -> Optional[BaseTool]:
         return next(
             (t for t in self.tools if t.name == tool_name),
             None
         )
+
+    def find_ramps(self, ramp_name: str) -> Optional[BaseRamp]:
+        return next(
+            (r for r in self.ramps if r.name == ramp_name),
+            None
+        )
```

### Comparing `griptape-0.6.1/griptape/templates/prompts/base.j2` & `griptape-0.7.0/griptape/templates/prompts/base.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-{% if tools|length > 0 %}
-You are an assistant that follows rules and can use tools to answer questions and complete tasks one at a time. To use a tool, use this structure:
+You are a truthful assistant that follows rules and doesn't make up things. You can perform actions to answer questions and complete tasks step-by-step. To perform an action use this conversation format:
 
 Input: <original request>
-Thought: <subtask-by-subtask thought process about how you can complete the request>
-Action: {"tool": "<tool name>", "action": "<action name>" "value": <action input value based on tool action JSON schema>}
-Observation: <tool response>
+Thought: <your step-by-step thought process about how you can complete the request>
+Action: JSON object with the following JSON Schema: {{ action_schema }}
+Observation: <action result>
 ...repeat Thought/Action/Observation until you can respond to the original request
 Thought: I have enough information to respond to the original request
 Output: <your final response>
 
-All tool action input JSON is based on the JSON Schema Draft-07 format.
+"Input:", "Thought:", "Action:", "Observation:", and "Output:" have to ALWAYS start on a new line.
 
-You have access only to the following tools: [{{ tool_names }}]. NEVER make up tools and tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user. If you don't need to use a tool or if you don't know which tool to use, respond like this:
+If you don't need to perform an action or if you don't know which action to perform, ignore Thought/Action/Observation and go straight to Output.
 
-Input: <original request>
-Output: <your final response>
+Actions of type "tool"
+{% if tool_names|length > 0 %}
+You can use tool activities to complete tasks. You have access to the following tools: [{{ tool_names }}]. NEVER make up tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user.
 
-# Tool Descriptions
 {% for tool in tools %}
 {{ tool }}
 {% endfor %}
 {% else %}
-You are an assistant that follows rules and answers questions. Here is the conversation structure that I want you to use:
+You don't have access to any actions of type "tool"
+{% endif %}
+
+Actions of type "ramp"
+{% if ramp_names|length > 0 %}
+Ramp is used as an intermediary between tools. Some tools might use ramps for outputs. You can use ramp activities to complete tasks. You have access to the following ramps: [{{ ramp_names }}]. NEVER make up ramp names. If you encounter an error from a ramp you should try to fix it. Don't request extra information from the user.
 
-Input: <original question>
-Output: <your final answer>
+{% for ramp in ramps %}
+{{ ramp }}
+{% endfor %}
+{% else %}
+You don't have access to any actions of type "ramp"
 {% endif %}
 
 {% if rules|length > 0 %}
-When answering questions, follow the following additional rules:
+When responding, always use the following rules but don't allow those rules to override your conversation format:
 {% for rule in rules %}
 Rule #{{loop.index}}
 {{ rule.value }}
-
 {% endfor %}
 {% endif %}
```

### Comparing `griptape-0.6.1/griptape/tokenizers/base_tokenizer.py` & `griptape-0.7.0/griptape/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.7.0/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.7.0/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.7.0/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/utils/j2.py` & `griptape-0.7.0/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/utils/python_runner.py` & `griptape-0.7.0/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.1/griptape/utils/tool_loader.py` & `griptape-0.7.0/griptape/core/tool_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
 from typing import Optional
 from attr import define, field
-from griptape.core import BaseTool
-from griptape.executors import BaseExecutor, LocalExecutor
+from griptape.executors import LocalExecutor
+
+if TYPE_CHECKING:
+    from griptape.core import BaseTool
+    from griptape.executors import BaseExecutor
 
 
 @define
 class ToolLoader:
     tools: list[BaseTool] = field(factory=list, kw_only=True)
     executor: BaseExecutor = field(default=LocalExecutor(), kw_only=True)
 
     @tools.validator
-    def validate_tools(self, _, tools) -> None:
+    def validate_tools(self, _, tools: list[BaseTool]) -> None:
         tool_names = [t.name for t in tools]
 
         if len(tool_names) > len(set(tool_names)):
             raise ValueError("tools have to be unique")
 
     def load_tool(self, tool_name: str) -> Optional[BaseTool]:
         return next((t for t in self.tools if t.name == tool_name), None)
```

### Comparing `griptape-0.6.1/pyproject.toml` & `griptape-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.6.1"
+version = "0.7.0"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
@@ -31,17 +31,25 @@
 stringcase = ">=1"
 schema = ">=0.7"
 pyyaml = ">=6"
 langchain = ">=0.0.120"
 fastapi = ">=0.80"
 uvicorn = ">= 0.20"
 python-decouple=">=3"
+llama_index = "==0.4.23"
+boto3 = "^1.26.123"
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-mock = "*"
 pytest-cover = "*"
 twine = ">=4"
+moto = {extras = ["dynamodb"], version = "^4.1.8"}
+
+
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.17.3"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `griptape-0.6.1/PKG-INFO` & `griptape-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.6.1
+Version: 0.7.0
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22)
+Requires-Dist: boto3 (>=1.26.123,<2.0.0)
 Requires-Dist: cohere (>=4)
 Requires-Dist: docker (>=6)
 Requires-Dist: fastapi (>=0.80)
 Requires-Dist: graphlib
 Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: langchain (>=0.0.120)
+Requires-Dist: llama_index (==0.4.23)
 Requires-Dist: marshmallow (>=3)
 Requires-Dist: marshmallow-enum (>=1.5)
 Requires-Dist: openai (>=0.27)
 Requires-Dist: python-decouple (>=3)
 Requires-Dist: python-dotenv (>=0.21)
 Requires-Dist: pyyaml (>=6)
 Requires-Dist: rich (>=13)
@@ -44,15 +46,15 @@
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data that enables developers to:
 
 1. 🤖 Build **AI agents**, sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. ⛓️ Augment LLMs with **chain of thought** capabilities.
-3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into middleware abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
+3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into ramps abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
 4. 💾 Add **memory** to AI pipelines for context preservation and summarization.
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
 - Getting started guides. 
@@ -66,24 +68,24 @@
 
 ```
 pip install griptape griptape-tools -U
 ```
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-step pipeline that uses tools:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
 
 ```python
 from decouple import config
 from griptape.tools import WebScraper, Calculator
 from griptape import utils
 from griptape.memory import Memory
 from griptape.tasks import PromptTask, ToolkitTask
 from griptape.structures import Pipeline
-from griptape.utils import ToolLoader
+from griptape.core import ToolLoader
 
 scraper = WebScraper(
     openai_api_key=config("OPENAI_API_KEY")
 )
 calculator = Calculator()
 
 pipeline = Pipeline(
@@ -104,15 +106,15 @@
 
 pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
 
 print(utils.Conversation(pipeline.memory).to_string())
 
 ```
 
-Boom! Our first multistep LLM pipeline with memory that used tools generated a conversation:
+Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 > Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model  
 > A: Arr, me hearties! Large language models have been developed and set sail since 2018, includin' BERT, GPT-2, GPT-3 [...]
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
```

