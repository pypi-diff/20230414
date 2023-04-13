# Comparing `tmp/skatepark_lib-0.8.0.tar.gz` & `tmp/skatepark_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skatepark_lib-0.8.0.tar", max compression
+gzip compressed data, was "skatepark_lib-0.9.0.tar", max compression
```

## Comparing `skatepark_lib-0.8.0.tar` & `skatepark_lib-0.9.0.tar`

### file list

```diff
@@ -1,140 +1,79 @@
--rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 skatepark_lib-0.8.0/LICENSE
--rw-r--r--   0        0        0    19575 2023-04-09 19:26:37.130061 skatepark_lib-0.8.0/README.md
--rw-r--r--   0        0        0      873 2023-04-09 20:05:08.331594 skatepark_lib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 skatepark_lib-0.8.0/skatepark/__init__.py
--rw-r--r--   0        0        0      258 2023-04-09 19:16:37.935258 skatepark_lib-0.8.0/skatepark/artifacts/__init__.py
--rw-r--r--   0        0        0      427 2023-04-09 19:16:37.880969 skatepark_lib-0.8.0/skatepark/artifacts/error_output.py
--rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 skatepark_lib-0.8.0/skatepark/artifacts/structure_artifact.py
--rw-r--r--   0        0        0      529 2023-04-09 19:16:37.958840 skatepark_lib-0.8.0/skatepark/artifacts/text_output.py
--rw-r--r--   0        0        0      383 2023-04-09 19:16:37.961557 skatepark_lib-0.8.0/skatepark/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 skatepark_lib-0.8.0/skatepark/drivers/memory/__init__.py
--rw-r--r--   0        0        0      590 2023-04-09 19:16:37.834614 skatepark_lib-0.8.0/skatepark/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      263 2023-04-09 19:16:37.853167 skatepark_lib-0.8.0/skatepark/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 skatepark_lib-0.8.0/skatepark/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     2481 2023-04-09 19:16:37.884254 skatepark_lib-0.8.0/skatepark/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0     1113 2023-04-09 19:16:37.902211 skatepark_lib-0.8.0/skatepark/drivers/prompt/prompt_driver.py
--rw-r--r--   0        0        0      375 2023-04-09 19:16:37.971957 skatepark_lib-0.8.0/skatepark/memory/__init__.py
--rw-r--r--   0        0        0      782 2023-04-09 19:16:37.905682 skatepark_lib-0.8.0/skatepark/memory/buffer_pipeline_memory.py
--rw-r--r--   0        0        0     1865 2023-04-09 19:16:37.968000 skatepark_lib-0.8.0/skatepark/memory/pipeline_memory.py
--rw-r--r--   0        0        0      379 2023-04-09 19:16:37.974902 skatepark_lib-0.8.0/skatepark/memory/pipeline_run.py
--rw-r--r--   0        0        0     2095 2023-04-09 19:16:37.944454 skatepark_lib-0.8.0/skatepark/memory/summary_pipeline_memory.py
--rw-r--r--   0        0        0      127 2023-04-09 19:16:37.937590 skatepark_lib-0.8.0/skatepark/rules/__init__.py
--rw-r--r--   0        0        0      462 2023-04-09 19:16:37.962841 skatepark_lib-0.8.0/skatepark/rules/json.py
--rw-r--r--   0        0        0      496 2023-04-09 19:16:37.851877 skatepark_lib-0.8.0/skatepark/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 skatepark_lib-0.8.0/skatepark/rules/rule.py
--rw-r--r--   0        0        0     3186 2023-04-09 19:16:37.918235 skatepark_lib-0.8.0/skatepark/schemas/__init__.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 skatepark_lib-0.8.0/skatepark/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 skatepark_lib-0.8.0/skatepark/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      358 2023-04-09 19:16:37.960243 skatepark_lib-0.8.0/skatepark/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      415 2023-04-09 19:16:37.856681 skatepark_lib-0.8.0/skatepark/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 skatepark_lib-0.8.0/skatepark/schemas/memory/__init__.py
--rw-r--r--   0        0        0      372 2023-04-09 19:16:37.970264 skatepark_lib-0.8.0/skatepark/schemas/memory/buffer_pipeline_memory_schema.py
--rw-r--r--   0        0        0      427 2023-04-09 19:16:37.886475 skatepark_lib-0.8.0/skatepark/schemas/memory/pipeline_memory_schema.py
--rw-r--r--   0        0        0      376 2023-04-09 19:16:37.903213 skatepark_lib-0.8.0/skatepark/schemas/memory/pipeline_run_schema.py
--rw-r--r--   0        0        0      470 2023-04-09 19:16:37.838956 skatepark_lib-0.8.0/skatepark/schemas/memory/summary_pipeline_memory_schema.py
--rw-r--r--   0        0        0     5941 2023-04-09 19:16:37.926014 skatepark_lib-0.8.0/skatepark/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      266 2023-04-09 19:16:37.921761 skatepark_lib-0.8.0/skatepark/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 skatepark_lib-0.8.0/skatepark/schemas/steps/__init__.py
--rw-r--r--   0        0        0      457 2023-04-09 19:16:37.928827 skatepark_lib-0.8.0/skatepark/schemas/steps/prompt_step_schema.py
--rw-r--r--   0        0        0      461 2023-04-09 19:16:37.849997 skatepark_lib-0.8.0/skatepark/schemas/steps/step_schema.py
--rw-r--r--   0        0        0      544 2023-04-09 19:16:37.845354 skatepark_lib-0.8.0/skatepark/schemas/steps/tool_step_schema.py
--rw-r--r--   0        0        0      582 2023-04-09 19:16:37.926929 skatepark_lib-0.8.0/skatepark/schemas/steps/toolkit_step_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.8.0/skatepark/schemas/structures/__init__.py
--rw-r--r--   0        0        0      305 2023-04-09 19:16:37.833580 skatepark_lib-0.8.0/skatepark/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      511 2023-04-09 19:16:37.947893 skatepark_lib-0.8.0/skatepark/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      259 2023-04-09 19:16:37.950990 skatepark_lib-0.8.0/skatepark/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.8.0/skatepark/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      354 2023-04-09 19:16:37.844498 skatepark_lib-0.8.0/skatepark/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      291 2023-04-09 19:16:37.930199 skatepark_lib-0.8.0/skatepark/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.8.0/skatepark/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      338 2023-04-09 19:16:37.832543 skatepark_lib-0.8.0/skatepark/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070827 skatepark_lib-0.8.0/skatepark/schemas/tools/__init__.py
--rw-r--r--   0        0        0      276 2023-04-09 19:16:37.943094 skatepark_lib-0.8.0/skatepark/schemas/tools/aws_tool_schema.py
--rw-r--r--   0        0        0      262 2023-04-09 19:16:37.831353 skatepark_lib-0.8.0/skatepark/schemas/tools/calculator_tool_schema.py
--rw-r--r--   0        0        0      343 2023-04-09 19:16:37.966665 skatepark_lib-0.8.0/skatepark/schemas/tools/data_scientist_tool_schema.py
--rw-r--r--   0        0        0      419 2023-04-09 19:16:37.847123 skatepark_lib-0.8.0/skatepark/schemas/tools/email_sender_tool_schema.py
--rw-r--r--   0        0        0      487 2023-04-09 19:16:37.957846 skatepark_lib-0.8.0/skatepark/schemas/tools/google_search_tool_schema.py
--rw-r--r--   0        0        0      423 2023-04-09 19:16:37.878817 skatepark_lib-0.8.0/skatepark/schemas/tools/google_sheets_reader_tool_schema.py
--rw-r--r--   0        0        0      423 2023-04-09 19:16:37.932437 skatepark_lib-0.8.0/skatepark/schemas/tools/google_sheets_writer_tool_schema.py
--rw-r--r--   0        0        0      256 2023-04-09 19:16:37.919391 skatepark_lib-0.8.0/skatepark/schemas/tools/ping_pong_tool_schema.py
--rw-r--r--   0        0        0      355 2023-04-09 19:16:37.895875 skatepark_lib-0.8.0/skatepark/schemas/tools/sql_client_tool_schema.py
--rw-r--r--   0        0        0      305 2023-04-09 19:16:37.841684 skatepark_lib-0.8.0/skatepark/schemas/tools/web_scraper_tool_schema.py
--rw-r--r--   0        0        0      244 2023-04-09 19:16:37.897058 skatepark_lib-0.8.0/skatepark/schemas/tools/wiki_tool_schema.py
--rw-r--r--   0        0        0      416 2023-04-09 19:16:37.940985 skatepark_lib-0.8.0/skatepark/steps/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-09 19:16:37.910730 skatepark_lib-0.8.0/skatepark/steps/base_tool_step.py
--rw-r--r--   0        0        0     1575 2023-04-09 19:16:37.846177 skatepark_lib-0.8.0/skatepark/steps/prompt_step.py
--rw-r--r--   0        0        0     3641 2023-04-09 19:16:37.904356 skatepark_lib-0.8.0/skatepark/steps/step.py
--rw-r--r--   0        0        0      412 2023-04-09 19:16:37.914630 skatepark_lib-0.8.0/skatepark/steps/tool_step.py
--rw-r--r--   0        0        0     5248 2023-04-09 19:16:37.976012 skatepark_lib-0.8.0/skatepark/steps/tool_substep.py
--rw-r--r--   0        0        0      400 2023-04-09 19:16:37.850918 skatepark_lib-0.8.0/skatepark/steps/toolkit_step.py
--rw-r--r--   0        0        0      219 2023-04-09 19:16:37.849121 skatepark_lib-0.8.0/skatepark/structures/__init__.py
--rw-r--r--   0        0        0     3966 2023-04-09 19:16:37.885297 skatepark_lib-0.8.0/skatepark/structures/pipeline.py
--rw-r--r--   0        0        0     3733 2023-04-09 19:16:37.837949 skatepark_lib-0.8.0/skatepark/structures/structure.py
--rw-r--r--   0        0        0     3022 2023-04-09 19:16:37.842546 skatepark_lib-0.8.0/skatepark/structures/workflow.py
--rw-r--r--   0        0        0      199 2023-04-09 19:16:37.888328 skatepark_lib-0.8.0/skatepark/summarizers/__init__.py
--rw-r--r--   0        0        0      998 2023-04-09 19:16:37.933621 skatepark_lib-0.8.0/skatepark/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      499 2023-04-09 19:16:37.927872 skatepark_lib-0.8.0/skatepark/summarizers/summarizer.py
--rw-r--r--   0        0        0     1433 2023-03-24 16:30:49.955192 skatepark_lib-0.8.0/skatepark/templates/prompts/context.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 skatepark_lib-0.8.0/skatepark/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 skatepark_lib-0.8.0/skatepark/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 skatepark_lib-0.8.0/skatepark/templates/prompts/run_context.j2
--rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 skatepark_lib-0.8.0/skatepark/templates/prompts/steps/prompt.j2
--rw-r--r--   0        0        0      359 2023-03-19 16:50:11.403035 skatepark_lib-0.8.0/skatepark/templates/prompts/steps/tool/substep.j2
--rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 skatepark_lib-0.8.0/skatepark/templates/prompts/steps/tool/substeps.j2
--rw-r--r--   0        0        0      175 2023-03-19 16:50:11.403268 skatepark_lib-0.8.0/skatepark/templates/prompts/steps/tool/tool.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 skatepark_lib-0.8.0/skatepark/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      209 2023-03-12 18:01:18.915639 skatepark_lib-0.8.0/skatepark/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 skatepark_lib-0.8.0/skatepark/templates/prompts/workflow.j2
--rw-r--r--   0        0        0     1120 2023-04-09 19:16:37.839852 skatepark_lib-0.8.0/skatepark/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 00:10:24.597398 skatepark_lib-0.8.0/skatepark/tools/aws/__init__.py
--rw-r--r--   0        0        0      769 2023-04-09 19:16:37.879914 skatepark_lib-0.8.0/skatepark/tools/aws/aws_tool.py
--rw-r--r--   0        0        0      377 2023-03-19 16:50:11.403696 skatepark_lib-0.8.0/skatepark/tools/aws/examples.j2
--rw-r--r--   0        0        0      446 2023-03-12 20:40:41.958970 skatepark_lib-0.8.0/skatepark/tools/aws/schema.json
--rw-r--r--   0        0        0        0 2023-03-07 16:53:11.944208 skatepark_lib-0.8.0/skatepark/tools/calculator/__init__.py
--rw-r--r--   0        0        0      215 2023-04-09 19:16:37.969117 skatepark_lib-0.8.0/skatepark/tools/calculator/calculator_tool.py
--rw-r--r--   0        0        0      577 2023-03-19 16:50:11.403886 skatepark_lib-0.8.0/skatepark/tools/calculator/examples.j2
--rw-r--r--   0        0        0      498 2023-03-24 16:30:49.955782 skatepark_lib-0.8.0/skatepark/tools/calculator/schema.json
--rw-r--r--   0        0        0        0 2023-03-07 16:53:11.944628 skatepark_lib-0.8.0/skatepark/tools/data_scientist/__init__.py
--rw-r--r--   0        0        0      508 2023-04-09 19:16:37.836787 skatepark_lib-0.8.0/skatepark/tools/data_scientist/data_scientist_tool.py
--rw-r--r--   0        0        0      962 2023-03-19 16:50:11.404327 skatepark_lib-0.8.0/skatepark/tools/data_scientist/examples.j2
--rw-r--r--   0        0        0      453 2023-03-09 17:10:04.855497 skatepark_lib-0.8.0/skatepark/tools/data_scientist/schema.json
--rw-r--r--   0        0        0        0 2023-03-24 16:30:49.955818 skatepark_lib-0.8.0/skatepark/tools/email_sender/__init__.py
--rw-r--r--   0        0        0     1262 2023-04-09 19:16:37.936364 skatepark_lib-0.8.0/skatepark/tools/email_sender/email_sender_tool.py
--rw-r--r--   0        0        0      571 2023-04-09 19:16:37.973575 skatepark_lib-0.8.0/skatepark/tools/email_sender/examples.j2
--rw-r--r--   0        0        0      795 2023-03-24 16:30:49.956404 skatepark_lib-0.8.0/skatepark/tools/email_sender/schema.json
--rw-r--r--   0        0        0        0 2023-03-24 16:30:49.956479 skatepark_lib-0.8.0/skatepark/tools/google_search/__init__.py
--rw-r--r--   0        0        0      916 2023-03-24 16:30:49.956647 skatepark_lib-0.8.0/skatepark/tools/google_search/examples.j2
--rw-r--r--   0        0        0     2284 2023-04-09 19:16:37.889702 skatepark_lib-0.8.0/skatepark/tools/google_search/google_search_tool.py
--rw-r--r--   0        0        0      445 2023-03-24 16:30:49.956977 skatepark_lib-0.8.0/skatepark/tools/google_search/schema.json
--rw-r--r--   0        0        0        0 2023-03-09 17:10:04.855988 skatepark_lib-0.8.0/skatepark/tools/google_sheets_reader/__init__.py
--rw-r--r--   0        0        0      463 2023-04-09 19:26:37.126587 skatepark_lib-0.8.0/skatepark/tools/google_sheets_reader/examples.j2
--rw-r--r--   0        0        0     1267 2023-04-09 19:16:37.901255 skatepark_lib-0.8.0/skatepark/tools/google_sheets_reader/google_sheets_reader_tool.py
--rw-r--r--   0        0        0     1336 2023-03-09 17:10:04.856649 skatepark_lib-0.8.0/skatepark/tools/google_sheets_reader/schema.json
--rw-r--r--   0        0        0        0 2023-03-09 17:10:04.856720 skatepark_lib-0.8.0/skatepark/tools/google_sheets_writer/__init__.py
--rw-r--r--   0        0        0      447 2023-03-19 16:50:11.404927 skatepark_lib-0.8.0/skatepark/tools/google_sheets_writer/examples.j2
--rw-r--r--   0        0        0     1263 2023-04-09 19:16:37.908407 skatepark_lib-0.8.0/skatepark/tools/google_sheets_writer/google_sheets_writer_tool.py
--rw-r--r--   0        0        0     1808 2023-03-10 17:02:35.587913 skatepark_lib-0.8.0/skatepark/tools/google_sheets_writer/schema.json
--rw-r--r--   0        0        0        0 2023-03-07 16:53:11.945249 skatepark_lib-0.8.0/skatepark/tools/pingpong/__init__.py
--rw-r--r--   0        0        0      152 2023-04-09 19:16:37.882033 skatepark_lib-0.8.0/skatepark/tools/pingpong/ping_pong_tool.py
--rw-r--r--   0        0        0      384 2023-03-09 17:10:04.857263 skatepark_lib-0.8.0/skatepark/tools/pingpong/schema.json
--rw-r--r--   0        0        0        0 2023-03-10 19:50:27.271158 skatepark_lib-0.8.0/skatepark/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      826 2023-03-19 16:50:11.405099 skatepark_lib-0.8.0/skatepark/tools/sql_client/examples.j2
--rw-r--r--   0        0        0      504 2023-03-10 19:50:27.271425 skatepark_lib-0.8.0/skatepark/tools/sql_client/schema.json
--rw-r--r--   0        0        0      810 2023-04-09 19:16:37.883152 skatepark_lib-0.8.0/skatepark/tools/sql_client/sql_client_tool.py
--rw-r--r--   0        0        0     1587 2023-04-09 19:16:37.942035 skatepark_lib-0.8.0/skatepark/tools/tool.py
--rw-r--r--   0        0        0        0 2023-03-24 16:30:49.957471 skatepark_lib-0.8.0/skatepark/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      533 2023-04-09 19:26:37.133618 skatepark_lib-0.8.0/skatepark/tools/web_scraper/examples.j2
--rw-r--r--   0        0        0     1223 2023-03-24 16:30:49.957861 skatepark_lib-0.8.0/skatepark/tools/web_scraper/schema.json
--rw-r--r--   0        0        0     2053 2023-04-09 19:16:37.939792 skatepark_lib-0.8.0/skatepark/tools/web_scraper/web_scraper_tool.py
--rw-r--r--   0        0        0        0 2023-03-07 16:53:11.945821 skatepark_lib-0.8.0/skatepark/tools/wiki/__init__.py
--rw-r--r--   0        0        0      344 2023-03-19 16:50:11.405286 skatepark_lib-0.8.0/skatepark/tools/wiki/examples.j2
--rw-r--r--   0        0        0      753 2023-03-09 17:10:04.857772 skatepark_lib-0.8.0/skatepark/tools/wiki/schema.json
--rw-r--r--   0        0        0     1356 2023-04-09 19:16:37.946455 skatepark_lib-0.8.0/skatepark/tools/wiki/wiki_tool.py
--rw-r--r--   0        0        0      554 2023-04-09 19:16:37.912063 skatepark_lib-0.8.0/skatepark/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 skatepark_lib-0.8.0/skatepark/utils/command_runner.py
--rw-r--r--   0        0        0      526 2023-04-09 19:16:37.955854 skatepark_lib-0.8.0/skatepark/utils/conversation.py
--rw-r--r--   0        0        0     1245 2023-04-09 19:16:37.965303 skatepark_lib-0.8.0/skatepark/utils/j2.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 skatepark_lib-0.8.0/skatepark/utils/python_runner.py
--rw-r--r--   0        0        0     1790 2023-04-09 19:16:37.920470 skatepark_lib-0.8.0/skatepark/utils/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      629 2023-03-12 17:04:41.065886 skatepark_lib-0.8.0/skatepark/utils/tokenizer.py
--rw-r--r--   0        0        0    20756 1970-01-01 00:00:00.000000 skatepark_lib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 skatepark_lib-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3896 2023-04-13 22:14:02.910363 skatepark_lib-0.9.0/README.md
+-rw-r--r--   0        0        0      782 2023-04-13 22:24:14.751322 skatepark_lib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 skatepark_lib-0.9.0/skatepark/__init__.py
+-rw-r--r--   0        0        0      258 2023-04-09 19:16:37.935258 skatepark_lib-0.9.0/skatepark/artifacts/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-09 19:16:37.880969 skatepark_lib-0.9.0/skatepark/artifacts/error_output.py
+-rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 skatepark_lib-0.9.0/skatepark/artifacts/structure_artifact.py
+-rw-r--r--   0        0        0      529 2023-04-09 19:16:37.958840 skatepark_lib-0.9.0/skatepark/artifacts/text_output.py
+-rw-r--r--   0        0        0      383 2023-04-09 19:16:37.961557 skatepark_lib-0.9.0/skatepark/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 skatepark_lib-0.9.0/skatepark/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      590 2023-04-09 19:16:37.834614 skatepark_lib-0.9.0/skatepark/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      263 2023-04-09 19:16:37.853167 skatepark_lib-0.9.0/skatepark/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 skatepark_lib-0.9.0/skatepark/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     2481 2023-04-09 19:16:37.884254 skatepark_lib-0.9.0/skatepark/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0     1113 2023-04-09 19:16:37.902211 skatepark_lib-0.9.0/skatepark/drivers/prompt/prompt_driver.py
+-rw-r--r--   0        0        0      375 2023-04-09 19:16:37.971957 skatepark_lib-0.9.0/skatepark/memory/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-09 19:16:37.905682 skatepark_lib-0.9.0/skatepark/memory/buffer_pipeline_memory.py
+-rw-r--r--   0        0        0     1865 2023-04-09 19:16:37.968000 skatepark_lib-0.9.0/skatepark/memory/pipeline_memory.py
+-rw-r--r--   0        0        0      379 2023-04-09 19:16:37.974902 skatepark_lib-0.9.0/skatepark/memory/pipeline_run.py
+-rw-r--r--   0        0        0     2095 2023-04-09 19:16:37.944454 skatepark_lib-0.9.0/skatepark/memory/summary_pipeline_memory.py
+-rw-r--r--   0        0        0      127 2023-04-09 19:16:37.937590 skatepark_lib-0.9.0/skatepark/rules/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-09 19:16:37.962841 skatepark_lib-0.9.0/skatepark/rules/json.py
+-rw-r--r--   0        0        0      496 2023-04-09 19:16:37.851877 skatepark_lib-0.9.0/skatepark/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 skatepark_lib-0.9.0/skatepark/rules/rule.py
+-rw-r--r--   0        0        0     1878 2023-04-13 22:23:24.642957 skatepark_lib-0.9.0/skatepark/schemas/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 skatepark_lib-0.9.0/skatepark/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 skatepark_lib-0.9.0/skatepark/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      358 2023-04-09 19:16:37.960243 skatepark_lib-0.9.0/skatepark/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      415 2023-04-09 19:16:37.856681 skatepark_lib-0.9.0/skatepark/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 skatepark_lib-0.9.0/skatepark/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-09 19:16:37.970264 skatepark_lib-0.9.0/skatepark/schemas/memory/buffer_pipeline_memory_schema.py
+-rw-r--r--   0        0        0      427 2023-04-09 19:16:37.886475 skatepark_lib-0.9.0/skatepark/schemas/memory/pipeline_memory_schema.py
+-rw-r--r--   0        0        0      376 2023-04-09 19:16:37.903213 skatepark_lib-0.9.0/skatepark/schemas/memory/pipeline_run_schema.py
+-rw-r--r--   0        0        0      470 2023-04-09 19:16:37.838956 skatepark_lib-0.9.0/skatepark/schemas/memory/summary_pipeline_memory_schema.py
+-rw-r--r--   0        0        0     5941 2023-04-09 19:16:37.926014 skatepark_lib-0.9.0/skatepark/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      266 2023-04-09 19:16:37.921761 skatepark_lib-0.9.0/skatepark/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 skatepark_lib-0.9.0/skatepark/schemas/steps/__init__.py
+-rw-r--r--   0        0        0      457 2023-04-09 19:16:37.928827 skatepark_lib-0.9.0/skatepark/schemas/steps/prompt_step_schema.py
+-rw-r--r--   0        0        0      461 2023-04-09 19:16:37.849997 skatepark_lib-0.9.0/skatepark/schemas/steps/step_schema.py
+-rw-r--r--   0        0        0      565 2023-04-13 22:11:19.209260 skatepark_lib-0.9.0/skatepark/schemas/steps/toolkit_step_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      305 2023-04-09 19:16:37.833580 skatepark_lib-0.9.0/skatepark/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      511 2023-04-09 19:16:37.947893 skatepark_lib-0.9.0/skatepark/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      259 2023-04-09 19:16:37.950990 skatepark_lib-0.9.0/skatepark/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      354 2023-04-09 19:16:37.844498 skatepark_lib-0.9.0/skatepark/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      291 2023-04-09 19:16:37.930199 skatepark_lib-0.9.0/skatepark/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 skatepark_lib-0.9.0/skatepark/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      338 2023-04-09 19:16:37.832543 skatepark_lib-0.9.0/skatepark/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      277 2023-04-13 22:23:24.638728 skatepark_lib-0.9.0/skatepark/steps/__init__.py
+-rw-r--r--   0        0        0     1598 2023-04-13 22:11:19.209719 skatepark_lib-0.9.0/skatepark/steps/prompt_step.py
+-rw-r--r--   0        0        0     3628 2023-04-13 22:11:19.209986 skatepark_lib-0.9.0/skatepark/steps/step.py
+-rw-r--r--   0        0        0     5879 2023-04-13 22:23:24.641106 skatepark_lib-0.9.0/skatepark/steps/tool_substep.py
+-rw-r--r--   0        0        0     2868 2023-04-13 22:23:24.631616 skatepark_lib-0.9.0/skatepark/steps/toolkit_step.py
+-rw-r--r--   0        0        0      219 2023-04-09 19:16:37.849121 skatepark_lib-0.9.0/skatepark/structures/__init__.py
+-rw-r--r--   0        0        0     3966 2023-04-09 19:16:37.885297 skatepark_lib-0.9.0/skatepark/structures/pipeline.py
+-rw-r--r--   0        0        0     3813 2023-04-13 22:23:24.644750 skatepark_lib-0.9.0/skatepark/structures/structure.py
+-rw-r--r--   0        0        0     3022 2023-04-09 19:16:37.842546 skatepark_lib-0.9.0/skatepark/structures/workflow.py
+-rw-r--r--   0        0        0      199 2023-04-09 19:16:37.888328 skatepark_lib-0.9.0/skatepark/summarizers/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-09 19:16:37.933621 skatepark_lib-0.9.0/skatepark/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      499 2023-04-09 19:16:37.927872 skatepark_lib-0.9.0/skatepark/summarizers/summarizer.py
+-rw-r--r--   0        0        0     1502 2023-04-13 22:11:19.211340 skatepark_lib-0.9.0/skatepark/templates/prompts/context.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 skatepark_lib-0.9.0/skatepark/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 skatepark_lib-0.9.0/skatepark/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 skatepark_lib-0.9.0/skatepark/templates/prompts/run_context.j2
+-rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/prompt.j2
+-rw-r--r--   0        0        0      359 2023-03-19 16:50:11.403035 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/substep.j2
+-rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/substeps.j2
+-rw-r--r--   0        0        0      175 2023-03-19 16:50:11.403268 skatepark_lib-0.9.0/skatepark/templates/prompts/steps/tool/tool.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 skatepark_lib-0.9.0/skatepark/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      173 2023-04-13 22:11:19.211596 skatepark_lib-0.9.0/skatepark/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 skatepark_lib-0.9.0/skatepark/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      470 2023-04-13 22:11:19.211853 skatepark_lib-0.9.0/skatepark/utils/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 19:16:37.955854 skatepark_lib-0.9.0/skatepark/utils/conversation.py
+-rw-r--r--   0        0        0     1245 2023-04-09 19:16:37.965303 skatepark_lib-0.9.0/skatepark/utils/j2.py
+-rw-r--r--   0        0        0     1790 2023-04-09 19:16:37.920470 skatepark_lib-0.9.0/skatepark/utils/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      629 2023-03-12 17:04:41.065886 skatepark_lib-0.9.0/skatepark/utils/tokenizer.py
+-rw-r--r--   0        0        0      461 2023-04-13 22:11:19.211981 skatepark_lib-0.9.0/skatepark/utils/tool_loader.py
+-rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 skatepark_lib-0.9.0/PKG-INFO
```

### Comparing `skatepark_lib-0.8.0/LICENSE` & `skatepark_lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/pyproject.toml` & `skatepark_lib-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 [tool.poetry]
 name = "skatepark-lib"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python framework for AI workflows and pipelines."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/skatepark"
 
 packages = [
     {include = "skatepark"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
+griptape-core = ">= 0.7.2"
 python-dotenv = ">=0.21"
 openai = ">=0.27"
 attrs = ">=22"
 jinja2 = ">=3.1"
 jsonschema = ">=4"
 marshmallow = ">=3"
 marshmallow-enum = ">=1.5"
 graphlib = "*"
-llama_index = "0.4.23"
-wikipedia = "*"
 tiktoken = ">=0.3"
-gspread = "*"
-sqlalchemy = ">1"
 rich = ">=13"
-trafilatura = "*"
-requests = "*"
-warpspeed-googlesearch-python = ">=1.1.1"
 stopit = "*"
 
 [tool.poetry.group.test.dependencies]
+griptape-tools = ">= 0.5.1"
 pytest = "~=7.1"
 pytest-cover = "*"
 twine = ">=4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `skatepark_lib-0.8.0/skatepark/artifacts/text_output.py` & `skatepark_lib-0.9.0/skatepark/artifacts/text_output.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/drivers/memory/disk_memory_driver.py` & `skatepark_lib-0.9.0/skatepark/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/drivers/prompt/openai_prompt_driver.py` & `skatepark_lib-0.9.0/skatepark/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/drivers/prompt/prompt_driver.py` & `skatepark_lib-0.9.0/skatepark/drivers/prompt/prompt_driver.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/memory/buffer_pipeline_memory.py` & `skatepark_lib-0.9.0/skatepark/memory/buffer_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/memory/pipeline_memory.py` & `skatepark_lib-0.9.0/skatepark/memory/pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/memory/summary_pipeline_memory.py` & `skatepark_lib-0.9.0/skatepark/memory/summary_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/schemas/polymorphic_schema.py` & `skatepark_lib-0.9.0/skatepark/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/schemas/steps/tool_step_schema.py` & `skatepark_lib-0.9.0/skatepark/schemas/steps/toolkit_step_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from marshmallow import fields, post_load
 from skatepark.schemas import PolymorphicSchema, StepSchema
 
 
-class ToolStepSchema(StepSchema):
+class ToolkitStepSchema(StepSchema):
     prompt_template = fields.Str(required=True)
-    max_substeps = fields.Int()
-    tool = fields.Nested(PolymorphicSchema(), required=True)
+    max_substeps = fields.Int(allow_none=True)
+    tool_names = fields.List(fields.Str(), required=True)
     context = fields.Dict(keys=fields.Str(), values=fields.Raw())
     driver = fields.Nested(PolymorphicSchema(), allow_none=True)
 
     @post_load
     def make_obj(self, data, **kwargs):
-        from skatepark.steps import ToolStep
+        from skatepark.steps import ToolkitStep
 
-        return ToolStep(**data)
+        return ToolkitStep(**data)
```

### Comparing `skatepark_lib-0.8.0/skatepark/steps/base_tool_step.py` & `skatepark_lib-0.9.0/skatepark/steps/toolkit_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
-from skatepark.tools import Tool
+from griptape.core import BaseTool
 from skatepark.utils import J2
 from skatepark.steps import PromptStep
 from skatepark.artifacts import TextOutput, ErrorOutput
 
 if TYPE_CHECKING:
     from skatepark.steps import ToolSubstep
 
 
 @define
-class BaseToolStep(PromptStep, ABC):
+class ToolkitStep(PromptStep, ABC):
     DEFAULT_MAX_SUBSTEPS = 20
 
+    tool_names: list[str] = field(kw_only=True)
     max_substeps: int = field(default=DEFAULT_MAX_SUBSTEPS, kw_only=True)
     _substeps: list[ToolSubstep] = field(factory=list)
 
+    @property
+    def tools(self) -> list[BaseTool]:
+        return [
+            t for t in [self.structure.tool_loader.load_tool(t) for t in self.tool_names] if t is not None
+        ]
+
     def run(self) -> TextOutput:
         from skatepark.steps import ToolSubstep
 
         self._substeps.clear()
 
         substep = self.add_substep(
             ToolSubstep(
@@ -71,10 +78,12 @@
         if len(self._substeps) > 0:
             self._substeps[-1].add_child(substep)
 
         self._substeps.append(substep)
 
         return substep
 
-    @abstractmethod
-    def find_tool(self, tool_name: str) -> Optional[Tool]:
-        ...
+    def find_tool(self, tool_name: str) -> Optional[BaseTool]:
+        return next(
+            (t for t in self.tools if t.name == tool_name),
+            None
+        )
```

### Comparing `skatepark_lib-0.8.0/skatepark/steps/prompt_step.py` & `skatepark_lib-0.9.0/skatepark/steps/prompt_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if TYPE_CHECKING:
     from skatepark.drivers import PromptDriver
 
 
 @define
 class PromptStep(Step):
-    prompt_template: str = field()
+    prompt_template: str = field(default="{{ args[0] }}")
     context: dict[str, any] = field(factory=dict, kw_only=True)
     driver: Optional[PromptDriver] = field(default=None, kw_only=True)
 
     def before_run(self) -> None:
         super().before_run()
 
         self.structure.logger.info(f"Step {self.id}\nInput: {self.render_prompt()}")
```

### Comparing `skatepark_lib-0.8.0/skatepark/steps/step.py` & `skatepark_lib-0.9.0/skatepark/steps/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
             self.before_run()
 
             self.output = self.run()
 
             self.after_run()
         except Exception as e:
-            self.structure.logger.error(f"Step {self.id}\nError: {type(e).__name__ }({e})")
+            self.structure.logger.error(f"Step {self.id}\n{e}", exc_info=True)
 
             self.output = ErrorOutput(str(e), exception=e, step=self)
         finally:
             self.state = Step.State.FINISHED
 
             return self.output
```

### Comparing `skatepark_lib-0.8.0/skatepark/steps/tool_substep.py` & `skatepark_lib-0.9.0/skatepark/steps/tool_substep.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,69 +3,73 @@
 import re
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import validate
 from skatepark.artifacts import TextOutput, ErrorOutput
 from skatepark.steps import PromptStep
-from skatepark.tools import Tool
+from griptape.core import BaseTool
 from skatepark.utils import J2
 
 if TYPE_CHECKING:
     from skatepark.artifacts import StructureArtifact
-    from skatepark.steps import BaseToolStep
+    from skatepark.steps import ToolkitStep
 
 
 @define
 class ToolSubstep(PromptStep):
     THOUGHT_PATTERN = r"^Thought:\s*(.*)$"
     ACTION_PATTERN = r"^Action:\s*({.*})$"
     OUTPUT_PATTERN = r"^Output:\s?([\s\S]*)$"
     INVALID_ACTION_ERROR_MSG = f"invalid action input, try again"
 
-    tool_step_id: Optional[str] = field(default=None, kw_only=True)
+    parent_step_id: Optional[str] = field(default=None, kw_only=True)
     thought: Optional[str] = field(default=None, kw_only=True)
     tool_name: Optional[str] = field(default=None, kw_only=True)
-    tool_input: Optional[str] = field(default=None, kw_only=True)
+    tool_action: Optional[str] = field(default=None, kw_only=True)
+    tool_value: Optional[str] = field(default=None, kw_only=True)
 
-    __tool: Optional[Tool] = None
+    _tool: Optional[BaseTool] = None
 
-    def attach(self, tool_step: BaseToolStep):
-        self.tool_step_id = tool_step.id
-        self.structure = tool_step.structure
+    def attach(self, parent_step: ToolkitStep):
+        self.parent_step_id = parent_step.id
+        self.structure = parent_step.structure
         self.__init_from_prompt(self.render_prompt())
 
     @property
-    def tool_step(self) -> Optional[BaseToolStep]:
-        return self.structure.find_step(self.tool_step_id)
+    def toolkit_step(self) -> Optional[ToolkitStep]:
+        return self.structure.find_step(self.parent_step_id)
 
     @property
     def parents(self) -> list[ToolSubstep]:
-        return [self.tool_step.find_substep(parent_id) for parent_id in self.parent_ids]
+        return [self.toolkit_step.find_substep(parent_id) for parent_id in self.parent_ids]
 
     @property
     def children(self) -> list[ToolSubstep]:
-        return [self.tool_step.find_substep(child_id) for child_id in self.child_ids]
+        return [self.toolkit_step.find_substep(child_id) for child_id in self.child_ids]
 
     def before_run(self) -> None:
         self.structure.logger.info(f"Substep {self.id}\n{self.render_prompt()}")
 
     def run(self) -> StructureArtifact:
         try:
             if self.tool_name == "error":
-                self.output = ErrorOutput(self.tool_input, step=self)
+                self.output = ErrorOutput(self.tool_value, step=self)
             else:
-                if self.__tool:
-                    observation = self.__tool.run(self.tool_input)
+                if self._tool:
+                    observation = self.structure.tool_loader.executor.execute(
+                        getattr(self._tool, self.tool_action),
+                        self.tool_value.encode()
+                    ).decode()
                 else:
                     observation = "tool not found"
 
                 self.output = TextOutput(observation)
         except Exception as e:
-            self.structure.logger.error(f"Substep {self.id}\nError: {type(e).__name__ }({e})")
+            self.structure.logger.error(f"Substep {self.id}\n{e}", exc_info=True)
 
             self.output = ErrorOutput(str(e), exception=e, step=self)
         finally:
             return self.output
 
     def after_run(self) -> None:
         self.structure.logger.info(f"Substep {self.id}\nObservation: {self.output.value}")
@@ -105,37 +109,46 @@
             try:
                 parsed_value = ast.literal_eval(action_matches[-1])
 
                 # Load the tool name; throw exception if the key is not present
                 if self.tool_name is None:
                     self.tool_name = parsed_value["tool"]
 
+                # Load the tool action; throw exception if the key is not present
+                if self.tool_action is None:
+                    self.tool_action = parsed_value["action"]
+
                 # Load the tool itself
                 if self.tool_name:
-                    self.__tool = self.tool_step.find_tool(self.tool_name)
+                    self._tool = self.toolkit_step.find_tool(self.tool_name)
 
                 # Validate input based on tool schema
-                if self.__tool:
-                    validate(instance=parsed_value, schema=self.__tool.schema)
-
-                # Load optional input; don't throw exceptions if key is not present
-                if self.tool_input is None:
-                    self.tool_input = parsed_value.get("input")
+                if self._tool:
+                    validate(
+                        instance={
+                            "value": parsed_value["value"]
+                        },
+                        schema=self._tool.action_schema(getattr(self._tool, self.tool_action))
+                    )
+
+                # Load optional input value; don't throw exceptions if key is not present
+                if self.tool_value is None:
+                    self.tool_value = str(parsed_value.get("value"))
 
             except SyntaxError as e:
-                self.structure.logger.error(f"Step {self.tool_step.id}\nSyntax error: {e}")
+                self.structure.logger.error(f"Step {self.toolkit_step.id}\nSyntax error: {e}")
 
                 self.tool_name = "error"
-                self.tool_input = f"syntax error: {e}"
+                self.tool_value = f"syntax error: {e}"
             except ValidationError as e:
-                self.structure.logger.error(f"Step {self.tool_step.id}\nInvalid JSON: {e}")
+                self.structure.logger.error(f"Step {self.toolkit_step.id}\nInvalid JSON: {e}")
 
                 self.tool_name = "error"
-                self.tool_input = f"JSON validation error: {e}"
+                self.tool_value = f"JSON validation error: {e}"
             except Exception as e:
-                self.structure.logger.error(f"Step {self.tool_step.id}\nError parsing tool action: {e}")
+                self.structure.logger.error(f"Step {self.toolkit_step.id}\nError parsing tool action: {e}")
 
                 self.tool_name = "error"
-                self.tool_input = f"error: {self.INVALID_ACTION_ERROR_MSG}"
+                self.tool_value = f"error: {self.INVALID_ACTION_ERROR_MSG}"
 
         if self.output is None and len(output_matches) > 0:
             self.output = TextOutput(output_matches[-1])
```

### Comparing `skatepark_lib-0.8.0/skatepark/structures/pipeline.py` & `skatepark_lib-0.9.0/skatepark/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/structures/structure.py` & `skatepark_lib-0.9.0/skatepark/structures/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import Optional, Union, TYPE_CHECKING
 from attr import define, field, Factory
 from rich.logging import RichHandler
 from skatepark.drivers import PromptDriver, OpenAiPromptDriver
-from skatepark.utils import J2
+from skatepark.utils import J2, ToolLoader
 
 if TYPE_CHECKING:
     from skatepark.rules import Rule
     from skatepark.steps import Step
 
 
 @define
@@ -21,14 +21,16 @@
 
     id: str = field(default=Factory(lambda: uuid.uuid4().hex), kw_only=True)
     type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     prompt_driver: PromptDriver = field(default=OpenAiPromptDriver(), kw_only=True)
     rules: list[Rule] = field(factory=list, kw_only=True)
     steps: list[Step] = field(factory=list, kw_only=True)
     custom_logger: Optional[Logger] = field(default=None, kw_only=True)
+    logger_level: int = field(default=logging.INFO, kw_only=True)
+    tool_loader: ToolLoader = field(default=ToolLoader(), kw_only=True)
 
     _execution_args: tuple = ()
     _logger: Optional[Logger] = None
 
     def __attrs_post_init__(self):
         for step in self.steps:
             step.structure = self
@@ -42,14 +44,15 @@
         if self.custom_logger:
             return self.custom_logger
         else:
             if self._logger is None:
                 self._logger = logging.getLogger(self.LOGGER_NAME)
 
                 self._logger.propagate = False
+                self._logger.level = self.logger_level
 
                 self._logger.handlers = [
                     RichHandler(
                         show_time=True,
                         show_path=False
                     )
                 ]
@@ -68,22 +71,17 @@
     def find_step(self, step_id: str) -> Optional[Step]:
         return next((step for step in self.steps if step.id == step_id), None)
 
     def add_steps(self, *steps: Step) -> list[Step]:
         return [self.add_step(s) for s in steps]
 
     def prompt_stack(self, step: Step) -> list[str]:
-        from skatepark.steps import ToolStep, ToolkitStep
+        from skatepark.steps import ToolkitStep
 
-        if isinstance(step, ToolStep):
-            tools = [step.tool]
-        elif isinstance(step, ToolkitStep):
-            tools = step.tools
-        else:
-            tools = []
+        tools = step.tools if isinstance(step, ToolkitStep) else []
 
         stack = [
             J2("prompts/context.j2").render(
                 rules=self.rules,
                 tool_names=str.join(", ", [tool.name for tool in tools]),
                 tools=[J2("prompts/tool.j2").render(tool=tool) for tool in tools]
             )
```

### Comparing `skatepark_lib-0.8.0/skatepark/structures/workflow.py` & `skatepark_lib-0.9.0/skatepark/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/summarizers/prompt_driver_summarizer.py` & `skatepark_lib-0.9.0/skatepark/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/templates/prompts/context.j2` & `skatepark_lib-0.9.0/skatepark/templates/prompts/context.j2`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% if tools|length > 0 %}
 You are an assistant that can use tools to answer user questions. To use a tool, follow this format:
 
 Input: <original question>
 Thought: <step-by-step thought process about how you can obtain the answer by using tools>
-Action: {"tool": "<tool name>", "input": <json object, array, or string>}
+Action: {"tool": "<tool name>", "action": "<action name>" "value": <action input based on JSON schema>}
 Observation: <tool response>
 Thought: <step-by-step thought process>
-Action: {"tool": "<tool name>", "input": <json object, array, or string>}
+Action: {"tool": "<tool name>", "action": "<action name>" "value": <action input based on JSON schema>}
 Observation: <tool response>
 ...repeat until you can answer the question
-Thought: I have enough information to answer the question
+Thought: I have enough information to answer the original question
 Output: <your final answer>
 
 You have access only to the following tools: [{{ tool_names }}]. NEVER make up tools and tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user. If you don't need to use a tool or if you don't know which tool to use, respond like this:
 
 Input: <original question>
 Output: <your final answer>
```

### Comparing `skatepark_lib-0.8.0/skatepark/utils/conversation.py` & `skatepark_lib-0.9.0/skatepark/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/utils/j2.py` & `skatepark_lib-0.9.0/skatepark/utils/j2.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/utils/tiktoken_tokenizer.py` & `skatepark_lib-0.9.0/skatepark/utils/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `skatepark_lib-0.8.0/skatepark/utils/tokenizer.py` & `skatepark_lib-0.9.0/skatepark/utils/tokenizer.py`

 * *Files identical despite different names*

