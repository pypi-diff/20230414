# Comparing `tmp/kernel_sidecar-0.5.1.tar.gz` & `tmp/kernel_sidecar-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernel_sidecar-0.5.1.tar", max compression
+gzip compressed data, was "kernel_sidecar-0.5.2.tar", max compression
```

## Comparing `kernel_sidecar-0.5.1.tar` & `kernel_sidecar-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-04-05 13:27:11.474784 kernel_sidecar-0.5.1/LICENSE
--rw-r--r--   0        0        0     9053 2023-04-05 13:27:11.474784 kernel_sidecar-0.5.1/README.md
--rw-r--r--   0        0        0     1174 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/__init__.py
--rw-r--r--   0        0        0     4209 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/actions.py
--rw-r--r--   0        0        0     2347 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/cli.py
--rw-r--r--   0        0        0    22564 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/client.py
--rw-r--r--   0        0        0     5207 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/comms.py
--rw-r--r--   0        0        0        0 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/__init__.py
--rw-r--r--   0        0        0      902 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/base.py
--rw-r--r--   0        0        0     1580 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/debug.py
--rw-r--r--   0        0        0     5919 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/output.py
--rw-r--r--   0        0        0     4395 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/log_utils.py
--rw-r--r--   0        0        0        0 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/models/__init__.py
--rw-r--r--   0        0        0    14883 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/models/messages.py
--rw-r--r--   0        0        0     2334 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/models/notebook.py
--rw-r--r--   0        0        0     9369 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/models/requests.py
--rw-r--r--   0        0        0     4707 2023-04-05 13:27:11.478784 kernel_sidecar-0.5.1/src/kernel_sidecar/nb_builder.py
--rw-r--r--   0        0        0    10395 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.1/setup.py
--rw-r--r--   0        0        0     9875 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/LICENSE
+-rw-r--r--   0        0        0     9197 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/README.md
+-rw-r--r--   0        0        0     1174 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/__init__.py
+-rw-r--r--   0        0        0     4209 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/actions.py
+-rw-r--r--   0        0        0     2678 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/cli.py
+-rw-r--r--   0        0        0    24262 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/client.py
+-rw-r--r--   0        0        0     5207 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/comms.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/__init__.py
+-rw-r--r--   0        0        0      902 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/base.py
+-rw-r--r--   0        0        0     1580 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/debug.py
+-rw-r--r--   0        0        0     5919 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/output.py
+-rw-r--r--   0        0        0     4395 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/log_utils.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/__init__.py
+-rw-r--r--   0        0        0    14883 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/messages.py
+-rw-r--r--   0        0        0     2334 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/notebook.py
+-rw-r--r--   0        0        0     9369 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/requests.py
+-rw-r--r--   0        0        0     4707 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/nb_builder.py
+-rw-r--r--   0        0        0      261 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/settings.py
+-rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.2/setup.py
+-rw-r--r--   0        0        0    10019 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.2/PKG-INFO
```

### Comparing `kernel_sidecar-0.5.1/LICENSE` & `kernel_sidecar-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/README.md` & `kernel_sidecar-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 Usage: sidecar [OPTIONS]
 
 Options:
   -f FILE                         Kernel connection file  [required]
   --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]
   --execute TEXT                  Execute code string instead of sending
                                   kernel info request
+  --tail / --no-tail              Continue tailing ZMQ after connecting or
+                                  executing code  [default: no-tail]
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 ```
```

#### html2text {}

```diff
@@ -62,15 +62,16 @@
 Jupyter Notebook document (`models/notebook.py`), which should be consistent
 with `nbformat` parsing / structure - Request messages sent to the Kernel over
 ZMQ (`models/requests.py`) - Messages received over ZMQ from the Kernel
 (`models/messages.py`) ## CLI `kernel-sidecar` ships a small CLI for testing a
 connection to a Kernel. ```bash â¯ sidecar --help Usage: sidecar [OPTIONS]
 Options: -f FILE Kernel connection file [required] --debug / --no-debug Turn on
 DEBUG logging [default: no-debug] --execute TEXT Execute code string instead of
