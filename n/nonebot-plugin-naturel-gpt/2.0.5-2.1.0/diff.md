# Comparing `tmp/nonebot_plugin_naturel_gpt-2.0.5.tar.gz` & `tmp/nonebot_plugin_naturel_gpt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_naturel_gpt-2.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.0.tar", max compression
```

## Comparing `nonebot_plugin_naturel_gpt-2.0.5.tar` & `nonebot_plugin_naturel_gpt-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.0.5/LICENSE
--rw-r--r--   0        0        0     2319 2023-04-05 16:12:46.781524 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/__init__.py
--rw-r--r--   0        0        0    25036 2023-04-05 16:12:46.783455 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/chat.py
--rw-r--r--   0        0        0     5984 2023-03-31 09:56:17.960037 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/chat_manager.py
--rw-r--r--   0        0        0    23008 2023-04-05 16:12:46.784459 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/command_func.py
--rw-r--r--   0        0        0    12093 2023-04-05 16:12:46.785455 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/config.py
--rw-r--r--   0        0        0     6159 2023-04-05 16:12:46.780526 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/Extension.py
--rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/logger.py
--rw-r--r--   0        0        0    26790 2023-04-05 16:12:46.787451 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/matcher.py
--rw-r--r--   0        0        0     9868 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/openai_func.py
--rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/persistent_data_manager.py
--rw-r--r--   0        0        0      484 2023-03-16 11:26:31.740167 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/singleton.py
--rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/store.py
--rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/text_func.py
--rw-r--r--   0        0        0     4350 2023-03-31 09:56:17.964030 nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/utils.py
--rw-r--r--   0        0        0      577 2023-04-05 19:20:47.710169 nonebot_plugin_naturel_gpt-2.0.5/pyproject.toml
--rw-r--r--   0        0        0    46261 2023-04-05 19:21:36.064258 nonebot_plugin_naturel_gpt-2.0.5/README.md
--rw-r--r--   0        0        0    46326 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2319 2023-04-05 16:12:46.781524 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/__init__.py
+-rw-r--r--   0        0        0    25967 2023-04-14 14:31:43.610190 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat.py
+-rw-r--r--   0        0        0     5984 2023-03-31 09:56:17.960037 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat_manager.py
+-rw-r--r--   0        0        0    23008 2023-04-05 16:12:46.784459 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/command_func.py
+-rw-r--r--   0        0        0    12717 2023-04-14 13:54:29.320533 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/config.py
+-rw-r--r--   0        0        0     6159 2023-04-05 16:12:46.780526 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/Extension.py
+-rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/logger.py
+-rw-r--r--   0        0        0    34619 2023-04-14 16:29:00.530610 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/matcher.py
+-rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
+-rw-r--r--   0        0        0     6269 2023-04-14 14:50:18.078484 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
+-rw-r--r--   0        0        0     9912 2023-04-08 05:19:53.226132 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/openai_func.py
+-rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/persistent_data_manager.py
+-rw-r--r--   0        0        0      484 2023-03-16 11:26:31.740167 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/singleton.py
+-rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/store.py
+-rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/text_func.py
+-rw-r--r--   0        0        0     4350 2023-03-31 09:56:17.964030 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/utils.py
+-rw-r--r--   0        0        0      577 2023-04-13 19:28:04.696750 nonebot_plugin_naturel_gpt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    49844 2023-04-14 16:31:16.401955 nonebot_plugin_naturel_gpt-2.1.0/README.md
+-rw-r--r--   0        0        0    49862 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/LICENSE` & `nonebot_plugin_naturel_gpt-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/__init__.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/chat.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             if config.DEBUG_LEVEL > 0: logger.info(f"增强记忆比较: {response} vs {mem_value} = {compare_score}")
             if compare_score > config.CHAT_MEMORY_ENHANCE_THRESHOLD:
                 self.set_memory(mem_key, mem_value)
                 if config.DEBUG_LEVEL > 0: logger.info(f"记忆 {mem_key} 相似度 {compare_score} 超过阈值 {config.CHAT_MEMORY_ENHANCE_THRESHOLD}, 增强记忆")
                 return True
         return False
 
-    def get_chat_prompt_template(self, userid:str = None)-> str:
+    def get_chat_prompt_template(self, userid:str = None, chat_type:str = '')-> str:
         """对话 prompt 模板生成"""
         # 印象描述
         impression_text = f"[impression]\n{self._chat_preset.chat_impressions[userid].chat_impression}\n\n" \
             if userid in self._chat_preset.chat_impressions else ''  # 用户印象描述
 
         # 记忆模块
         memory_text = ''
@@ -181,15 +181,20 @@
                 chat_history = self._chat_data.chat_history[-1]
                 break
 
         # 对话历史摘要
         summary = f"\n\n[Summary]: {self._chat_data.chat_summarized}" if self._chat_data.chat_summarized else ''  # 如果有对话历史摘要，则添加摘要
 
         # 扩展描述
-        ext_descs = ''.join([global_extensions[ek].generate_description(chat_history) for ek in global_extensions.keys()])
+        if chat_type != 'server':   # 如果是聊天模式，则显示所有支持聊天的扩展
+            # ext_descs = ''.join([global_extensions[ek].generate_description(chat_history) for ek in global_extensions.keys()])
+            ext_descs = ''.join([global_extensions[ek].generate_description(chat_history) for ek in global_extensions.keys() if 'chat' in global_extensions[ek].get_config().get('available', ['chat'])])
+        else:   # 如果是MC服务器，则只显示服务器扩展
+            ext_descs = ''.join([global_extensions[ek].generate_description(chat_history) for ek in global_extensions.keys() if 'server' in global_extensions[ek].get_config().get('available', ['server'])])
+
         # 扩展使用示例
         extension_text = (
             f"[Extension functions: You can use the following extension functions. The extension module can be invoked multiple times in a single response.]\n"
             # 'Including the above content in a chat message will call the extension module for processing.\n'
             # 'importrant: The extension option is available if and only if in the following strict format. Multiple options can be used in one response.\n'
             # '- Random > min:a; max:b (send a random number between a and b)'
             # 'Following the following format in the response will invoke the extension module for the corresponding implementation. The extension module can be invoked multiple times in a single response.\n'
@@ -225,19 +230,27 @@
         #     f"\n{summary}\n{impression_text}\n{memory}"
         #     f"{extension_text}"
         #     f"{res_rule_prompt}"
         #     f"\n[Chat History (current time: {time.strftime('%Y-%m-%d %H:%M:%S')})]\n"
         #     f"\n{chat_history}\n{self.chat_presets['preset_key']}:"
         # )
 
+        # 在 MC 服务器下 prompt 支持
+        MC_prompt = (
+            f"You are now in a Minecraft game server."
+        ) if chat_type == 'server' else ''
+        chat_history_title = (
+            "Minecraft game server chat log"
+        ) if chat_type == 'server' else "Chat History"
+
         # 返回对话 prompt 模板
         return [
             {'role': 'system', 'content': ( # 系统消息
                 # f"You must strictly follow the user's instructions to give {self.chat_presets['preset_key']}'s response."
-                f"You must follow the user's instructions to play the specified role in the first person and give the response information according to the changed role. If necessary, you can generate a reply in the specified format to call the extension function."
+                f"{MC_prompt}You must follow the user's instructions to play the specified role in the first person and give the response information according to the changed role. If necessary, you can generate a reply in the specified format to call the extension function."
                 f"\n{extension_text}"
                 f"\n{res_rule_prompt}"
             )},
             {'role': 'user', 'content': (   # 用户消息(演示场景)
                 f"[Character setting]\nAI is an assistant robot.\n\n"
                 # "[memory (max length: 16 - Delete the unimportant memory in time before exceed it)]"
                 f"[history memory (max length: {config.MEMORY_MAX_LENGTH} - Please delete the unimportant memory in time before exceed it)]\n"
@@ -250,15 +263,15 @@
             )},
             {'role': 'assistant', 'content': (  # 助手消息(演示输出)
                 "ok, I will send an email, please wait a moment /#email&example@mail.com&test title&hello this is a test#/ *; I have sent an e-mail. Did you get it?"
             )},
             {'role': 'user', 'content': (   # 用户消息(实际场景)
                 f"[Character setting]\n{self._chat_preset.bot_self_introl}\n\n"
                 f"{memory}{impression_text}{summary}"
-                f"\n[Chat History (current time: {time.strftime('%Y-%m-%d %H:%M:%S %A')})]\n"
+                f"\n[{chat_history_title} (current time: {time.strftime('%Y-%m-%d %H:%M:%S %A')})]\n"
                 f"\n{chat_history}\n\n{self._chat_preset.preset_key}:(Generate the response content of {self._chat_preset.preset_key}, excluding '{self._chat_preset.preset_key}:', Do not generate any reply from anyone else.)"
             )},
         ]
 
 
     # region --------------------以下为基本信息获取函数和属性--------------------
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/chat_manager.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/command_func.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/command_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/config.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,14 +132,29 @@
 
     NG_EXT_LOAD_LIST: List[ExtConfig]
     """加载的扩展列表"""
 
     NG_CHECK_USER_NAME_HYPHEN:bool # 如果用户名中包含连字符，ChatGPT会将前半部分识别为名字，但一般情况下后半部分才是我们想被称呼的名字, eg. 策划-李华
     """检查用户名中的连字符"""
 
+    ENABLE_MC_CONNECT: bool
+    """是否启用MC服务器连接"""
+
+    MC_COMMAND_PREFIX: List[str]
+    """MC服务器人格指令前缀"""
+
+    MC_RCON_HOST: str
+    """MC服务器RCON地址"""
+
+    MC_RCON_PORT: int
+    """MC服务器RCON端口"""
+
+    MC_RCON_PASSWORD: str
+    """MC服务器RCON密码"""
+
     DEBUG_LEVEL: int
     """debug level, [0, 1, 2, 3], 0 为关闭，等级越高debug信息越详细"""
 
 # 配置文件模板(把全部默认值写到Config定义里比较乱，因此保留此默认值对象,作为真实的默认值)
 CONFIG_TEMPLATE = {
     "OPENAI_API_KEYS": [    # OpenAI API Key 列表
         'sk-xxxxxxxxxxxxx',
@@ -235,14 +250,21 @@
         'EXT_NAME': 'ext_random',
         'IS_ACTIVE': False,
         'EXT_CONFIG': {'arg': 'arg_value'},
     }],     # 加载的扩展列表
 
     'NG_CHECK_USER_NAME_HYPHEN': False, # 检查用户名中的连字符
 
+    'ENABLE_MC_CONNECT': False,  # 是否启用MC服务器
+    'MC_COMMAND_PREFIX': ['!', '！'],  # MC服务器指令前缀
+    'MC_RCON_HOST': '127.0.0.1',  # MC服务器RCON地址
+    'MC_RCON_PORT': 25575,  # MC服务器RCON端口
+    'MC_RCON_PASSWORD': '',  # MC服务器RCON密码
+
+
     'DEBUG_LEVEL': 0  # debug level, [0, 1, 2], 0 为关闭，等级越高debug信息越详细
 }
 
 driver = get_driver()
 global_config = GlobalConfig.parse_obj(driver.config)
 config_path = global_config.ng_config_path
 config:Config = None # type: ignore
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/Extension.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/Extension.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/matcher.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/matcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿import asyncio
-import difflib
+import json
 import random
 import re
 import time
 import os
 import traceback
 from typing import Awaitable, List, Dict, Callable, Optional, Set, Tuple
 from nonebot import get_driver
@@ -16,21 +16,33 @@
 from .utils import *
 from .chat import Chat
 from .persistent_data_manager import PersistentDataManager
 from .chat_manager import ChatManager
 from .Extension import Extension, global_extensions
 from .openai_func import TextGenerator
 from .command_func import CommandManager, cmd
+
 try:
     import nonebot_plugin_htmlrender
     from .text_func import text_to_img
 except:
+    logger.warning('未安装 nonebot_plugin_htmlrender 插件，无法使用 text_to_img')
     config.ENABLE_MSG_TO_IMG = False
     config.ENABLE_COMMAND_TO_IMG = False
 
