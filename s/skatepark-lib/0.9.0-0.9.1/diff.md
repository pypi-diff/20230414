# Comparing `tmp/skatepark_lib-0.9.0.tar.gz` & `tmp/skatepark_lib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skatepark_lib-0.9.0.tar", max compression
+gzip compressed data, was "skatepark_lib-0.9.1.tar", max compression
```

## Comparing `skatepark_lib-0.9.0.tar` & `skatepark_lib-0.9.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 skatepark_lib-0.9.0/LICENSE
--rw-r--r--   0        0        0     3896 2023-04-13 22:14:02.910363 skatepark_lib-0.9.0/README.md
--rw-r--r--   0        0        0      782 2023-04-13 22:24:14.751322 skatepark_lib-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 skatepark_lib-0.9.0/skatepark/__init__.py
--rw-r--r--   0        0        0      258 2023-04-09 19:16:37.935258 skatepark_lib-0.9.0/skatepark/artifacts/__init__.py
--rw-r--r--   0        0        0      427 2023-04-09 19:16:37.880969 skatepark_lib-0.9.0/skatepark/artifacts/error_output.py
--rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 skatepark_lib-0.9.0/skatepark/artifacts/structure_artifact.py
--rw-r--r--   0        0        0      529 2023-04-09 19:16:37.958840 skatepark_lib-0.9.0/skatepark/artifacts/text_output.py
--rw-r--r--   0        0        0      383 2023-04-09 19:16:37.961557 skatepark_lib-0.9.0/skatepark/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 skatepark_lib-0.9.0/skatepark/drivers/memory/__init__.py
--rw-r--r--   0        0        0      590 2023-04-09 19:16:37.834614 skatepark_lib-0.9.0/skatepark/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      263 2023-04-09 19:16:37.853167 skatepark_lib-0.9.0/skatepark/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 skatepark_lib-0.9.0/skatepark/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     2481 2023-04-09 19:16:37.884254 skatepark_lib-0.9.0/skatepark/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0     1113 2023-04-09 19:16:37.902211 skatepark_lib-0.9.0/skatepark/drivers/prompt/prompt_driver.py
--rw-r--r--   0        0        0      375 2023-04-09 19:16:37.971957 skatepark_lib-0.9.0/skatepark/memory/__init__.py
--rw-r--r--   0        0        0      782 2023-04-09 19:16:37.905682 skatepark_lib-0.9.0/skatepark/memory/buffer_pipeline_memory.py
--rw-r--r--   0        0        0     1865 2023-04-09 19:16:37.968000 skatepark_lib-0.9.0/skatepark/memory/pipeline_memory.py
--rw-r--r--   0        0        0      379 2023-04-09 19:16:37.974902 skatepark_lib-0.9.0/skatepark/memory/pipeline_run.py
--rw-r--r--   0        0        0     2095 2023-04-09 19:16:37.944454 skatepark_lib-0.9.0/skatepark/memory/summary_pipeline_memory.py
--rw-r--r--   0        0        0      127 2023-04-09 19:16:37.937590 skatepark_lib-0.9.0/skatepark/rules/__init__.py
--rw-r--r--   0        0        0      462 2023-04-09 19:16:37.962841 skatepark_lib-0.9.0/skatepark/rules/json.py
--rw-r--r--   0        0        0      496 2023-04-09 19:16:37.851877 skatepark_lib-0.9.0/skatepark/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 skatepark_lib-0.9.0/skatepark/rules/rule.py
--rw-r--r--   0        0        0     1878 2023-04-13 22:23:24.642957 skatepark_lib-0.9.0/skatepark/schemas/__init__.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 skatepark_lib-0.9.0/skatepark/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 skatepark_lib-0.9.0/skatepark/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      358 2023-04-09 19:16:37.960243 skatepark_lib-0.9.0/skatepark/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      415 2023-04-09 19:16:37.856681 skatepark_lib-0.9.0/skatepark/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 skatepark_lib-0.9.0/skatepark/schemas/memory/__init__.py
--rw-r--r--   0        0        0      372 2023-04-09 19:16:37.970264 skatepark_lib-0.9.0/skatepark/schemas/memory/buffer_pipeline_memory_schema.py
--rw-r--r--   0        0        0      427 2023-04-09 19:16:37.886475 skatepark_lib-0.9.0/skatepark/schemas/memory/pipeline_memory_schema.py
--rw-r--r--   0        0        0      376 2023-04-09 19:16:37.903213 skatepark_lib-0.9.0/skatepark/schemas/memory/pipeline_run_schema.py
--rw-r--r--   0        0        0      470 2023-04-09 19:16:37.838956 skatepark_lib-0.9.0/skatepark/schemas/memory/summary_pipeline_memory_schema.py
--rw-r--r--   0        0        0     5941 2023-04-09 19:16:37.926014 skatepark_lib-0.9.0/skatepark/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      266 2023-04-09 19:16:37.921761 skatepark_lib-0.9.0/skatepark/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 skatepark_lib-0.9.0/skatepark/schemas/steps/__init__.py
--rw-r--r--   0        0        0      457 2023-04-09 19:16:37.928827 skatepark_lib-0.9.0/skatepark/schemas/steps/prompt_step_schema.py
--rw-r--r--   0        0        0      461 2023-04-09 19:16:37.849997 skatepark_lib-0.9.0/skatepark/schemas/steps/step_schema.py
--rw-r--r--   0        0        0      565 2023-04-13 22:11:19.209260 skatepark_lib-0.9.0/skatepark/schemas/steps/toolkit_step_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/structures/__init__.py
--rw-r--r--   0        0        0      305 2023-04-09 19:16:37.833580 skatepark_lib-0.9.0/skatepark/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      511 2023-04-09 19:16:37.947893 skatepark_lib-0.9.0/skatepark/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      259 2023-04-09 19:16:37.950990 skatepark_lib-0.9.0/skatepark/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      354 2023-04-09 19:16:37.844498 skatepark_lib-0.9.0/skatepark/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      291 2023-04-09 19:16:37.930199 skatepark_lib-0.9.0/skatepark/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      338 2023-04-09 19:16:37.832543 skatepark_lib-0.9.0/skatepark/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      277 2023-04-13 22:23:24.638728 skatepark_lib-0.9.0/skatepark/steps/__init__.py
--rw-r--r--   0        0        0     1598 2023-04-13 22:11:19.209719 skatepark_lib-0.9.0/skatepark/steps/prompt_step.py
--rw-r--r--   0        0        0     3628 2023-04-13 22:11:19.209986 skatepark_lib-0.9.0/skatepark/steps/step.py
--rw-r--r--   0        0        0     5879 2023-04-13 22:23:24.641106 skatepark_lib-0.9.0/skatepark/steps/tool_substep.py
--rw-r--r--   0        0        0     2868 2023-04-13 22:23:24.631616 skatepark_lib-0.9.0/skatepark/steps/toolkit_step.py
--rw-r--r--   0        0        0      219 2023-04-09 19:16:37.849121 skatepark_lib-0.9.0/skatepark/structures/__init__.py
--rw-r--r--   0        0        0     3966 2023-04-09 19:16:37.885297 skatepark_lib-0.9.0/skatepark/structures/pipeline.py
--rw-r--r--   0        0        0     3813 2023-04-13 22:23:24.644750 skatepark_lib-0.9.0/skatepark/structures/structure.py
--rw-r--r--   0        0        0     3022 2023-04-09 19:16:37.842546 skatepark_lib-0.9.0/skatepark/structures/workflow.py
--rw-r--r--   0        0        0      199 2023-04-09 19:16:37.888328 skatepark_lib-0.9.0/skatepark/summarizers/__init__.py
--rw-r--r--   0        0        0      998 2023-04-09 19:16:37.933621 skatepark_lib-0.9.0/skatepark/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      499 2023-04-09 19:16:37.927872 skatepark_lib-0.9.0/skatepark/summarizers/summarizer.py
--rw-r--r--   0        0        0     1502 2023-04-13 22:11:19.211340 skatepark_lib-0.9.0/skatepark/templates/prompts/context.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 skatepark_lib-0.9.0/skatepark/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 skatepark_lib-0.9.0/skatepark/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 skatepark_lib-0.9.0/skatepark/templates/prompts/run_context.j2
--rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/prompt.j2
--rw-r--r--   0        0        0      359 2023-03-19 16:50:11.403035 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/substep.j2
--rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/substeps.j2
--rw-r--r--   0        0        0      175 2023-03-19 16:50:11.403268 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/tool.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 skatepark_lib-0.9.0/skatepark/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      173 2023-04-13 22:11:19.211596 skatepark_lib-0.9.0/skatepark/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 skatepark_lib-0.9.0/skatepark/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      470 2023-04-13 22:11:19.211853 skatepark_lib-0.9.0/skatepark/utils/__init__.py
--rw-r--r--   0        0        0      526 2023-04-09 19:16:37.955854 skatepark_lib-0.9.0/skatepark/utils/conversation.py
--rw-r--r--   0        0        0     1245 2023-04-09 19:16:37.965303 skatepark_lib-0.9.0/skatepark/utils/j2.py
--rw-r--r--   0        0        0     1790 2023-04-09 19:16:37.920470 skatepark_lib-0.9.0/skatepark/utils/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      629 2023-03-12 17:04:41.065886 skatepark_lib-0.9.0/skatepark/utils/tokenizer.py
--rw-r--r--   0        0        0      461 2023-04-13 22:11:19.211981 skatepark_lib-0.9.0/skatepark/utils/tool_loader.py
--rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 skatepark_lib-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 skatepark_lib-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3896 2023-04-13 22:14:02.910363 skatepark_lib-0.9.1/README.md
+-rw-r--r--   0        0        0      782 2023-04-14 20:13:18.292695 skatepark_lib-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 skatepark_lib-0.9.1/skatepark/__init__.py
+-rw-r--r--   0        0        0      258 2023-04-09 19:16:37.935258 skatepark_lib-0.9.1/skatepark/artifacts/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-09 19:16:37.880969 skatepark_lib-0.9.1/skatepark/artifacts/error_output.py
+-rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 skatepark_lib-0.9.1/skatepark/artifacts/structure_artifact.py
+-rw-r--r--   0        0        0      529 2023-04-09 19:16:37.958840 skatepark_lib-0.9.1/skatepark/artifacts/text_output.py
+-rw-r--r--   0        0        0      383 2023-04-09 19:16:37.961557 skatepark_lib-0.9.1/skatepark/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 skatepark_lib-0.9.1/skatepark/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      590 2023-04-09 19:16:37.834614 skatepark_lib-0.9.1/skatepark/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      263 2023-04-09 19:16:37.853167 skatepark_lib-0.9.1/skatepark/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 skatepark_lib-0.9.1/skatepark/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     2481 2023-04-09 19:16:37.884254 skatepark_lib-0.9.1/skatepark/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0     1113 2023-04-09 19:16:37.902211 skatepark_lib-0.9.1/skatepark/drivers/prompt/prompt_driver.py
+-rw-r--r--   0        0        0      375 2023-04-09 19:16:37.971957 skatepark_lib-0.9.1/skatepark/memory/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-09 19:16:37.905682 skatepark_lib-0.9.1/skatepark/memory/buffer_pipeline_memory.py
+-rw-r--r--   0        0        0     1865 2023-04-09 19:16:37.968000 skatepark_lib-0.9.1/skatepark/memory/pipeline_memory.py
+-rw-r--r--   0        0        0      379 2023-04-09 19:16:37.974902 skatepark_lib-0.9.1/skatepark/memory/pipeline_run.py
+-rw-r--r--   0        0        0     2095 2023-04-09 19:16:37.944454 skatepark_lib-0.9.1/skatepark/memory/summary_pipeline_memory.py
+-rw-r--r--   0        0        0      127 2023-04-09 19:16:37.937590 skatepark_lib-0.9.1/skatepark/rules/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-09 19:16:37.962841 skatepark_lib-0.9.1/skatepark/rules/json.py
+-rw-r--r--   0        0        0      496 2023-04-09 19:16:37.851877 skatepark_lib-0.9.1/skatepark/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 skatepark_lib-0.9.1/skatepark/rules/rule.py
+-rw-r--r--   0        0        0     1878 2023-04-13 22:23:24.642957 skatepark_lib-0.9.1/skatepark/schemas/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 skatepark_lib-0.9.1/skatepark/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 skatepark_lib-0.9.1/skatepark/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      358 2023-04-09 19:16:37.960243 skatepark_lib-0.9.1/skatepark/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      415 2023-04-09 19:16:37.856681 skatepark_lib-0.9.1/skatepark/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 skatepark_lib-0.9.1/skatepark/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-09 19:16:37.970264 skatepark_lib-0.9.1/skatepark/schemas/memory/buffer_pipeline_memory_schema.py
+-rw-r--r--   0        0        0      427 2023-04-09 19:16:37.886475 skatepark_lib-0.9.1/skatepark/schemas/memory/pipeline_memory_schema.py
+-rw-r--r--   0        0        0      376 2023-04-09 19:16:37.903213 skatepark_lib-0.9.1/skatepark/schemas/memory/pipeline_run_schema.py
+-rw-r--r--   0        0        0      470 2023-04-09 19:16:37.838956 skatepark_lib-0.9.1/skatepark/schemas/memory/summary_pipeline_memory_schema.py
+-rw-r--r--   0        0        0     5941 2023-04-09 19:16:37.926014 skatepark_lib-0.9.1/skatepark/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      266 2023-04-09 19:16:37.921761 skatepark_lib-0.9.1/skatepark/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 skatepark_lib-0.9.1/skatepark/schemas/steps/__init__.py
+-rw-r--r--   0        0        0      457 2023-04-09 19:16:37.928827 skatepark_lib-0.9.1/skatepark/schemas/steps/prompt_step_schema.py
+-rw-r--r--   0        0        0      461 2023-04-09 19:16:37.849997 skatepark_lib-0.9.1/skatepark/schemas/steps/step_schema.py
+-rw-r--r--   0        0        0      565 2023-04-13 22:11:19.209260 skatepark_lib-0.9.1/skatepark/schemas/steps/toolkit_step_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.1/skatepark/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      305 2023-04-09 19:16:37.833580 skatepark_lib-0.9.1/skatepark/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      511 2023-04-09 19:16:37.947893 skatepark_lib-0.9.1/skatepark/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      259 2023-04-09 19:16:37.950990 skatepark_lib-0.9.1/skatepark/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.1/skatepark/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      354 2023-04-09 19:16:37.844498 skatepark_lib-0.9.1/skatepark/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      291 2023-04-09 19:16:37.930199 skatepark_lib-0.9.1/skatepark/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.1/skatepark/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      338 2023-04-09 19:16:37.832543 skatepark_lib-0.9.1/skatepark/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      277 2023-04-13 22:23:24.638728 skatepark_lib-0.9.1/skatepark/steps/__init__.py
+-rw-r--r--   0        0        0     1598 2023-04-13 22:11:19.209719 skatepark_lib-0.9.1/skatepark/steps/prompt_step.py
+-rw-r--r--   0        0        0     3628 2023-04-13 22:11:19.209986 skatepark_lib-0.9.1/skatepark/steps/step.py
+-rw-r--r--   0        0        0     5880 2023-04-14 20:08:02.343830 skatepark_lib-0.9.1/skatepark/steps/tool_substep.py
+-rw-r--r--   0        0        0     2868 2023-04-13 22:23:24.631616 skatepark_lib-0.9.1/skatepark/steps/toolkit_step.py
+-rw-r--r--   0        0        0      219 2023-04-09 19:16:37.849121 skatepark_lib-0.9.1/skatepark/structures/__init__.py
+-rw-r--r--   0        0        0     3966 2023-04-09 19:16:37.885297 skatepark_lib-0.9.1/skatepark/structures/pipeline.py
+-rw-r--r--   0        0        0     3813 2023-04-13 22:23:24.644750 skatepark_lib-0.9.1/skatepark/structures/structure.py
+-rw-r--r--   0        0        0     3022 2023-04-09 19:16:37.842546 skatepark_lib-0.9.1/skatepark/structures/workflow.py
+-rw-r--r--   0        0        0      199 2023-04-09 19:16:37.888328 skatepark_lib-0.9.1/skatepark/summarizers/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-09 19:16:37.933621 skatepark_lib-0.9.1/skatepark/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      499 2023-04-09 19:16:37.927872 skatepark_lib-0.9.1/skatepark/summarizers/summarizer.py
+-rw-r--r--   0        0        0     1502 2023-04-13 22:11:19.211340 skatepark_lib-0.9.1/skatepark/templates/prompts/context.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 skatepark_lib-0.9.1/skatepark/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 skatepark_lib-0.9.1/skatepark/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 skatepark_lib-0.9.1/skatepark/templates/prompts/run_context.j2
+-rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 skatepark_lib-0.9.1/skatepark/templates/prompts/steps/prompt.j2
+-rw-r--r--   0        0        0      359 2023-03-19 16:50:11.403035 skatepark_lib-0.9.1/skatepark/templates/prompts/steps/tool/substep.j2
+-rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 skatepark_lib-0.9.1/skatepark/templates/prompts/steps/tool/substeps.j2
+-rw-r--r--   0        0        0      175 2023-03-19 16:50:11.403268 skatepark_lib-0.9.1/skatepark/templates/prompts/steps/tool/tool.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 skatepark_lib-0.9.1/skatepark/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      173 2023-04-13 22:11:19.211596 skatepark_lib-0.9.1/skatepark/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 skatepark_lib-0.9.1/skatepark/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      470 2023-04-13 22:11:19.211853 skatepark_lib-0.9.1/skatepark/utils/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 19:16:37.955854 skatepark_lib-0.9.1/skatepark/utils/conversation.py
+-rw-r--r--   0        0        0     1245 2023-04-09 19:16:37.965303 skatepark_lib-0.9.1/skatepark/utils/j2.py
+-rw-r--r--   0        0        0     1790 2023-04-09 19:16:37.920470 skatepark_lib-0.9.1/skatepark/utils/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      629 2023-03-12 17:04:41.065886 skatepark_lib-0.9.1/skatepark/utils/tokenizer.py
+-rw-r--r--   0        0        0      461 2023-04-13 22:11:19.211981 skatepark_lib-0.9.1/skatepark/utils/tool_loader.py
+-rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 skatepark_lib-0.9.1/PKG-INFO
```

### Comparing `skatepark_lib-0.9.0/LICENSE` & `skatepark_lib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/README.md` & `skatepark_lib-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/pyproject.toml` & `skatepark_lib-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skatepark-lib"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python framework for AI workflows and pipelines."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/skatepark"
 
 packages = [
```

### Comparing `skatepark_lib-0.9.0/skatepark/artifacts/text_output.py` & `skatepark_lib-0.9.1/skatepark/artifacts/text_output.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/drivers/memory/disk_memory_driver.py` & `skatepark_lib-0.9.1/skatepark/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/drivers/prompt/openai_prompt_driver.py` & `skatepark_lib-0.9.1/skatepark/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/drivers/prompt/prompt_driver.py` & `skatepark_lib-0.9.1/skatepark/drivers/prompt/prompt_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/memory/buffer_pipeline_memory.py` & `skatepark_lib-0.9.1/skatepark/memory/buffer_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/memory/pipeline_memory.py` & `skatepark_lib-0.9.1/skatepark/memory/pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/memory/summary_pipeline_memory.py` & `skatepark_lib-0.9.1/skatepark/memory/summary_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/schemas/__init__.py` & `skatepark_lib-0.9.1/skatepark/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/schemas/polymorphic_schema.py` & `skatepark_lib-0.9.1/skatepark/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/schemas/steps/toolkit_step_schema.py` & `skatepark_lib-0.9.1/skatepark/schemas/steps/toolkit_step_schema.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/steps/prompt_step.py` & `skatepark_lib-0.9.1/skatepark/steps/prompt_step.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/steps/step.py` & `skatepark_lib-0.9.1/skatepark/steps/step.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/steps/tool_substep.py` & `skatepark_lib-0.9.1/skatepark/steps/tool_substep.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,10 +145,9 @@
                 self.tool_name = "error"
                 self.tool_value = f"JSON validation error: {e}"
             except Exception as e:
                 self.structure.logger.error(f"Step {self.toolkit_step.id}\nError parsing tool action: {e}")
 
                 self.tool_name = "error"
                 self.tool_value = f"error: {self.INVALID_ACTION_ERROR_MSG}"
-
-        if self.output is None and len(output_matches) > 0:
+        elif self.output is None and len(output_matches) > 0:
             self.output = TextOutput(output_matches[-1])
```

### Comparing `skatepark_lib-0.9.0/skatepark/steps/toolkit_step.py` & `skatepark_lib-0.9.1/skatepark/steps/toolkit_step.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/structures/pipeline.py` & `skatepark_lib-0.9.1/skatepark/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/structures/structure.py` & `skatepark_lib-0.9.1/skatepark/structures/structure.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/structures/workflow.py` & `skatepark_lib-0.9.1/skatepark/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/summarizers/prompt_driver_summarizer.py` & `skatepark_lib-0.9.1/skatepark/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/templates/prompts/context.j2` & `skatepark_lib-0.9.1/skatepark/templates/prompts/context.j2`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/utils/conversation.py` & `skatepark_lib-0.9.1/skatepark/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/utils/j2.py` & `skatepark_lib-0.9.1/skatepark/utils/j2.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/utils/tiktoken_tokenizer.py` & `skatepark_lib-0.9.1/skatepark/utils/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/skatepark/utils/tokenizer.py` & `skatepark_lib-0.9.1/skatepark/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.9.0/PKG-INFO` & `skatepark_lib-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skatepark-lib
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python framework for AI workflows and pipelines.
 Home-page: https://github.com/griptape-ai/skatepark
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

