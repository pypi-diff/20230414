# Comparing `tmp/chatcli_gpt-0.4.0.tar.gz` & `tmp/chatcli_gpt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcli_gpt-0.4.0.tar", max compression
+gzip compressed data, was "chatcli_gpt-0.5.0.tar", max compression
```

## Comparing `chatcli_gpt-0.4.0.tar` & `chatcli_gpt-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.4.0/LICENSE
--rw-r--r--   0        0        0     3498 2023-04-10 16:46:32.407744 chatcli_gpt-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.4.0/chatcli_gpt/__init__.py
--rw-r--r--   0        0        0       34 2023-03-26 16:42:54.474450 chatcli_gpt-0.4.0/chatcli_gpt/__main__.py
--rw-r--r--   0        0        0    14346 2023-04-11 14:13:07.411332 chatcli_gpt-0.4.0/chatcli_gpt/chatcli.py
--rw-r--r--   0        0        0     7808 2023-04-11 13:59:19.090439 chatcli_gpt-0.4.0/chatcli_gpt/log.py
--rw-r--r--   0        0        0     2847 2023-04-11 13:20:15.453209 chatcli_gpt-0.4.0/chatcli_gpt/plugins.py
--rw-r--r--   0        0        0      915 2023-04-11 13:13:54.910005 chatcli_gpt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4651 1970-01-01 00:00:00.000000 chatcli_gpt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3498 2023-04-10 16:46:32.407744 chatcli_gpt-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.5.0/chatcli_gpt/__init__.py
+-rw-r--r--   0        0        0       34 2023-03-26 16:42:54.474450 chatcli_gpt-0.5.0/chatcli_gpt/__main__.py
+-rw-r--r--   0        0        0    16466 2023-04-14 14:50:08.474830 chatcli_gpt-0.5.0/chatcli_gpt/chatcli.py
+-rw-r--r--   0        0        0      757 2023-04-14 10:35:38.365222 chatcli_gpt-0.5.0/chatcli_gpt/conversation.py
+-rw-r--r--   0        0        0     7661 2023-04-14 14:27:59.909325 chatcli_gpt-0.5.0/chatcli_gpt/log.py
+-rw-r--r--   0        0        0     3997 2023-04-14 14:39:01.261820 chatcli_gpt-0.5.0/chatcli_gpt/plugins.py
+-rw-r--r--   0        0        0      961 2023-04-14 14:56:06.525301 chatcli_gpt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 chatcli_gpt-0.5.0/PKG-INFO
```

### Comparing `chatcli_gpt-0.4.0/LICENSE` & `chatcli_gpt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.4.0/README.md` & `chatcli_gpt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.4.0/chatcli_gpt/chatcli.py` & `chatcli_gpt-0.5.0/chatcli_gpt/chatcli.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .log import (
     write_log,
     search_conversations,
     conversation_log,
     create_initial_log,
 )
 from .plugins import evaluate_plugins