+if config.ENABLE_MC_CONNECT:
+    try:
+        from nonebot.adapters.spigot import Bot as SpigotBot
+        from nonebot.adapters.spigot import Event as SpigotEvent
+        from .MCrcon.mcrcon import MCRcon   # fork from: https://github.com/Uncaught-Exceptions/MCRcon
+    except:
+        logger.warning('未安装 nonebot_plugin_spigot 适配器，无法使用 SpigotBot')
+        config.ENABLE_MC_CONNECT = False
+
+
 permission_check_func:Callable[[Matcher, MessageEvent, Bot, str, str], Awaitable[Tuple[bool,str]]] = None
 is_progress:bool = False
 
 msg_sent_set:Set[str] = set() # bot 自己发送的消息
 
 """消息发送钩子，用于记录自己发送的消息(默认不开启，只有在用户自定义了message_sent事件之后message_sent事件才会被发送到 on_message 回调)"""
 # @Bot.on_called_api
@@ -38,15 +50,15 @@
     global msg_sent_set
     if result and (api in ['send_msg', 'send_group_msg', 'send_private_msg']):
         msg_id = result.get('message_id', None)
         if msg_id:
             msg_sent_set.add(f"{bot.self_id}_{msg_id}")
 
 """ ======== 注册消息响应器 ======== """
-# 注册消息响应器 收到任意消息时触发
+# 注册qq消息响应器 收到任意消息时触发
 matcher:Matcher = on_message(priority=config.NG_MSG_PRIORITY, block=config.NG_BLOCK_OTHERS)
 @matcher.handle()
 async def handler(matcher_:Matcher, event: MessageEvent, bot:Bot) -> None:
     global msg_sent_set
     if event.post_type == 'message_sent': # 通过bot.send发送的消息不处理
         msg_key = f"{bot.self_id}_{event.message_id}"
         if msg_key in msg_sent_set:
@@ -108,14 +120,117 @@
         event.is_tome() or wake_up,
         matcher,
         chat_type,
         chat_key,
         sender_name,
     )
 
+# 注册MC消息响应器
+if config.ENABLE_MC_CONNECT:
+    mc_matcher:Matcher = on_message(priority=config.NG_MSG_PRIORITY-2, block=False)
+    @mc_matcher.handle()
+    async def handler(matcher_:Matcher, event: SpigotEvent, bot:SpigotBot) -> None:
+        # 处理消息前先检查权限
+        (permit_success, _) = await permission_check_func(matcher=matcher_, event=event, bot=bot, cmd=None, type='message')
+        if not permit_success:
+            return
+
+        try:
+            ejson_dict = json.loads(event.json())
+            server_from = event.server_name
+            sender_name = ejson_dict['player']['nickname']
+            chat_text = str(event.get_message())
+        except Exception as e:
+            logger.warning(f"[MC: {server_from}] 获取消息发送者信息失败: {e} 跳过处理...")
+            return
+
+        # 判断用户账号是否被屏蔽
+        if sender_name in config.FORBIDDEN_USERS:
+            if config.DEBUG_LEVEL > 0: logger.info(f"用户 {sender_name} 被屏蔽，拒绝处理消息")
+            return
+
+        resTmplate = (  # 测试用，获取消息的相关信息
+            f"收到消息: {chat_text}"
+            f"\n消息描述: {event.get_event_description()}"
+            f"\n发送者: {sender_name}"
+            f"\n消息来源: {server_from}"
+            f"\nJSON: {event.json()}"
+        )
+        if config.DEBUG_LEVEL > 1: logger.info(resTmplate)
+
+        # 如果是忽略前缀 或者 消息为空，则跳过处理
+        if chat_text.strip().startswith(config.IGNORE_PREFIX) or not chat_text:   
+            if config.DEBUG_LEVEL > 1: logger.info("忽略前缀或消息为空，跳过处理...") # 纯图片消息也会被判定为空消息
+            return
+
+        # 判断消息来源
+        if isinstance(event, SpigotEvent):
+            chat_key = 'MC_Server_' + server_from
+            chat_type = 'server'
+        else:
+            if config.DEBUG_LEVEL > 0: logger.info("未知消息来源: " + event.get_session_id())
+            return
+
+        #region 指令处理分支 (由于Spigot适配器似乎不支持指令，所以整合进消息响应流)
+        command_prefix_check = False
+        for prefix in config.MC_COMMAND_PREFIX:
+            if chat_text.startswith(prefix):
+                command_prefix_check = True
+                raw_cmd = chat_text[len(prefix):].strip()
+                break
+
+        if command_prefix_check:
+            global is_progress  # 是否产生编辑进度
+            is_progress = False
+            if config.DEBUG_LEVEL > 0: logger.info(f"接收到指令: {raw_cmd} | 来源: {chat_key} (MC) | 发送者: {sender_name})")
+            # 判断是否是禁止使用的用户
+            if sender_name in config.FORBIDDEN_USERS:
+                await mc_matcher.finish(f"您的账号({sender_name})已被禁用，请联系管理员。")
+
+            chat:Chat = ChatManager.instance.get_or_create_chat(chat_key=chat_key)
+            chat_presets_dict = chat.chat_data.preset_datas
+
+            # 执行命令前先检查权限
+            if sender_name not in config.ADMIN_USERID:
+                await mc_matcher.finish("对不起！你没有权限进行此操作 ＞﹏＜")
+
+            # 执行命令
+            res = cmd.execute(
+                chat=chat,
+                command=raw_cmd,
+                chat_presets_dict=chat_presets_dict,
+            )
+
+            if res:
+                if res.get('msg'):     # 如果有返回消息则发送
+                    await mc_matcher.send(res.get('msg'))  
+                elif res.get('error'):
+                    await mc_matcher.finish(f"执行命令时出现错误: {res.get('error')}")  # 如果有返回错误则发送s
+
+            else:
+                await mc_matcher.finish("输入的命令好像有点问题呢... 请检查下再试试吧！ ╮(>_<)╭")
+
+            if res.get('is_progress'): # 如果有编辑进度，进行数据保存
+                # 更新所有全局预设到会话预设中
+                if config.DEBUG_LEVEL > 0: logger.info(f"用户: {sender_name} 进行了人格预设编辑: {cmd}")
+                PersistentDataManager.instance.save_to_file()  # 保存数据
+            return
+        #endregion
+
+        # 进行消息响应
+        await do_msg_response(
+            sender_name,
+            chat_text,
+            event.is_tome(),
+            mc_matcher,
+            chat_type,
+            chat_key,
+            sender_name,
+        )
+
 
 """ ======== 注册通知响应器 ======== """
 # 欢迎新成员通知响应器
 welcome:Matcher = on_notice(priority=20, block=False)
 @welcome.handle()  # 监听 welcom
 async def _(matcher_:Matcher, event: GroupIncreaseNoticeEvent, bot:Bot):  # event: GroupIncreaseNoticeEvent  群成员增加事件
     if config.DEBUG_LEVEL > 0: logger.info(f"收到通知: {event}")
@@ -154,17 +269,68 @@
         welcome,
         chat_type,
         chat_key,
         '[System]',
         True
     )
 
+# 注册MC通知响应器
+if config.ENABLE_MC_CONNECT:
+    mc_notice_matcher:Matcher = on_notice(priority=20, block=False)
+    @mc_notice_matcher.handle()
+    async def handler(matcher_:Matcher, event: SpigotEvent, bot:SpigotBot) -> None:
+        try:
+            server_from = event.server_name
+            event_description = event.get_event_description()
+        except Exception as e:
+            logger.warning(f"[MC: {server_from}] 获取消息发送者信息失败: {e} 跳过处理...")
+            return
+
+        # 判断消息来源
+        if isinstance(event, SpigotEvent):
+            chat_key = 'MC_Server_' + server_from
+            chat_type = 'server'
+        else:
+            if config.DEBUG_LEVEL > 0: logger.info("未知消息来源: " + event.get_session_id())
+            return
+        
+        # 使用正则从消息："Notice {event_name} from {user_name}@[Server:{self.server_name}]: {event_name}" 中提取出玩家名和事件名(Join/Leave)
+        try:
+            event_name = event_description.split(']:')[1].strip()
+            user_name = re.search(r'from (.+?)@', event_description).group(1)
+        except Exception as e:
+            logger.warning(f"[MC: {server_from}] 正则提取消息内容失败: {e} 跳过处理...")
+            return
+        
+        wake_up = False
+
+        if event_name == 'Join':
+            notice_text = f'{user_name} 加入了服务器!'
+            wake_up = True
+        elif event_name == 'Quit':
+            notice_text = f'{user_name} 离开了服务器!'
+        elif event_name == 'Death':
+            notice_text = f'{user_name} 死于意外!'
+            wake_up = True
+
+        # 进行消息响应
+        await do_msg_response(
+            user_name,
+            notice_text,
+            False,
+            mc_notice_matcher,
+            chat_type,
+            chat_key,
+            '[Minecraft Server]',
+            wake_up
+        )
+
 
 """ ======== 注册指令响应器 ======== """
-# 人格设定指令 用于设定人格的相关参数
+# QQ:人格设定指令 用于设定人格的相关参数
 identity:Matcher = on_command("identity", aliases={"人格设定", "人格", "rg"}, rule=to_me(), priority=config.NG_MSG_PRIORITY - 1, block=True)
 @identity.handle()
 async def _(matcher_:Matcher, event: MessageEvent, bot:Bot, arg: Message = CommandArg()):
     global is_progress  # 是否产生编辑进度
     is_progress = False
     # 判断是否是禁止使用的用户
     if event.get_user_id() in config.FORBIDDEN_USERS:
@@ -248,15 +414,16 @@
 
     # 其它人格唤醒判断
     if chat.get_chat_preset_key().lower() not in trigger_text.lower() and chat.enable_auto_switch_identity:
         for preset_key in chat.preset_keys:
             if preset_key.lower() in trigger_text.lower():
                 chat.change_presettings(preset_key)
                 logger.info(f"检测到 {preset_key} 的唤醒词，切换到 {preset_key} 的人格")
-                await matcher.send(f'[NG] 已切换到 {preset_key} (￣▽￣)-ok !')
+                if chat_type != 'server':
+                    await matcher.send(f'[NG] 已切换到 {preset_key} (￣▽￣)-ok !')
                 wake_up = True
                 break
 
     current_preset_key = chat.get_chat_preset_key()
 
     # 判断是否需要回复
     if (    # 如果不是 bot 相关的信息，则直接返回
@@ -296,15 +463,15 @@
     # 沉默期中降低响应"提及"的概率，沉默期中被直接at，则恢复一定兴趣值提升兴趣值并取消沉默期
     # 兴趣值会影响回复的速度，兴趣值越高，回复速度越快
     # 发言概率贡献比例 = (随机值: 10% + 话题参与度: 50% + 兴趣值: 40%) * 发言几率基数(0.01~1.0)
 
     sta_time:float = time.time()
 
     # 生成对话 prompt 模板
-    prompt_template = chat.get_chat_prompt_template(userid=trigger_userid)
+    prompt_template = chat.get_chat_prompt_template(userid=trigger_userid, chat_type=chat_type)
     # 生成 log 输出用的 prompt 模板
     log_prompt_template = '\n'.join([f"[{m['role']}]\n{m['content']}\n" for m in prompt_template]) if isinstance(prompt_template, list) else prompt_template
     if config.DEBUG_LEVEL > 0:
         # logger.info("对话 prompt 模板: \n" + str(log_prompt_template))
         # 保存 prompt 模板到日志文件
         with open(os.path.join(config.NG_LOG_PATH, f"{chat_key}.{time.strftime('%Y-%m-%d %H-%M-%S')}.prompt.log"), 'a', encoding='utf-8') as f:
             f.write(f"prompt 模板: \n{log_prompt_template}\n")
@@ -407,69 +574,88 @@
 
     # # 代码块插入到回复列表的最后
     # for code_block in code_blocks:
     #     reply_list.append({'code_block': code_block})
 
     if config.DEBUG_LEVEL > 0: logger.info(f"回复序列内容: {reply_list}")
 
+    # 回复前缀
+    reply_prefix = f'<{chat.get_chat_preset_key()}> ' if (chat_type == 'server') else ''
+
     res_times = config.NG_MAX_RESPONSE_PER_MSG  # 获取每条消息最大回复次数
     # 根据回复内容列表逐条发送回复
     for idx, reply in enumerate(reply_list):
         # 判断回复内容是否为str
         if isinstance(reply, str) and reply.strip():
             # 判断文本内容是否为纯符号(包括空格，换行、英文标点、中文标点)并且长度小于3
             if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply.strip()):
                 if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号文本: {reply.strip()}，跳过发送...")
                 continue
             if config.ENABLE_MSG_TO_IMG:
                 img = await text_to_img(reply.strip())
                 await matcher.send(MessageSegment.image(img))
             else:
-                await matcher.send(reply.strip())
+                await matcher.send(f"{reply_prefix}{reply.strip()}")
         else:
             for key in reply:   # 遍历回复内容类型字典
-                if key == 'text' and reply.get(key) and reply.get(key).strip(): # 发送文本
+                if key == 'text' and reply.get(key) and reply.get(key).strip(): # 发送普通文本
                     # 判断文本内容是否为纯符号(包括空格，换行、英文标点、中文标点)并且长度为1
                     if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply.get(key).strip()):
                         if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号文本: {reply.get(key).strip()}，跳过发送...")
                         continue
-                    await matcher.send(reply.get(key).strip())
+                    await matcher.send(f"{reply_prefix}{reply.get(key).strip()}")
+
                 elif key == 'image' and reply.get(key): # 发送图片
                     await matcher.send(MessageSegment.image(file=reply.get(key, '')))
                     logger.info(f"回复图片消息: {reply.get(key)}")
+
                 elif key == 'voice' and reply.get(key): # 发送语音
                     logger.info(f"回复语音消息: {reply.get(key)}")
                     await matcher.send(Message(MessageSegment.record(file=reply.get(key), cache=0)))
+
                 elif key == 'code_block' and reply.get(key):  # 发送代码块
                     await matcher.send(Message(reply.get(key).strip()))
+
                 elif key == 'memory' and reply.get(key):  # 记忆存储
                     logger.info(f"存储记忆: {reply.get(key)}")
                     chat.set_memory(reply.get(key).get('key'), reply.get(key).get('value'))
                     if config.DEBUG_LEVEL > 0:
                         if reply.get(key).get('key') and reply.get(key).get('value'):
                             await matcher.send(f"[debug]: 记住了 {reply.get(key).get('key')} = {reply.get(key).get('value')}")
                         elif reply.get(key).get('key') and reply.get(key).get('value') is None:
                             await matcher.send(f"[debug]: 忘记了 {reply.get(key).get('key')}")
+
                 elif key == 'notify' and reply.get(key):  # 通知消息
                     if 'sender' in reply.get(key) and 'msg' in reply.get(key):
                         loop_data['notify'] = reply.get(key)
                     else:
                         logger.warning(f"通知消息格式错误: {reply.get(key)}")
+
                 elif key == 'wake_up' and reply.get(key):  # 重新调用对话
                     logger.info(f"重新调用对话: {reply.get(key)}")
                     wake_up = reply.get(key)
+
                 elif key == 'timer' and reply.get(key):  # 定时器
                     logger.info(f"设置定时器: {reply.get(key)}")
                     loop_data['timer'] = reply.get(key)
+
                 elif key == 'preset' and reply.get(key):  # 更新对话预设
                     if chat.update_preset(preset_key=chat.preset_key, bot_self_introl=reply.get(key))[0]:
                         logger.info(f"更新对话预设: {reply.get(key)} 成功")
                     else:
                         logger.warning(f"更新对话预设: {reply.get(key)} 失败")
 
+                elif key == 'rcon' and reply.get(key):  # RCON指令
+                    try:
+                        with MCRcon(config.MC_RCON_HOST, config.MC_RCON_PASSWORD, int(config.MC_RCON_PORT), timeout=10) as mcr:
+                            resp = mcr.command(reply.get(key))
+                            logger.info(f"发送MC-RCON指令: {reply.get(key)} | 响应: {resp}")
+                    except:
+                        logger.warning(f"发送MC-RCON指令: {reply.get(key)} 失败")
+
                 res_times -= 1
                 if res_times < 1:  # 如果回复次数超过限制，则跳出循环
                     break
         await asyncio.sleep(1.5)  # 每条回复之间间隔1.5秒
 
     cost_token = tg.cal_token_count(str(prompt_template) + raw_res)  # 计算对话结果的 token 数量
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/openai_func.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/openai_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         logger.error("请求 OpenAi 发生错误，请检查 Api Key 是否正确或者查看控制台相关日志")
         return res, False
 
     # 对话文本生成
     def get_chat_response(self, key:str, prompt, custom:dict = {}):
         openai.api_key = key
         try:
-            if self.config['model'].startswith('gpt-3.5-turbo'):
+            if self.config['model'].startswith('gpt-3.5-turbo') or self.config['model'].startswith('gpt-4'):
                 response = openai.ChatCompletion.create(
                     model=self.config['model'],
                     messages=prompt if isinstance(prompt, list) else [  # 如果是列表则直接使用，否则按照以下格式转换
                         {'role': 'system', 'content': f"You must strictly follow the user's instructions to give {custom.get('bot_name', 'bot')}'s response."},
                         {'role': 'user', 'content': prompt},
                     ],
                     temperature=self.config['temperature'],
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/persistent_data_manager.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/persistent_data_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/store.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/text_func.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/text_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/nonebot_plugin_naturel_gpt/utils.py` & `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/pyproject.toml` & `nonebot_plugin_naturel_gpt-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-naturel-gpt"
-version = "2.0.5"
+version = "2.1.0"
 description = "一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口"
 authors = ["KroMiose"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_naturel_gpt"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/README.md` & `nonebot_plugin_naturel_gpt-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     <a href="https://pypi.python.org/pypi/nonebot-plugin-naturel-gpt">
         <img src="https://img.shields.io/pypi/v/nonebot-plugin-naturel-gpt.svg" alt="pypi">
     </a>
     <img src="https://img.shields.io/badge/python-3.8+-6a9.svg" alt="python">
     <a href="https://jq.qq.com/?_wv=1027&k=71t9iCT7">
         <img src="https://img.shields.io/badge/加入交流群-636925153-c42.svg" alt="python">
     </a>
-    <h2>🎉 [2023/3/16] 项目重构 🎉</h2>
-    <p>项目重构整理基本完成，敬请期待重构后更多功能性更新<br/>
-    感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
+    <h2>🏠 [2023/4/14] v2.1 Minecraft服务器接入与游戏指令扩展支持 🗺️</h2>
+    <p>本次更新后支持将 bot 接入 MC 服务器，并且支持 bot 使用游戏内指令扩展</p>
+    <h2>🎉 [2023/3/16] v2.0 项目重构完成 🎉</h2>
+    <p>感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
     <h2>✏️ [2023/3/2] v1.4 更新: 支持ChatGPT模型 ✏️</h2>
     <p>本次更新后插件开始支持官方ChatGPT模型接口，token定价仅为GPT3的 1/10, 回复质量更高 响应速度更快</p>
     <h2>🧩 [2023/2/18] v1.3 更新: 自定义扩展支持 🧩</h2>
     <p>本次更新后插件开始支持自定义扩展，您可以直接通过自然语言直接调用多种扩展功能，包括 文本/图片/语音/邮件...</p>
     <p>提供了一些<a href="#%E5%AE%98%E6%96%B9%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8">样例扩展(点击前往)</a>，支持仅使用少量的代码就能实现各种自定义功能</p>
     <p>!  <strong><a href="#%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8"> 点击前往 -> 扩展列表 </a></strong> !</p>
 </div>
@@ -104,24 +105,29 @@
 | NG_DATA_PATH                  | str   | 数据文件目录                               | ./data/naturel_gpt/            | 保存实现数据持久化                                                                      |
 | NG_ENABLE_EXT                 | bool  | 是否启用聊天自定义扩展                     | True                           | 开启后 bot 可使用扩展功能，会额外消耗 token（取决于扩展描述，如未安装任何扩展务必关闭） |
 | NG_EXT_PATH                   | str   | 扩展脚本文件目录                           | ./data/naturel_gpt/extensions/ | 用于保存扩展脚本的路径                                                                  |
 | NG_EXT_LOAD_LIST              | str   | 加载扩展列表                               |                                | 只有在此列表中的扩展会被 bot 使用                                                       |
 | WORD_FOR_FORBIDDEN            | array | 自定义禁止触发词，以字符串列表方式填入     | []                             | 消息中含有列表中的词将呗拒绝唤醒 bot（优先级高于触发词）                                |
 | WORD_FOR_WAKE_UP              | array | 自定义触发词，以字符串列表方式填入         | []                             | 消息中含有列表中的词将唤醒 bot                                                          |
 | NG_MSG_PRIORITY               | int   | 消息响应优先级                             | 99                             | 大于 1，数值越大优先级越低                                                              |
-| NG_TO_ME                      | bool  | 响应命令是否需要@bot                        | False                          |                                                                                         |
+| NG_TO_ME                      | bool  | 响应命令是否需要@bot                       | False                          |                                                                                         |
 | ENABLE_COMMAND_TO_IMG         | bool  | 是否将 rg 相关指令通过图片输出             | False                          |                                                                                         |
 | ENABLE_MSG_TO_IMG             | bool  | 是否将机器人回复通过图片输出               | False                          |                                                                                         |
 | NG_BLOCK_OTHERS               | bool  | 是否拦截其它插件的响应                     | False                          | 开启后可能导致优先级低于本插件的其他插件不响应                                          |
 | NG_MAX_RESPONSE_PER_MSG       | int   | 每条消息最大回复次数                       | 5                              | 限制 bot 针对每条信息最大回复次数，避免封禁                                             |
 | NG_ENABLE_MSG_SPLIT           | bool  | 是否允许消息分割发送                       | True                           | 如果允许，bot 有可能会在一次回复中发送多条消息                                          |
 | NG_ENABLE_AWAKE_IDENTITIES    | bool  | 是否允许自动唤醒其它人格                   | True                           | 如果允许，bot 在检测到未启用人格呼叫时会自动唤醒并切换人格                              |
 | FORBIDDEN_USERS               | array | 黑名单用户 id，以字符串列表方式填入        | ['']                           | 黑名单中的用户消息不会被记录和响应设                                                    |
 | UNLOCK_CONTENT_LIMIT          | bool  | 是否解锁内容限制                           | False                          | 可能导致 OpenAi 账号风险，请自行承担后果                                                |
 | OPENAI_PROXY_SERVER           | str   | 请求 OpenAI 的代理服务器                   | ''                             | 填写示例 '127.0.0.1:1234' 或 'username:password@127.0.0.1:1234'                         |
+| ENABLE_MC_CONNECT             | bool  | 是否开启 MC 服务器连接                     | False                          | 开启后可连接到 Minecraft 服务器                                                         |
+| MC_COMMAND_PREFIX             | array | MC 服务器中人格编辑指令前缀                | ['!', '！']                    | MC 服务器中人格编辑指令前缀                                                             |
+| MC_RCON_HOST                  | str   | MC 服务器 RCON 地址                        | '127.0.0.1'                    | MC 服务器 RCON 地址                                                                     |
+| MC_RCON_PORT                  | int   | MC 服务器 RCON 端口                        | 25575                          | MC 服务器 RCON 端口                                                                     |
+| MC_RCON_PASSWORD              | str   | MC 服务器 RCON 密码                        | '123456'                       | MC 服务器 RCON 密码                                                                     |
 | DEBUG_LEVEL                   | int   | DEBUG 等级                                 | 0                              | 等级越高 debug 信息越详细                                                               |
 
 </code> </pre> </details>
 
 ## 🪄 指令说明
 
 ### 基本命令——"rg"(需要加上在 NoneBot 中设定的指令前缀)
@@ -467,25 +473,33 @@
 > bot 更新人格后会丢失原人格预设，如需保留请自行备份
 
 - 扩展文件: ext_evolution.py
 - 说明: 赋予 bot 自主发展人格的能力，允许 bot 自主设定更新人设
 - 配置项:
   - notify_type: 触发更新时通知类型 0: 无通知; 1: 仅触发提示; 2: 新预设完整通知 (默认: 1)
 
+#### > [Minecraft 服务器专用] 执行服务器命令模块
+
+- 扩展文件: ext_mc_command.py
+- 说明: 赋予 bot 执行 Minecraft 服务器命令的能力，鉴权基于字符串匹配，请谨慎使用过滤高危命令，黑白名单匹配的内容包括指令前缀 `/`
+- 配置项:
+  - match_white_list: 匹配指令内容白名单列表 (列表中至少一个字符串应被包含在命令中，为空则不限制)
+  - match_black_list: 匹配指令内容黑名单列表 (列表中所有字符串都不应被包含在命令中，为空则不限制，优先级高于白名单)
+
 #### > 主动记忆能力扩展模块 (因 bot 使用积极性不佳，暂移入备份，不推荐使用)
 
 - 扩展文件: ext_remember.py & ext_forget.py
 - 说明: 赋予 bot 主动管理记忆的能力，使用时请同时启用 记忆|遗忘 扩展
 
 ### 编写自定义扩展
 
 > 自行编写扩展需要具有一定的 Python 编程基础，如果您有相关能力可直接参考本仓库 `/extensions/` 目录下的扩展进行编写(非常简单！) 自行编写的扩展安装流程与上述相同
 > 注意：该功能尚处于早期阶段，扩展编写在未来版本有可能随时变化！
 
-✨ 如果您想分享您自行开发的扩展，可向本仓库提交 pr，将您的扩展命名为 `share_ext_xxx.py`('xxx'部分可自行命名，请勿与已存在的扩展名冲突) 并上传至本仓库的 `/share_exts/` 目录下，欢迎您成为本项目的贡献者！
+✨ 如果您想分享您自行开发的扩展，可向本仓库提交 pr，将您的扩展命名为 `ext_xxx.py`('xxx'部分可自行命名，请勿与已存在的扩展名冲突) 并上传至本仓库的 `/extensions/` 目录下，欢迎您成为本项目的贡献者！
 
 #### 基本的扩展模块模板
 
 <details> <summary>🔍点击查看扩展模块编写模板</summary> <pre><code>
 
 ```python
 from .Extension import Extension
@@ -507,14 +521,16 @@
     "author": "",
     # 版本
     "version": "0.0.1"
     # 扩展简介
     "intro": "简介信息（查看扩展详情显示）",
     # 调用时是否打断响应 启用后将会在调用后截断后续响应内容
     "interrupt": True,
+    # 可用会话类型 (server即MC服务器 | chat即QQ聊天)
+    "available": ['server'],
 }
 
 class CustomExtension(Extension):
     async def call(self, arg_dict: dict, ctx_data: dict) -> dict:
         """ 当扩展被调用时执行的函数 *由扩展自行实现*
 
         参数:
@@ -532,51 +548,82 @@
 
     def __init__(self, custom_config: dict):
         super().__init__(ext_config.copy(), custom_config)
 ```
 
 </code></pre> </details>
 
+## 🗺️ MC 服务器支持
+
+> 允许 bot 接入 Minecraft 服务器，并可在服务器中执行指令
+> 使用前需要编辑配置文件并开启 ENABLE_MC_CONNECT 项
+
+### 适配器安装
+
+> 插件使用 spigot 适配器接收服务器消息推送和文字发送
+
+使用 `nb adapter install nonebot-adapter-spigot` 指令安装适配器
+
+#### MC 服务器端支持安装
+
+参考 [MC_qq 安装文档](https://17theword.github.io/mc_qq/install/mcrcon_plugin.html#minecraft-server-%E7%AB%AF) 中的 `Minecraft Server 端` 步骤安装服务端插件
+
+注意事项 1：配置文件中 `websocket_url: "ws://127.0.0.1:8765"` 的值部分应改为 `ws://Nonebot服务器ip:Nonebot监听端口/spigot/ws`
+
+注意事项 2：如果你的 MC 服务端和 Nonebot 服务端不在同一台服务器上，需要在 `.env` 中将 NoneBot 的监听地址改为 `0.0.0.0` 并放行对应端口，否则将导致连接失败
+
+#### RCON 配置
+> RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
+
+1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
+2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
+
 ## 🎢 更新日志
 
-## [2023/4/6] v2.0.5
+## [2023/4/15] v2.1.0 Minecraft 服务器支持
+
+- 增加了 Minecraft 服务器接入支持
+- 增加了 Minecraft 服务器指令执行支持和相关扩展模块
+- 为绘图扩展增加了代理配置项支持 (感谢 @tonato-01 提供 pr)
+
+## [2023/4/6] v2.0.5 RENAME 指令 | json 导出支持
 
 - 解析消息中的@时保持与用户看到的一致 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 优化日志输出的 DEBUG_LEVEL 限制 (感谢 @Misaka-Mikoto-Tech 提供 pr)
-- 优化聊天消息prompt的换行生成逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
+- 优化聊天消息 prompt 的换行生成逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 增加 `rg rename` 改名指令，用于修改人格名 (感谢 @Misaka-Mikoto-Tech 提供 pr) (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 解析消息中的@时保持与用户看到的一致 (感谢 @Misaka-Mikoto-Tech 提供 pr)
-- patch logger使插件名称显示为中文 (感谢 @chenxuan353 提供 pr)
-- 添加记忆文件(原.pkl)使用JSON读取与保存功能 (与原pickle兼容) (感谢 @chenxuan353 提供 pr)
+- patch logger 使插件名称显示为中文 (感谢 @chenxuan353 提供 pr)
+- 添加记忆文件(原.pkl)使用 JSON 读取与保存功能 (与原 pickle 兼容) (感谢 @chenxuan353 提供 pr)
 - 优化部分代码类型注解 (感谢 @chenxuan353 提供 pr)
-- 搜索扩展(ext_search.py) 优化，禁止bot短时间内反复搜索和搜索重复内容
+- 搜索扩展(ext_search.py) 优化，禁止 bot 短时间内反复搜索和搜索重复内容
 
 ## [2023/3/26] v2.0.4
 
 - 修复 @全体成员 时解析报错问题
 - 增加扩展更新人格支持，同时增加了一个 evolution 扩展模块，允许 bot 自主更新人格
 - 响应规则中增加一条禁止复读规则
 
-## [2023/3/26] v2.0.3
+## [2023/3/26] v2.0.3 图片输出支持
 
 - 输出内容转图片: 使用 htmlrender 将 TA 的回复转换为图片，降低风控几率 (可选开关，感谢 @HMScygnet 提供 pr)
 - 等待 OpenAI 响应过程中切换人格预设或响应超时后停止处理消息 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 修正编辑和删除预设判断是否锁定以及是否是默认预设和正在使用的预设的逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 增加调用扩展时预检支持打断响应，优化搜索扩展执行效果，避免 bot 自行脑补搜索结果的情况
 - 修正一些指令帮助信息的内容错误
 - 修正通过指令安装扩展时的编码问题
 - 修正纯符号过滤判断逻辑
 
-## [2023/3/21] v2.0.2
+## [2023/3/21] v2.0.2 扩展下载指令支持
 
 - 切换人格时的聊天输出改为非 DEBUG 模式下也会发送
 - 增加了扩展 安装/删除 指令，可直接从 GitHub 上获取到最新扩展
 - 精简了非 DEBUG 模式下的控制台输出
 
-## [2023/3/20] v2.0.1
+## [2023/3/20] v2.0.1 VIOCEVOX 语音扩展
 
 - 修正 `-global` 的控制权限和逻辑 (感谢 [@Misaka-Mikoto-Tech](https://github.com/) 提供 pr)
 - 增加了一个新的语音扩展 `ext_VOICEVOX` 能够更便捷地实现本地部署 (感谢 @恋如雨止 提供技术支持)
 - 修正回复内容首尾的空行问题；修正短纯符号回复内容未正常过滤的问题
 - 修正私聊会话权限设定
 
 ## [2023/3/18] v2.0.0 项目重构 🎉
```

#### html2text {}

```diff
@@ -3,16 +3,19 @@
                â¨ æ´äººæ§å(æäºº)çGPTèå¤©Aiæä»¶! â¨
  ð§¬ æ¯æå¤ä¸ªäººæ ¼èªå®ä¹ / åæ¢ | å°½æåæ¥ä½ çæ³è±¡åå§ï¼
                                     âï¸
       ð§¬ é¢è®¾æ¶éå±äº«è¡¨(æ¬¢è¿åäº«åç§èªå®ä¹äººè®¾) ð§¬
  ð å¦æåæ¬¢è¯·ç¹ä¸ªâ­å§ï¼æ¨çæ¯æå°±æ¯ææç»­æ´æ°çå¨å
                                      ð
                       [license] [pypi] [python] [python]
-                ***** ð [2023/3/16] é¡¹ç®éæ ð *****
-  é¡¹ç®éææ´çåºæ¬å®æï¼æ¬è¯·æå¾éæåæ´å¤åè½æ§æ´æ°
+***** ð  [2023/4/14] v2.1 Minecraftæå¡å¨æ¥å¥ä¸æ¸¸ææä»¤æ©å±æ¯æ
+                                 ðºï¸ *****
+      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥ MC æå¡å¨ï¼å¹¶ä¸æ¯æ bot
+                          ä½¿ç¨æ¸¸æåæä»¤æ©å±
+           ***** ð [2023/3/16] v2.0 é¡¹ç®éæå®æ ð *****
       æè°¢@Misaka-Mikoto-Techå¤§ä½¬å¯¹é¡¹ç®éææä¾çå¤§åæ¯æ
      ***** âï¸ [2023/3/2] v1.4 æ´æ°: æ¯æChatGPTæ¨¡å âï¸ *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æå®æ¹ChatGPTæ¨¡åæ¥å£ï¼tokenå®ä»·ä»ä¸ºGPT3ç
                   1/10, åå¤è´¨éæ´é« ååºéåº¦æ´å¿«
      ***** ð§© [2023/2/18] v1.3 æ´æ°: èªå®ä¹æ©å±æ¯æ ð§© *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æèªå®ä¹æ©å±ï¼æ¨å¯ä»¥ç´æ¥éè¿èªç¶è¯­è¨ç´æ¥è°ç¨å¤ç§æ©å±åè½ï¼åæ¬
                         ææ¬/å¾ç/è¯­é³/é®ä»¶...
@@ -225,14 +228,30 @@
 | UNLOCK_CONTENT_LIMIT          | bool  | æ¯å¦è§£éåå®¹éå¶
 | False                          | å¯è½å¯¼è´ OpenAi
 è´¦å·é£é©ï¼è¯·èªè¡æ¿æåæ
 |
 | OPENAI_PROXY_SERVER           | str   | è¯·æ± OpenAI çä»£çæå¡å¨
 | ''                             | å¡«åç¤ºä¾ '127.0.0.1:1234' æ 'username:
 password@127.0.0.1:1234'                         |
+| ENABLE_MC_CONNECT             | bool  | æ¯å¦å¼å¯ MC æå¡å¨è¿æ¥
+| False                          | å¼å¯åå¯è¿æ¥å° Minecraft æå¡å¨
+|
+| MC_COMMAND_PREFIX             | array | MC
+æå¡å¨ä¸­äººæ ¼ç¼è¾æä»¤åç¼                | ['!', 'ï¼']
+| MC æå¡å¨ä¸­äººæ ¼ç¼è¾æä»¤åç¼
+|
+| MC_RCON_HOST                  | str   | MC æå¡å¨ RCON å°å
+| '127.0.0.1'                    | MC æå¡å¨ RCON å°å
+|
+| MC_RCON_PORT                  | int   | MC æå¡å¨ RCON ç«¯å£
+| 25575                          | MC æå¡å¨ RCON ç«¯å£
+|
+| MC_RCON_PASSWORD              | str   | MC æå¡å¨ RCON å¯ç 
+| '123456'                       | MC æå¡å¨ RCON å¯ç 
+|
 | DEBUG_LEVEL                   | int   | DEBUG ç­çº§
 | 0                              | ç­çº§è¶é« debug ä¿¡æ¯è¶è¯¦ç»
 |
 
 
  ## ðª æä»¤è¯´æ ### åºæ¬å½ä»¤ââ"rg"(éè¦å ä¸å¨ NoneBot
 ä¸­è®¾å®çæä»¤åç¼) - å«ç§°: "äººæ ¼"ã"äººæ ¼è®¾å®"ã"identity" -
@@ -552,27 +571,35 @@
 OREOREO) - æ©å±æä»¶: ext_paint.py - è¯´æ: è°ç¨ openai
 ç»å¾æ¥å£ï¼å®ç°èªç¶è¯­è¨è°ç¨ç»ç»ï¼æ¥å£å±ç¨æ¬æä»¶ç Api
 Key #### > è¿åæ¨¡å > bot
 æ´æ°äººæ ¼åä¼ä¸¢å¤±åäººæ ¼é¢è®¾ï¼å¦éä¿çè¯·èªè¡å¤ä»½ -
 æ©å±æä»¶: ext_evolution.py - è¯´æ: èµäº bot
 èªä¸»åå±äººæ ¼çè½åï¼åè®¸ bot èªä¸»è®¾å®æ´æ°äººè®¾ - éç½®é¡¹:
 - notify_type: è§¦åæ´æ°æ¶éç¥ç±»å 0: æ éç¥; 1: ä»è§¦åæç¤º; 2:
-æ°é¢è®¾å®æ´éç¥ (é»è®¤: 1) #### > ä¸»å¨è®°å¿è½åæ©å±æ¨¡å (å 
-bot ä½¿ç¨ç§¯ææ§ä¸ä½³ï¼æç§»å¥å¤ä»½ï¼ä¸æ¨èä½¿ç¨) - æ©å±æä»¶:
+æ°é¢è®¾å®æ´éç¥ (é»è®¤: 1) #### > [Minecraft æå¡å¨ä¸ç¨]
+æ§è¡æå¡å¨å½ä»¤æ¨¡å - æ©å±æä»¶: ext_mc_command.py - è¯´æ: èµäº
+bot æ§è¡ Minecraft
+æå¡å¨å½ä»¤çè½åï¼é´æåºäºå­ç¬¦ä¸²å¹éï¼è¯·è°¨æä½¿ç¨è¿æ»¤é«å±å½ä»¤ï¼é»ç½ååå¹éçåå®¹åæ¬æä»¤åç¼
+`/` - éç½®é¡¹: - match_white_list: å¹éæä»¤åå®¹ç½åååè¡¨
+(åè¡¨ä¸­è³å°ä¸ä¸ªå­ç¬¦ä¸²åºè¢«åå«å¨å½ä»¤ä¸­ï¼ä¸ºç©ºåä¸éå¶) -
+match_black_list: å¹éæä»¤åå®¹é»åååè¡¨
+(åè¡¨ä¸­ææå­ç¬¦ä¸²é½ä¸åºè¢«åå«å¨å½ä»¤ä¸­ï¼ä¸ºç©ºåä¸éå¶ï¼ä¼åçº§é«äºç½åå)
+#### > ä¸»å¨è®°å¿è½åæ©å±æ¨¡å (å  bot
+ä½¿ç¨ç§¯ææ§ä¸ä½³ï¼æç§»å¥å¤ä»½ï¼ä¸æ¨èä½¿ç¨) - æ©å±æä»¶:
 ext_remember.py & ext_forget.py - è¯´æ: èµäº bot
 ä¸»å¨ç®¡çè®°å¿çè½åï¼ä½¿ç¨æ¶è¯·åæ¶å¯ç¨ è®°å¿|éå¿ æ©å± ###
 ç¼åèªå®ä¹æ©å± > èªè¡ç¼åæ©å±éè¦å·æä¸å®ç Python
 ç¼ç¨åºç¡ï¼å¦ææ¨æç¸å³è½åå¯ç´æ¥åèæ¬ä»åº `/extensions/
 ` ç®å½ä¸çæ©å±è¿è¡ç¼å(éå¸¸ç®åï¼)
 èªè¡ç¼åçæ©å±å®è£æµç¨ä¸ä¸è¿°ç¸å >
 æ³¨æï¼è¯¥åè½å°å¤äºæ©æé¶æ®µï¼æ©å±ç¼åå¨æªæ¥çæ¬æå¯è½éæ¶ååï¼
 â¨ å¦ææ¨æ³åäº«æ¨èªè¡å¼åçæ©å±ï¼å¯åæ¬ä»åºæäº¤
-prï¼å°æ¨çæ©å±å½åä¸º `share_ext_xxx.py`
+prï¼å°æ¨çæ©å±å½åä¸º `ext_xxx.py`
 ('xxx'é¨åå¯èªè¡å½åï¼è¯·å¿ä¸å·²å­å¨çæ©å±åå²çª)
-å¹¶ä¸ä¼ è³æ¬ä»åºç `/share_exts/
+å¹¶ä¸ä¼ è³æ¬ä»åºç `/extensions/
 ` ç®å½ä¸ï¼æ¬¢è¿æ¨æä¸ºæ¬é¡¹ç®çè´¡ç®èï¼ ####
 åºæ¬çæ©å±æ¨¡åæ¨¡æ¿  ðç¹å»æ¥çæ©å±æ¨¡åç¼åæ¨¡æ¿
 
 
 ```python
 from .Extension import Extension
 
@@ -600,14 +627,16 @@
     # çæ¬
     "version": "0.0.1"
     # æ©å±ç®ä»
     "intro": "ç®ä»ä¿¡æ¯ï¼æ¥çæ©å±è¯¦ææ¾ç¤ºï¼",
     # è°ç¨æ¶æ¯å¦ææ­ååº
 å¯ç¨åå°ä¼å¨è°ç¨åæªæ­åç»­ååºåå®¹
     "interrupt": True,
+    # å¯ç¨ä¼è¯ç±»å (serverå³MCæå¡å¨ | chatå³QQèå¤©)
+    "available": ['server'],
 }
 
 class CustomExtension(Extension):
     async def call(self, arg_dict: dict, ctx_data: dict) -> dict:
         """ å½æ©å±è¢«è°ç¨æ¶æ§è¡çå½æ° *ç±æ©å±èªè¡å®ç°*
 
         åæ°:
@@ -624,50 +653,73 @@
             'voice': f"http://...",  # è¯­é³url
         }
 
     def __init__(self, custom_config: dict):
         super().__init__(ext_config.copy(), custom_config)
 ```
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/6] v2.0.5 -
+ ## ðºï¸ MC æå¡å¨æ¯æ > åè®¸ bot æ¥å¥ Minecraft
+æå¡å¨ï¼å¹¶å¯å¨æå¡å¨ä¸­æ§è¡æä»¤ >
+ä½¿ç¨åéè¦ç¼è¾éç½®æä»¶å¹¶å¼å¯ ENABLE_MC_CONNECT é¡¹ ###
+ééå¨å®è£ > æä»¶ä½¿ç¨ spigot
+ééå¨æ¥æ¶æå¡å¨æ¶æ¯æ¨éåæå­åé ä½¿ç¨ `nb adapter install
+nonebot-adapter-spigot` æä»¤å®è£ééå¨ #### MC æå¡å¨ç«¯æ¯æå®è£
+åè [MC_qq å®è£ææ¡£](https://17theword.github.io/mc_qq/install/
+mcrcon_plugin.html#minecraft-server-%E7%AB%AF) ä¸­ç `Minecraft Server ç«¯`
+æ­¥éª¤å®è£æå¡ç«¯æä»¶ æ³¨æäºé¡¹ 1ï¼éç½®æä»¶ä¸­ `websocket_url:
+"ws://127.0.0.1:8765"` çå¼é¨ååºæ¹ä¸º `ws://Nonebotæå¡å¨ip:
+Nonebotçå¬ç«¯å£/spigot/ws` æ³¨æäºé¡¹ 2ï¼å¦æä½ ç MC æå¡ç«¯å
+Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
+ççå¬å°åæ¹ä¸º `0.0.0.0`
+å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
+Minecraft
+æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
+RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
+`enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ## ð¢ æ´æ°æ¥å¿
+## [2023/4/15] v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft
+æå¡å¨æ¥å¥æ¯æ - å¢å äº Minecraft
+æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
+ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
+[2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
-Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯promptçæ¢è¡çæé»è¾ (æè°¢
-@Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
+Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
+(æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
 æ¹åæä»¤ï¼ç¨äºä¿®æ¹äººæ ¼å (æè°¢ @Misaka-Mikoto-Tech æä¾ pr)
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
-Tech æä¾ pr) - patch loggerä½¿æä»¶åç§°æ¾ç¤ºä¸ºä¸­æ (æè°¢
-@chenxuan353 æä¾ pr) - æ·»å è®°å¿æä»¶
-(å.pkl)ä½¿ç¨JSONè¯»åä¸ä¿å­åè½ (ä¸åpickleå¼å®¹) (æè°¢
-@chenxuan353 æä¾ pr) - ä¼åé¨åä»£ç ç±»åæ³¨è§£ (æè°¢ @chenxuan353
-æä¾ pr) - æç´¢æ©å±(ext_search.py)
-ä¼åï¼ç¦æ­¢botç­æ¶é´ååå¤æç´¢åæç´¢éå¤åå®¹ ## [2023/3/26]
-v2.0.4 - ä¿®å¤ @å¨ä½æå æ¶è§£ææ¥éé®é¢ -
+Tech æä¾ pr) - patch logger ä½¿æä»¶åç§°æ¾ç¤ºä¸ºä¸­æ (æè°¢
+@chenxuan353 æä¾ pr) - æ·»å è®°å¿æä»¶(å.pkl)ä½¿ç¨ JSON
+è¯»åä¸ä¿å­åè½ (ä¸å pickle å¼å®¹) (æè°¢ @chenxuan353 æä¾ pr) -
+ä¼åé¨åä»£ç ç±»åæ³¨è§£ (æè°¢ @chenxuan353 æä¾ pr) - æç´¢æ©å±
+(ext_search.py) ä¼åï¼ç¦æ­¢ bot
+ç­æ¶é´ååå¤æç´¢åæç´¢éå¤åå®¹ ## [2023/3/26] v2.0.4 - ä¿®å¤
+@å¨ä½æå æ¶è§£ææ¥éé®é¢ -
 å¢å æ©å±æ´æ°äººæ ¼æ¯æï¼åæ¶å¢å äºä¸ä¸ª evolution
 æ©å±æ¨¡åï¼åè®¸ bot èªä¸»æ´æ°äººæ ¼ -
-ååºè§åä¸­å¢å ä¸æ¡ç¦æ­¢å¤è¯»è§å ## [2023/3/26] v2.0.3 -
-è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
+ååºè§åä¸­å¢å ä¸æ¡ç¦æ­¢å¤è¯»è§å ## [2023/3/26] v2.0.3
+å¾çè¾åºæ¯æ - è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
 çåå¤è½¬æ¢ä¸ºå¾çï¼éä½é£æ§å ç (å¯éå¼å³ï¼æè°¢ @HMScygnet
 æä¾ pr) - ç­å¾ OpenAI
 ååºè¿ç¨ä¸­åæ¢äººæ ¼é¢è®¾æååºè¶æ¶ååæ­¢å¤çæ¶æ¯ (æè°¢
 @Misaka-Mikoto-Tech æä¾ pr) -
 ä¿®æ­£ç¼è¾åå é¤é¢è®¾å¤æ­æ¯å¦éå®ä»¥åæ¯å¦æ¯é»è®¤é¢è®¾åæ­£å¨ä½¿ç¨çé¢è®¾çé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) -
 å¢å è°ç¨æ©å±æ¶é¢æ£æ¯æææ­ååºï¼ä¼åæç´¢æ©å±æ§è¡ææï¼é¿å
 bot èªè¡èè¡¥æç´¢ç»æçæåµ -
 ä¿®æ­£ä¸äºæä»¤å¸®å©ä¿¡æ¯çåå®¹éè¯¯ -
 ä¿®æ­£éè¿æä»¤å®è£æ©å±æ¶çç¼ç é®é¢ -
-ä¿®æ­£çº¯ç¬¦å·è¿æ»¤å¤æ­é»è¾ ## [2023/3/21] v2.0.2 -
-åæ¢äººæ ¼æ¶çèå¤©è¾åºæ¹ä¸ºé DEBUG æ¨¡å¼ä¸ä¹ä¼åé -
-å¢å äºæ©å± å®è£/å é¤ æä»¤ï¼å¯ç´æ¥ä» GitHub
-ä¸è·åå°ææ°æ©å± - ç²¾ç®äºé DEBUG æ¨¡å¼ä¸çæ§å¶å°è¾åº ##
-[2023/3/20] v2.0.1 - ä¿®æ­£ `-global` çæ§å¶æéåé»è¾ (æè°¢
-[@Misaka-Mikoto-Tech](https://github.com/) æä¾ pr) -
-å¢å äºä¸ä¸ªæ°çè¯­é³æ©å± `ext_VOICEVOX`
+ä¿®æ­£çº¯ç¬¦å·è¿æ»¤å¤æ­é»è¾ ## [2023/3/21] v2.0.2
+æ©å±ä¸è½½æä»¤æ¯æ - åæ¢äººæ ¼æ¶çèå¤©è¾åºæ¹ä¸ºé DEBUG
+æ¨¡å¼ä¸ä¹ä¼åé - å¢å äºæ©å± å®è£/å é¤ æä»¤ï¼å¯ç´æ¥ä»
+GitHub ä¸è·åå°ææ°æ©å± - ç²¾ç®äºé DEBUG
+æ¨¡å¼ä¸çæ§å¶å°è¾åº ## [2023/3/20] v2.0.1 VIOCEVOX è¯­é³æ©å± -
+ä¿®æ­£ `-global` çæ§å¶æéåé»è¾ (æè°¢ [@Misaka-Mikoto-Tech](https:/
+/github.com/) æä¾ pr) - å¢å äºä¸ä¸ªæ°çè¯­é³æ©å± `ext_VOICEVOX`
 è½å¤æ´ä¾¿æ·å°å®ç°æ¬å°é¨ç½² (æè°¢ @æå¦é¨æ­¢ æä¾ææ¯æ¯æ)
 -
 ä¿®æ­£åå¤åå®¹é¦å°¾çç©ºè¡é®é¢ï¼ä¿®æ­£ç­çº¯ç¬¦å·åå¤åå®¹æªæ­£å¸¸è¿æ»¤çé®é¢
 - ä¿®æ­£ç§èä¼è¯æéè®¾å® ## [2023/3/18] v2.0.0 é¡¹ç®éæ ð >
 âââ æ³¨æï¼æ¬æ¬¡æ´æ°éè¦å é¤å bot è®°å¿æä»¶éæ°çæ
 (å³./data/naturel_gpt
 æä»¶å¤¹)ï¼å¦åå¯è½äº§çæ æ³é¢è®¡çéè¯¯ï¼åæ¶å»ºè®®å°éç½®æä»¶ä¸å¹¶å é¤éæ°çæï¼æ­¤æä½ä¼**ä¸¢å¤±**ææç¼è¾è¿çäººæ ¼é¢è®¾ï¼å¦æä½ éè¦å¨æ´æ°åç»§ç»­ä½¿ç¨ï¼è¯·ä½¿ç¨
```

### Comparing `nonebot_plugin_naturel_gpt-2.0.5/PKG-INFO` & `nonebot_plugin_naturel_gpt-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-naturel-gpt
-Version: 2.0.5
+Version: 2.1.0
 Summary: 一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口
 License: Apache-2.0
 Author: KroMiose
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -36,17 +36,18 @@
     <a href="https://pypi.python.org/pypi/nonebot-plugin-naturel-gpt">
         <img src="https://img.shields.io/pypi/v/nonebot-plugin-naturel-gpt.svg" alt="pypi">
     </a>
     <img src="https://img.shields.io/badge/python-3.8+-6a9.svg" alt="python">
     <a href="https://jq.qq.com/?_wv=1027&k=71t9iCT7">
         <img src="https://img.shields.io/badge/加入交流群-636925153-c42.svg" alt="python">
     </a>
-    <h2>🎉 [2023/3/16] 项目重构 🎉</h2>
-    <p>项目重构整理基本完成，敬请期待重构后更多功能性更新<br/>
-    感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
+    <h2>🏠 [2023/4/14] v2.1 Minecraft服务器接入与游戏指令扩展支持 🗺️</h2>
+    <p>本次更新后支持将 bot 接入 MC 服务器，并且支持 bot 使用游戏内指令扩展</p>
+    <h2>🎉 [2023/3/16] v2.0 项目重构完成 🎉</h2>
+    <p>感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
     <h2>✏️ [2023/3/2] v1.4 更新: 支持ChatGPT模型 ✏️</h2>
     <p>本次更新后插件开始支持官方ChatGPT模型接口，token定价仅为GPT3的 1/10, 回复质量更高 响应速度更快</p>
     <h2>🧩 [2023/2/18] v1.3 更新: 自定义扩展支持 🧩</h2>
     <p>本次更新后插件开始支持自定义扩展，您可以直接通过自然语言直接调用多种扩展功能，包括 文本/图片/语音/邮件...</p>
     <p>提供了一些<a href="#%E5%AE%98%E6%96%B9%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8">样例扩展(点击前往)</a>，支持仅使用少量的代码就能实现各种自定义功能</p>
     <p>!  <strong><a href="#%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8"> 点击前往 -> 扩展列表 </a></strong> !</p>
 </div>
@@ -125,24 +126,29 @@
 | NG_DATA_PATH                  | str   | 数据文件目录                               | ./data/naturel_gpt/            | 保存实现数据持久化                                                                      |
 | NG_ENABLE_EXT                 | bool  | 是否启用聊天自定义扩展                     | True                           | 开启后 bot 可使用扩展功能，会额外消耗 token（取决于扩展描述，如未安装任何扩展务必关闭） |
 | NG_EXT_PATH                   | str   | 扩展脚本文件目录                           | ./data/naturel_gpt/extensions/ | 用于保存扩展脚本的路径                                                                  |
 | NG_EXT_LOAD_LIST              | str   | 加载扩展列表                               |                                | 只有在此列表中的扩展会被 bot 使用                                                       |
 | WORD_FOR_FORBIDDEN            | array | 自定义禁止触发词，以字符串列表方式填入     | []                             | 消息中含有列表中的词将呗拒绝唤醒 bot（优先级高于触发词）                                |
 | WORD_FOR_WAKE_UP              | array | 自定义触发词，以字符串列表方式填入         | []                             | 消息中含有列表中的词将唤醒 bot                                                          |
 | NG_MSG_PRIORITY               | int   | 消息响应优先级                             | 99                             | 大于 1，数值越大优先级越低                                                              |
-| NG_TO_ME                      | bool  | 响应命令是否需要@bot                        | False                          |                                                                                         |
+| NG_TO_ME                      | bool  | 响应命令是否需要@bot                       | False                          |                                                                                         |
 | ENABLE_COMMAND_TO_IMG         | bool  | 是否将 rg 相关指令通过图片输出             | False                          |                                                                                         |
 | ENABLE_MSG_TO_IMG             | bool  | 是否将机器人回复通过图片输出               | False                          |                                                                                         |
 | NG_BLOCK_OTHERS               | bool  | 是否拦截其它插件的响应                     | False                          | 开启后可能导致优先级低于本插件的其他插件不响应                                          |
 | NG_MAX_RESPONSE_PER_MSG       | int   | 每条消息最大回复次数                       | 5                              | 限制 bot 针对每条信息最大回复次数，避免封禁                                             |
 | NG_ENABLE_MSG_SPLIT           | bool  | 是否允许消息分割发送                       | True                           | 如果允许，bot 有可能会在一次回复中发送多条消息                                          |
 | NG_ENABLE_AWAKE_IDENTITIES    | bool  | 是否允许自动唤醒其它人格                   | True                           | 如果允许，bot 在检测到未启用人格呼叫时会自动唤醒并切换人格                              |
 | FORBIDDEN_USERS               | array | 黑名单用户 id，以字符串列表方式填入        | ['']                           | 黑名单中的用户消息不会被记录和响应设                                                    |
 | UNLOCK_CONTENT_LIMIT          | bool  | 是否解锁内容限制                           | False                          | 可能导致 OpenAi 账号风险，请自行承担后果                                                |
 | OPENAI_PROXY_SERVER           | str   | 请求 OpenAI 的代理服务器                   | ''                             | 填写示例 '127.0.0.1:1234' 或 'username:password@127.0.0.1:1234'                         |
+| ENABLE_MC_CONNECT             | bool  | 是否开启 MC 服务器连接                     | False                          | 开启后可连接到 Minecraft 服务器                                                         |
+| MC_COMMAND_PREFIX             | array | MC 服务器中人格编辑指令前缀                | ['!', '！']                    | MC 服务器中人格编辑指令前缀                                                             |
+| MC_RCON_HOST                  | str   | MC 服务器 RCON 地址                        | '127.0.0.1'                    | MC 服务器 RCON 地址                                                                     |
+| MC_RCON_PORT                  | int   | MC 服务器 RCON 端口                        | 25575                          | MC 服务器 RCON 端口                                                                     |
+| MC_RCON_PASSWORD              | str   | MC 服务器 RCON 密码                        | '123456'                       | MC 服务器 RCON 密码                                                                     |
 | DEBUG_LEVEL                   | int   | DEBUG 等级                                 | 0                              | 等级越高 debug 信息越详细                                                               |
 
 </code> </pre> </details>
 
 ## 🪄 指令说明
 
 ### 基本命令——"rg"(需要加上在 NoneBot 中设定的指令前缀)
@@ -488,25 +494,33 @@
 > bot 更新人格后会丢失原人格预设，如需保留请自行备份
 
 - 扩展文件: ext_evolution.py
 - 说明: 赋予 bot 自主发展人格的能力，允许 bot 自主设定更新人设
 - 配置项:
   - notify_type: 触发更新时通知类型 0: 无通知; 1: 仅触发提示; 2: 新预设完整通知 (默认: 1)
 
+#### > [Minecraft 服务器专用] 执行服务器命令模块
+
+- 扩展文件: ext_mc_command.py
+- 说明: 赋予 bot 执行 Minecraft 服务器命令的能力，鉴权基于字符串匹配，请谨慎使用过滤高危命令，黑白名单匹配的内容包括指令前缀 `/`
+- 配置项:
+  - match_white_list: 匹配指令内容白名单列表 (列表中至少一个字符串应被包含在命令中，为空则不限制)
+  - match_black_list: 匹配指令内容黑名单列表 (列表中所有字符串都不应被包含在命令中，为空则不限制，优先级高于白名单)
+
 #### > 主动记忆能力扩展模块 (因 bot 使用积极性不佳，暂移入备份，不推荐使用)
 
 - 扩展文件: ext_remember.py & ext_forget.py
 - 说明: 赋予 bot 主动管理记忆的能力，使用时请同时启用 记忆|遗忘 扩展
 
 ### 编写自定义扩展
 
 > 自行编写扩展需要具有一定的 Python 编程基础，如果您有相关能力可直接参考本仓库 `/extensions/` 目录下的扩展进行编写(非常简单！) 自行编写的扩展安装流程与上述相同
 > 注意：该功能尚处于早期阶段，扩展编写在未来版本有可能随时变化！
 
-✨ 如果您想分享您自行开发的扩展，可向本仓库提交 pr，将您的扩展命名为 `share_ext_xxx.py`('xxx'部分可自行命名，请勿与已存在的扩展名冲突) 并上传至本仓库的 `/share_exts/` 目录下，欢迎您成为本项目的贡献者！
+✨ 如果您想分享您自行开发的扩展，可向本仓库提交 pr，将您的扩展命名为 `ext_xxx.py`('xxx'部分可自行命名，请勿与已存在的扩展名冲突) 并上传至本仓库的 `/extensions/` 目录下，欢迎您成为本项目的贡献者！
 
 #### 基本的扩展模块模板
 
 <details> <summary>🔍点击查看扩展模块编写模板</summary> <pre><code>
 
 ```python
 from .Extension import Extension
@@ -528,14 +542,16 @@
     "author": "",
     # 版本
     "version": "0.0.1"
     # 扩展简介
     "intro": "简介信息（查看扩展详情显示）",
     # 调用时是否打断响应 启用后将会在调用后截断后续响应内容
     "interrupt": True,
+    # 可用会话类型 (server即MC服务器 | chat即QQ聊天)
+    "available": ['server'],
 }
 
 class CustomExtension(Extension):
     async def call(self, arg_dict: dict, ctx_data: dict) -> dict:
         """ 当扩展被调用时执行的函数 *由扩展自行实现*
 
         参数:
@@ -553,51 +569,82 @@
 
     def __init__(self, custom_config: dict):
         super().__init__(ext_config.copy(), custom_config)
 ```
 
 </code></pre> </details>
 
+## 🗺️ MC 服务器支持
+
+> 允许 bot 接入 Minecraft 服务器，并可在服务器中执行指令
+> 使用前需要编辑配置文件并开启 ENABLE_MC_CONNECT 项
+
+### 适配器安装
+
+> 插件使用 spigot 适配器接收服务器消息推送和文字发送
+
+使用 `nb adapter install nonebot-adapter-spigot` 指令安装适配器
+
+#### MC 服务器端支持安装
+
+参考 [MC_qq 安装文档](https://17theword.github.io/mc_qq/install/mcrcon_plugin.html#minecraft-server-%E7%AB%AF) 中的 `Minecraft Server 端` 步骤安装服务端插件
+
+注意事项 1：配置文件中 `websocket_url: "ws://127.0.0.1:8765"` 的值部分应改为 `ws://Nonebot服务器ip:Nonebot监听端口/spigot/ws`
+
+注意事项 2：如果你的 MC 服务端和 Nonebot 服务端不在同一台服务器上，需要在 `.env` 中将 NoneBot 的监听地址改为 `0.0.0.0` 并放行对应端口，否则将导致连接失败
+
+#### RCON 配置
+> RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
+
+1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
+2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
+
 ## 🎢 更新日志
 
-## [2023/4/6] v2.0.5
+## [2023/4/15] v2.1.0 Minecraft 服务器支持
+
+- 增加了 Minecraft 服务器接入支持
+- 增加了 Minecraft 服务器指令执行支持和相关扩展模块
+- 为绘图扩展增加了代理配置项支持 (感谢 @tonato-01 提供 pr)
+
+## [2023/4/6] v2.0.5 RENAME 指令 | json 导出支持
 
 - 解析消息中的@时保持与用户看到的一致 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 优化日志输出的 DEBUG_LEVEL 限制 (感谢 @Misaka-Mikoto-Tech 提供 pr)
-- 优化聊天消息prompt的换行生成逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
+- 优化聊天消息 prompt 的换行生成逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 增加 `rg rename` 改名指令，用于修改人格名 (感谢 @Misaka-Mikoto-Tech 提供 pr) (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 解析消息中的@时保持与用户看到的一致 (感谢 @Misaka-Mikoto-Tech 提供 pr)
-- patch logger使插件名称显示为中文 (感谢 @chenxuan353 提供 pr)
-- 添加记忆文件(原.pkl)使用JSON读取与保存功能 (与原pickle兼容) (感谢 @chenxuan353 提供 pr)
+- patch logger 使插件名称显示为中文 (感谢 @chenxuan353 提供 pr)
+- 添加记忆文件(原.pkl)使用 JSON 读取与保存功能 (与原 pickle 兼容) (感谢 @chenxuan353 提供 pr)
 - 优化部分代码类型注解 (感谢 @chenxuan353 提供 pr)
-- 搜索扩展(ext_search.py) 优化，禁止bot短时间内反复搜索和搜索重复内容
+- 搜索扩展(ext_search.py) 优化，禁止 bot 短时间内反复搜索和搜索重复内容
 
 ## [2023/3/26] v2.0.4
 
 - 修复 @全体成员 时解析报错问题
 - 增加扩展更新人格支持，同时增加了一个 evolution 扩展模块，允许 bot 自主更新人格
 - 响应规则中增加一条禁止复读规则
 
-## [2023/3/26] v2.0.3
+## [2023/3/26] v2.0.3 图片输出支持
 
 - 输出内容转图片: 使用 htmlrender 将 TA 的回复转换为图片，降低风控几率 (可选开关，感谢 @HMScygnet 提供 pr)
 - 等待 OpenAI 响应过程中切换人格预设或响应超时后停止处理消息 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 修正编辑和删除预设判断是否锁定以及是否是默认预设和正在使用的预设的逻辑 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 增加调用扩展时预检支持打断响应，优化搜索扩展执行效果，避免 bot 自行脑补搜索结果的情况
 - 修正一些指令帮助信息的内容错误
 - 修正通过指令安装扩展时的编码问题
 - 修正纯符号过滤判断逻辑
 
-## [2023/3/21] v2.0.2
+## [2023/3/21] v2.0.2 扩展下载指令支持
 
 - 切换人格时的聊天输出改为非 DEBUG 模式下也会发送
 - 增加了扩展 安装/删除 指令，可直接从 GitHub 上获取到最新扩展
 - 精简了非 DEBUG 模式下的控制台输出
 
-## [2023/3/20] v2.0.1
+## [2023/3/20] v2.0.1 VIOCEVOX 语音扩展
 
 - 修正 `-global` 的控制权限和逻辑 (感谢 [@Misaka-Mikoto-Tech](https://github.com/) 提供 pr)
 - 增加了一个新的语音扩展 `ext_VOICEVOX` 能够更便捷地实现本地部署 (感谢 @恋如雨止 提供技术支持)
 - 修正回复内容首尾的空行问题；修正短纯符号回复内容未正常过滤的问题
 - 修正私聊会话权限设定
 
 ## [2023/3/18] v2.0.0 项目重构 🎉
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.0 Summary:
 ä¸ä¸ªåºäºNoneBotæ¡æ¶çAièå¤©æä»¶ï¼å¯¹æ¥OpenAiææ¬çææ¥å£
 License: Apache-2.0 Author: KroMiose Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot
@@ -14,16 +14,19 @@
                â¨ æ´äººæ§å(æäºº)çGPTèå¤©Aiæä»¶! â¨
  ð§¬ æ¯æå¤ä¸ªäººæ ¼èªå®ä¹ / åæ¢ | å°½æåæ¥ä½ çæ³è±¡åå§ï¼
                                     âï¸
       ð§¬ é¢è®¾æ¶éå±äº«è¡¨(æ¬¢è¿åäº«åç§èªå®ä¹äººè®¾) ð§¬
  ð å¦æåæ¬¢è¯·ç¹ä¸ªâ­å§ï¼æ¨çæ¯æå°±æ¯ææç»­æ´æ°çå¨å
                                      ð
                       [license] [pypi] [python] [python]
-                ***** ð [2023/3/16] é¡¹ç®éæ ð *****
-  é¡¹ç®éææ´çåºæ¬å®æï¼æ¬è¯·æå¾éæåæ´å¤åè½æ§æ´æ°
+***** ð  [2023/4/14] v2.1 Minecraftæå¡å¨æ¥å¥ä¸æ¸¸ææä»¤æ©å±æ¯æ
+                                 ðºï¸ *****
+      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥ MC æå¡å¨ï¼å¹¶ä¸æ¯æ bot
+                          ä½¿ç¨æ¸¸æåæä»¤æ©å±
+           ***** ð [2023/3/16] v2.0 é¡¹ç®éæå®æ ð *****
       æè°¢@Misaka-Mikoto-Techå¤§ä½¬å¯¹é¡¹ç®éææä¾çå¤§åæ¯æ
      ***** âï¸ [2023/3/2] v1.4 æ´æ°: æ¯æChatGPTæ¨¡å âï¸ *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æå®æ¹ChatGPTæ¨¡åæ¥å£ï¼tokenå®ä»·ä»ä¸ºGPT3ç
                   1/10, åå¤è´¨éæ´é« ååºéåº¦æ´å¿«
      ***** ð§© [2023/2/18] v1.3 æ´æ°: èªå®ä¹æ©å±æ¯æ ð§© *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æèªå®ä¹æ©å±ï¼æ¨å¯ä»¥ç´æ¥éè¿èªç¶è¯­è¨ç´æ¥è°ç¨å¤ç§æ©å±åè½ï¼åæ¬
                         ææ¬/å¾ç/è¯­é³/é®ä»¶...
@@ -236,14 +239,30 @@
 | UNLOCK_CONTENT_LIMIT          | bool  | æ¯å¦è§£éåå®¹éå¶
 | False                          | å¯è½å¯¼è´ OpenAi
 è´¦å·é£é©ï¼è¯·èªè¡æ¿æåæ
 |
 | OPENAI_PROXY_SERVER           | str   | è¯·æ± OpenAI çä»£çæå¡å¨
 | ''                             | å¡«åç¤ºä¾ '127.0.0.1:1234' æ 'username:
 password@127.0.0.1:1234'                         |
+| ENABLE_MC_CONNECT             | bool  | æ¯å¦å¼å¯ MC æå¡å¨è¿æ¥
+| False                          | å¼å¯åå¯è¿æ¥å° Minecraft æå¡å¨
+|
+| MC_COMMAND_PREFIX             | array | MC
+æå¡å¨ä¸­äººæ ¼ç¼è¾æä»¤åç¼                | ['!', 'ï¼']
+| MC æå¡å¨ä¸­äººæ ¼ç¼è¾æä»¤åç¼
+|
+| MC_RCON_HOST                  | str   | MC æå¡å¨ RCON å°å
+| '127.0.0.1'                    | MC æå¡å¨ RCON å°å
+|
+| MC_RCON_PORT                  | int   | MC æå¡å¨ RCON ç«¯å£
+| 25575                          | MC æå¡å¨ RCON ç«¯å£
+|
+| MC_RCON_PASSWORD              | str   | MC æå¡å¨ RCON å¯ç 
+| '123456'                       | MC æå¡å¨ RCON å¯ç 
+|
 | DEBUG_LEVEL                   | int   | DEBUG ç­çº§
 | 0                              | ç­çº§è¶é« debug ä¿¡æ¯è¶è¯¦ç»
 |
 
 
  ## ðª æä»¤è¯´æ ### åºæ¬å½ä»¤ââ"rg"(éè¦å ä¸å¨ NoneBot
 ä¸­è®¾å®çæä»¤åç¼) - å«ç§°: "äººæ ¼"ã"äººæ ¼è®¾å®"ã"identity" -
@@ -563,27 +582,35 @@
 OREOREO) - æ©å±æä»¶: ext_paint.py - è¯´æ: è°ç¨ openai
 ç»å¾æ¥å£ï¼å®ç°èªç¶è¯­è¨è°ç¨ç»ç»ï¼æ¥å£å±ç¨æ¬æä»¶ç Api
 Key #### > è¿åæ¨¡å > bot
 æ´æ°äººæ ¼åä¼ä¸¢å¤±åäººæ ¼é¢è®¾ï¼å¦éä¿çè¯·èªè¡å¤ä»½ -
 æ©å±æä»¶: ext_evolution.py - è¯´æ: èµäº bot
 èªä¸»åå±äººæ ¼çè½åï¼åè®¸ bot èªä¸»è®¾å®æ´æ°äººè®¾ - éç½®é¡¹:
 - notify_type: è§¦åæ´æ°æ¶éç¥ç±»å 0: æ éç¥; 1: ä»è§¦åæç¤º; 2:
-æ°é¢è®¾å®æ´éç¥ (é»è®¤: 1) #### > ä¸»å¨è®°å¿è½åæ©å±æ¨¡å (å 
-bot ä½¿ç¨ç§¯ææ§ä¸ä½³ï¼æç§»å¥å¤ä»½ï¼ä¸æ¨èä½¿ç¨) - æ©å±æä»¶:
+æ°é¢è®¾å®æ´éç¥ (é»è®¤: 1) #### > [Minecraft æå¡å¨ä¸ç¨]
+æ§è¡æå¡å¨å½ä»¤æ¨¡å - æ©å±æä»¶: ext_mc_command.py - è¯´æ: èµäº
+bot æ§è¡ Minecraft
+æå¡å¨å½ä»¤çè½åï¼é´æåºäºå­ç¬¦ä¸²å¹éï¼è¯·è°¨æä½¿ç¨è¿æ»¤é«å±å½ä»¤ï¼é»ç½ååå¹éçåå®¹åæ¬æä»¤åç¼
+`/` - éç½®é¡¹: - match_white_list: å¹éæä»¤åå®¹ç½åååè¡¨
+(åè¡¨ä¸­è³å°ä¸ä¸ªå­ç¬¦ä¸²åºè¢«åå«å¨å½ä»¤ä¸­ï¼ä¸ºç©ºåä¸éå¶) -
+match_black_list: å¹éæä»¤åå®¹é»åååè¡¨
+(åè¡¨ä¸­ææå­ç¬¦ä¸²é½ä¸åºè¢«åå«å¨å½ä»¤ä¸­ï¼ä¸ºç©ºåä¸éå¶ï¼ä¼åçº§é«äºç½åå)
+#### > ä¸»å¨è®°å¿è½åæ©å±æ¨¡å (å  bot
+ä½¿ç¨ç§¯ææ§ä¸ä½³ï¼æç§»å¥å¤ä»½ï¼ä¸æ¨èä½¿ç¨) - æ©å±æä»¶:
 ext_remember.py & ext_forget.py - è¯´æ: èµäº bot
 ä¸»å¨ç®¡çè®°å¿çè½åï¼ä½¿ç¨æ¶è¯·åæ¶å¯ç¨ è®°å¿|éå¿ æ©å± ###
 ç¼åèªå®ä¹æ©å± > èªè¡ç¼åæ©å±éè¦å·æä¸å®ç Python
 ç¼ç¨åºç¡ï¼å¦ææ¨æç¸å³è½åå¯ç´æ¥åèæ¬ä»åº `/extensions/
 ` ç®å½ä¸çæ©å±è¿è¡ç¼å(éå¸¸ç®åï¼)
 èªè¡ç¼åçæ©å±å®è£æµç¨ä¸ä¸è¿°ç¸å >
 æ³¨æï¼è¯¥åè½å°å¤äºæ©æé¶æ®µï¼æ©å±ç¼åå¨æªæ¥çæ¬æå¯è½éæ¶ååï¼
 â¨ å¦ææ¨æ³åäº«æ¨èªè¡å¼åçæ©å±ï¼å¯åæ¬ä»åºæäº¤
