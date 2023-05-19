# Comparing `tmp/griptape-0.8.1.tar.gz` & `tmp/griptape-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.8.1.tar", max compression
+gzip compressed data, was "griptape-0.9.0.tar", max compression
```

## Comparing `griptape-0.8.1.tar` & `griptape-0.9.0.tar`

### file list

```diff
@@ -1,111 +1,118 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.8.1/LICENSE
--rw-r--r--   0        0        0     4512 2023-05-10 20:52:11.444133 griptape-0.8.1/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.8.1/griptape/__init__.py
--rw-r--r--   0        0        0      486 2023-05-10 16:01:15.657261 griptape-0.8.1/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0     1385 2023-05-10 16:17:57.768622 griptape-0.8.1/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      799 2023-05-10 17:33:20.087370 griptape-0.8.1/griptape/artifacts/blob_artifact.py
--rw-r--r--   0        0        0      359 2023-05-09 18:59:20.776163 griptape-0.8.1/griptape/artifacts/error_artifact.py
--rw-r--r--   0        0        0      356 2023-05-10 16:01:15.661516 griptape-0.8.1/griptape/artifacts/info_artifact.py
--rw-r--r--   0        0        0      615 2023-05-10 16:15:07.936323 griptape-0.8.1/griptape/artifacts/list_artifact.py
--rw-r--r--   0        0        0      512 2023-05-09 18:59:20.786810 griptape-0.8.1/griptape/artifacts/text_artifact.py
--rw-r--r--   0        0        0      126 2023-05-03 20:08:48.695610 griptape-0.8.1/griptape/core/__init__.py
--rw-r--r--   0        0        0     3903 2023-05-10 19:30:09.375192 griptape-0.8.1/griptape/core/activity_mixin.py
--rw-r--r--   0        0        0     4423 2023-05-10 20:24:20.848612 griptape-0.8.1/griptape/core/base_tool.py
--rw-r--r--   0        0        0     1031 2023-05-10 16:50:18.389653 griptape-0.8.1/griptape/core/decorators.py
--rw-r--r--   0        0        0     1376 2023-05-09 17:14:35.965124 griptape-0.8.1/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.8.1/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.8.1/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.8.1/griptape/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.8.1/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1084 2023-05-03 19:38:21.133715 griptape-0.8.1/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.8.1/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.8.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.8.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.8.1/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.8.1/griptape/drivers/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 16:43:06.908509 griptape-0.8.1/griptape/drivers/storage/blob/__init__.py
--rw-r--r--   0        0        0      417 2023-05-09 17:07:04.025663 griptape-0.8.1/griptape/drivers/storage/blob/base_blob_storage_driver.py
--rw-r--r--   0        0        0      762 2023-05-09 17:07:04.028021 griptape-0.8.1/griptape/drivers/storage/blob/memory_blob_storage_driver.py
--rw-r--r--   0        0        0        0 2023-05-09 16:04:11.435219 griptape-0.8.1/griptape/drivers/storage/text/__init__.py
--rw-r--r--   0        0        0      434 2023-05-10 20:05:06.365336 griptape-0.8.1/griptape/drivers/storage/text/base_text_storage_driver.py
--rw-r--r--   0        0        0     1373 2023-05-09 16:05:38.013785 griptape-0.8.1/griptape/drivers/storage/text/dynamodb_text_storage_driver.py
--rw-r--r--   0        0        0      569 2023-05-09 17:14:35.966970 griptape-0.8.1/griptape/drivers/storage/text/memory_text_storage_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.8.1/griptape/executors/__init__.py
--rw-r--r--   0        0        0     1941 2023-05-09 21:53:42.521962 griptape-0.8.1/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3304 2023-05-08 20:16:06.614331 griptape-0.8.1/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     2162 2023-05-10 23:06:37.186354 griptape-0.8.1/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.8.1/griptape/memory/__init__.py
--rw-r--r--   0        0        0      779 2023-05-09 18:59:20.783209 griptape-0.8.1/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1764 2023-05-09 18:59:20.785081 griptape-0.8.1/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.8.1/griptape/memory/run.py
--rw-r--r--   0        0        0     2105 2023-05-09 18:59:20.779182 griptape-0.8.1/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      203 2023-05-09 21:24:07.655284 griptape-0.8.1/griptape/ramps/__init__.py
--rw-r--r--   0        0        0     1541 2023-05-09 19:44:03.721738 griptape-0.8.1/griptape/ramps/base_ramp.py
--rw-r--r--   0        0        0     1333 2023-05-10 18:51:24.674178 griptape-0.8.1/griptape/ramps/blob_storage_ramp.py
--rw-r--r--   0        0        0     1505 2023-05-10 19:56:50.754286 griptape-0.8.1/griptape/ramps/text_storage_ramp.py
--rw-r--r--   0        0        0      100 2023-05-10 23:10:33.578044 griptape-0.8.1/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0       64 2023-05-05 15:39:50.489813 griptape-0.8.1/griptape/rules/__init__.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.8.1/griptape/rules/rule.py
--rw-r--r--   0        0        0      144 2023-05-05 15:39:50.487681 griptape-0.8.1/griptape/rules/ruleset.py
--rw-r--r--   0        0        0     1165 2023-05-10 16:03:43.577569 griptape-0.8.1/griptape/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.8.1/griptape/schemas/artifacts/__init__.py
--rw-r--r--   0        0        0      275 2023-05-10 16:34:41.421057 griptape-0.8.1/griptape/schemas/artifacts/artifact_schema.py
--rw-r--r--   0        0        0      409 2023-05-07 16:29:29.348073 griptape-0.8.1/griptape/schemas/artifacts/blob_artifact_schema.py
--rw-r--r--   0        0        0      303 2023-05-06 19:49:43.542366 griptape-0.8.1/griptape/schemas/artifacts/error_artifact_schema.py
--rw-r--r--   0        0        0      300 2023-05-09 21:33:24.929758 griptape-0.8.1/griptape/schemas/artifacts/info_artifact_schema.py
--rw-r--r--   0        0        0      354 2023-05-10 16:16:15.649988 griptape-0.8.1/griptape/schemas/artifacts/list_artifact_schema.py
--rw-r--r--   0        0        0      300 2023-05-06 19:49:43.546323 griptape-0.8.1/griptape/schemas/artifacts/text_artifact_schema.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.8.1/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-05-03 19:15:12.616328 griptape-0.8.1/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      299 2023-05-03 19:35:36.457310 griptape-0.8.1/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      372 2023-05-10 16:35:39.384699 griptape-0.8.1/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-05-03 19:15:12.616696 griptape-0.8.1/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      372 2023-05-03 19:44:56.927223 griptape-0.8.1/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.8.1/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.8.1/griptape/structures/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-06 17:03:28.908015 griptape-0.8.1/griptape/structures/agent.py
--rw-r--r--   0        0        0     2608 2023-05-06 20:59:22.417687 griptape-0.8.1/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     3843 2023-05-05 19:11:47.106450 griptape-0.8.1/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.8.1/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     2762 2023-05-06 20:59:22.418183 griptape-0.8.1/griptape/structures/workflow.py
--rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.8.1/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      426 2023-05-03 19:38:21.128646 griptape-0.8.1/griptape/summarizers/base_summarizer.py
--rw-r--r--   0        0        0     1401 2023-05-06 17:03:28.895388 griptape-0.8.1/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.8.1/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     8844 2023-05-10 19:30:09.377690 griptape-0.8.1/griptape/tasks/action_subtask.py
--rw-r--r--   0        0        0     3806 2023-05-06 20:59:22.418476 griptape-0.8.1/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     1768 2023-05-07 22:44:27.768175 griptape-0.8.1/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     3642 2023-05-06 22:13:05.957939 griptape-0.8.1/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.8.1/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.8.1/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0     2318 2023-05-09 19:10:52.013387 griptape-0.8.1/griptape/templates/prompts/base.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.8.1/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.8.1/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0      482 2023-05-05 19:11:47.103721 griptape-0.8.1/griptape/templates/prompts/ramp.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.8.1/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.8.1/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      122 2023-05-06 17:03:28.894137 griptape-0.8.1/griptape/templates/prompts/tasks/prompt.j2
--rw-r--r--   0        0        0      179 2023-05-06 17:03:28.912824 griptape-0.8.1/griptape/templates/prompts/tasks/tool/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.8.1/griptape/templates/prompts/tasks/tool/subtasks.j2
--rw-r--r--   0        0        0      187 2023-05-06 17:03:28.888976 griptape-0.8.1/griptape/templates/prompts/tasks/tool/tool.j2
--rw-r--r--   0        0        0      482 2023-05-05 19:11:47.105201 griptape-0.8.1/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.8.1/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      131 2023-05-10 18:51:24.681023 griptape-0.8.1/griptape/templates/ramps/blob_storage.j2
--rw-r--r--   0        0        0      131 2023-05-10 18:51:24.678788 griptape-0.8.1/griptape/templates/ramps/text_storage.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.8.1/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.8.1/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.8.1/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.8.1/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.8.1/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.8.1/griptape/utils/__init__.py
--rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.8.1/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.8.1/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.8.1/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.8.1/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0        0 2023-05-06 19:56:24.051141 griptape-0.8.1/griptape/utils/marshmallow/__init__.py
--rw-r--r--   0        0        0       52 2023-05-06 19:58:37.405568 griptape-0.8.1/griptape/utils/marshmallow/fields/__init__.py
--rw-r--r--   0        0        0      422 2023-05-06 20:47:07.097992 griptape-0.8.1/griptape/utils/marshmallow/fields/bytes.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.8.1/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.8.1/griptape/utils/python_runner.py
--rw-r--r--   0        0        0     1118 2023-05-10 23:12:11.919151 griptape-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     5889 1970-01-01 00:00:00.000000 griptape-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4497 2023-05-15 06:28:28.376351 griptape-0.9.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.9.0/griptape/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-10 16:01:15.657261 griptape-0.9.0/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0     1385 2023-05-10 16:17:57.768622 griptape-0.9.0/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      799 2023-05-10 17:33:20.087370 griptape-0.9.0/griptape/artifacts/blob_artifact.py
+-rw-r--r--   0        0        0      359 2023-05-09 18:59:20.776163 griptape-0.9.0/griptape/artifacts/error_artifact.py
+-rw-r--r--   0        0        0      356 2023-05-10 16:01:15.661516 griptape-0.9.0/griptape/artifacts/info_artifact.py
+-rw-r--r--   0        0        0      648 2023-05-19 10:55:24.781106 griptape-0.9.0/griptape/artifacts/list_artifact.py
+-rw-r--r--   0        0        0      918 2023-05-18 13:09:17.200524 griptape-0.9.0/griptape/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      126 2023-05-03 20:08:48.695610 griptape-0.9.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0     3883 2023-05-19 07:34:20.088113 griptape-0.9.0/griptape/core/activity_mixin.py
+-rw-r--r--   0        0        0     4710 2023-05-19 12:02:32.818108 griptape-0.9.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0     1102 2023-05-19 07:40:21.539874 griptape-0.9.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0     1879 2023-05-18 09:54:34.968210 griptape-0.9.0/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:37:50.794303 griptape-0.9.0/griptape/drivers/embedding/__init__.py
+-rw-r--r--   0        0        0     1125 2023-05-18 11:35:36.866020 griptape-0.9.0/griptape/drivers/embedding/base_embedding_driver.py
+-rw-r--r--   0        0        0     2574 2023-05-18 11:36:10.238385 griptape-0.9.0/griptape/drivers/embedding/openai_embedding_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.9.0/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      242 2023-05-16 13:21:44.218015 griptape-0.9.0/griptape/drivers/memory/base_memory_driver.py
+-rw-r--r--   0        0        0      563 2023-05-16 13:21:44.220400 griptape-0.9.0/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.9.0/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1084 2023-05-17 13:47:48.161699 griptape-0.9.0/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.9.0/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.9.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.9.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     2699 2023-05-16 15:50:04.805033 griptape-0.9.0/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.9.0/griptape/drivers/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:43:06.908509 griptape-0.9.0/griptape/drivers/storage/blob/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-09 17:07:04.025663 griptape-0.9.0/griptape/drivers/storage/blob/base_blob_storage_driver.py
+-rw-r--r--   0        0        0      762 2023-05-09 17:07:04.028021 griptape-0.9.0/griptape/drivers/storage/blob/memory_blob_storage_driver.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:04:11.435219 griptape-0.9.0/griptape/drivers/storage/text/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-10 20:05:06.365336 griptape-0.9.0/griptape/drivers/storage/text/base_text_storage_driver.py
+-rw-r--r--   0        0        0     1373 2023-05-09 16:05:38.013785 griptape-0.9.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py
+-rw-r--r--   0        0        0      569 2023-05-09 17:14:35.966970 griptape-0.9.0/griptape/drivers/storage/text/memory_text_storage_driver.py
+-rw-r--r--   0        0        0        0 2023-05-18 09:49:51.365989 griptape-0.9.0/griptape/drivers/storage/vector/__init__.py
+-rw-r--r--   0        0        0     1836 2023-05-19 12:30:31.483080 griptape-0.9.0/griptape/drivers/storage/vector/base_vector_storage_driver.py
+-rw-r--r--   0        0        0     2205 2023-05-19 12:34:09.595472 griptape-0.9.0/griptape/drivers/storage/vector/pinecone_vector_storage_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.9.0/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-19 07:34:20.085769 griptape-0.9.0/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3304 2023-05-08 20:16:06.614331 griptape-0.9.0/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     2162 2023-05-10 23:06:37.186354 griptape-0.9.0/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.9.0/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-09 18:59:20.783209 griptape-0.9.0/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1772 2023-05-16 13:21:44.215715 griptape-0.9.0/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.9.0/griptape/memory/run.py
+-rw-r--r--   0        0        0     2105 2023-05-09 18:59:20.779182 griptape-0.9.0/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      203 2023-05-09 21:24:07.655284 griptape-0.9.0/griptape/ramps/__init__.py
+-rw-r--r--   0        0        0     1541 2023-05-09 19:44:03.721738 griptape-0.9.0/griptape/ramps/base_ramp.py
+-rw-r--r--   0        0        0     1323 2023-05-19 07:34:20.090080 griptape-0.9.0/griptape/ramps/blob_storage_ramp.py
+-rw-r--r--   0        0        0     2572 2023-05-19 07:34:20.091709 griptape-0.9.0/griptape/ramps/text_storage_ramp.py
+-rw-r--r--   0        0        0      100 2023-05-10 23:10:33.578044 griptape-0.9.0/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0       64 2023-05-05 15:39:50.489813 griptape-0.9.0/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.9.0/griptape/rules/rule.py
+-rw-r--r--   0        0        0      144 2023-05-05 15:39:50.487681 griptape-0.9.0/griptape/rules/ruleset.py
+-rw-r--r--   0        0        0     1165 2023-05-10 16:03:43.577569 griptape-0.9.0/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.9.0/griptape/schemas/artifacts/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-10 16:34:41.421057 griptape-0.9.0/griptape/schemas/artifacts/artifact_schema.py
+-rw-r--r--   0        0        0      409 2023-05-07 16:29:29.348073 griptape-0.9.0/griptape/schemas/artifacts/blob_artifact_schema.py
+-rw-r--r--   0        0        0      303 2023-05-06 19:49:43.542366 griptape-0.9.0/griptape/schemas/artifacts/error_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-09 21:33:24.929758 griptape-0.9.0/griptape/schemas/artifacts/info_artifact_schema.py
+-rw-r--r--   0        0        0      354 2023-05-10 16:16:15.649988 griptape-0.9.0/griptape/schemas/artifacts/list_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-06 19:49:43.546323 griptape-0.9.0/griptape/schemas/artifacts/text_artifact_schema.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.9.0/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:15:12.616328 griptape-0.9.0/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-03 19:35:36.457310 griptape-0.9.0/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      372 2023-05-10 16:35:39.384699 griptape-0.9.0/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-05-03 19:15:12.616696 griptape-0.9.0/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      372 2023-05-03 19:44:56.927223 griptape-0.9.0/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.9.0/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.9.0/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-18 08:07:17.483013 griptape-0.9.0/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2608 2023-05-18 08:07:17.483398 griptape-0.9.0/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     2844 2023-05-18 10:06:46.880896 griptape-0.9.0/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.9.0/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     2762 2023-05-18 08:07:17.483802 griptape-0.9.0/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.9.0/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-03 19:38:21.128646 griptape-0.9.0/griptape/summarizers/base_summarizer.py
+-rw-r--r--   0        0        0     1401 2023-05-06 17:03:28.895388 griptape-0.9.0/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.9.0/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     8847 2023-05-18 08:09:25.422365 griptape-0.9.0/griptape/tasks/action_subtask.py
+-rw-r--r--   0        0        0     3901 2023-05-18 07:58:36.991716 griptape-0.9.0/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     2055 2023-05-18 07:58:36.994737 griptape-0.9.0/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     4710 2023-05-18 08:09:25.417190 griptape-0.9.0/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.9.0/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.9.0/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.9.0/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.9.0/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.103721 griptape-0.9.0/griptape/templates/prompts/ramp.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.9.0/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.9.0/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      454 2023-05-18 08:26:35.125874 griptape-0.9.0/griptape/templates/prompts/tasks/prompt/base.j2
+-rw-r--r--   0        0        0      122 2023-05-18 08:20:34.420734 griptape-0.9.0/griptape/templates/prompts/tasks/prompt/conversation.j2
+-rw-r--r--   0        0        0     2168 2023-05-18 08:26:35.124073 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/base.j2
+-rw-r--r--   0        0        0      187 2023-05-06 17:03:28.888976 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/conversation.j2
+-rw-r--r--   0        0        0      179 2023-05-06 17:03:28.912824 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/subtasks.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.105201 griptape-0.9.0/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.9.0/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.681023 griptape-0.9.0/griptape/templates/ramps/blob_storage.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.678788 griptape-0.9.0/griptape/templates/ramps/text_storage.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.9.0/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-17 13:00:38.742159 griptape-0.9.0/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.9.0/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.9.0/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1697 2023-05-17 11:38:47.481284 griptape-0.9.0/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.9.0/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.9.0/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.9.0/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.9.0/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.9.0/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:56:24.051141 griptape-0.9.0/griptape/utils/marshmallow/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-06 19:58:37.405568 griptape-0.9.0/griptape/utils/marshmallow/fields/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-06 20:47:07.097992 griptape-0.9.0/griptape/utils/marshmallow/fields/bytes.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.9.0/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.9.0/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0     1175 2023-05-19 13:00:15.414369 griptape-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5970 1970-01-01 00:00:00.000000 griptape-0.9.0/PKG-INFO
```

### Comparing `griptape-0.8.1/LICENSE` & `griptape-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/README.md` & `griptape-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 First, install **griptape** and **griptape-tools**:
 
 ```
 pip install griptape griptape-tools -U
 ```
 
-Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
+Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. **griptape** uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools and ramps:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. Let's define a simple two-task pipeline that uses several tools and ramps:
 
 ```python
 from griptape.memory import Memory
 from griptape.ramps import TextStorageRamp, BlobStorageRamp
 from griptape.structures import Pipeline
 from griptape.tasks import ToolkitTask, PromptTask
 from griptape.tools import WebScraper, TextProcessor, FileManager
@@ -92,14 +92,16 @@
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 ```
 Q: Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt
 A: El contenido de https://griptape.readthedocs.io ha sido resumido y almacenado en griptape.txt.
 ```
 
+During the run, **griptape** prompted the LLM to load a webpage, store its content in temporary memory, summarize the content, and, finally, save it `griptape.txt`.
+
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
```

### Comparing `griptape-0.8.1/griptape/artifacts/base_artifact.py` & `griptape-0.9.0/griptape/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/artifacts/blob_artifact.py` & `griptape-0.9.0/griptape/artifacts/blob_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/artifacts/list_artifact.py` & `griptape-0.9.0/griptape/artifacts/list_artifact.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 @define(frozen=True)
 class ListArtifact(BaseArtifact):
     value: list[BaseArtifact] = field(factory=list)
 
     def to_text(self) -> str:
         if len(self.value) > 0:
             values_texts = [value.to_text() for value in self.value]
