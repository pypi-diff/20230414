# Comparing `tmp/diator-0.1.0.tar.gz` & `tmp/diator-0.1.1.tar.gz`

## Comparing `diator-0.1.0.tar` & `diator-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 diator-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/mediator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/py.typed
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/container/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/container/di.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/container/protocol.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/container/rodi.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/dispatcher/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/dispatcher/default.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/dispatcher/dispatch_result.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/dispatcher/protocol.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/events/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/events/event.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/events/event_emitter.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/events/event_handler.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/events/map.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/message_brokers/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/message_brokers/azure.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/message_brokers/protocol.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/message_brokers/redis.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/middlewares/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/middlewares/base.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/middlewares/logging.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/requests/__init__.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/requests/map.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/requests/request.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 diator-0.1.0/src/diator/requests/request_handler.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 diator-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 diator-0.1.0/LICENSE.rst
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 diator-0.1.0/README.md
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 diator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 diator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 diator-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/__init__.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/mediator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/py.typed
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/di.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/protocol.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/rodi.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/__init__.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/default.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/dispatch_result.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/protocol.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event_emitter.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event_handler.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/map.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/azure.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/protocol.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/redis.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/base.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/logging.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/map.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/request.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/request_handler.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 diator-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 diator-0.1.1/LICENSE.rst
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 diator-0.1.1/README.md
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 diator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 diator-0.1.1/PKG-INFO
```

### Comparing `diator-0.1.0/src/diator/mediator.py` & `diator-0.1.1/src/diator/mediator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
       redis_client = Redis()  # async redis client
       message_broker = RedisMessageBroker(redis_client)
       event_map = EventMap()
       event_map.bind(UserJoinedDomainEvent, UserJoinedDomainEventHandler)
       request_map = RequestMap()
       request_map.bind(JoinUserCommand, JoinUserCommandHandler)
-      event_emitter = EventEmitter(message_broker, event_emitter, container)
+      event_emitter = EventEmitter(event_map, container, message_broker)
 
       mediator = Mediator(
         event_emitter=event_emitter,
         request_map=request_map,
         container=container
       )
```

### Comparing `diator-0.1.0/src/diator/response.py` & `diator-0.1.1/src/diator/response.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/container/di.py` & `diator-0.1.1/src/diator/container/di.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/container/rodi.py` & `diator-0.1.1/src/diator/container/rodi.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/dispatcher/default.py` & `diator-0.1.1/src/diator/dispatcher/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ) -> None:
         self._request_map = request_map
         self._container = container
         self._middleware_chain = middleware_chain or MiddlewareChain()
 
     async def dispatch(self, request: Request) -> DispatchResult:
         handler_type = self._request_map.get(type(request))
+
         handler = await self._container.resolve(handler_type)
 
         wrapped_handle = self._middleware_chain.wrap(handler.handle)
 
         response = await wrapped_handle(request)
 
         return DispatchResult(response=response, events=handler.events)
```

### Comparing `diator-0.1.0/src/diator/events/event.py` & `diator-0.1.1/src/diator/events/event.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/events/event_emitter.py` & `diator-0.1.1/src/diator/events/event_emitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,33 @@
     Usage::
 
       redis_client = Redis()  # async redis client
       message_broker = RedisMessageBroker(redis_client)
       event_map =  EventMap()
       event_map.bind(UserJoinedDomainEvent, UserJoinedDomainEventHandler)
 