-prï¼å°æ¨çæ©å±å½åä¸º `share_ext_xxx.py`
+prï¼å°æ¨çæ©å±å½åä¸º `ext_xxx.py`
 ('xxx'é¨åå¯èªè¡å½åï¼è¯·å¿ä¸å·²å­å¨çæ©å±åå²çª)
-å¹¶ä¸ä¼ è³æ¬ä»åºç `/share_exts/
+å¹¶ä¸ä¼ è³æ¬ä»åºç `/extensions/
 ` ç®å½ä¸ï¼æ¬¢è¿æ¨æä¸ºæ¬é¡¹ç®çè´¡ç®èï¼ ####
 åºæ¬çæ©å±æ¨¡åæ¨¡æ¿  ðç¹å»æ¥çæ©å±æ¨¡åç¼åæ¨¡æ¿
 
 
 ```python
 from .Extension import Extension
 
@@ -611,14 +638,16 @@
     # çæ¬
     "version": "0.0.1"
     # æ©å±ç®ä»
     "intro": "ç®ä»ä¿¡æ¯ï¼æ¥çæ©å±è¯¦ææ¾ç¤ºï¼",
     # è°ç¨æ¶æ¯å¦ææ­ååº
 å¯ç¨åå°ä¼å¨è°ç¨åæªæ­åç»­ååºåå®¹
     "interrupt": True,