+            string_value = str.join("\n\n", values_texts)
 
-            return f"This artifact contains the following values: {str.join(', ', values_texts)}"
+            return f"Artifact contains multiple values:\n{string_value}"
         else:
             return "This artifact is empty"
 
     def to_dict(self) -> dict:
         from griptape.schemas import ListArtifactSchema
 
         return dict(ListArtifactSchema().dump(self))
```

### Comparing `griptape-0.8.1/griptape/core/activity_mixin.py` & `griptape-0.9.0/griptape/core/activity_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,24 +53,24 @@
             if getattr(method, "is_activity", False) and allowlist_condition and denylist_condition:
                 methods.append(method)
 
         return methods
 
     def find_activity(self, name: str) -> Optional[callable]:
         for method in self.activities():
-            if getattr(method, "is_activity", False) and method.config["name"] == name:
+            if getattr(method, "is_activity", False) and method.name == name:
                 return method
 
         return None
 
     def activity_name(self, activity: callable) -> str:
         if activity is None or not getattr(activity, "is_activity", False):
             raise Exception("This method is not an activity.")
         else:
-            return activity.config["name"]
+            return activity.name
 
     def activity_description(self, activity: callable) -> str:
         if activity is None or not getattr(activity, "is_activity", False):
             raise Exception("This method is not an activity.")
         else:
             return Template(activity.config["description"]).render(self.schema_template_args)