-sending kernel info request --install-completion
+sending kernel info request --tail / --no-tail Continue tailing ZMQ after
+connecting or executing code [default: no-tail] --install-completion
 [bash|zsh|fish|powershell|pwsh] Install completion for the specified shell. --
 show-completion [bash|zsh|fish|powershell|pwsh] Show completion for the
 specified shell, to copy it or customize the installation. --help Show this
 message and exit. ``` Try it out by starting an IPython kernel in one terminal
 and using the CLI in another. ```bash python -m ipykernel_launcher --debug -f /
 tmp/kernel.json ``` ```bash kernel-sidecar on î  release-0.3.2 [$?] is ð¦
 v0.3.1 via ð v3.11.0 (kernel-sidecar-py3.11) â¯ sidecar -f /tmp/kernel.json
```

### Comparing `kernel_sidecar-0.5.1/pyproject.toml` & `kernel_sidecar-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kernel-sidecar"
-version = "0.5.1"
+version = "0.5.2"
 description = "A sidecar "
 authors = ["Matt Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "kernel_sidecar", from = "src"}]
 repository = "https://github.com/kafonek/kernel-sidecar"
```

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/actions.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/actions.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/cli.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from jupyter_client import KernelConnectionInfo
 
 from kernel_sidecar.client import KernelSidecarClient
 from kernel_sidecar.handlers.base import Handler
 from kernel_sidecar.handlers.debug import DebugHandler
 from kernel_sidecar.log_utils import setup_logging
 from kernel_sidecar.models import messages
+from kernel_sidecar.settings import get_settings
 
 logger = logging.getLogger(__name__)
 
 app = typer.Typer(no_args_is_help=True)
 
 
 class OutputHandler(Handler):
@@ -34,39 +35,46 @@
 
 
 async def execute_code(connection_info: KernelConnectionInfo, code: str):
     async with KernelSidecarClient(connection_info) as kernel:
         await kernel.execute_request(code=code, handlers=[OutputHandler()])
 
 
-async def connect(connection_info: KernelConnectionInfo):
+async def connect(connection_info: KernelConnectionInfo, tail: bool):
     async with KernelSidecarClient(connection_info) as kernel:
         handler = DebugHandler()
         await kernel.kernel_info_request(handlers=[handler])
         kernel_info: messages.KernelInfoReply = handler.get_last_msg("kernel_info_reply")
         logger.info(pprint.pformat(kernel_info.content.dict()))
+        if tail:
+            while True:
+                await asyncio.sleep(0.01)
 
 
 @app.command()
 def main(
     connection_file: pathlib.Path = typer.Option(
         ..., "-f", help="Kernel connection file", exists=True, dir_okay=False
     ),
     debug: bool = typer.Option(default=False, help="Turn on DEBUG logging"),
     execute: Optional[str] = typer.Option(
         default=None, help="Execute code string instead of sending kernel info request"
     ),
+    tail: Optional[bool] = typer.Option(
+        default=False, help="Continue tailing ZMQ after connecting or executing code"
+    ),
 ):
     if debug:
+        get_settings().pprint_logs = True
         setup_logging(log_level=logging.DEBUG)
     else:
         setup_logging()
     connection_info = json.loads(connection_file.read_text())
     logger.info(f"Attempting to connect:\n{pprint.pformat(connection_info)}")
     if execute:
         asyncio.run(execute_code(connection_info, execute))
     else:
-        asyncio.run(connect(connection_info))
+        asyncio.run(connect(connection_info, tail=tail))
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/client.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from zmq.asyncio import Context
 from zmq.utils.monitor import recv_monitor_message
 
 from kernel_sidecar import actions
 from kernel_sidecar.comms import CommHandler, CommManager, WidgetHandler
 from kernel_sidecar.handlers.base import Handler
 from kernel_sidecar.models import messages, requests
+from kernel_sidecar.settings import get_settings
 
 logger = logging.getLogger(__name__)
 
 
 class CommTargetNotFound(Exception):
     pass
 
@@ -71,15 +72,15 @@
        CommManager, which will process and/or route comm_open, comm_msg, and comm_close messages
     """
 
     _message_model = messages.Message
     # ^^ discriminator model to parse messages coming in from ZMQ. Override this if you have
     # custom message models defined somewhere besides kernel_sidecar.models.messages
     # should be type: Annotated[Union[models...], Field(discriminator='msg_type')]
-    _handler_timeout: float = None  # optional timeout when awaiting Action handlers
+    _handler_timeout: Optional[float] = None  # optional timeout when awaiting Action handlers
     jupyter_widget_handler: Type[CommHandler] = WidgetHandler
 
     def __init__(
         self,
         connection_info: KernelConnectionInfo,
         max_message_size: Optional[int] = None,
         default_handlers: List[Handler] = None,
@@ -167,20 +168,26 @@
         try:
             channel: ZMQSocketChannel = getattr(self.kc, f"{action.request._channel}_channel")
             channel.send(action.request.dict())
             action.sent = True
             # Update the .actions dictionary so that we route any observed messages coming to us
             # over ZMQ into this action for handling callbacks
             self.actions[action.msg_id] = action
-            logger.debug(
-                f"Sent {action.request.header.msg_type} to kernel",
-                extra={"body": pprint.pformat(action.request.dict())},
-            )
+
+            log_msg = f"Sent {action.request.header.msg_type} to kernel"
+            log_extra = {}
+            if get_settings().pprint_logs:
+                log_extra["body"] = pprint.pformat(action.request.dict())
+            logger.debug(log_msg, extra=log_extra)
         except Exception as e:
-            logger.exception("Error sending message", extra={"body": action.request.dict()})
+            log_msg = f"Error sending {action.request.header.msg_type} message over ZMQ"
+            log_extra = {}
+            if get_settings().pprint_logs:
+                log_extra["body"] = pprint.pformat(action.request.dict())
+            logger.error(log_msg, extra=log_extra, exc_info=True)
             raise e
         return action
 
     def kernel_info_request(
         self, handlers: List[Callable[[messages.Message], Awaitable[None]]] = None
     ) -> actions.KernelAction:
         req = requests.KernelInfoRequest()
@@ -370,20 +377,25 @@
         """Takes messages seen on zmq and drops them into our internal asyncio.Queue"""
         while True:
             try:
                 if not channel.is_alive():
                     await asyncio.sleep(0.001)
                     continue
                 raw_msg: dict = await channel.get_msg()
-                msg_type = raw_msg.get("msg_type", "")
-                logger.debug(
-                    f"Message {msg_type} on {channel_name}",
-                    extra={"body": pprint.pformat(raw_msg), "channel": channel_name},
-                )
                 self.mq.put_nowait(raw_msg)
+                msg_type = raw_msg.get("msg_type", "")
+
+                # When using kernel-sidecar in a production app, we noticed that pprint.pformat
+                # caused OOMs due to pprint.pformat trying to format large messages (e.g.
+                # display_data for large Dataframes formatted with dx.py).
+                log_msg = f"Message {msg_type} on {channel_name}"
+                log_extra = {"channel": channel_name}
+                if get_settings().pprint_logs:
+                    log_extra["body"] = pprint.pformat(raw_msg)
+                logger.debug(log_msg, extra=log_extra)
             except asyncio.CancelledError:
                 break
             except Exception as e:
                 logger.exception("Error retrieving message from zmq")
                 raise e
 
     async def process_message(self):
@@ -391,47 +403,62 @@
         Takes messages from our internal asyncio.Queue, parses them into pydantic models using
         a discriminator pattern (see messages.py), and delegates them to the appropriate Action
         which will further delegate them to handle_<msg_type> methods defined in the Action model.
 
         Action handlers are awaited before the next message is processed.
         """
         while True:
+            # Pull dictionaries off the internal message queue
+            raw_msg: dict = await self.mq.get()
+
+            # kernel status "starting" is one example of messages with no parent header
+            if not raw_msg.get("parent_header"):
+                await self.handle_missing_parent_msg_id(raw_msg)
+                continue
+
+            # Getting a ValidationError here probably means we need to add new Message models
             try:
-                raw_msg: dict = await self.mq.get()
-                if not raw_msg.get("parent_header"):
-                    await self.handle_missing_parent_msg_id(raw_msg)
-                    continue
-                try:
-                    msg = pydantic.parse_obj_as(messages.Message, raw_msg)
-                except pydantic.ValidationError as e:
-                    await self.handle_unparseable_message(raw_msg, e)
-                if msg.parent_header.msg_id not in self.actions:
-                    await self.handle_untracked_action(msg)
-                    continue
+                msg = pydantic.parse_obj_as(messages.Message, raw_msg)
+            except pydantic.ValidationError as e:
+                await self.handle_unparseable_message(raw_msg, e)
+
+            # Getting an "untracked action" probably means another client is talking to the Kernel
+            # over ZMQ and sending in requests
+            if msg.parent_header.msg_id not in self.actions:
+                await self.handle_untracked_action(msg)
+                continue
+
+            # Happy path: we have an Action for the parent request of messages we see coming in
+            action = self.actions[msg.parent_header.msg_id]
+
+            # Log warning if we think we're seeing responses for a new Action and haven't completed
+            # the previously running action, e.g. we start getting status / content responses for
+            # a new execute_request when we haven't seen execute_reply / status idle for a previous
+            # execute request
+            if self.running_action and self.running_action is not action:
+                logger.warning(
+                    f"Observed message for {action} while {self.running_action} has not "
+                    "completed. This is a sign that expected messages didn't come over ZMQ or "
+                    "the Action needs a different expected_reply_msg_type. Setting "
+                    "running_action.done to True to avoid app hanging."
+                )
 
-                action = self.actions[msg.parent_header.msg_id]
-                ra = self.running_action
-                if ra and ra is not action:
-                    logger.warning(
-                        f"Observed message for {action} while {ra} has not completed. This is a "
-                        "sign that expected messages didn't come over ZMQ or the Action needs a "
-                        "different expected_reply_msg_type. Setting running_action.done to True to "
-                        "avoid app hanging."
-                    )
+                self.running_action.done.set()
+                self.running_action.running = False
 
-                    ra.done.set()
-                    ra.running = False
+            # Optional timeout for callbacks
+            try:
                 await asyncio.wait_for(action.handle_message(msg), timeout=self._handler_timeout)
-
             except asyncio.CancelledError:
-                logger.debug("Message processing Task cancelled")
-                break
-            except Exception as e:
+                logger.warning(f"Timeout handling callbacks for {action}")
+                continue
+            except:  # noqa: E722
+                # Important decision to not raise the exception here so that one failed callback
+                # does not stop the entire process inbound message coroutine loop
                 logger.exception("Error while handling message")
-                raise e
 
     async def handle_missing_parent_msg_id(self, raw_msg: dict):
         """
         Almost all messages should have a parent_header.msg_id which we can use to delegate to
         Action handlers. Any messages without a parent_header msg_id can be logged or handled
         here.
```

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/comms.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/comms.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/base.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/debug.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/debug.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/handlers/output.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/output.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/log_utils.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/log_utils.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/models/messages.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/models/messages.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/models/notebook.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/models/notebook.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/models/requests.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/models/requests.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/src/kernel_sidecar/nb_builder.py` & `kernel_sidecar-0.5.2/src/kernel_sidecar/nb_builder.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.1/setup.py` & `kernel_sidecar-0.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 {'cli': ['structlog', 'typer']}
 
 entry_points = \
 {'console_scripts': ['sidecar = kernel_sidecar.cli:app']}
 
 setup_kwargs = {
     'name': 'kernel-sidecar',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'A sidecar ',
-    'long_description': '<p align="center">\nKernel Sidecar\n</p>\n\n<p align="center">\n<img alt="Pypi" src="https://img.shields.io/pypi/v/kernel-sidecar">\n<a href="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml">\n    <img src="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml/badge.svg" alt="Tests" />\n</a>\n<img alt="Python versions" src="https://img.shields.io/pypi/pyversions/kernel-sidecar">\n</p>\n\n# Kernel-Sidecar\n\nThis package offers the building blocks for creating a "Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture, one or many frontends manage the document model (code cells, outputs, metadata, etc) and send requests to a single Kernel. Each frontend observes responses on different ZMQ channels (`iopub`, `shell`, etc) but may end up with some inconsistency based on the Kernel only sending certain responses to the client that made the request.\n\nIn a `kernel-sidecar` architecture, all frontend clients talk to the `kernel-sidecar` client, and only the `kernel-sidecar` client communicates with the Kernel over ZMQ. That pattern offers several potential features:\n - Keep a document model within `kernel-sidecar` or the backend architecture\n - Add "extension"-esque capabilities on the backend such as auto-linting code on execute\n - Eliminate inconsistencies in what messages individual frontends receive because of Kernel replies\n - Model all requests, replies, and the Notebook document with Pydantic\n\n## Installation\n\n```bash\npip install kernel-sidecar\n```\n\n# Key Concepts\n## KernelSidecarClient\n\nA manager that uses `jupyter_client` under the hood to create ZMQ connections and watch for messages coming in over different ZMQ channels (`iopub`, `shell`, etc. An important assumption here is that `kernel-sidecar` is the only client talking to the Kernel, which means every message observed coming from the Kernel should be a reply (based on `parent_header_msg.msg_id`) to a request sent from this client.\n\nWhen the `KernelSidecarClient` send a request to the Kernel, it is wrapped in an `KernelAction` class. Every message received from the Kernel is delegated to the requesting Action and triggers callbacks attached to the Action class.\n\n## Actions\n\nActions in `kernel-sidecar` encompass a request-reply cycle, including an `await action` syntax, where the Action is complete when the Kernel has reported its status returning to `idle` and optionally emitted a reply appropriate for the request. For instance, an `execute_request` is "done" when the `status` has been reported as `idle` *and* the Kernel has emitted an `execute_reply`, both with the `parent_header_msg.msg_id` the same as the `execute_request` `header.msg_id`.\n\nIn a nutshell, an `actions.KernelAction` takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses (or just `async functions`) and creates an `awaitable` instance. `kernel.send(action)` submits the Request over ZMQ, and registers the Action so that all observed messages get routed to that Action to be handled by the Handlers/callbacks.\n\nMost of the time, you should be able to just use convience functions in the `KernelSidecarClient` class to create the actions. See `tests/test_actions.py` for many examples of using Actions and Handlers.\n\n## Handlers\n\nWhen the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods `handle_<msg_type>`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.\n\n## Comms\n\nComms are a flexible way for a client and the Kernel to send messages outside of the `execute_request` format. The most widely used package that utilizes Comms is probably `ipywidgets`, but Comms in general are a very powerful tool for a Sidecar application. A Comm can be opened by either the Sidecar or the Kernel. A target for that Comm should be registered on the other side before the open happens. It\'s probably most typical to register a Comm target in the Kernel by sending an `execute_request`, then sending a `comm_open` from the Sidecar side. See `tests/test_comms.py` for examples.\n\nOnce a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will automatically route all `comm_msg` messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but it\'s necessary because `comm_msg` can come in as a result of `execute_request`\'s or `comm_msg`\'s or potentially other messages. So the `CommManager` -> `CommHandler` routing basically needs to be applied to every message the `KernelSidecarClient` receives over ZMQ.\n\n\n## Models\n\n`kernel-sidecar` has Pydantic models for:\n - The Jupyter Notebook document (`models/notebook.py`), which should be consistent with `nbformat` parsing / structure\n - Request messages sent to the Kernel over ZMQ (`models/requests.py`)\n - Messages received over ZMQ from the Kernel (`models/messages.py`)\n\n\n## CLI\n\n`kernel-sidecar` ships a small CLI for testing a connection to a Kernel.\n\n```bash\n❯ sidecar --help\nUsage: sidecar [OPTIONS]\n\nOptions:\n  -f FILE                         Kernel connection file  [required]\n  --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]\n  --execute TEXT                  Execute code string instead of sending\n                                  kernel info request\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n```\n\nTry it out by starting an IPython kernel in one terminal and using the CLI in another.\n\n```bash\npython -m ipykernel_launcher --debug -f /tmp/kernel.json\n```\n\n```bash\nkernel-sidecar on \ue0a0 release-0.3.2 [$?] is 📦 v0.3.1 via 🐍 v3.11.0 (kernel-sidecar-py3.11) \n❯ sidecar -f /tmp/kernel.json\n2023-03-10T14:31:59.992235Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:32:00.026503Z [info     ] {\'banner\': \'Python 3.11.0 (main, Nov  7 2022, 09:38:45) [GCC 9.4.0]\\n\'\n           "Type \'copyright\', \'credits\' or \'license\' for more information\\n"\n           "IPython 8.10.0 -- An enhanced Interactive Python. Type \'?\' for "\n           \'help.\\n\',\n \'debugger\': None,\n \'help_links\': [{\'text\': \'Python Reference\',\n                 \'url\': \'https://docs.python.org/3.11\'},\n                {\'text\': \'IPython Reference\',\n                 \'url\': \'https://ipython.org/documentation.html\'},\n                {\'text\': \'NumPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/numpy/reference/\'},\n                {\'text\': \'SciPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/scipy/reference/\'},\n                {\'text\': \'Matplotlib Reference\',\n                 \'url\': \'https://matplotlib.org/contents.html\'},\n                {\'text\': \'SymPy Reference\',\n                 \'url\': \'http://docs.sympy.org/latest/index.html\'},\n                {\'text\': \'pandas Reference\',\n                 \'url\': \'https://pandas.pydata.org/pandas-docs/stable/\'}],\n \'implementation\': \'ipython\',\n \'implementation_version\': \'8.10.0\',\n \'language_info\': {\'codemirror_mode\': {\'name\': \'ipython\', \'version\': 3},\n                   \'file_extension\': \'.py\',\n                   \'mimetype\': \'text/x-python\',\n                   \'name\': \'python\',\n                   \'nbconvert_exporter\': \'python\',\n                   \'pygments_lexer\': \'ipython3\',\n                   \'version\': \'3.11.0\'},\n \'protocol_version\': \'5.3\',\n \'status\': \'ok\'} [kernel_sidecar.cli] filename=cli.py func_name=connect lineno=44\n```\n\n```bash\n❯ sidecar -f /tmp/kernel.json --execute "print(\'Hello, World\'); 1/0"\n2023-03-10T14:33:27.394935Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:33:27.629630Z [info     ] Hello, World\n                  [kernel_sidecar.cli] filename=cli.py func_name=handle_stream lineno=23\n2023-03-10T14:33:27.702700Z [error    ] division by zero               [kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31\n```\n',
+    'long_description': '<p align="center">\nKernel Sidecar\n</p>\n\n<p align="center">\n<img alt="Pypi" src="https://img.shields.io/pypi/v/kernel-sidecar">\n<a href="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml">\n    <img src="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml/badge.svg" alt="Tests" />\n</a>\n<img alt="Python versions" src="https://img.shields.io/pypi/pyversions/kernel-sidecar">\n</p>\n\n# Kernel-Sidecar\n\nThis package offers the building blocks for creating a "Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture, one or many frontends manage the document model (code cells, outputs, metadata, etc) and send requests to a single Kernel. Each frontend observes responses on different ZMQ channels (`iopub`, `shell`, etc) but may end up with some inconsistency based on the Kernel only sending certain responses to the client that made the request.\n\nIn a `kernel-sidecar` architecture, all frontend clients talk to the `kernel-sidecar` client, and only the `kernel-sidecar` client communicates with the Kernel over ZMQ. That pattern offers several potential features:\n - Keep a document model within `kernel-sidecar` or the backend architecture\n - Add "extension"-esque capabilities on the backend such as auto-linting code on execute\n - Eliminate inconsistencies in what messages individual frontends receive because of Kernel replies\n - Model all requests, replies, and the Notebook document with Pydantic\n\n## Installation\n\n```bash\npip install kernel-sidecar\n```\n\n# Key Concepts\n## KernelSidecarClient\n\nA manager that uses `jupyter_client` under the hood to create ZMQ connections and watch for messages coming in over different ZMQ channels (`iopub`, `shell`, etc. An important assumption here is that `kernel-sidecar` is the only client talking to the Kernel, which means every message observed coming from the Kernel should be a reply (based on `parent_header_msg.msg_id`) to a request sent from this client.\n\nWhen the `KernelSidecarClient` send a request to the Kernel, it is wrapped in an `KernelAction` class. Every message received from the Kernel is delegated to the requesting Action and triggers callbacks attached to the Action class.\n\n## Actions\n\nActions in `kernel-sidecar` encompass a request-reply cycle, including an `await action` syntax, where the Action is complete when the Kernel has reported its status returning to `idle` and optionally emitted a reply appropriate for the request. For instance, an `execute_request` is "done" when the `status` has been reported as `idle` *and* the Kernel has emitted an `execute_reply`, both with the `parent_header_msg.msg_id` the same as the `execute_request` `header.msg_id`.\n\nIn a nutshell, an `actions.KernelAction` takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses (or just `async functions`) and creates an `awaitable` instance. `kernel.send(action)` submits the Request over ZMQ, and registers the Action so that all observed messages get routed to that Action to be handled by the Handlers/callbacks.\n\nMost of the time, you should be able to just use convience functions in the `KernelSidecarClient` class to create the actions. See `tests/test_actions.py` for many examples of using Actions and Handlers.\n\n## Handlers\n\nWhen the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods `handle_<msg_type>`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.\n\n## Comms\n\nComms are a flexible way for a client and the Kernel to send messages outside of the `execute_request` format. The most widely used package that utilizes Comms is probably `ipywidgets`, but Comms in general are a very powerful tool for a Sidecar application. A Comm can be opened by either the Sidecar or the Kernel. A target for that Comm should be registered on the other side before the open happens. It\'s probably most typical to register a Comm target in the Kernel by sending an `execute_request`, then sending a `comm_open` from the Sidecar side. See `tests/test_comms.py` for examples.\n\nOnce a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will automatically route all `comm_msg` messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but it\'s necessary because `comm_msg` can come in as a result of `execute_request`\'s or `comm_msg`\'s or potentially other messages. So the `CommManager` -> `CommHandler` routing basically needs to be applied to every message the `KernelSidecarClient` receives over ZMQ.\n\n\n## Models\n\n`kernel-sidecar` has Pydantic models for:\n - The Jupyter Notebook document (`models/notebook.py`), which should be consistent with `nbformat` parsing / structure\n - Request messages sent to the Kernel over ZMQ (`models/requests.py`)\n - Messages received over ZMQ from the Kernel (`models/messages.py`)\n\n\n## CLI\n\n`kernel-sidecar` ships a small CLI for testing a connection to a Kernel.\n\n```bash\n❯ sidecar --help\nUsage: sidecar [OPTIONS]\n\nOptions:\n  -f FILE                         Kernel connection file  [required]\n  --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]\n  --execute TEXT                  Execute code string instead of sending\n                                  kernel info request\n  --tail / --no-tail              Continue tailing ZMQ after connecting or\n                                  executing code  [default: no-tail]\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n```\n\nTry it out by starting an IPython kernel in one terminal and using the CLI in another.\n\n```bash\npython -m ipykernel_launcher --debug -f /tmp/kernel.json\n```\n\n```bash\nkernel-sidecar on \ue0a0 release-0.3.2 [$?] is 📦 v0.3.1 via 🐍 v3.11.0 (kernel-sidecar-py3.11) \n❯ sidecar -f /tmp/kernel.json\n2023-03-10T14:31:59.992235Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:32:00.026503Z [info     ] {\'banner\': \'Python 3.11.0 (main, Nov  7 2022, 09:38:45) [GCC 9.4.0]\\n\'\n           "Type \'copyright\', \'credits\' or \'license\' for more information\\n"\n           "IPython 8.10.0 -- An enhanced Interactive Python. Type \'?\' for "\n           \'help.\\n\',\n \'debugger\': None,\n \'help_links\': [{\'text\': \'Python Reference\',\n                 \'url\': \'https://docs.python.org/3.11\'},\n                {\'text\': \'IPython Reference\',\n                 \'url\': \'https://ipython.org/documentation.html\'},\n                {\'text\': \'NumPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/numpy/reference/\'},\n                {\'text\': \'SciPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/scipy/reference/\'},\n                {\'text\': \'Matplotlib Reference\',\n                 \'url\': \'https://matplotlib.org/contents.html\'},\n                {\'text\': \'SymPy Reference\',\n                 \'url\': \'http://docs.sympy.org/latest/index.html\'},\n                {\'text\': \'pandas Reference\',\n                 \'url\': \'https://pandas.pydata.org/pandas-docs/stable/\'}],\n \'implementation\': \'ipython\',\n \'implementation_version\': \'8.10.0\',\n \'language_info\': {\'codemirror_mode\': {\'name\': \'ipython\', \'version\': 3},\n                   \'file_extension\': \'.py\',\n                   \'mimetype\': \'text/x-python\',\n                   \'name\': \'python\',\n                   \'nbconvert_exporter\': \'python\',\n                   \'pygments_lexer\': \'ipython3\',\n                   \'version\': \'3.11.0\'},\n \'protocol_version\': \'5.3\',\n \'status\': \'ok\'} [kernel_sidecar.cli] filename=cli.py func_name=connect lineno=44\n```\n\n```bash\n❯ sidecar -f /tmp/kernel.json --execute "print(\'Hello, World\'); 1/0"\n2023-03-10T14:33:27.394935Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:33:27.629630Z [info     ] Hello, World\n                  [kernel_sidecar.cli] filename=cli.py func_name=handle_stream lineno=23\n2023-03-10T14:33:27.702700Z [error    ] division by zero               [kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31\n```\n',
     'author': 'Matt Kafonek',
     'author_email': 'matt.kafonek@noteable.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kafonek/kernel-sidecar',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['kernel_sidecar', 'kernel_sidecar.handlers',
 'kernel_sidecar.models'] package_data = \ {'': ['*']} install_requires = \
 ['jupyter-client>=7.3.4', 'pydantic>=1.10.4,<2.0.0'] extras_require = \ {'cli':
 ['structlog', 'typer']} entry_points = \ {'console_scripts': ['sidecar =
 kernel_sidecar.cli:app']} setup_kwargs = { 'name': 'kernel-sidecar', 'version':
-'0.5.1', 'description': 'A sidecar ', 'long_description': '
+'0.5.2', 'description': 'A sidecar ', 'long_description': '
                               \nKernel Sidecar\n
 \n\n
                   \n[Pypi]\n\n_[Tests]\n\n[Python versions]\n
 \n\n# Kernel-Sidecar\n\nThis package offers the building blocks for creating a
 "Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture,
 one or many frontends manage the document model (code cells, outputs, metadata,
 etc) and send requests to a single Kernel. Each frontend observes responses on
@@ -72,15 +72,16 @@
 notebook.py`), which should be consistent with `nbformat` parsing / structure\n
 - Request messages sent to the Kernel over ZMQ (`models/requests.py`)\n -
 Messages received over ZMQ from the Kernel (`models/messages.py`)\n\n\n##
 CLI\n\n`kernel-sidecar` ships a small CLI for testing a connection to a
 Kernel.\n\n```bash\nâ¯ sidecar --help\nUsage: sidecar [OPTIONS]\n\nOptions:\n
 -f FILE Kernel connection file [required]\n --debug / --no-debug Turn on DEBUG
 logging [default: no-debug]\n --execute TEXT Execute code string instead of
-sending\n kernel info request\n --install-completion
+sending\n kernel info request\n --tail / --no-tail Continue tailing ZMQ after
+connecting or\n executing code [default: no-tail]\n --install-completion
 [bash|zsh|fish|powershell|pwsh]\n Install completion for the specified shell.\n
 --show-completion [bash|zsh|fish|powershell|pwsh]\n Show completion for the
 specified shell, to\n copy it or customize the installation.\n --help Show this
 message and exit.\n```\n\nTry it out by starting an IPython kernel in one
 terminal and using the CLI in another.\n\n```bash\npython -m ipykernel_launcher
 --debug -f /tmp/kernel.json\n```\n\n```bash\nkernel-sidecar on \ue0a0 release-
 0.3.2 [$?] is ð¦ v0.3.1 via ð v3.11.0 (kernel-sidecar-py3.11) \nâ¯
```

### Comparing `kernel_sidecar-0.5.1/PKG-INFO` & `kernel_sidecar-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernel-sidecar
-Version: 0.5.1
+Version: 0.5.2
 Summary: A sidecar 
 Home-page: https://github.com/kafonek/kernel-sidecar
 License: MIT
 Author: Matt Kafonek
 Author-email: matt.kafonek@noteable.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -92,14 +92,16 @@
 Usage: sidecar [OPTIONS]
 
 Options:
   -f FILE                         Kernel connection file  [required]
   --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]
   --execute TEXT                  Execute code string instead of sending
                                   kernel info request
+  --tail / --no-tail              Continue tailing ZMQ after connecting or
+                                  executing code  [default: no-tail]
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.1 Summary: A sidecar
+Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.2 Summary: A sidecar
 Home-page: https://github.com/kafonek/kernel-sidecar License: MIT Author: Matt
 Kafonek Author-email: matt.kafonek@noteable.io Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli Requires-Dist: jupyter-client (>=7.3.4) Requires-Dist:
@@ -73,15 +73,16 @@
 Jupyter Notebook document (`models/notebook.py`), which should be consistent
 with `nbformat` parsing / structure - Request messages sent to the Kernel over
 ZMQ (`models/requests.py`) - Messages received over ZMQ from the Kernel
 (`models/messages.py`) ## CLI `kernel-sidecar` ships a small CLI for testing a
 connection to a Kernel. ```bash â¯ sidecar --help Usage: sidecar [OPTIONS]
 Options: -f FILE Kernel connection file [required] --debug / --no-debug Turn on
 DEBUG logging [default: no-debug] --execute TEXT Execute code string instead of
-sending kernel info request --install-completion
+sending kernel info request --tail / --no-tail Continue tailing ZMQ after
+connecting or executing code [default: no-tail] --install-completion
 [bash|zsh|fish|powershell|pwsh] Install completion for the specified shell. --
 show-completion [bash|zsh|fish|powershell|pwsh] Show completion for the
 specified shell, to copy it or customize the installation. --help Show this
 message and exit. ``` Try it out by starting an IPython kernel in one terminal
 and using the CLI in another. ```bash python -m ipykernel_launcher --debug -f /
 tmp/kernel.json ``` ```bash kernel-sidecar on î  release-0.3.2 [$?] is ð¦
 v0.3.1 via ð v3.11.0 (kernel-sidecar-py3.11) â¯ sidecar -f /tmp/kernel.json
```