+    # å¯ç¨ä¼è¯ç±»å (serverå³MCæå¡å¨ | chatå³QQèå¤©)
+    "available": ['server'],
 }
 
 class CustomExtension(Extension):
     async def call(self, arg_dict: dict, ctx_data: dict) -> dict:
         """ å½æ©å±è¢«è°ç¨æ¶æ§è¡çå½æ° *ç±æ©å±èªè¡å®ç°*
 
         åæ°:
@@ -635,50 +664,73 @@
             'voice': f"http://...",  # è¯­é³url
         }
 
     def __init__(self, custom_config: dict):
         super().__init__(ext_config.copy(), custom_config)
 ```
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/6] v2.0.5 -
+ ## ðºï¸ MC æå¡å¨æ¯æ > åè®¸ bot æ¥å¥ Minecraft
+æå¡å¨ï¼å¹¶å¯å¨æå¡å¨ä¸­æ§è¡æä»¤ >
+ä½¿ç¨åéè¦ç¼è¾éç½®æä»¶å¹¶å¼å¯ ENABLE_MC_CONNECT é¡¹ ###
+ééå¨å®è£ > æä»¶ä½¿ç¨ spigot
+ééå¨æ¥æ¶æå¡å¨æ¶æ¯æ¨éåæå­åé ä½¿ç¨ `nb adapter install
+nonebot-adapter-spigot` æä»¤å®è£ééå¨ #### MC æå¡å¨ç«¯æ¯æå®è£
+åè [MC_qq å®è£ææ¡£](https://17theword.github.io/mc_qq/install/
+mcrcon_plugin.html#minecraft-server-%E7%AB%AF) ä¸­ç `Minecraft Server ç«¯`
+æ­¥éª¤å®è£æå¡ç«¯æä»¶ æ³¨æäºé¡¹ 1ï¼éç½®æä»¶ä¸­ `websocket_url:
+"ws://127.0.0.1:8765"` çå¼é¨ååºæ¹ä¸º `ws://Nonebotæå¡å¨ip:
+Nonebotçå¬ç«¯å£/spigot/ws` æ³¨æäºé¡¹ 2ï¼å¦æä½ ç MC æå¡ç«¯å
+Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
+ççå¬å°åæ¹ä¸º `0.0.0.0`
+å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
+Minecraft
+æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
+RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
+`enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ## ð¢ æ´æ°æ¥å¿
+## [2023/4/15] v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft
+æå¡å¨æ¥å¥æ¯æ - å¢å äº Minecraft
+æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
+ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
+[2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
-Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯promptçæ¢è¡çæé»è¾ (æè°¢
-@Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
+Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
+(æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
 æ¹åæä»¤ï¼ç¨äºä¿®æ¹äººæ ¼å (æè°¢ @Misaka-Mikoto-Tech æä¾ pr)
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
-Tech æä¾ pr) - patch loggerä½¿æä»¶åç§°æ¾ç¤ºä¸ºä¸­æ (æè°¢
-@chenxuan353 æä¾ pr) - æ·»å è®°å¿æä»¶
-(å.pkl)ä½¿ç¨JSONè¯»åä¸ä¿å­åè½ (ä¸åpickleå¼å®¹) (æè°¢
-@chenxuan353 æä¾ pr) - ä¼åé¨åä»£ç ç±»åæ³¨è§£ (æè°¢ @chenxuan353
-æä¾ pr) - æç´¢æ©å±(ext_search.py)
-ä¼åï¼ç¦æ­¢botç­æ¶é´ååå¤æç´¢åæç´¢éå¤åå®¹ ## [2023/3/26]
-v2.0.4 - ä¿®å¤ @å¨ä½æå æ¶è§£ææ¥éé®é¢ -
+Tech æä¾ pr) - patch logger ä½¿æä»¶åç§°æ¾ç¤ºä¸ºä¸­æ (æè°¢
+@chenxuan353 æä¾ pr) - æ·»å è®°å¿æä»¶(å.pkl)ä½¿ç¨ JSON
+è¯»åä¸ä¿å­åè½ (ä¸å pickle å¼å®¹) (æè°¢ @chenxuan353 æä¾ pr) -
+ä¼åé¨åä»£ç ç±»åæ³¨è§£ (æè°¢ @chenxuan353 æä¾ pr) - æç´¢æ©å±
+(ext_search.py) ä¼åï¼ç¦æ­¢ bot
+ç­æ¶é´ååå¤æç´¢åæç´¢éå¤åå®¹ ## [2023/3/26] v2.0.4 - ä¿®å¤
+@å¨ä½æå æ¶è§£ææ¥éé®é¢ -
 å¢å æ©å±æ´æ°äººæ ¼æ¯æï¼åæ¶å¢å äºä¸ä¸ª evolution
 æ©å±æ¨¡åï¼åè®¸ bot èªä¸»æ´æ°äººæ ¼ -
-ååºè§åä¸­å¢å ä¸æ¡ç¦æ­¢å¤è¯»è§å ## [2023/3/26] v2.0.3 -
-è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
+ååºè§åä¸­å¢å ä¸æ¡ç¦æ­¢å¤è¯»è§å ## [2023/3/26] v2.0.3
+å¾çè¾åºæ¯æ - è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
 çåå¤è½¬æ¢ä¸ºå¾çï¼éä½é£æ§å ç (å¯éå¼å³ï¼æè°¢ @HMScygnet
 æä¾ pr) - ç­å¾ OpenAI
 ååºè¿ç¨ä¸­åæ¢äººæ ¼é¢è®¾æååºè¶æ¶ååæ­¢å¤çæ¶æ¯ (æè°¢
 @Misaka-Mikoto-Tech æä¾ pr) -
 ä¿®æ­£ç¼è¾åå é¤é¢è®¾å¤æ­æ¯å¦éå®ä»¥åæ¯å¦æ¯é»è®¤é¢è®¾åæ­£å¨ä½¿ç¨çé¢è®¾çé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) -
 å¢å è°ç¨æ©å±æ¶é¢æ£æ¯æææ­ååºï¼ä¼åæç´¢æ©å±æ§è¡ææï¼é¿å
 bot èªè¡èè¡¥æç´¢ç»æçæåµ -
 ä¿®æ­£ä¸äºæä»¤å¸®å©ä¿¡æ¯çåå®¹éè¯¯ -
 ä¿®æ­£éè¿æä»¤å®è£æ©å±æ¶çç¼ç é®é¢ -
-ä¿®æ­£çº¯ç¬¦å·è¿æ»¤å¤æ­é»è¾ ## [2023/3/21] v2.0.2 -
-åæ¢äººæ ¼æ¶çèå¤©è¾åºæ¹ä¸ºé DEBUG æ¨¡å¼ä¸ä¹ä¼åé -
-å¢å äºæ©å± å®è£/å é¤ æä»¤ï¼å¯ç´æ¥ä» GitHub
-ä¸è·åå°ææ°æ©å± - ç²¾ç®äºé DEBUG æ¨¡å¼ä¸çæ§å¶å°è¾åº ##
-[2023/3/20] v2.0.1 - ä¿®æ­£ `-global` çæ§å¶æéåé»è¾ (æè°¢
-[@Misaka-Mikoto-Tech](https://github.com/) æä¾ pr) -
-å¢å äºä¸ä¸ªæ°çè¯­é³æ©å± `ext_VOICEVOX`
+ä¿®æ­£çº¯ç¬¦å·è¿æ»¤å¤æ­é»è¾ ## [2023/3/21] v2.0.2
+æ©å±ä¸è½½æä»¤æ¯æ - åæ¢äººæ ¼æ¶çèå¤©è¾åºæ¹ä¸ºé DEBUG
+æ¨¡å¼ä¸ä¹ä¼åé - å¢å äºæ©å± å®è£/å é¤ æä»¤ï¼å¯ç´æ¥ä»
+GitHub ä¸è·åå°ææ°æ©å± - ç²¾ç®äºé DEBUG
+æ¨¡å¼ä¸çæ§å¶å°è¾åº ## [2023/3/20] v2.0.1 VIOCEVOX è¯­é³æ©å± -
+ä¿®æ­£ `-global` çæ§å¶æéåé»è¾ (æè°¢ [@Misaka-Mikoto-Tech](https:/
+/github.com/) æä¾ pr) - å¢å äºä¸ä¸ªæ°çè¯­é³æ©å± `ext_VOICEVOX`
 è½å¤æ´ä¾¿æ·å°å®ç°æ¬å°é¨ç½² (æè°¢ @æå¦é¨æ­¢ æä¾ææ¯æ¯æ)
 -
 ä¿®æ­£åå¤åå®¹é¦å°¾çç©ºè¡é®é¢ï¼ä¿®æ­£ç­çº¯ç¬¦å·åå¤åå®¹æªæ­£å¸¸è¿æ»¤çé®é¢
 - ä¿®æ­£ç§èä¼è¯æéè®¾å® ## [2023/3/18] v2.0.0 é¡¹ç®éæ ð >
 âââ æ³¨æï¼æ¬æ¬¡æ´æ°éè¦å é¤å bot è®°å¿æä»¶éæ°çæ
 (å³./data/naturel_gpt
 æä»¶å¤¹)ï¼å¦åå¯è½äº§çæ æ³é¢è®¡çéè¯¯ï¼åæ¶å»ºè®®å°éç½®æä»¶ä¸å¹¶å é¤éæ°çæï¼æ­¤æä½ä¼**ä¸¢å¤±**ææç¼è¾è¿çäººæ ¼é¢è®¾ï¼å¦æä½ éè¦å¨æ´æ°åç»§ç»­ä½¿ç¨ï¼è¯·ä½¿ç¨
```