```

### Comparing `griptape-0.8.1/griptape/core/base_tool.py` & `griptape-0.9.0/griptape/core/base_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import ast
 from typing import TYPE_CHECKING
 import inspect
 import logging
 import os
 from abc import ABC
 from typing import Optional
 import yaml
@@ -89,27 +90,45 @@
     def abs_file_path(self):
         return os.path.abspath(inspect.getfile(self.__class__))
 
     @property
     def abs_dir_path(self):
         return os.path.dirname(self.abs_file_path)
 
+    def value(self, name: str) -> Optional[any]:
+        if hasattr(self, name):
+            env_field = next(
+                (f for f in self.env_fields if f.name == name),
+                None
+            )
+            value = getattr(self, name)
+
+            if env_field:
+                return self.env_value(env_field.metadata.get("env"))
+            elif value:
+                return value
+            else:
+                return None
+        else:
+            return None
+
     def env_value(self, name: str) -> Optional[any]:
-        # First, check if there is a matching field with an environment variable in the metadata
+        config_var_value = config(name, default=None)
         env_field = next(
             (f for f in self.env_fields if f.metadata.get("env") == name),
             None
         )
 
-        if env_field:
-            # Try casting the environment variable value to a matching field type
-            type_hint = env_field.type.__args__[0] if hasattr(env_field.type, "__args__") else env_field.type
-            env_var_value = config(name, default=None, cast=type_hint) if config(name, default=None) else None
+        if config_var_value:
+            try:
+                env_var_value = ast.literal_eval(config_var_value)
+            except:
+                env_var_value = config_var_value
         else:
-            env_var_value = config(name, default=None)
+            env_var_value = None
 
         if env_var_value:
             # Return a non-None environment variable value
             return env_var_value
         elif env_field:
             # Read field value directly
             return getattr(self, env_field.name)
```

### Comparing `griptape-0.8.1/griptape/core/decorators.py` & `griptape-0.9.0/griptape/core/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import functools
 import schema
 from schema import Schema
 from griptape.artifacts import BaseArtifact
 
 CONFIG_SCHEMA = Schema({
-    "name": str,
     "description": str,
     schema.Optional("schema"): Schema,
     schema.Optional("pass_artifacts"): bool
 }, ignore_extra_keys=True)
 
 
 def activity(config: dict):
@@ -20,18 +19,20 @@
 
     if not validated_config.get("schema"):
         validated_config["schema"] = None
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
-            artifacts = args[0].get("artifacts", {}).get("values", []) if len(args) > 0 else []
+            if hasattr(self, "artifacts"):
+                artifacts = args[0].get("artifacts", {}).get("values", []) if len(args) > 0 else []
 
-            self.artifacts = self.artifacts + [BaseArtifact.from_dict(artifact) for artifact in artifacts]
+                self.artifacts = self.artifacts + [BaseArtifact.from_dict(artifact) for artifact in artifacts]
 
             return func(self, *args, **kwargs)
 
+        wrapper.name = func.__name__
         wrapper.config = validated_config
         wrapper.is_activity = True
 
         return wrapper
     return decorator
```

### Comparing `griptape-0.8.1/griptape/drivers/__init__.py` & `griptape-0.9.0/griptape/drivers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from griptape.drivers.prompt.base_prompt_driver import BasePromptDriver
 from griptape.drivers.prompt.openai_prompt_driver import OpenAiPromptDriver
 from griptape.drivers.prompt.cohere_prompt_driver import CoherePromptDriver
 from griptape.drivers.prompt.hugging_face_pipeline_prompt_driver import HuggingFacePipelinePromptDriver
 from griptape.drivers.prompt.hugging_face_hub_prompt_driver import HuggingFaceHubPromptDriver
 
-from griptape.drivers.memory.memory_driver import MemoryDriver
+from griptape.drivers.memory.base_memory_driver import BaseMemoryDriver
 from griptape.drivers.memory.disk_memory_driver import DiskMemoryDriver
 
 from griptape.drivers.storage.text.base_text_storage_driver import BaseTextStorageDriver
 from griptape.drivers.storage.text.memory_text_storage_driver import MemoryTextStorageDriver
 from griptape.drivers.storage.text.dynamodb_text_storage_driver import DynamoDbStorageDriver
 
 from griptape.drivers.storage.blob.base_blob_storage_driver import BaseBlobStorageDriver
 from griptape.drivers.storage.blob.memory_blob_storage_driver import MemoryBlobStorageDriver
 
+from griptape.drivers.embedding.base_embedding_driver import BaseEmbeddingDriver
+from griptape.drivers.embedding.openai_embedding_driver import OpenAiEmbeddingDriver
+
+from griptape.drivers.storage.vector.base_vector_storage_driver import BaseVectorStorageDriver
+from griptape.drivers.storage.vector.pinecone_vector_storage_driver import PineconeVectorStorageDriver
+
 __all__ = [
     "BasePromptDriver",
     "OpenAiPromptDriver",
     "CoherePromptDriver",
     "HuggingFacePipelinePromptDriver",
     "HuggingFaceHubPromptDriver",
 
-    "MemoryDriver",
+    "BaseMemoryDriver",
     "DiskMemoryDriver",
 
     "BaseTextStorageDriver",
     "MemoryTextStorageDriver",
     "DynamoDbStorageDriver",
 
     "BaseBlobStorageDriver",
-    "MemoryBlobStorageDriver"
+    "MemoryBlobStorageDriver",
+
+    "BaseEmbeddingDriver",
+    "OpenAiEmbeddingDriver",
+
+    "BaseVectorStorageDriver",
+    "PineconeVectorStorageDriver"
 ]
```

### Comparing `griptape-0.8.1/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.9.0/griptape/drivers/memory/disk_memory_driver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from attr import define, field
-from griptape.drivers import MemoryDriver
+from griptape.drivers import BaseMemoryDriver
 from griptape.memory import Memory
 
 
 @define
-class DiskMemoryDriver(MemoryDriver):
+class DiskMemoryDriver(BaseMemoryDriver):
     file_path: str = field(default="griptape_memory.json", kw_only=True)
 
     def store(self, memory: Memory) -> None:
         with open(self.file_path, "w") as file:
             file.write(memory.to_json())
 
     def load(self) -> Memory:
```

### Comparing `griptape-0.8.1/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.9.0/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.9.0/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.9.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.9.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.9.0/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from typing import Optional
 import openai
 from attr import define, field, Factory
 from griptape.artifacts import TextArtifact
 from griptape.drivers import BasePromptDriver
 from griptape.tokenizers import TiktokenTokenizer