+from .conversation import Conversation
 
 MODELS = [
     "gpt-4",
     "gpt-3.5-turbo",
 ]
 
 MESSAGE_COLORS = {
@@ -43,24 +44,54 @@
 
 
 def cli_search_options(command):
     @click.argument("offset", type=int, required=False)
     @click.option("-s", "--search", help="Select by search term")
     @click.option("-t", "--tag", help="Select by tag")
     @functools.wraps(command)
-    def wrapper(offset, *args, search=None, tag=None, **kwargs):
+    def wrapper(*args, offset=None, search=None, tag=None, **kwargs):
         return command(
             *args,
             search_options={"offset": offset, "search": search, "tag": tag},
             **kwargs,
         )
 
     return wrapper
 
 
+def select_conversation(command):
+    @click.argument("offset", type=int, required=False)
+    @click.option("-s", "--search", help="Select by search term")
+    @click.option("-t", "--tag", help="Select by tag")
+    @functools.wraps(command)
+    def wrapper(*args, offset=None, search=None, tag=None, **kwargs):
+        return command(
+            *args,
+            conversation=get_logged_conversation(offset=offset, search=search, tag=tag),
+            **kwargs,
+        )
+
+    return wrapper
+
+
+def filter_conversations(command):
+    @click.argument("offsets", type=int, nargs=-1)
+    @click.option("-s", "--search", help="Select by search term")
+    @click.option("-t", "--tag", help="Select by tag")
+    @functools.wraps(command)
+    def wrapper(*args, offsets=None, search=None, tag=None, **kwargs):
+        return command(
+            *args,
+            conversations=search_conversations(offsets=offsets, search=search, tag=tag),
+            **kwargs,
+        )
+
+    return wrapper
+
+
 @cli.command(help="Ask a question of ChatGPT.")
 @click.option("-q", "--quick", is_flag=True, help="Just handle a one single-line question.")
 @click.option(
     "-c",
     "--continue_conversation",
     "--continue",
     is_flag=True,
@@ -75,61 +106,58 @@
     help="Add a file to the conversation for context.",
 )
 @click.option("-r", "--retry", is_flag=True, help="Retry previous question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
 @click.option("--model", type=click.Choice(MODELS))
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
 @cli_search_options
-def chat(quick, continue_conversation, personality, file, retry, stream, model, additional_plugins, search_options):
-    if (continue_conversation or retry) and not search_options["offset"]:
+def chat(search_options, **kwargs):
+    if (kwargs["continue_conversation"] or kwargs["retry"]) and not search_options["offset"]:
         search_options["offset"] = 1
-    elif personality and not search_options["tag"] and not search_options["search"] and not search_options["offset"]:
-        search_options["tag"] = "^" + personality
+    elif (
+        kwargs["personality"]
+        and not search_options["tag"]
+        and not search_options["search"]
+        and not search_options["offset"]
+    ):
+        search_options["tag"] = "^" + kwargs["personality"]
 
     conversation = get_logged_conversation(**search_options)
-    request_messages = conversation["messages"]
 
-    for filename in file:
+    for filename in kwargs["file"]:
         with open(filename, encoding="utf-8") as fh:
             file_contents = fh.read()
-        request_messages.append(
+
+        conversation.append(
             {
                 "role": "user",
-                "content": f"The file {file} contains:\n```\n{file_contents}```",
+                "content": f"The file {filename!r} contains:\n```\n{file_contents}```",
             }
         )
 
-    tags = conversation.get("tags", [])
-    if tags and not tags[-1].startswith("^"):
+    tags = conversation.tags
+    if tags and not is_personality(tags[-1]):
         tags_to_apply = [tags[-1]]
     else:
         tags_to_apply = []
 
-    plugins = conversation["plugins"]
-    plugins.extend(additional_plugins)
+    conversation.plugins.extend(kwargs["additional_plugins"])
+    conversation.tags = tags_to_apply
+    conversation.model = kwargs["model"] or conversation.model or "gpt-3.5-turbo"
+
+    quick = kwargs["quick"] or not os.isatty(0)
+    multiline = not quick
+
+    if kwargs["retry"]:
+        conversation.messages.pop()
+        add_answer(conversation, stream=kwargs["stream"])
+        if kwargs["quick"]:
+            return
 
-    model = model or conversation["model"] or "gpt-3.5-turbo"
-
-    if retry:
-        response = answer(request_messages[:-1], model, plugins, stream=stream, tags=tags_to_apply)
-        if not quick:
-            request_messages.append(response)
-            run_conversation(request_messages, model, plugins, stream=stream, tags=tags_to_apply)
-    elif quick or not os.isatty(0):
-        run_conversation(
-            request_messages,
-            model,
-            plugins,
-            stream=stream,
-            tags=tags_to_apply,
-            quick=True,
-            multiline=False,
-        )
-    else:
-        run_conversation(request_messages, model, plugins, stream=stream, tags=tags_to_apply)
+    run_conversation(conversation, multiline=multiline, quick=quick, stream=kwargs["stream"])
 
 
 @cli.command(help="Create initial conversation log.")
 @click.option("-r", "--reinit", is_flag=True, help="re-initialize the personalities to default values")
 def init(reinit):
     try:
         create_initial_log(reinit)
@@ -140,147 +168,187 @@
 
 @cli.command(help="Add a message to a new or existing conversation.")
 @click.option("--multiline/--singleline", default=True)
 @click.option("-p", "--personality")
 @click.option("--role", type=click.Choice(["system", "user", "assistant"]), default="system")
 @click.option("--plugin", multiple="True", help="Activate plugins.")
 @click.option("--model", type=click.Choice(MODELS), default="gpt-3.5-turbo")
+@click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
 @cli_search_options
-def add(personality, role, plugin, multiline, search_options, model):
+def add(personality, role, plugin, multiline, search_options, **kwargs):
     if any(search_options.values()):
         conversation = get_logged_conversation(**search_options)
-        messages = conversation["messages"]
     else:
-        messages = []
+        conversation = Conversation()
+
+    tags = conversation.tags
+    if tags and not is_personality(tags[-1]):
+        tags_to_apply = [tags[-1]]
+    else:
+        tags_to_apply = []
+
+    conversation.plugins.extend(kwargs["additional_plugins"])
+    conversation.tags = tags_to_apply
+    conversation.model = kwargs["model"] or conversation.model or "gpt-3.5-turbo"
 
-    tags = []
     if personality:
-        tags.append("^" + personality)
+        conversation.tags.append("^" + personality)
 
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
     description = prompt(multiline=True)
-    messages.append({"role": role, "content": description})
-    write_log(messages=messages, tags=tags, plugins=plugin, model=model)
+    conversation.append({"role": role, "content": description})
+    write_log(conversation)
+
+
+def merge_list(input_list, additions):
+    for item in additions:
+        if item not in input_list:
+            input_list.append(item)
+
+
+@cli.command(help="Create a new conversation by merging existing conversations.")
+@click.option("-p", "--personality", help="Set personality for new conversation.")
+@filter_conversations
+def merge(conversations, personality):
+    merged_conversation = {
+        "messages": [],
+        "tags": [],
+        "plugins": [],
+        "model": None,
+    }
+    if personality:
+        merged_conversation["tags"].append("^" + personality)
+
+    for _, item in reversed(list(conversations)):
+        merge_list(merged_conversation["messages"], item.messages)
+        merge_list(merged_conversation["tags"], (tag for tag in item.tags if not is_personality(tag)))
+        merge_list(merged_conversation["plugins"], item.plugins)
+        merged_conversation["model"] = item.model or merged_conversation["model"]
+
+    write_log(Conversation(**merged_conversation))
 
 
 @cli.command(help="List tags.", name="tags")
 def list_tags():
     tags = set()
     for conversation in conversation_log():
-        for tag in conversation.get("tags", []):
+        for tag in conversation.tags:
             tags.add(tag)
     for tag in sorted(tags):
         click.echo(tag)
 
 
 @cli.command(help="Add tags to an conversation.", name="tag")
-@click.argument("tag")
-@cli_search_options
-def add_tag(tag, search_options):
-    conversation = get_logged_conversation(**search_options)
-    new_tags = [t for t in conversation.get("tags", []) if t != tag]
-    new_tags.append(tag)
+@click.argument("new_tag")
+@select_conversation
+def add_tag(new_tag, conversation):
+    new_tags = [tag for tag in conversation.tags if tag != new_tag]
+    new_tags.append(new_tag)
+    conversation.tags = new_tags
 
-    write_log(messages=conversation["messages"], tags=new_tags)
+    write_log(conversation)
 
 
 @cli.command(help="Remove tags from an conversation.")
-@click.argument("tag")
-@cli_search_options
-def untag(tag, search_options):
-    conversation = get_logged_conversation(**search_options)
-    new_tags = [t for t in conversation.get("tags", []) if t != tag]
-    write_log(messages=conversation["messages"], tags=new_tags)
+@click.argument("tag_to_remove")
+@select_conversation
+def untag(tag_to_remove, conversation):
+    conversation.tags = [tag for tag in conversation.tags if tag != tag_to_remove]
+    write_log(conversation)
 
 
 @cli.command(help="Current tag")
-@cli_search_options
-def show_tag(search_options):
-    conversation = get_logged_conversation(**search_options)
-    tags = conversation.get("tags", [])
-
-    if tags:
-        click.echo(tags[-1])
+@select_conversation
+def show_tag(conversation):
+    if conversation.tags:
+        click.echo(conversation.tags[-1])
 
 
 @cli.command(help="Show a conversation.")
-@cli_search_options
+@select_conversation
 @click.option(
     "-l/-s",
     "--long/--short",
     help="Show full conversation or just the most recent message.",
 )
-def show(long, search_options):
-    conversation = get_logged_conversation(**search_options)
+@click.option("--format-json", "--json", is_flag=True, help="Output conversation in JSON format.")
+def show(long, conversation, format_json):
+    if format_json:
+        click.echo(conversation.to_json())
+        return
+
     if long:
-        messages = conversation["messages"]
+        messages = conversation.messages
     else:
-        messages = conversation["messages"][-1:]
+        messages = conversation.messages[-1:]
 
     for message in messages:
         prefix = ""
         if message["role"] == "user":
             prefix = ">> "
         click.echo(click.style(prefix + message["content"], fg=MESSAGE_COLORS[message["role"]]))
 
 
 @cli.command(help="List all the questions we've asked")
-@cli_search_options
+@filter_conversations
 @click.option("-l", "--limit", type=int, help="Limit number of results")
 @click.option("-u", "--usage", is_flag=True, help="Show token usage")
 @click.option("--cost", is_flag=True, help="Show token cost")
 @click.option("--plugins", is_flag=True, help="Show enabled plugins")
 @click.option("--model", is_flag=True, help="Show model")
-def log(limit, usage, cost, plugins, search_options, model):
-    for offset, conversation in reversed(list(itertools.islice(search_conversations(**search_options), limit))):
+@click.option("--format-json", "--json", is_flag=True, help="Output conversation in JSON format.")
+def log(conversations, limit, usage, cost, plugins, model, format_json):
+    for offset, conversation in reversed(list(itertools.islice(conversations, limit))):
+        if format_json:
+            click.echo(conversation.to_json())
+            continue
         try:
             question = find_recent_message(lambda message: message["role"] != "assistant", conversation)["content"]
         except ValueError:
-            question = conversation["messages"][-1]["content"]
+            question = conversation.messages[-1]["content"]
         trimmed_message = question.strip().split("\n", 1)[0][:80]
 
         fields = []
         offset = click.style(f"{offset: 4d}:", fg="blue")
         fields.append(offset)
 
         if usage:
-            if conversation["usage"]:
-                total_tokens = conversation["usage"]["total_tokens"]
+            if conversation.usage:
+                total_tokens = conversation.usage["total_tokens"]
             else:
                 total_tokens = 0
             fields.append(f"{total_tokens: 5d}")
 
         if cost:
             fields.append(f"${conversation_cost(conversation): 2.3f}")
 
         fields.append(trimmed_message)
-        if conversation.get("tags"):
-            fields.append(click.style(f"{','.join(conversation['tags'])}", fg="green"))
+        if conversation.tags:
+            fields.append(click.style(",".join(conversation.tags), fg="green"))
 
         if plugins:
-            fields.append(f"{','.join(conversation['plugins'])}")
+            fields.append(",".join(conversation.plugins))
 
         if model:
-            fields.append(click.style(f"{conversation['model']}", fg="yellow"))
+            fields.append(click.style(conversation.model, fg="yellow"))
 
         click.echo(" ".join(fields))
 
 
-def run_conversation(request_messages, model, plugins, tags=None, stream=True, multiline=True, quick=False):
+def run_conversation(conversation, stream=True, multiline=True, quick=False):
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
 
     while True:
         question = prompt(multiline=multiline)
         if not question:
             break
-        request_messages.append({"role": "user", "content": question})
-        response_message = answer(request_messages, model, plugins, stream=stream, tags=tags)
-        request_messages.append(response_message)
+        conversation.append({"role": "user", "content": question})
+        add_answer(conversation, stream=stream)
 
         if quick:
             break
 
 
 def prompt(multiline=True):
     if os.isatty(0):
@@ -334,100 +402,101 @@
     return {
         "prompt_tokens": request_tokens,
         "completion_tokens": completion_tokens,
         "total_tokens": request_tokens + completion_tokens,
     }
 
 
-def answer(request_messages, model, plugins, stream=True, tags=None):
+@cli.command(help="Add an answer to a question")
+@click.option("--stream/--sync", default=True, help="Stream or sync mode.")
+@select_conversation
+def answer(conversation, stream):
+    add_answer(conversation, stream=stream)
+
+
+def add_answer(conversation, stream=True):
     if stream:
-        completion = stream_request(request_messages, model)
+        completion = stream_request(conversation.messages, conversation.model)
     else:
-        completion = synchroneous_request(request_messages, model)
+        completion = synchroneous_request(conversation.messages, conversation.model)
 
     # TODO: handle multiple choices
     response_message = completion["choices"][0]["message"]
-
+    conversation.append(response_message)
     write_log(
-        messages=request_messages + [response_message],
+        conversation,
         completion=completion,
-        usage=completion_usage(request_messages, model, completion),
-        tags=tags,
-        plugins=plugins,
-        model=model,
+        usage=completion_usage(conversation.messages[:-1], conversation.model, completion),
     )
 
     # TODO:
     # - [ ] wrote more plugins and see what's good interface for plugins
     # - [ ] middleware pattern for plugins
-    if plugins:
-        plugin_response = evaluate_plugins(response_message["content"], plugins)
+    if conversation.plugins:
+        plugin_response = evaluate_plugins(response_message["content"], conversation.plugins)
 
         if plugin_response:
-            request_messages.append(response_message)
-            request_messages.append({"role": "user", "content": plugin_response})
+            conversation.append({"role": "user", "content": plugin_response})
             click.echo(click.style(plugin_response, fg=(200, 180, 90)))
-            return answer(
-                request_messages,
-                model,
-                plugins,
-                stream=stream,
-                tags=tags,
-            )
+            return add_answer(conversation, stream=stream)
 
     return response_message
 
 
 def conversation_cost(conversation):
-    if not conversation["usage"]:
+    if not conversation.usage:
         return 0
-    model = conversation["completion"]["model"]
+    model = conversation.completion["model"]
     if model not in USAGE_COSTS:
         model = "-".join(model.split("-")[:-1])
     model_price = USAGE_COSTS[model]
 
-    usage = conversation["usage"]
+    usage = conversation.usage
     return (
         model_price["prompt_tokens"] * usage["prompt_tokens"] / 1000
         + model_price["completion_tokens"] * usage["completion_tokens"] / 1000
     )
 
 
 def find_recent_message(predicate, conversation):
-    for message in reversed(conversation["messages"]):
+    for message in reversed(conversation.messages):
         if predicate(message):
             return message
     raise ValueError("No matching message found")
 
 
 @cli.command(help="Display number of tokens and token cost.", name="usage")
 @click.option("--today", is_flag=True, help="Show usage for today only.")
 def show_usage(today):
     conversations = conversation_log()
 
     def is_today(conversation):
-        return dateutil.parser.parse(conversation["timestamp"]).date() == datetime.date.today()
+        return dateutil.parser.parse(conversation.timestamp).date() == datetime.date.today()
 
     if today:
         conversations = [c for c in conversations if is_today(c)]
-    tokens = sum(conversation["usage"]["total_tokens"] for conversation in conversations if conversation["usage"])
+    tokens = sum(conversation.usage["total_tokens"] for conversation in conversations if conversation.usage)
 
     total_cost = sum(conversation_cost(conversation) for conversation in conversations)
     click.echo(f"Tokens: {tokens}")
     click.echo(f"Cost: ${total_cost:.2f}")
 
 
 def get_logged_conversation(offset, search=None, tag=None):
+    offsets = [offset] if offset else []
     try:
-        return next(search_conversations(offset, search, tag))[1]
+        return next(search_conversations(offsets, search, tag))[1]
     except StopIteration:
         click.echo("Matching conversation not found", file=sys.stderr)
         sys.exit(1)
 
 
+def is_personality(tag):
+    return tag.startswith("^")
+
 
 def main():
     try:
         cli()
     except FileNotFoundError as error:
         click.echo(f"{error}: Chatcli not initialized. Run `chatcli init` first.")
         sys.exit(1)
```

### Comparing `chatcli_gpt-0.4.0/chatcli_gpt/log.py` & `chatcli_gpt-0.5.0/chatcli_gpt/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
+import os.path
 import sys
 import shutil
 from pathlib import Path
 import datetime
 import json
 from textwrap import dedent
 
+from .conversation import Conversation
+
 INITIAL_PERSONALITIES = {
     "concise": {
         "content": "You are a helpful, expert linux user and programmer. You give concise answers, providing code where possible.",
     },
     "code": {"content": "You only answer questions with a single example code block only, and no other explanations."},
     "commit": {
         "content": """
@@ -80,57 +83,82 @@
             RESULT:
             ```
             hello world!
             ```
             Answer questions about by running commands and using the results you receive.
         """,
     },
+    "wolfram": {
+        "plugins": ["wolfram"],
+        "model": "gpt-4",
+        "content": """
+            You can use wolfram alpha to access various facts about the world, and to solve equations.
+
+            For example:
+
+            WOLFRAM("What is the capital of France?")
+
+            You will get the answer to your queries as a result block. Use the answers to help you answer the question.
+        """,
+    },
+    "save": {
+        "plugins": ["save"],
+        "model": "gpt-4",
+        "content": """
+            You can save file contents by using a save block.
+
+            For example:
+
+            SAVE("hello.py")
+            ```
+            print("hello, world!")
+            ```
+        """,
+    },
 }
 
 CHAT_LOG = os.environ.get("CHATCLI_LOGFILE", ".chatcli.log")
+LOG_FILE_VERSION = "0.4"
 
 
-def write_log(messages, completion=None, usage=None, tags=None, plugins=None, path=None, model=None):
-    assert isinstance(messages, list)
-    assert isinstance(tags, list) or tags is None
-    assert isinstance(completion, dict) or completion is None
-    assert isinstance(usage, dict) or usage is None
-    assert isinstance(plugins, (list, tuple)) or plugins is None
-    assert isinstance(model, str) or model is None
-    timestamp = datetime.datetime.now().isoformat()
-
+def write_log(conversation, usage=None, completion=None, path=None):
     path = path or find_log()
-
+    timestamp = datetime.datetime.now().isoformat()
     with open(path, "a", buffering=1, encoding="utf-8") as fh:
         fh.write(
             json.dumps(
                 {
-                    "messages": messages,
+                    "messages": conversation.messages,
                     "completion": completion,
                     "usage": usage,
-                    "tags": tags or [],
+                    "tags": conversation.tags or [],
                     "timestamp": timestamp,
-                    "plugins": plugins or [],
-                    "model": model,
+                    "plugins": conversation.plugins or [],
+                    "model": conversation.model,
                 }
             )
             + "\n"
         )
 
 
 def create_initial_log(reinit):
     if not reinit and Path(CHAT_LOG).exists():
         raise FileExistsError(CHAT_LOG)
 
+    with Path(CHAT_LOG).open("w", encoding="utf-8") as fh:
+        fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
+
     for key, value in INITIAL_PERSONALITIES.items():
         write_log(
-            messages=[{"role": "system", "content": dedent(value["content"].strip())}],
-            tags=["^" + key],
-            plugins=value.get("plugins"),
-            model=value.get("model"),
+            Conversation(
+                messages=[{"role": "system", "content": dedent(value["content"]).strip()}],
+                tags=["^" + key],
+                plugins=value.get("plugins"),
+                model=value.get("model"),
+            ),
             path=CHAT_LOG,
         )
 
 
 def conversation_log():
     log_path = find_log()
     with log_path.open(encoding="utf-8") as fh:
@@ -139,67 +167,48 @@
         if version is None:
             fh.close()
             lines = list(convert_log_pre_0_4(log_path))
             backup_file = log_path.with_suffix(".log.bak.0_3")
             sys.stderr.write(f"Upgrading log file. Making backup in: {backup_file}\n")
             shutil.copyfile(log_path, backup_file)
             with log_path.open("w", encoding="utf-8") as fh:
-                fh.write(json.dumps({"version": "0.4"}) + "\n")
+                fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
                 for line in lines:
                     fh.write(line + "\n")
-            return [json.loads(line) for line in lines]
-        return [json.loads(line) for line in fh]
+            return [Conversation(**json.loads(line)) for line in lines]
+        return [Conversation(**json.loads(line)) for line in fh]
 
 
 def find_log():
     path = CHAT_LOG
     for directory in Path(path).resolve().parents:
         if (directory / path).exists():
             return directory / path
     raise FileNotFoundError(CHAT_LOG)
 
 
-def search_conversations(offset, search, tag):
+def search_conversations(offsets, search, tag):
     for idx, conversation in enumerate(reversed(conversation_log()), start=1):
-        if offset and idx != offset:
+        if offsets and idx not in offsets:
             continue
 
-        if len(conversation["messages"]) > 1:
-            question = conversation["messages"][-2]["content"]
-        else:
-            question = conversation["messages"][-1]["content"]
-
-        if search and search not in question:
+        if search and search not in conversation:
             continue
-        if tag and tag not in conversation.get("tags", []):
+        if tag and tag not in conversation.tags:
             continue
         yield idx, conversation
 
 
 def convert_log_pre_0_4(filename):
     with open(filename, "r", encoding="utf-8") as fh:
         for line in fh:
             data = json.loads(line)
 
-            if "request" in data:
-                if data["response"]:
-                    assistant_message = data["response"]["choices"][0]["message"]
-                    if "role" not in assistant_message:
-                        assistant_message["role"] = "assistant"
-                    messages = data["request"] + [assistant_message]
-                    usage = data["response"].get("usage")
-                else:
-                    messages = data["request"]
-                    usage = None
-            elif "response" in data:
-                messages = [data["response"]["choices"][0]["message"]]
-                usage = data["response"]["usage"]
-            else:
-                messages = data["messages"]
-                usage = data["usage"]
+            messages = data["messages"]
+            usage = data["usage"]
 
             if usage and "request_tokens" in usage:
                 usage["prompt_tokens"] = usage["request_tokens"]
                 del usage["request_tokens"]
 
             tags = data.get("tags", [])
             completion = data.get("completion") or data.get("response")
```

### Comparing `chatcli_gpt-0.4.0/pyproject.toml` & `chatcli_gpt-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatcli-gpt"
-version = "0.4.0"
+version = "0.5.0"
 description = "A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations."
 readme = "README.md"
 license = "MIT"
 authors = ["Adam Kelly <adam@cthulahoops.org>"]
 repository = "https://github.com/cthulahoops/chatcli"
 
 [tool.poetry.dependencies]
@@ -16,20 +16,22 @@
 click-default-group = "^1.2.2"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 tiktoken = "^0.3.2"
 python-dateutil = "^2.8.2"
 duckduckgo-search = "^2.8.5"
 pillow = "^9.4.0"
+wolframalpha = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pylint = "^2.17.1"
+pytest-cov = "^4.0.0"
 
 [tool.poetry.scripts]
 chatcli = "chatcli_gpt.chatcli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chatcli_gpt-0.4.0/PKG-INFO` & `chatcli_gpt-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcli-gpt
-Version: 0.4.0
+Version: 0.5.0
 Summary: A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations.
 Home-page: https://github.com/cthulahoops/chatcli
 License: MIT
 Author: Adam Kelly
 Author-email: adam@cthulahoops.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.2,<0.4.0)
+Requires-Dist: wolframalpha (>=5.0.0,<6.0.0)
 Project-URL: Repository, https://github.com/cthulahoops/chatcli
 Description-Content-Type: text/markdown
 
 # ChatCLI
 
 ChatCLI is a command-line tool that uses the OpenAI GPT-3.5/GPT-4 API to
 provide a chat bot interface that can answer your questions. It provides a
```