-      event_emitter = EventEmitter(message_broker, event_emitter, container)
+      event_emitter = EventEmitter(event_map, container, message_broker)
 
       # Uses UserJoinedDomainEventHandler for handling event:
       await event_emitter.emit(user_joined_domain_event)
 
       # Sends event to the Redis Pub/Sub:
       await event_emitter.emit(user_joined_notification_event)
 
     """
 
-    def __init__(self, message_broker: MessageBroker, event_map: EventMap, container: Container) -> None:
-        self._message_broker = message_broker
+    def __init__(
+        self,
+        event_map: EventMap,
+        container: Container,
+        message_broker: MessageBroker | None = None,
+    ) -> None:
         self._event_map = event_map
         self._container = container
+        self._message_broker = message_broker
 
     @singledispatchmethod
     async def emit(self, event: Event) -> None:
         ...
 
     @emit.register
     async def _(self, event: DomainEvent) -> None:
@@ -53,26 +58,32 @@
                 type(event).__name__,
                 handler_type.__name__,
             )
             await handler.handle(event)
 
     @emit.register
     async def _(self, event: NotificationEvent) -> None:
+        if not self._message_broker:
+            raise RuntimeError("To use NotificationEvent, message_broker argument must be specified.")
+
         message = _build_message(event)
 
         logger.debug(
             "Sending Notification Event(%s) to message broker %s",
             event.event_id,
             type(self._message_broker).__name__,
         )
 
         await self._message_broker.send_message(message)
 
     @emit.register
     async def _(self, event: ECSTEvent) -> None:
+        if not self._message_broker:
+            raise RuntimeError("To use ECSTEvent, message_broker argument must be specified.")
+
         message = _build_message(event)
 
         logger.debug(
             "Sending ECST event(%s) to message broker %s",
             event.event_id,
             type(self._message_broker).__name__,
         )
```

### Comparing `diator-0.1.0/src/diator/events/event_handler.py` & `diator-0.1.1/src/diator/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/events/map.py` & `diator-0.1.1/src/diator/events/map.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,7 +15,10 @@
         self._event_map[event_type].append(handler_type)
 
     def get(self, event_type: Type[E]) -> list[Type[EventHandler[E]]]:
         return self._event_map[event_type]
 
     def get_events(self) -> list[Type[DomainEvent]]:
         return list(self._event_map.keys())
+
+    def __str__(self) -> str:
+        return str(self._event_map)
```

### Comparing `diator-0.1.0/src/diator/message_brokers/azure.py` & `diator-0.1.1/src/diator/message_brokers/azure.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/message_brokers/protocol.py` & `diator-0.1.1/src/diator/message_brokers/protocol.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/message_brokers/redis.py` & `diator-0.1.1/src/diator/message_brokers/redis.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/middlewares/base.py` & `diator-0.1.1/src/diator/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/middlewares/logging.py` & `diator-0.1.1/src/diator/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/requests/map.py` & `diator-0.1.1/src/diator/requests/map.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,10 +18,13 @@
     def get(self, request_type: Type[Request]) -> Type[RequestHandler]:
         handler_type = self._request_map.get(request_type)
         if not handler_type:
             raise RequestHandlerDoesNotExist("RequestHandler not found matching Request type.")
 
         return handler_type
 
+    def __str__(self) -> str:
+        return str(self._request_map)
+
 
 class RequestHandlerDoesNotExist(Exception):
     ...
```

### Comparing `diator-0.1.0/src/diator/requests/request.py` & `diator-0.1.1/src/diator/requests/request.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/src/diator/requests/request_handler.py` & `diator-0.1.1/src/diator/requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/.gitignore` & `diator-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/LICENSE.rst` & `diator-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `diator-0.1.0/README.md` & `diator-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 - Supports multiple message brokers, such as [Redis Pub/Sub](https://redis.io/docs/manual/pubsub/) and [Azure Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-messaging-overview)
 - Easy to integrate with existing codebases
 
 ## Installation :triangular_ruler:
 
 Install the Diator library with [pip](https://pypi.org/project/diator/)
 
+```bash
+pip install diator
+```
+
+There are also several installation options:
+
 - To use Redis as Message Broker
 
     ```bash
     pip install diator[redis]
     ```
 
 - Or Azure Service Bus
@@ -132,15 +138,15 @@
 - **Event-carried state transfer (ECST)** - messages notify subscribers about changes in the producer’s internal state.
 
 ```python
 from diator.events import DomainEvent, NotificationEvent, ECSTEvent
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
-class UserJoinedDomainEvent(Event):  # will be handled by an event handler
+class UserJoinedDomainEvent(DomainEvent):  # will be handled by an event handler
     user_id: int = dataclasses.field()
     meeting_id: int = dataclasses.field()
     timestamp: datetime = dataclasses.field()
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class UserJoinedNotificationEvent(NotificationEvent):  # will be sent to a message broker
@@ -203,27 +209,27 @@
 from di import Container, bind_by_type  # using di lib as di-framework
 from diator.container.di import DIContainer
 
 
 def setup_di() -> DIContainer:
     external_container = Container()
 
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(UserJoinedDomainEventHandler, scope="request"), 
             UserJoinedDomainEventHandler
         )
     )
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(JoinMeetingCommandHandler, scope="request"),
             JoinMeetingCommandHandler,
         )
     )
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(ReadMeetingQueryHandler, scope="request"),
             ReadMeetingQueryHandler,
         )
     )
 
     container = DIContainer()
```

### Comparing `diator-0.1.0/pyproject.toml` & `diator-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "diator"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Murad Akhundov", email = "akhundov1murad@gmail.com" }]
 description = "Diator is a Python library for implementing CQRS pattern in your Python applications."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `diator-0.1.0/PKG-INFO` & `diator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Diator is a Python library for implementing CQRS pattern in your Python applications.
 Project-URL: Homepage, https://github.com/akhundMurad/diator
 Project-URL: Bug Tracker, https://github.com/akhundMurad/diator/issues
 Author-email: Murad Akhundov <akhundov1murad@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.rst
 Keywords: CQRS,async,asyncio,command,commands,di,diator,event,events,mediator,mediatr,queries,query
@@ -41,14 +41,20 @@
 - Supports multiple message brokers, such as [Redis Pub/Sub](https://redis.io/docs/manual/pubsub/) and [Azure Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-messaging-overview)
 - Easy to integrate with existing codebases
 
 ## Installation :triangular_ruler:
 
 Install the Diator library with [pip](https://pypi.org/project/diator/)
 
+```bash
+pip install diator
+```
+
+There are also several installation options:
+
 - To use Redis as Message Broker
 
     ```bash
     pip install diator[redis]
     ```
 
 - Or Azure Service Bus
@@ -164,15 +170,15 @@
 - **Event-carried state transfer (ECST)** - messages notify subscribers about changes in the producer’s internal state.
 
 ```python
 from diator.events import DomainEvent, NotificationEvent, ECSTEvent
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
-class UserJoinedDomainEvent(Event):  # will be handled by an event handler
+class UserJoinedDomainEvent(DomainEvent):  # will be handled by an event handler
     user_id: int = dataclasses.field()
     meeting_id: int = dataclasses.field()
     timestamp: datetime = dataclasses.field()
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class UserJoinedNotificationEvent(NotificationEvent):  # will be sent to a message broker
@@ -235,27 +241,27 @@
 from di import Container, bind_by_type  # using di lib as di-framework
 from diator.container.di import DIContainer
 
 
 def setup_di() -> DIContainer:
     external_container = Container()
 
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(UserJoinedDomainEventHandler, scope="request"), 
             UserJoinedDomainEventHandler
         )
     )
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(JoinMeetingCommandHandler, scope="request"),
             JoinMeetingCommandHandler,
         )
     )
-    container.bind(
+    external_container.bind(
         bind_by_type(
             Dependent(ReadMeetingQueryHandler, scope="request"),
             ReadMeetingQueryHandler,
         )
     )
 
     container = DIContainer()
```