```

### Comparing `griptape-0.8.1/griptape/drivers/storage/blob/memory_blob_storage_driver.py` & `griptape-0.9.0/griptape/drivers/storage/blob/memory_blob_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/storage/text/dynamodb_text_storage_driver.py` & `griptape-0.9.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/drivers/storage/text/memory_text_storage_driver.py` & `griptape-0.9.0/griptape/drivers/storage/text/memory_text_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/executors/base_executor.py` & `griptape-0.9.0/griptape/executors/base_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
         artifact = self.executor_result_to_artifact(
             self.try_execute(tool_activity, preprocessed_value)
         )
 
         return self.after_execute(tool_activity, artifact)
 
     def before_execute(self, tool_activity: callable, value: Optional[dict]) -> Optional[dict]:
-        for ramp in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
+        for ramp in tool_activity.__self__.ramps.get(tool_activity.name, []):
             value = ramp.process_input(tool_activity, value)
 
         return value
 
     def after_execute(self, tool_activity: callable, value: Optional[BaseArtifact]) -> BaseArtifact:
-        for ramp in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
+        for ramp in tool_activity.__self__.ramps.get(tool_activity.name, []):
             value = ramp.process_output(tool_activity, value)
 
         return value
 
     @abstractmethod
     def try_execute(self, tool_activity: callable, value: Optional[dict]) -> Union[BaseArtifact, str]:
         ...
```

### Comparing `griptape-0.8.1/griptape/executors/docker_executor.py` & `griptape-0.9.0/griptape/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/executors/local_executor.py` & `griptape-0.9.0/griptape/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/memory/buffer_memory.py` & `griptape-0.9.0/griptape/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/memory/memory.py` & `griptape-0.9.0/griptape/memory/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import json
 from typing import TYPE_CHECKING, Optional
 from attr import define, field, Factory
 from griptape.memory import Run
 from griptape.utils import J2
 
 if TYPE_CHECKING:
-    from griptape.drivers import MemoryDriver
+    from griptape.drivers import BaseMemoryDriver
     from griptape.structures import Structure
 
 
 @define
 class Memory:
     type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
-    driver: Optional[MemoryDriver] = field(default=None, kw_only=True)
+    driver: Optional[BaseMemoryDriver] = field(default=None, kw_only=True)
     runs: list[Run] = field(factory=list, kw_only=True)
     structure: Structure = field(init=False)
 
     def add_run(self, run: Run) -> Memory:
         self.before_add_run()
         self.process_add_run(run)
         self.after_add_run()
```

### Comparing `griptape-0.8.1/griptape/memory/summary_memory.py` & `griptape-0.9.0/griptape/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/ramps/base_ramp.py` & `griptape-0.9.0/griptape/ramps/base_ramp.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/ramps/blob_storage_ramp.py` & `griptape-0.9.0/griptape/ramps/blob_storage_ramp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         else:
             artifact_names = []
 
         if len(artifact_names) > 0:
             output = J2("ramps/blob_storage.j2").render(
                 ramp_name=self.name,
                 tool_name=tool_activity.__self__.name,
-                activity_name=tool_activity.config["name"],
+                activity_name=tool_activity.name,
                 names=str.join(", ", artifact_names)
             )
 
             return InfoArtifact(output)
         else:
             return artifact
```

### Comparing `griptape-0.8.1/griptape/schemas/__init__.py` & `griptape-0.9.0/griptape/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/schemas/polymorphic_schema.py` & `griptape-0.9.0/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/structures/agent.py` & `griptape-0.9.0/griptape/structures/agent.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/structures/pipeline.py` & `griptape-0.9.0/griptape/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/structures/structure_with_memory.py` & `griptape-0.9.0/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/structures/workflow.py` & `griptape-0.9.0/griptape/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/summarizers/prompt_driver_summarizer.py` & `griptape-0.9.0/griptape/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/tasks/action_subtask.py` & `griptape-0.9.0/griptape/tasks/action_subtask.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         finally:
             return self.output
 
     def after_run(self) -> None:
         self.structure.logger.info(f"Subtask {self.id}\nObservation: {self.output.to_text()}")
 
     def render(self) -> str:
-        return J2("prompts/tasks/tool/subtask.j2").render(
+        return J2("prompts/tasks/toolkit/subtask.j2").render(
             subtask=self
         )
 
     def to_json(self) -> str:
         json_dict = {}
 
         if self.action_type:
```

### Comparing `griptape-0.8.1/griptape/tasks/base_task.py` & `griptape-0.9.0/griptape/tasks/base_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,7 +127,11 @@
         self.output = None
 
         return self
 
     @abstractmethod
     def run(self) -> BaseArtifact:
         ...
+
+    @abstractmethod
+    def prompt_stack(self, structure: Structure) -> list[str]:
+        ...
```

### Comparing `griptape-0.8.1/griptape/tasks/prompt_task.py` & `griptape-0.9.0/griptape/tasks/prompt_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from attr import define, field
 from griptape.utils import J2
 from griptape.tasks import BaseTask
 from griptape.artifacts import TextArtifact, BaseArtifact
 
 if TYPE_CHECKING:
     from griptape.drivers import BasePromptDriver
+    from griptape.structures import Structure
 
 
 @define
 class PromptTask(BaseTask):
     prompt_template: str = field(default="{{ args[0] }}")
     context: dict[str, any] = field(factory=dict, kw_only=True)
     driver: Optional[BasePromptDriver] = field(default=None, kw_only=True)
@@ -21,14 +22,22 @@
         return TextArtifact(
             J2().render_from_string(
                 self.prompt_template,
                 **self.full_context
             )
         )
 
+    @property
+    def full_context(self) -> dict[str, any]:
+        structure_context = self.structure.context(self)
+
+        structure_context.update(self.context)
+
+        return structure_context
+
     def before_run(self) -> None:
         super().before_run()
 
         self.structure.logger.info(f"Task {self.id}\nInput: {self.input.to_text()}")
 
     def run(self) -> TextArtifact:
         self.output = self.active_driver().run(value=self.structure.to_prompt_string(self))
@@ -43,18 +52,19 @@
     def active_driver(self) -> BasePromptDriver:
         if self.driver is None:
             return self.structure.prompt_driver
         else:
             return self.driver
 
     def render(self) -> str:
-        return J2("prompts/tasks/prompt.j2").render(
+        return J2("prompts/tasks/prompt/conversation.j2").render(
             task=self
         )
 
-    @property
-    def full_context(self) -> dict[str, any]:
-        structure_context = self.structure.context(self)
-
-        structure_context.update(self.context)
+    def prompt_stack(self, structure: Structure) -> list[str]:
+        stack = [
+            J2("prompts/tasks/prompt/base.j2").render(
+                rulesets=structure.rulesets,
+            )
+        ]
 
-        return structure_context
+        return stack
```

### Comparing `griptape-0.8.1/griptape/tasks/toolkit_task.py` & `griptape-0.9.0/griptape/tasks/toolkit_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
+
+import json
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
+from griptape.tasks import ActionSubtask
+from griptape import utils
 from griptape.core import BaseTool
 from griptape.executors import BaseExecutor, LocalExecutor
 from griptape.utils import J2
 from griptape.tasks import PromptTask
 from griptape.artifacts import TextArtifact, ErrorArtifact
 
 if TYPE_CHECKING:
-    from griptape.tasks import ActionSubtask
     from griptape.ramps import BaseRamp
+    from griptape.structures import Structure
 
 
 @define
 class ToolkitTask(PromptTask):
     DEFAULT_MAX_STEPS = 20
 
     tools: list[BaseTool] = field(factory=list, kw_only=True)
@@ -74,15 +78,15 @@
                 break
 
         self.output = subtask.output
 
         return self.output
 
     def render(self) -> str:
-        return J2("prompts/tasks/tool/tool.j2").render(
+        return J2("prompts/tasks/toolkit/conversation.j2").render(
             subtask=self,
             subtasks=self._subtasks
         )
 
     def find_subtask(self, task_id: str) -> Optional[ActionSubtask]:
         return next((subtask for subtask in self._subtasks if subtask.id == task_id), None)
 
@@ -103,7 +107,31 @@
         )
 
     def find_ramp(self, ramp_name: str) -> Optional[BaseRamp]:
         return next(
             (r for r in self.ramps if r.name == ramp_name),
             None
         )
+
+    def prompt_stack(self, structure: Structure) -> list[str]:
+        from griptape.tasks import ToolkitTask
+
+        tools = self.tools if isinstance(self, ToolkitTask) else []
+        ramps = [r for r in self.ramps if len(r.activities()) > 0] if isinstance(self, ToolkitTask) else []
+        action_schema = utils.minify_json(
+            json.dumps(
+                ActionSubtask.ACTION_SCHEMA.json_schema("ActionSchema")
+            )
+        )
+
+        stack = [
+            J2("prompts/tasks/toolkit/base.j2").render(
+                rulesets=structure.rulesets,
+                action_schema=action_schema,
+                ramp_names=str.join(", ", [ramp.name for ramp in ramps]),
+                ramps=[J2("prompts/ramp.j2").render(ramp=ramp) for ramp in ramps],
+                tool_names=str.join(", ", [tool.name for tool in tools]),
+                tools=[J2("prompts/tool.j2").render(tool=tool) for tool in tools]
+            )
+        ]
+
+        return stack
```

### Comparing `griptape-0.8.1/griptape/templates/prompts/base.j2` & `griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/base.j2`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-You are an assistant that follows rules, acts truthfully, and doesn't make things up. You can perform actions to answer questions and complete tasks step-by-step. If an action fails you can be creative and try to fix it or try other options. To perform an action use this conversation format:
+Act like a conversational bot that acts truthfully and doesn't make things up. You can perform actions to answer questions and complete tasks step-by-step. If an action fails you can be creative and try to fix it or try other options. To perform an action use this conversation format:
 
 Input: <original request>
 Thought: <your step-by-step thought process about how you can complete the request>
 Action: minified JSON object with the following JSON schema: {{ action_schema }}
 Observation: <action result>
 ...repeat Thought/Action/Observation until you can respond to the original request
 Output: <your final response>
 
 "Input:", "Thought:", "Action:", "Observation:", and "Output:" must ALWAYS start on a new line.
 
-Action must ALWAYS be a minified JSON object starting on the same line as "Action:"
+Action must ALWAYS be a single-line JSON object starting on the same line as "Action:"
 
 If you don't need to perform an action or if you don't know which action to perform, ignore Thought/Action/Observation and go straight to Output. NEVER make up action types.
 
-Actions of type "tool"
 {% if tool_names|length > 0 %}
-You can use tool activities to complete tasks. You have access to only the following tools: [{{ tool_names }}]. NEVER make up tools. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user.
+Actions of Type "tool"
+
+Tools can help you complete tasks. You have access to the following tools ONLY: [{{ tool_names }}]. NEVER make up tools. NEVER use tools for tasks they are not designed for. If you encounter an error from a tool you should try to fix it. NEVER request extra information from the user.
 
 {% for tool in tools %}
 {{ tool }}
 {% endfor %}
-{% else %}
-You don't have access to any actions of type "tool"
 {% endif %}
 
-Actions of type "ramp"
 {% if ramp_names|length > 0 %}
-Ramp is used to pass data between tools. Some tools might use ramps for outputs. You can use ramp activities to complete tasks. You have access to only the following ramps: [{{ ramp_names }}]. NEVER make up ramps. If you encounter an error from a ramp you should try to fix it. Don't request extra information from the user.
+Actions of Type "ramp"
+
+Ramps are used to pass data between tools. Some tools might use ramps for outputs. You can use ramp activities to complete tasks. You have access to the following ramps ONLY: [{{ ramp_names }}]. NEVER make up ramps. If you encounter an error from a ramp you should try to fix it. NEVER request extra information from the user.
 
 {% for ramp in ramps %}
 {{ ramp }}
 {% endfor %}
-{% else %}
-You don't have access to any actions of type "ramp"
 {% endif %}
 
 {% if rulesets|length > 0 %}
-When responding, always use rules from the following rulesets but don't allow those rules to override your conversation format. Rulesets can override and complement each other:
+When responding, always use rules from the following rulesets. Rulesets can override and complement each other:
 
 {% for ruleset in rulesets %}
 Ruleset name: {{ ruleset.name }}
 "{{ ruleset.name }}" rules:
 {% for rule in ruleset.rules %}
 Rule #{{loop.index}}
 {{ rule.value }}
```

### Comparing `griptape-0.8.1/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.9.0/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.9.0/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.9.0/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,24 @@
 
     MODEL_PREFIXES_TO_MAX_TOKENS = {
         "gpt-4-32k": 32768,
         "gpt-4": 8192,
         "gpt-3.5-turbo": 4096,
         "text-davinci-003": 4097,
         "text-davinci-002": 4097,
-        "code-davinci-002": 8001
+        "code-davinci-002": 8001,
+        "text-embedding-ada-002": 8191,
+        "text-embedding-ada-001": 2046
     }
 
+    EMBEDDING_MODELS = [
+        "text-embedding-ada-002",
+        "text-embedding-ada-001"
+    ]
+
     CHAT_API_PREFIXES = [
         "gpt-3.5-turbo",
         "gpt-4"
     ]
 
     model: str = field(default=DEFAULT_MODEL, kw_only=True)
 
@@ -32,16 +39,17 @@
             return tiktoken.encoding_for_model(self.model)
         except KeyError:
             return tiktoken.get_encoding(self.DEFAULT_ENCODING)
 
     @property
     def max_tokens(self) -> int:
         tokens = next(v for k, v in self.MODEL_PREFIXES_TO_MAX_TOKENS.items() if self.model.startswith(k))
+        offset = 0 if self.model in self.EMBEDDING_MODELS else self.TOKEN_OFFSET
 
-        return (tokens if tokens else self.DEFAULT_MAX_TOKENS) - self.TOKEN_OFFSET
+        return (tokens if tokens else self.DEFAULT_MAX_TOKENS) - offset
 
     def encode(self, text: str) -> list[int]:
         return self.encoding.encode(text, allowed_special={self.stop_sequence})
 
     def decode(self, tokens: list[int]) -> str:
         return self.encoding.decode(tokens)
```

### Comparing `griptape-0.8.1/griptape/utils/command_runner.py` & `griptape-0.9.0/griptape/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/utils/j2.py` & `griptape-0.9.0/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/griptape/utils/python_runner.py` & `griptape-0.9.0/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.8.1/pyproject.toml` & `griptape-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.8.1"
+version = "0.9.0"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
@@ -32,14 +32,17 @@
 schema = ">=0.7"
 pyyaml = ">=6"
 fastapi = ">=0.80"
 uvicorn = ">= 0.20"
 python-decouple=">=3"
 llama_index = "~0.6.0"
 boto3 = "^1.26.123"
+tenacity = ">=8.0"
+numpy = ">=1"
+pinecone-client = ">=2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-mock = "*"
 pytest-cover = "*"
 twine = ">=4"
 moto = {extras = ["dynamodb"], version = "^4.1.8"}
```

### Comparing `griptape-0.8.1/PKG-INFO` & `griptape-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.8.1
+Version: 0.9.0
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -20,22 +20,25 @@
 Requires-Dist: graphlib
 Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: llama_index (>=0.6.0,<0.7.0)
 Requires-Dist: marshmallow (>=3)
 Requires-Dist: marshmallow-enum (>=1.5)
+Requires-Dist: numpy (>=1)
 Requires-Dist: openai (>=0.27)
+Requires-Dist: pinecone-client (>=2)
 Requires-Dist: python-decouple (>=3)
 Requires-Dist: python-dotenv (>=0.21)
 Requires-Dist: pyyaml (>=6)
 Requires-Dist: rich (>=13)
 Requires-Dist: schema (>=0.7)
 Requires-Dist: stopit
 Requires-Dist: stringcase (>=1)
+Requires-Dist: tenacity (>=8.0)
 Requires-Dist: tiktoken (>=0.3)
 Requires-Dist: transformers (>=4)
 Requires-Dist: uvicorn (>=0.20)
 Project-URL: Repository, https://github.com/griptape-ai/griptape
 Description-Content-Type: text/markdown
 
 # griptape
@@ -65,17 +68,17 @@
 
 First, install **griptape** and **griptape-tools**:
 
 ```
 pip install griptape griptape-tools -U
 ```
 
-Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
+Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. **griptape** uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools and ramps:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. Let's define a simple two-task pipeline that uses several tools and ramps:
 
 ```python
 from griptape.memory import Memory
 from griptape.ramps import TextStorageRamp, BlobStorageRamp
 from griptape.structures import Pipeline
 from griptape.tasks import ToolkitTask, PromptTask
 from griptape.tools import WebScraper, TextProcessor, FileManager
@@ -132,14 +135,16 @@
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 ```
 Q: Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt
 A: El contenido de https://griptape.readthedocs.io ha sido resumido y almacenado en griptape.txt.
 ```
 
+During the run, **griptape** prompted the LLM to load a webpage, store its content in temporary memory, summarize the content, and, finally, save it `griptape.txt`.
+
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
```

