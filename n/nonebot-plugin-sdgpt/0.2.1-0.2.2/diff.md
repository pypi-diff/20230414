# Comparing `tmp/nonebot_plugin_sdgpt-0.2.1.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.1.tar` & `nonebot_plugin_sdgpt-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.1/LICENSE
--rw-r--r--   0        0        0     6752 2023-04-13 05:20:16.403047 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     5007 2023-04-13 05:26:32.824762 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     3440 2023-04-13 06:47:06.644004 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0     3616 2023-04-13 04:20:50.670050 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/configspec.ini
--rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     2983 2023-04-13 03:22:58.157097 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0      362 2023-04-13 02:43:26.492368 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1160 2023-04-13 06:49:05.865430 nonebot_plugin_sdgpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.1/README.md
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.2/LICENSE
+-rw-r--r--   0        0        0     9307 2023-04-14 05:57:29.503439 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     5179 2023-04-14 03:33:23.558251 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     4058 2023-04-14 03:50:34.726392 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     3670 2023-04-14 05:33:38.768842 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     2987 2023-04-14 02:02:57.821153 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0     1717 2023-04-14 05:11:14.277310 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1160 2023-04-14 06:04:08.961530 nonebot_plugin_sdgpt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.2/README.md
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/LICENSE` & `nonebot_plugin_sdgpt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,69 @@
 import asyncio
 import os
+import re
 import time
 from io import BytesIO
 
-from nonebot import on_command
+from nonebot import on_command, on_message
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 from .bot import bot_start, msg_end, Chat
 from .lib.cons import *
-from .lib.utils import load_preset
+from .lib.utils import load_preset, rules, getThis
 from webuiapi import webuiapi
 
 cfg = asyncio.run(bot_start())
 config = cfg['cfg']
 
 BotUse = config['Chat']['defaultAI']
 
 
 @event_postprocessor
 async def postprocessor():
     await msg_end()
 
 
-chat = on_command(config['Command']['chat'][1:])
-bing = on_command(config['Command']['bing'][1:])
-switchAI = on_command(config['Command']['switchAI'][1:])
-switch = on_command(config['Command']['switch'][1:])
-switchPreset = on_command(config['Command']['switchPreset'][1:])
-tag = on_command(config['Command']['tag'][1:])
-SD_webui = on_command(config['Command']['SD_webui'][1:])
+L_webuiapi = asyncio.Lock()
+chat = on_command(config['Command']['chat'][1:], priority=1, block=True)
+bing = on_command(config['Command']['bing'][1:], priority=1, block=True)
+switchAI = on_command(config['Command']['switchAI'][1:], priority=1, block=True)
+switch = on_command(config['Command']['switch'][1:], priority=1, block=True)
+switchPreset = on_command(config['Command']['switchPreset'][1:], priority=1, block=True)
+tag = on_command(config['Command']['tag'][1:], priority=1, block=True)
+SD_webui = on_command(config['Command']['SD_webui'][1:], priority=1, block=True)
+MSG = on_message(rule=to_me(), priority=2, block=True)
+
+
+@MSG.handle()
+async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent):
+    if not rules('msg', config, event): return
+
+    def asChat():
+        global BotUse
+        if BotUse in cfg:
+            return BotUse
+        else:
+            if 'chatgpt-api' in cfg: return 'chatgpt-api'
+            if 'chatgpt' in cfg: return 'chatgpt'
+            if 'bing' in cfg: return 'bing'
+            error('/chat', '你没有任何chatgpt接入')
+            return False
+
+    message = str(event.message)
+    BOT = asChat()
+    if len(message) == 0: return
+    if BOT:
+        info(BOT, '对话: ' + message)
+        await Chat(event, foo, BOT, message)
 
 
 @chat.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
+    if not rules('chat', config, event): return
+
     def asChatGPT():
         global BotUse
         if 'chatgpt' in BotUse:
             return BotUse
         else:
             if 'chatgpt-api' in cfg:
                 return 'chatgpt-api'
@@ -51,29 +79,32 @@
     if BOT:
         info(BOT, '对话: ' + message)
         await Chat(event, foo, BOT, message)
 
 
 @bing.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
+    if not rules('bing', config, event): return
+
     def asBing():
-        global BotUse
         if 'bing' not in cfg:
             error('bing', '你没有接入bing')
-            return False
+            return True
+        return 'bing'
 
     if asBing():
         message = args.extract_plain_text()
         if len(message) == 0: return
         info('bing', '对话: ' + message)
         await Chat(event, foo, 'bing', message)
 
 
 @tag.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
+    if not rules('tag', config, event): return
     def asChat():
         global BotUse
         if BotUse in cfg:
             return BotUse
         else:
             if 'chatgpt-api' in cfg: return 'chatgpt-api'
             if 'chatgpt' in cfg: return 'chatgpt'
@@ -87,14 +118,15 @@
     if BOT:
         info(BOT, '对话: ' + message)
         await Chat(event, foo, BOT, message, noStream=True, p='tag')
 
 
 @SD_webui.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
+    if not rules('SD_webui', config, event): return
     def asChat():
         global BotUse
         if BotUse in cfg:
             return BotUse
         else:
             if 'chatgpt-api' in cfg: return 'chatgpt-api'
             if 'chatgpt' in cfg: return 'chatgpt'
@@ -109,39 +141,42 @@
         info(BOT, '对话: ' + message)
         prompt = await Chat(event, foo, BOT, message, p='tag', noOut=True)
         sd = config['Stable-Diffusion']
         ip = sd['api_host']
         DIR = sd['save_path']
         info('Stable-Diffusion', '开始询问 api : ' + ip)
         ip = ip.split(':')
+
         api = webuiapi.WebUIApi(host=ip[0], port=ip[1])  # type: ignore
 
-        result1 = api.txt2img(
+        task = asyncio.to_thread(api.txt2img(
             prompt=prompt,
             negative_prompt=sd['negative_prompt'],
             steps=sd['step'],
-        )
-        image = result1.image
+        ))
+        async with L_webuiapi:
+            result = await task
+        image = result.image
         success('Stable-Diffusion', '返回图片')
         buffered = BytesIO()
         if DIR == '':
             DIR = '.'
             ID = 'OUT'
         else:
             lt = time.localtime(time.time())
             ID = time.strftime("%Y_%m_%d_%H%M%S", lt)
         image.save(f"{DIR}/{ID}.png", "PNG")
         image.save(buffered, format="PNG")
         await foo.send(event, MessageSegment.image(buffered), reply_message=config['Chat']['reply'])
         return
 
 
-
 @switchAI.handle()
 async def _(foo: Bot, event: Event, args: Message = CommandArg()):
+    if not rules('switchAI', config, event): return
     use = args.extract_plain_text()
     if len(args) == 0: return
     if use in config:
         global BotUse
         BotUse = use
         await switchAI.send('已切换到 ' + BotUse)
         suc('切换AI', BotUse)
@@ -149,40 +184,67 @@
         await switchAI.send('AI不存在')
         warn("切换AI", f'AI不存在 , {use} is not in: {cfg}')
 
 
 @switch.handle()
 async def _(event: Event, args: Message = CommandArg()):
     global config
+    if not rules('switch', config, event): return
     args = args.extract_plain_text().split(' ')
     if len(args) == 0: return
+    if args[0] == '群聊': args = ['Function','Group','groups',args[-1]]
+    if args[0] == '私聊': args = ['Function','Private','member',args[-1]]
+    if args[0] == '频道': args = ['Function', 'Guild', 'guilds', args[-1]]
     path = args[:-2]
     isOwner = (config['Bot']['owner'] == event.get_user_id())
     if config['Bot']['switchConfigEval'] is False and not isOwner:
         return warn('/switch', '无权限更改')
     if args[0] == 'Bot' and not isOwner:
         return warn('/switch', '无权限更改 Bot')
     now = config
     for i in path:
         now = now[i]
     if args[-1] in ['True', 'true', '1', 'on']:
         data = True
     elif args[-1] in ['False', 'false', '0', 'off']:
         data = False
+    elif args[-1] == '=this':
+        data = [getThis(event)]
+    elif args[-1] == '*':
+        data = ['*']
+    elif args[-1] == '+this':
+        if '*' in now[args[-2]]:
+            now[args[-2]].remove('*')
+        now[args[-2]].append(getThis(event))
+        data = now[args[-2]]
+    elif args[-1] == '-this':
+        try:
+            now[args[-2]].remove(getThis(event))
+        except:
+            return await switch.send('.'.join(args[:-1]) + '中没有' + str(getThis(event)))
+        data = now[args[-2]]
     else:
         data = args[-1]
+    if not isinstance(now[args[-2]], (int, float, str, bool, list)):
+        rep = {"'(access_token)': '[^’]*'": r"[$1]",
+               "'(api_key)': '[^']*'": r"[$2]",
+               "'(api_host)': '[^']*'": r"[$3]",
+        }
+        result = re.sub("|".join(rep.keys()), '[隐藏]', str(now[args[-2]]))
+        return await switch.send(result)
     now[args[-2]] = data
     config.write()
     print(config['Chat'])
     await switch.send('.'.join(args[:-1]) + '已改为' + str(data))
 
 
 @switchPreset.handle()
 async def _(event: Event, args: Message = CommandArg()):
     global config
+    if not rules('switchPreset', config, event): return
     args = args.extract_plain_text()
     if len(args) == 0: return
     isOwner = (config['Bot']['owner'] == event.get_user_id())
     if config['Bot']['switchConfigEval'] is False and not isOwner:
         return warn('/switch', '无权限更改')
     if args in config['preset']:
         config['runtime']['preset'] = config['preset'][args]
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import asyncio
 import os
 import re
 import time
+
+from celery import Celery
+
 from .lib.cons import *
 from .lib.base import *
 from .lib.utils import load_preset
 from .config import load as cfg_load
 from nonebot.adapters.onebot.v11.adapter import Message
 
 global dotenv_file
 global chatgpt
 global chatgpt_api
 global bing
 global config
 global defaultAI
 
-runs = {
-    'chatgpt': False,
-    'chatgpt-api': False,
-    'bing': False,
-}
-
 
 async def bot_start():
+    global L_chatgpt
+    global L_chatgpt_api
+    global L_bing
     global chatgpt
     global chatgpt_api
     global bing
     global config
     global defaultAI
     cfg = await cfg_load()
     if 'chatgpt' in cfg: chatgpt = cfg['chatgpt']
@@ -34,23 +34,26 @@
     if 'bing' in cfg: bing = cfg['bing']
     config = cfg['cfg']
     if config['Chat']['reload_presets']:
         config['runtime']['preset'] = ''
         config.write()
     defaultAI = config['Chat']['defaultAI']
 
+    L_chatgpt = asyncio.Lock()
+    #L_chatgpt_api = asyncio.Lock()
+    L_bing = asyncio.Lock()
+
     return cfg
 
 
 async def msg_end():
     return
 
 
 async def Chat(event, foo, BOT, message, p='', noStream=False, noOut=False):
-    global runs
     if noOut:
         noStream = True
     if len(p) == 0 and len(config['runtime']['preset']) > 2:
         p = await load_preset(config['Chat']['presets_dir'], config['runtime']['preset'])
         info('预设', p)
     elif len(p) > 0:
         p = await load_preset(config['Chat']['presets_dir'], config['preset'][p])
@@ -60,49 +63,45 @@
         stream = config['Function']['Group']['stream']
     elif type(event) == GuildMessageEvent:
         stream = config['Function']['Guild']['stream']
     elif type(event) == PrivateMessageEvent:
         stream = config['Function']['Private']['stream']
     else:
         return
-    while runs[BOT] is True:
-        await asyncio.sleep(1)
-
-    if runs[BOT] is False:
-        runs[BOT] = True
+    if noStream:
+        stream = False
+    if stream:
+        await ask_stream(event, foo, BOT, message, p)
+    else:
+        out = await ask(BOT, message, p)
         if noStream:
-            stream = False
-        if stream:
-            await ask_stream(event, foo, BOT, message, p)
-        else:
-            out = await ask(BOT, message, p)
-            if noStream:
-                out = re.sub(r".*\.AIP", "", out)
-            if noOut:
-                return out
-            await foo.send(event, out, reply_message=reply)
-            runs[BOT] = False
+            out = re.sub(r".*\.AIP", "", out)
+        if noOut:
+            return out
+        await foo.send(event, out, reply_message=reply)
 
 
 async def ask(bot, message, prompt=''):
     if bot == 'chatgpt':
-        if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
-        info('ASK', message)
-        async for data in chatgpt.ask(message):
-            out = data['message']
-        return out
+        async with L_chatgpt:
+            if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
+            info('ASK', message)
+            async for data in chatgpt.ask(message):
+                out = data['message']
+            return out
     if bot == 'chatgpt-api':
         chatgpt_api.system_prompt = prompt
         out = await chatgpt_api.ask_async(message)
         return out
     if bot == 'bing':
-        if len(prompt) > 1: message = promptBase + message
-        out = await bing.ask(message)
-        out = out['item']['messages'][-1]['text']
-        return out
+        async with L_bing:
+            if len(prompt) > 1: message = promptBase + message
+            out = await bing.ask(message)
+            out = out['item']['messages'][-1]['text']
+            return out
 
 
 async def ask_stream(event, func, bot, message, prompt=''):
     text = ''
     timeNow = time.time()
     wait_time = config['Chat']['stream_wait_time']
     end_str = tuple(config['Chat']['stream_endStr'])
@@ -127,29 +126,32 @@
             timeNow = time.time()
             info(name + 'time', out)
             await func.send(event, out)
             before = text
             return False
 
     if bot == 'chatgpt':
-        if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
-        async for data in chatgpt.ask(message):
-            text = data['message']
-            isEnd = await stream_process('chatgpt')
-            if isEnd and len(text.replace(before, '').replace(' ', '')) > 1:
-                await stream_process('chatgpt', text)
+        async with L_chatgpt:
+            if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
+            async for data in chatgpt.ask(message):
+                text = data['message']
+                isEnd = await stream_process('chatgpt')
+                if isEnd and len(text.replace(before, '').replace(' ', '')) > 1:
+                    await stream_process('chatgpt', text)
     if bot == 'chatgpt-api':
-        chatgpt_api.system_prompt = prompt
-        async for data in chatgpt_api.ask_stream_async(message):
-            text += data
-            isEnd = await stream_process('chatgpt-api')
-            if isEnd and len(text.replace(before, '').replace(' ', '')) > 1:
-                await stream_process('chatgpt-api', text)
+        async with L_chatgpt_api:
+            chatgpt_api.system_prompt = prompt
+            async for data in chatgpt_api.ask_stream_async(message):
+                text += data
+                isEnd = await stream_process('chatgpt-api')
+                if isEnd and len(text.replace(before, '').replace(' ', '')) > 1:
+                    await stream_process('chatgpt-api', text)
     if bot == 'bing':
-        if len(prompt) > 1: message = promptBase + message
-        async for data in bing.ask_stream(message):
-            isTrue, textdata = data
-            if type(textdata) == str:
-                text = textdata
-                await stream_process('Bing')
-            else:
-                await stream_process('bing', text)
+        async with L_bing:
+            if len(prompt) > 1: message = promptBase + message
+            async for data in bing.ask_stream(message):
+                isTrue, textdata = data
+                if type(textdata) == str:
+                    text = textdata
+                    await stream_process('Bing')
+                else:
+                    await stream_process('bing', text)
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/configspec.ini` & `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/configspec.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,226 +1,230 @@
-00000000: 5b42 6f74 5d0d 0a20 2069 705f 7465 7374  [Bot]..  ip_test
-00000010: 203d 2069 705f 7465 7374 5f73 7769 7463   = ip_test_switc
-00000020: 6828 6465 6661 756c 743d 5472 7565 290d  h(default=True).
-00000030: 0a20 2023 20e5 9ca8 e6a3 80e6 9fa5 e985  .  # ...........
-00000040: 8de7 bdae e697 b6e6 98af e590 a670 696e  .............pin
-00000050: 67e4 b880 e4b8 8b69 7020 20e5 a682 e69e  g......ip  .....
-00000060: 9c69 70e6 b2a1 e69c 89e9 97ae e9a2 98ef  .ip.............
-00000070: bc8c e585 b3e9 97ad 28e8 aebe e7bd aee4  ........(.......
-00000080: b8ba 4661 6c73 6529 e883 bde5 a29e e58a  ..False)........
-00000090: a0e5 90af e58a a8e9 809f e5ba a60d 0a20  ............... 
-000000a0: 2073 7769 7463 6843 6f6e 6669 6745 7661   switchConfigEva
-000000b0: 6c20 3d20 626f 6f6c 6561 6e28 6465 6661  l = boolean(defa
-000000c0: 756c 743d 4661 6c73 6529 0d0a 2020 2320  ult=False)..  # 
-000000d0: 2ae5 8db1 e999 a92a 20e6 98af e590 a620  *......* ...... 
-000000e0: e689 80e6 9c89 e4ba bae9 83bd e58f afe4  ................
-000000f0: bba5 e980 9ae8 bf87 20e6 8c87 e4bb a428  ........ ......(
-00000100: 7377 6974 6368 2920 e79b b4e6 8ea5 e4bf  switch) ........
-00000110: aee6 94b9 e985 8de7 bdae 2042 6f74 20e9  .......... Bot .
-00000120: 858d e7bd aee9 a1b9 e4b8 8be6 8980 e4bb  ................
-00000130: a5e9 a1b9 e79b aee9 99a4 e5a4 960d 0a20  ............... 
-00000140: 206f 776e 6572 203d 2069 6428 6465 6661   owner = id(defa
-00000150: 756c 743d 2727 290d 0a20 2023 20e4 b8bb  ult='')..  # ...
-00000160: e4ba bae7 9a84 2069 640d 0a20 2073 686f  ...... id..  sho
-00000170: 7720 3d20 626f 6f6c 6561 6e28 6465 6661  w = boolean(defa
-00000180: 756c 743d 5472 7565 290d 0a0d 0a5b 4368  ult=True)....[Ch
-00000190: 6174 5d0d 0a20 2070 7265 7365 7473 5f64  at]..  presets_d
-000001a0: 6972 203d 2064 6972 2864 6566 6175 6c74  ir = dir(default
-000001b0: 3d27 2e2f 7072 6573 6574 7327 290d 0a20  ='./presets').. 
-000001c0: 2023 20e9 a284 e8ae bee6 9687 e4bb b6e5   # .............
-000001d0: a4b9 0d0a 2020 7265 6c6f 6164 5f70 7265  ....  reload_pre
-000001e0: 7365 7473 203d 2062 6f6f 6c65 616e 2864  sets = boolean(d
-000001f0: 6566 6175 6c74 3d54 7275 6529 0d0a 2020  efault=True)..  
-00000200: 2320 e698 afe5 90a6 e6af 8fe6 aca1 e987  # ..............
-00000210: 8de5 90af e983 bde9 878d e7bd ae20 e9a2  ............. ..
-00000220: 84e8 aebe 0d0a 2020 7374 7265 616d 5f77  ......  stream_w
-00000230: 6169 745f 7469 6d65 203d 2069 6e74 6567  ait_time = integ
-00000240: 6572 2864 6566 6175 6c74 3d32 2c20 6d69  er(default=2, mi
-00000250: 6e3d 302c 206d 6178 3d32 3029 0d0a 2020  n=0, max=20)..  
-00000260: 2320 e9a2 91e9 8193 e586 8520 e588 86e6  # ......... ....
-00000270: 9da1 e58f 91e9 8081 e997 b4e9 9a94 2028  .............. (
-00000280: e7a7 9229 0d0a 2020 7374 7265 616d 5f65  ...)..  stream_e
-00000290: 6e64 5374 7220 3d20 6c69 7374 2864 6566  ndStr = list(def
-000002a0: 6175 6c74 3d6c 6973 7428 27ef bc9f 272c  ault=list('...',
-000002b0: 27e3 8082 272c 273f 272c 275c 6e27 2929  '...','?','\n'))
-000002c0: 0d0a 2020 2320 e9a2 91e9 8193 e586 8520  ..  # ......... 
-000002d0: e588 86e6 9da1 e58f 91e9 8081 e588 86e5  ................
-000002e0: 89b2 e4be 9de6 8dae 0d0a 2020 6465 6661  ..........  defa
-000002f0: 756c 7441 4920 3d20 6169 2864 6566 6175  ultAI = ai(defau
-00000300: 6c74 3d27 4368 6174 4750 545f 6170 6927  lt='ChatGPT_api'
-00000310: 290d 0a20 2023 20e9 bb98 e8ae a420 4149  )..  # ...... AI
-00000320: 0d0a 2020 7265 706c 7920 3d20 626f 6f6c  ..  reply = bool
-00000330: 6561 6e28 6465 6661 756c 743d 5472 7565  ean(default=True
-00000340: 290d 0a20 2023 20e6 98af e590 a6e5 9b9e  )..  # .........
-00000350: e5a4 8de7 94a8 e688 b720 28e5 a682 e69e  ......... (.....
-00000360: 9ce5 90af e794 a8e5 8886 e6ae b5e5 8f91  ................
-00000370: e980 812c e697 a0e8 aeba e8ae bee7 bdae  ...,............
-00000380: e4b8 8ee5 90a6 2ce9 83bd e4b8 8de6 98af  ......,.........
-00000390: e59b 9ee5 a48d e6b6 88e6 81af 290d 0a20  ............).. 
-000003a0: 2073 7769 7463 6820 3d20 626f 6f6c 6561   switch = boolea
-000003b0: 6e28 6465 6661 756c 743d 5472 7565 290d  n(default=True).
-000003c0: 0a0d 0a5b 436f 6d6d 616e 645d 0d0a 2020  ...[Command]..  
-000003d0: 2320 e6b3 a8e6 848f efbc 8ce5 91bd e4bb  # ..............
-000003e0: a4e5 bc80 e5a4 b4e7 acac e4b8 80e4 b8aa  ................
-000003f0: e5ad 97e7 aca6 e586 b3e5 ae9a e4ba 86e5  ................
-00000400: 91bd e4bb a4e5 898d e7bc 80ef bc8c e4b8  ................
-00000410: 94e6 8980 e69c 89e5 91bd e4bb a4e9 83bd  ................
-00000420: e5bf 85e9 a1bb e4bd bfe7 94a8 e79b b8e5  ................
-00000430: 908c e589 8de7 bc80 0d0a 2020 6269 6e67  ..........  bing
-00000440: 203d 2063 6d64 2864 6566 6175 6c74 3d27   = cmd(default='
-00000450: 2f62 696e 6727 290d 0a20 2063 6861 7420  /bing')..  chat 
-00000460: 3d20 636d 6428 6465 6661 756c 743d 272f  = cmd(default='/
-00000470: 6368 6174 2729 0d0a 2020 7461 6720 3d20  chat')..  tag = 
-00000480: 636d 6428 6465 6661 756c 743d 272f 7461  cmd(default='/ta
-00000490: 6727 290d 0a20 2053 445f 7765 6275 6920  g')..  SD_webui 
-000004a0: 3d20 636d 6428 6465 6661 756c 743d 272f  = cmd(default='/
-000004b0: 6169 2729 0d0a 2020 7377 6974 6368 4149  ai')..  switchAI
-000004c0: 203d 2063 6d64 2864 6566 6175 6c74 3d27   = cmd(default='
-000004d0: 2fe5 8887 e68d a241 4927 290d 0a20 2073  /......AI')..  s
-000004e0: 7769 7463 6820 3d20 636d 6428 6465 6661  witch = cmd(defa
-000004f0: 756c 743d 272f 7377 6974 6368 2729 0d0a  ult='/switch')..
-00000500: 2020 7377 6974 6368 5072 6573 6574 203d    switchPreset =
-00000510: 2063 6d64 2864 6566 6175 6c74 3d27 2fe5   cmd(default='/.
-00000520: 8887 e68d a2e9 a284 e8ae be27 290d 0a0d  ...........')...
-00000530: 0a5b 4149 5d0d 0a20 205b 5b63 6861 7467  .[AI]..  [[chatg
-00000540: 7074 5d5d 0d0a 2020 2020 6163 6365 7373  pt]]..    access
-00000550: 5f74 6f6b 656e 203d 2074 6f6b 656e 2864  _token = token(d
-00000560: 6566 6175 6c74 3d27 2729 0d0a 2020 2020  efault='')..    
-00000570: 2320 e88e b7e5 8f96 3a68 7474 7073 3a2f  # ......:https:/
-00000580: 2f63 6861 742e 6f70 656e 6169 2e63 6f6d  /chat.openai.com
-00000590: 2f61 7069 2f61 7574 682f 7365 7373 696f  /api/auth/sessio
-000005a0: 6e0d 0a20 2020 2070 726f 7879 203d 2070  n..    proxy = p
-000005b0: 726f 7879 2864 6566 6175 6c74 3d27 2729  roxy(default='')
-000005c0: 0d0a 0d0a 2020 5b5b 6368 6174 6770 742d  ....  [[chatgpt-
-000005d0: 6170 695d 5d0d 0a20 2020 2061 7069 5f6b  api]]..    api_k
-000005e0: 6579 203d 2061 7069 6b65 7928 6465 6661  ey = apikey(defa
-000005f0: 756c 743d 2727 290d 0a20 2020 2023 20e8  ult='')..    # .
-00000600: 8eb7 e58f 963a 6874 7470 733a 2f2f 706c  .....:https://pl
-00000610: 6174 666f 726d 2e6f 7065 6e61 692e 636f  atform.openai.co
-00000620: 6d2f 6163 636f 756e 742f 6170 692d 6b65  m/account/api-ke
-00000630: 7973 0d0a 2020 2020 6d6f 6465 6c20 3d20  ys..    model = 
-00000640: 6d6f 6465 6c28 6465 6661 756c 743d 2767  model(default='g
-00000650: 7074 2d33 2e35 2d74 7572 626f 2729 0d0a  pt-3.5-turbo')..
-00000660: 2020 2020 7072 6f78 7920 3d20 7072 6f78      proxy = prox
-00000670: 7928 6465 6661 756c 743d 2727 290d 0a0d  y(default='')...
-00000680: 0a20 205b 5b62 696e 675d 5d0d 0a20 2020  .  [[bing]]..   
-00000690: 2063 6f6f 6b69 6573 5f66 696c 655f 7061   cookies_file_pa
-000006a0: 7468 203d 2066 696c 6528 6465 6661 756c  th = file(defaul
-000006b0: 743d 272e 2f63 6f6f 6b69 6573 2e6a 736f  t='./cookies.jso
-000006c0: 6e27 290d 0a20 2020 2023 20e8 aebe e7bd  n')..    # .....
-000006d0: ae3a 6874 7470 733a 2f2f 6769 7468 7562  .:https://github
-000006e0: 2e63 6f6d 2f74 6878 3131 342f 5344 4750  .com/thx114/SDGP
-000006f0: 542f 7769 6b69 2f62 696e 672d 636f 6f6b  T/wiki/bing-cook
-00000700: 6965 730d 0a20 2020 2070 726f 7879 203d  ies..    proxy =
-00000710: 2070 726f 7879 2864 6566 6175 6c74 3d27   proxy(default='
-00000720: 2729 0d0a 0d0a 5b53 7461 626c 652d 4469  ')....[Stable-Di
-00000730: 6666 7573 696f 6e5d 0d0a 2020 6e65 6761  ffusion]..  nega
-00000740: 7469 7665 5f70 726f 6d70 7420 3d20 7374  tive_prompt = st
-00000750: 7269 6e67 2864 6566 6175 6c74 3d27 2877  ring(default='(w
-00000760: 6f72 7374 2071 7561 6c69 7479 2c20 6c6f  orst quality, lo
-00000770: 7720 7175 616c 6974 793a 312e 3429 2c4e  w quality:1.4),N
-00000780: 5346 572c 7231 3827 290d 0a20 2023 2053  SFW,r18')..  # S
-00000790: 4420 e7bb 98e7 94bb 20e5 8f8d e590 91e6  D ...... .......
-000007a0: 8f90 e7a4 bae8 af8d 0d0a 2020 6170 695f  ..........  api_
-000007b0: 686f 7374 203d 2069 7028 6465 6661 756c  host = ip(defaul
-000007c0: 743d 275e 3132 372e 302e 302e 313a 3738  t='^127.0.0.1:78
-000007d0: 3630 2729 0d0a 2020 2320 5344 20e7 9a84  60')..  # SD ...
-000007e0: 2061 7069 20e5 9cb0 e59d 8020 28e5 9ca8   api ...... (...
-000007f0: 5344 e590 afe5 8aa8 e58f 82e6 95b0 e79b  SD..............
-00000800: b4e6 8ea5 e58a a02d 2d61 7069 2ce5 9cb0  .......--api,...
-00000810: e59d 80e5 b0b1 e698 afe9 bb98 e8ae a4e5  ................
-00000820: 9cb0 e59d 8029 0d0a 2020 7361 7665 5f70  .....)..  save_p
-00000830: 6174 6820 3d20 6469 7228 6465 6661 756c  ath = dir(defaul
-00000840: 743d 272e 2f6f 7574 2729 0d0a 2020 2320  t='./out')..  # 
-00000850: 5344 20e7 949f e688 90e5 9bbe e789 87e5  SD .............
-00000860: ad98 e694 bee4 bd8d e7bd ae20 e5a6 82e6  ........... ....
-00000870: 9e9c e8ae bee7 bdae e4b8 bae7 a9ba efbc  ................
-00000880: 8ce5 8899 e4b8 8de5 ad98 e694 bee5 9bbe  ................
-00000890: e789 870d 0a20 2073 7465 7020 3d20 696e  .....  step = in
-000008a0: 7465 6765 7228 6465 6661 756c 743d 3237  teger(default=27
-000008b0: 290d 0a0d 0a5b 4675 6e63 7469 6f6e 5d0d  )....[Function].
-000008c0: 0a20 2023 e6b3 a8e6 848f 20e7 99bd e590  .  #...... .....
-000008d0: 8de5 8d95 20e5 90af e794 a8e5 8a9f e883  .... ...........
-000008e0: bd20 7377 6974 6368 20e5 85a8 e983 a8e6  . switch .......
-000008f0: b2a1 e586 99e5 ae8c efbc 8ce4 b88d e883  ................
-00000900: bde7 949f e695 880d 0a20 205b 5b47 726f  .........  [[Gro
-00000910: 7570 5d5d 0d0a 2020 2020 6772 6f75 7073  up]]..    groups
-00000920: 203d 206c 6973 7428 6465 6661 756c 743d   = list(default=
-00000930: 6c69 7374 2827 2a27 2929 0d0a 2020 2020  list('*'))..    
-00000940: 2320 e7be a4e8 818a e799 bde5 908d e58d  # ..............
-00000950: 95ef bc8c e8ae bee7 bdae e4b8 ba20 2a2c  ............. *,
-00000960: 20e4 bba3 e8a1 a8e4 b88d e999 90e5 88b6   ...............
-00000970: 0d0a 2020 2020 6675 6e63 7469 6f6e 203d  ..    function =
-00000980: 206c 6973 7428 6465 6661 756c 743d 6c69   list(default=li
-00000990: 7374 2827 6269 6e67 272c 2027 6368 6174  st('bing', 'chat
-000009a0: 272c 2027 7461 6727 2c20 2761 6927 2c20  ', 'tag', 'ai', 
-000009b0: 276d 7367 2729 290d 0a20 2020 2023 20e5  'msg'))..    # .
-000009c0: 90af e794 a8e7 9a84 e58a 9fe8 83bd efbc  ................
-000009d0: 8ce5 908d e7a7 b0e4 bba5 436f 6d6d 616e  ..........Comman
-000009e0: 64e4 b8ad e5b7 a6e4 bea7 e985 8de7 bdae  d...............
-000009f0: e590 8de4 b8ba e587 860d 0a20 2020 2073  ...........    s
-00000a00: 7472 6561 6d20 3d20 626f 6f6c 6561 6e28  tream = boolean(
-00000a10: 6465 6661 756c 743d 4661 6c73 6529 0d0a  default=False)..
-00000a20: 2020 2020 2320 e698 afe5 90a6 e590 afe7      # ..........
-00000a30: 94a8 e588 86e6 aeb5 e58f 91e9 8081 0d0a  ................
-00000a40: 2020 2020 7377 6974 6368 203d 2062 6f6f      switch = boo
-00000a50: 6c65 616e 2864 6566 6175 6c74 3d54 7275  lean(default=Tru
-00000a60: 6529 0d0a 0d0a 2020 5b5b 5072 6976 6174  e)....  [[Privat
-00000a70: 655d 5d0d 0a20 2020 206d 656d 6265 7220  e]]..    member 
-00000a80: 3d20 6c69 7374 2864 6566 6175 6c74 3d6c  = list(default=l
-00000a90: 6973 7428 272a 2729 2920 2320 e7a7 81e8  ist('*')) # ....
-00000aa0: 818a e799 bde5 908d e58d 95ef bc8c e8ae  ................
-00000ab0: bee7 bdae e4b8 ba20 2a2c 20e4 bba3 e8a1  ....... *, .....
-00000ac0: a8e4 b88d e999 90e5 88b6 0d0a 2020 2020  ............    
-00000ad0: 2320 e7a7 81e8 818a e799 bde5 908d e58d  # ..............
-00000ae0: 95ef bc8c e8ae bee7 bdae e4b8 ba20 2a2c  ............. *,
-00000af0: 20e4 bba3 e8a1 a8e4 b88d e999 90e5 88b6   ...............
-00000b00: 0d0a 2020 2020 6675 6e63 7469 6f6e 203d  ..    function =
-00000b10: 206c 6973 7428 6465 6661 756c 743d 6c69   list(default=li
-00000b20: 7374 2827 6269 6e67 272c 2027 6368 6174  st('bing', 'chat
-00000b30: 272c 2027 7461 6727 2c20 2761 6927 2c20  ', 'tag', 'ai', 
-00000b40: 276d 7367 2729 290d 0a20 2020 2023 20e5  'msg'))..    # .
-00000b50: 90af e794 a8e7 9a84 e58a 9fe8 83bd efbc  ................
-00000b60: 8ce5 908d e7a7 b0e4 bba5 436f 6d6d 616e  ..........Comman
-00000b70: 64e4 b8ad e5b7 a6e4 bea7 e985 8de7 bdae  d...............
-00000b80: e590 8de4 b8ba e587 860d 0a20 2020 2073  ...........    s
-00000b90: 7472 6561 6d20 3d20 626f 6f6c 6561 6e28  tream = boolean(
-00000ba0: 6465 6661 756c 743d 4661 6c73 6529 0d0a  default=False)..
-00000bb0: 2020 2020 2320 e698 afe5 90a6 e590 afe7      # ..........
-00000bc0: 94a8 e588 86e6 aeb5 e58f 91e9 8081 0d0a  ................
-00000bd0: 2020 2020 7377 6974 6368 203d 2062 6f6f      switch = boo
-00000be0: 6c65 616e 2864 6566 6175 6c74 3d54 7275  lean(default=Tru
-00000bf0: 6529 0d0a 0d0a 2020 5b5b 4775 696c 645d  e)....  [[Guild]
-00000c00: 5d0d 0a20 2020 2067 7569 6c64 7320 3d20  ]..    guilds = 
-00000c10: 6c69 7374 2864 6566 6175 6c74 3d6c 6973  list(default=lis
-00000c20: 7428 272a 2729 290d 0a20 2020 2023 20e9  t('*'))..    # .
-00000c30: a291 e981 93e7 99bd e590 8de5 8d95 efbc  ................
-00000c40: 8ce8 aebe e7bd aee4 b8ba 202a 2c20 e4bb  .......... *, ..
-00000c50: a3e8 a1a8 e4b8 8de9 9990 e588 b60d 0a20  ............... 
-00000c60: 2020 2066 756e 6374 696f 6e20 3d20 6c69     function = li
-00000c70: 7374 2864 6566 6175 6c74 3d6c 6973 7428  st(default=list(
-00000c80: 2762 696e 6727 2c20 2763 6861 7427 2c20  'bing', 'chat', 
-00000c90: 2774 6167 272c 2027 6169 272c 2027 6d73  'tag', 'ai', 'ms
-00000ca0: 6727 2929 0d0a 2020 2020 2320 e590 afe7  g'))..    # ....
-00000cb0: 94a8 e79a 84e5 8a9f e883 bdef bc8c e590  ................
-00000cc0: 8de7 a7b0 e4bb a543 6f6d 6d61 6e64 e4b8  .......Command..
-00000cd0: ade5 b7a6 e4be a7e9 858d e7bd aee5 908d  ................
-00000ce0: e4b8 bae5 8786 0d0a 2020 2020 7374 7265  ........    stre
-00000cf0: 616d 203d 2062 6f6f 6c65 616e 2864 6566  am = boolean(def
-00000d00: 6175 6c74 3d54 7275 6529 0d0a 2020 2020  ault=True)..    
-00000d10: 2320 e698 afe5 90a6 e590 afe7 94a8 e588  # ..............
-00000d20: 86e6 aeb5 e58f 91e9 8081 0d0a 2020 2020  ............    
-00000d30: 7377 6974 6368 203d 2062 6f6f 6c65 616e  switch = boolean
-00000d40: 2864 6566 6175 6c74 3d54 7275 6529 0d0a  (default=True)..
-00000d50: 0d0a 5b70 7265 7365 745d 0d0a 2020 23e9  ..[preset]..  #.
-00000d60: a284 e8ae bee6 b3a8 e586 8cef bc8c e586  ................
-00000d70: b3e5 ae9a e4ba 86e5 8887 e68d a2e9 a284  ................
-00000d80: e8ae bee6 8c87 e4bb a4e7 9a84 e9a2 84e8  ................
-00000d90: aebe e590 8de7 a7b0 0d0a 2020 7461 6720  ..........  tag 
-00000da0: 3d20 7072 6573 6574 2864 6566 6175 6c74  = preset(default
-00000db0: 3d27 5072 6f6d 7074 4765 6e65 7261 746f  ='PromptGenerato
-00000dc0: 722e 7478 7427 290d 0a0d 0a5b 7275 6e74  r.txt')....[runt
-00000dd0: 696d 655d 0d0a 2020 23e8 bf90 e8a1 8ce6  ime]..  #.......
-00000de0: 97b6 e985 8de7 bdae efbc 8ce9 809a e5b8  ................
-00000df0: b8e4 b88d e99c 80e8 a681 e4bf aee6 94b9  ................
-00000e00: 0d0a 2020 7072 6573 6574 203d 2061 6e79  ..  preset = any
-00000e10: 2864 6566 6175 6c74 3d27 2729 0d0a 0d0a  (default='')....
+00000000: 5b42 6f74 5d0d 0a23 e59c a8e6 a380 e69f  [Bot]..#........
+00000010: a5e9 858d e7bd aee6 97b6 e698 afe5 90a6  ................
+00000020: 7069 6e67 e4b8 80e4 b88b 6970 2020 e5a6  ping......ip  ..
+00000030: 82e6 9e9c 6970 e6b2 a1e6 9c89 e997 aee9  ....ip..........
+00000040: a298 efbc 8ce5 85b3 e997 ad28 e8ae bee7  ...........(....
+00000050: bdae e4b8 ba46 616c 7365 29e8 83bd e5a2  .....False).....
+00000060: 9ee5 8aa0 e590 afe5 8aa8 e980 9fe5 baa6  ................
+00000070: 0d0a 2020 6970 5f74 6573 7420 3d20 6970  ..  ip_test = ip
+00000080: 5f74 6573 745f 7377 6974 6368 2864 6566  _test_switch(def
+00000090: 6175 6c74 3d54 7275 6529 0d0a 232a e58d  ault=True)..#*..
+000000a0: b1e9 99a9 2ae6 98af e590 a620 e689 80e6  ....*...... ....
+000000b0: 9c89 e4ba bae9 83bd e58f afe4 bba5 e980  ................
+000000c0: 9ae8 bf87 20e6 8c87 e4bb a428 7377 6974  .... ......(swit
+000000d0: 6368 2920 e79b b4e6 8ea5 e4bf aee6 94b9  ch) ............
+000000e0: e985 8de7 bdae 202c 426f 7420 e985 8de7  ...... ,Bot ....
+000000f0: bdae e9a1 b9e4 b88b e689 80e6 9c89 e9a1  ................
+00000100: b9e7 9bae e999 a4e5 a496 0d0a 2020 7377  ............  sw
+00000110: 6974 6368 436f 6e66 6967 4576 616c 203d  itchConfigEval =
+00000120: 2062 6f6f 6c65 616e 2864 6566 6175 6c74   boolean(default
+00000130: 3d46 616c 7365 290d 0a23 e4b8 bbe4 baba  =False)..#......
+00000140: e79a 8469 640d 0a20 206f 776e 6572 203d  ...id..  owner =
+00000150: 2069 6428 6465 6661 756c 743d 2727 290d   id(default='').
+00000160: 0a0d 0a0d 0a5b 4368 6174 5d0d 0a23 e9a2  .....[Chat]..#..
+00000170: 84e8 aebe e696 87e4 bbb6 e5a4 b90d 0a20  ............... 
+00000180: 2070 7265 7365 7473 5f64 6972 203d 2064   presets_dir = d
+00000190: 6972 2864 6566 6175 6c74 3d27 2e2f 7072  ir(default='./pr
+000001a0: 6573 6574 7327 290d 0a23 e698 afe5 90a6  esets')..#......
+000001b0: e6af 8fe6 aca1 e987 8de5 90af e983 bde9  ................
+000001c0: 878d e7bd ae20 e9a2 84e8 aebe 0d0a 2020  ..... ........  
+000001d0: 7265 6c6f 6164 5f70 7265 7365 7473 203d  reload_presets =
+000001e0: 2062 6f6f 6c65 616e 2864 6566 6175 6c74   boolean(default
+000001f0: 3d54 7275 6529 0d0a 23e9 a291 e981 93e5  =True)..#.......
+00000200: 8685 e588 86e6 9da1 e58f 91e9 8081 e997  ................
+00000210: b4e9 9a94 2028 e7a7 9229 0d0a 2020 7374  .... (...)..  st
+00000220: 7265 616d 5f77 6169 745f 7469 6d65 203d  ream_wait_time =
+00000230: 2069 6e74 6567 6572 2864 6566 6175 6c74   integer(default
+00000240: 3d32 2c20 6d69 6e3d 302c 206d 6178 3d32  =2, min=0, max=2
+00000250: 3029 0d0a 23e9 a291 e981 93e5 8685 e588  0)..#...........
+00000260: 86e6 9da1 e58f 91e9 8081 e588 86e5 89b2  ................
+00000270: e4be 9de6 8dae 0d0a 2020 7374 7265 616d  ........  stream
+00000280: 5f65 6e64 5374 7220 3d20 6c69 7374 2864  _endStr = list(d
+00000290: 6566 6175 6c74 3d6c 6973 7428 27ef bc9f  efault=list('...
+000002a0: 272c 27e3 8082 272c 273f 272c 275c 6e27  ','...','?','\n'
+000002b0: 2929 0d0a 23e9 bb98 e8ae a441 490d 0a20  ))..#......AI.. 
+000002c0: 2064 6566 6175 6c74 4149 203d 2061 6928   defaultAI = ai(
+000002d0: 6465 6661 756c 743d 2743 6861 7447 5054  default='ChatGPT
+000002e0: 5f61 7069 2729 0d0a 23e6 98af e590 a6e5  _api')..#.......
+000002f0: 9b9e e5a4 8de7 94a8 e688 b728 e5a6 82e6  ...........(....
+00000300: 9e9c e590 afe7 94a8 e588 86e6 aeb5 e58f  ................
+00000310: 91e9 8081 2ce6 97a0 e8ae bae8 aebe e7bd  ....,...........
+00000320: aee4 b88e e590 a62c e983 bde4 b88d e698  .......,........
+00000330: afe5 9b9e e5a4 8de6 b688 e681 af29 0d0a  .............)..
+00000340: 2020 7265 706c 7920 3d20 626f 6f6c 6561    reply = boolea
+00000350: 6e28 6465 6661 756c 743d 5472 7565 290d  n(default=True).
+00000360: 0a23 4368 6174 e5bc 80e5 85b3 0d0a 2020  .#Chat........  
+00000370: 7377 6974 6368 203d 2062 6f6f 6c65 616e  switch = boolean
+00000380: 2864 6566 6175 6c74 3d54 7275 6529 0d0a  (default=True)..
+00000390: 0d0a 5b43 6f6d 6d61 6e64 5d0d 0a20 2023  ..[Command]..  #
+000003a0: 20e6 b3a8 e684 8fef bc8c e591 bde4 bba4   ...............
+000003b0: e5bc 80e5 a4b4 e7ac ace4 b880 e4b8 aae5  ................
+000003c0: ad97 e7ac a6e5 86b3 e5ae 9ae4 ba86 e591  ................
+000003d0: bde4 bba4 e589 8de7 bc80 efbc 8ce4 b894  ................
+000003e0: e689 80e6 9c89 e591 bde4 bba4 e983 bde5  ................
+000003f0: bf85 e9a1 bbe4 bdbf e794 a8e7 9bb8 e590  ................
+00000400: 8ce5 898d e7bc 800d 0a20 2062 696e 6720  .........  bing 
+00000410: 3d20 636d 6428 6465 6661 756c 743d 272f  = cmd(default='/
+00000420: 6269 6e67 2729 0d0a 2020 6368 6174 203d  bing')..  chat =
+00000430: 2063 6d64 2864 6566 6175 6c74 3d27 2f63   cmd(default='/c
+00000440: 6861 7427 290d 0a20 2074 6167 203d 2063  hat')..  tag = c
+00000450: 6d64 2864 6566 6175 6c74 3d27 2f74 6167  md(default='/tag
+00000460: 2729 0d0a 2020 5344 5f77 6562 7569 203d  ')..  SD_webui =
+00000470: 2063 6d64 2864 6566 6175 6c74 3d27 2f61   cmd(default='/a
+00000480: 6927 290d 0a20 2073 7769 7463 6841 4920  i')..  switchAI 
+00000490: 3d20 636d 6428 6465 6661 756c 743d 272f  = cmd(default='/
+000004a0: e588 87e6 8da2 4149 2729 0d0a 2020 7377  ......AI')..  sw
+000004b0: 6974 6368 203d 2063 6d64 2864 6566 6175  itch = cmd(defau
+000004c0: 6c74 3d27 2f73 7769 7463 6827 290d 0a20  lt='/switch').. 
+000004d0: 2073 7769 7463 6850 7265 7365 7420 3d20   switchPreset = 
+000004e0: 636d 6428 6465 6661 756c 743d 272f e588  cmd(default='/..
+000004f0: 87e6 8da2 e9a2 84e8 aebe 2729 0d0a 0d0a  ..........')....
+00000500: 5b41 495d 0d0a 2020 5b5b 6368 6174 6770  [AI]..  [[chatgp
+00000510: 745d 5d0d 0a20 2023 6163 6365 7373 5f74  t]]..  #access_t
+00000520: 6f6b 656e e88e b7e5 8f96 3a68 7474 7073  oken......:https
+00000530: 3a2f 2f63 6861 742e 6f70 656e 6169 2e63  ://chat.openai.c
+00000540: 6f6d 2f61 7069 2f61 7574 682f 7365 7373  om/api/auth/sess
+00000550: 696f 6e0d 0a20 2020 2061 6363 6573 735f  ion..    access_
+00000560: 746f 6b65 6e20 3d20 746f 6b65 6e28 6465  token = token(de
+00000570: 6661 756c 743d 2727 290d 0a20 2023 e4bb  fault='')..  #..
+00000580: a3e7 9086 0d0a 2020 2020 7072 6f78 7920  ......    proxy 
+00000590: 3d20 7072 6f78 7928 6465 6661 756c 743d  = proxy(default=
+000005a0: 2727 290d 0a0d 0a20 205b 5b63 6861 7467  '')....  [[chatg
+000005b0: 7074 2d61 7069 5d5d 0d0a 2020 2361 7069  pt-api]]..  #api
+000005c0: 6b65 79e8 8eb7 e58f 963a 6874 7470 733a  key......:https:
+000005d0: 2f2f 706c 6174 666f 726d 2e6f 7065 6e61  //platform.opena
+000005e0: 692e 636f 6d2f 6163 636f 756e 742f 6170  i.com/account/ap
+000005f0: 692d 6b65 7973 0d0a 2020 2020 6170 695f  i-keys..    api_
+00000600: 6b65 7920 3d20 6170 696b 6579 2864 6566  key = apikey(def
+00000610: 6175 6c74 3d27 2729 0d0a 2020 23e6 a8a1  ault='')..  #...
+00000620: e59e 8b0d 0a20 2020 206d 6f64 656c 203d  .....    model =
+00000630: 206d 6f64 656c 2864 6566 6175 6c74 3d27   model(default='
+00000640: 6770 742d 332e 352d 7475 7262 6f27 290d  gpt-3.5-turbo').
+00000650: 0a20 2023 e4bb a3e7 9086 0d0a 2020 2020  .  #........    
+00000660: 7072 6f78 7920 3d20 7072 6f78 7928 6465  proxy = proxy(de
+00000670: 6661 756c 743d 2727 290d 0a0d 0a20 205b  fault='')....  [
+00000680: 5b62 696e 675d 5d0d 0a20 2023 636f 6f6b  [bing]]..  #cook
+00000690: 6965 73e6 9687 e4bb b6e8 b7af e5be 8420  ies............ 
+000006a0: e8ae bee7 bdae 3a68 7474 7073 3a2f 2f67  ......:https://g
+000006b0: 6974 6875 622e 636f 6d2f 7468 7831 3134  ithub.com/thx114
+000006c0: 2f53 4447 5054 2f77 696b 692f 6269 6e67  /SDGPT/wiki/bing
+000006d0: 2d63 6f6f 6b69 6573 0d0a 2020 2020 636f  -cookies..    co
+000006e0: 6f6b 6965 735f 6669 6c65 5f70 6174 6820  okies_file_path 
+000006f0: 3d20 6669 6c65 2864 6566 6175 6c74 3d27  = file(default='
+00000700: 2e2f 636f 6f6b 6965 732e 6a73 6f6e 2729  ./cookies.json')
+00000710: 0d0a 2020 23e4 bba3 e790 860d 0a20 2020  ..  #........   
+00000720: 2070 726f 7879 203d 2070 726f 7879 2864   proxy = proxy(d
+00000730: 6566 6175 6c74 3d27 2729 0d0a 0d0a 5b53  efault='')....[S
+00000740: 7461 626c 652d 4469 6666 7573 696f 6e5d  table-Diffusion]
+00000750: 0d0a 2020 23e5 8f8d e590 91e6 8f90 e7a4  ..  #...........
+00000760: bae8 af8d 0d0a 2020 6e65 6761 7469 7665  ......  negative
+00000770: 5f70 726f 6d70 7420 3d20 7374 7269 6e67  _prompt = string
+00000780: 2864 6566 6175 6c74 3d27 2877 6f72 7374  (default='(worst
+00000790: 2071 7561 6c69 7479 2c20 6c6f 7720 7175   quality, low qu
+000007a0: 616c 6974 793a 312e 3429 2c4e 5346 572c  ality:1.4),NSFW,
+000007b0: 7231 3827 290d 0a20 2023 5344 e79a 8461  r18')..  #SD...a
+000007c0: 7069 e59c b0e5 9d80 2028 e59c a853 44e5  pi...... (...SD.
+000007d0: 90af e58a a8e5 8f82 e695 b0e7 9bb4 e68e  ................
+000007e0: a5e5 8aa0 2d2d 6170 692c e59c b0e5 9d80  ....--api,......
+000007f0: e5b0 b1e6 98af e9bb 98e8 aea4 e59c b0e5  ................
+00000800: 9d80 290d 0a20 2061 7069 5f68 6f73 7420  ..)..  api_host 
+00000810: 3d20 6970 2864 6566 6175 6c74 3d27 5e31  = ip(default='^1
+00000820: 3237 2e30 2e30 2e31 3a37 3836 3027 290d  27.0.0.1:7860').
+00000830: 0a20 2023 5344 e794 9fe6 8890 e59b bee7  .  #SD..........
+00000840: 8987 e5ad 98e6 94be e4bd 8de7 bdae 20e5  .............. .
+00000850: a682 e69e 9ce8 aebe e7bd aee4 b8ba e7a9  ................
+00000860: baef bc8c e588 99e4 b88d e5ad 98e6 94be  ................
+00000870: e59b bee7 8987 0d0a 2020 7361 7665 5f70  ........  save_p
+00000880: 6174 6820 3d20 6469 7228 6465 6661 756c  ath = dir(defaul
+00000890: 743d 272e 2f6f 7574 2729 0d0a 2020 2353  t='./out')..  #S
+000008a0: 44e7 949f e688 90e5 9bbe e789 8720 e6b8  D............ ..
+000008b0: b2e6 9f93 e6ad a5e6 95b0 0d0a 2020 7374  ............  st
+000008c0: 6570 203d 2069 6e74 6567 6572 2864 6566  ep = integer(def
+000008d0: 6175 6c74 3d32 3729 0d0a 0d0a 5b46 756e  ault=27)....[Fun
+000008e0: 6374 696f 6e5d 0d0a 2020 5b5b 4772 6f75  ction]..  [[Grou
+000008f0: 705d 5d0d 0a20 2023 20e7 bea4 e881 8ae7  p]]..  # .......
+00000900: 99bd e590 8de5 8d95 efbc 8ce8 aebe e7bd  ................
+00000910: aee4 b8ba 202a 2c20 e4bb a3e8 a1a8 e4b8  .... *, ........
+00000920: 8de9 9990 e588 b60d 0a20 2020 2067 726f  .........    gro
+00000930: 7570 7320 3d20 6c69 7374 2864 6566 6175  ups = list(defau
+00000940: 6c74 3d6c 6973 7428 272a 2729 290d 0a20  lt=list('*')).. 
+00000950: 2023 20e5 90af e794 a8e7 9a84 e58a 9fe8   # .............
+00000960: 83bd efbc 8ce5 908d e7a7 b0e4 bba5 436f  ..............Co
+00000970: 6d6d 616e 64e4 b8ad e5b7 a6e4 bea7 e985  mmand...........
+00000980: 8de7 bdae e590 8de4 b8ba e587 8620 286d  ............. (m
+00000990: 7367 20e6 98af 2040 e69c bae5 99a8 e4ba  sg ... @........
+000009a0: ba20 e590 8ee8 818a e5a4 a929 2c2a e4b8  . .........),*..
+000009b0: bae4 b88d e999 90e5 88b6 0d0a 2020 2020  ............    
+000009c0: 6675 6e63 7469 6f6e 203d 206c 6973 7428  function = list(
+000009d0: 6465 6661 756c 743d 6c69 7374 2827 2a27  default=list('*'
+000009e0: 2929 0d0a 2020 2320 e698 afe5 90a6 e590  ))..  # ........
+000009f0: afe7 94a8 e588 86e6 aeb5 e58f 91e9 8081  ................
+00000a00: 0d0a 2020 2020 7374 7265 616d 203d 2062  ..    stream = b
+00000a10: 6f6f 6c65 616e 2864 6566 6175 6c74 3d46  oolean(default=F
+00000a20: 616c 7365 290d 0a20 2023 20e7 bea4 e881  alse)..  # .....
+00000a30: 8ae6 80bb e5bc 80e5 85b3 0d0a 2020 2020  ............    
+00000a40: 7377 6974 6368 203d 2062 6f6f 6c65 616e  switch = boolean
+00000a50: 2864 6566 6175 6c74 3d54 7275 6529 0d0a  (default=True)..
+00000a60: 0d0a 2020 5b5b 5072 6976 6174 655d 5d0d  ..  [[Private]].
+00000a70: 0a20 2023 20e7 a781 e881 8ae7 99bd e590  .  # ...........
+00000a80: 8de5 8d95 efbc 8ce8 aebe e7bd aee4 b8ba  ................
+00000a90: 202a 2c20 e4bb a3e8 a1a8 e4b8 8de9 9990   *, ............
+00000aa0: e588 b60d 0a20 2020 206d 656d 6265 7220  .....    member 
+00000ab0: 3d20 6c69 7374 2864 6566 6175 6c74 3d6c  = list(default=l
+00000ac0: 6973 7428 272a 2729 2920 2320 e7a7 81e8  ist('*')) # ....
+00000ad0: 818a e799 bde5 908d e58d 95ef bc8c e8ae  ................
+00000ae0: bee7 bdae e4b8 ba20 2a2c 20e4 bba3 e8a1  ....... *, .....
+00000af0: a8e4 b88d e999 90e5 88b6 0d0a 2020 2320  ............  # 
+00000b00: e590 afe7 94a8 e79a 84e5 8a9f e883 bdef  ................
+00000b10: bc8c e590 8de7 a7b0 e4bb a543 6f6d 6d61  ...........Comma
+00000b20: 6e64 e4b8 ade5 b7a6 e4be a7e9 858d e7bd  nd..............
+00000b30: aee5 908d e4b8 bae5 8786 2028 6d73 6720  .......... (msg 
+00000b40: e698 af20 40e6 9cba e599 a8e4 baba 20e5  ... @......... .
+00000b50: 908e e881 8ae5 a4a9 292c 2ae4 b8ba e4b8  ........),*.....
+00000b60: 8de9 9990 e588 b60d 0a20 2020 2066 756e  .........    fun
+00000b70: 6374 696f 6e20 3d20 6c69 7374 2864 6566  ction = list(def
+00000b80: 6175 6c74 3d6c 6973 7428 272a 2729 290d  ault=list('*')).
+00000b90: 0a20 2023 20e6 98af e590 a6e5 90af e794  .  # ...........
+00000ba0: a8e5 8886 e6ae b5e5 8f91 e980 810d 0a20  ............... 
+00000bb0: 2020 2073 7472 6561 6d20 3d20 626f 6f6c     stream = bool
+00000bc0: 6561 6e28 6465 6661 756c 743d 4661 6c73  ean(default=Fals
+00000bd0: 6529 0d0a 2020 2320 e7a7 81e8 818a e680  e)..  # ........
+00000be0: bbe5 bc80 e585 b30d 0a20 2020 2073 7769  .........    swi
+00000bf0: 7463 6820 3d20 626f 6f6c 6561 6e28 6465  tch = boolean(de
+00000c00: 6661 756c 743d 5472 7565 290d 0a0d 0a20  fault=True).... 
+00000c10: 205b 5b47 7569 6c64 5d5d 0d0a 2020 2320   [[Guild]]..  # 
+00000c20: e9a2 91e9 8193 e799 bde5 908d e58d 95ef  ................
+00000c30: bc8c e8ae bee7 bdae e4b8 ba20 2a2c 20e4  ........... *, .
+00000c40: bba3 e8a1 a8e4 b88d e999 90e5 88b6 0d0a  ................
+00000c50: 2020 2020 6775 696c 6473 203d 206c 6973      guilds = lis
+00000c60: 7428 6465 6661 756c 743d 6c69 7374 2827  t(default=list('
+00000c70: 2a27 2929 0d0a 2020 2320 e590 afe7 94a8  *'))..  # ......
+00000c80: e79a 84e5 8a9f e883 bdef bc8c e590 8de7  ................
+00000c90: a7b0 e4bb a543 6f6d 6d61 6e64 e4b8 ade5  .....Command....
+00000ca0: b7a6 e4be a7e9 858d e7bd aee5 908d e4b8  ................
+00000cb0: bae5 8786 2028 6d73 6720 e698 af20 40e6  .... (msg ... @.
+00000cc0: 9cba e599 a8e4 baba 20e5 908e e881 8ae5  ........ .......
+00000cd0: a4a9 292c 2ae4 b8ba e4b8 8de9 9990 e588  ..),*...........
+00000ce0: b60d 0a20 2020 2066 756e 6374 696f 6e20  ...    function 
+00000cf0: 3d20 6c69 7374 2864 6566 6175 6c74 3d6c  = list(default=l
+00000d00: 6973 7428 272a 2729 290d 0a20 2023 20e6  ist('*'))..  # .
+00000d10: 98af e590 a6e5 90af e794 a8e5 8886 e6ae  ................
+00000d20: b5e5 8f91 e980 810d 0a20 2020 2073 7472  .........    str
+00000d30: 6561 6d20 3d20 626f 6f6c 6561 6e28 6465  eam = boolean(de
+00000d40: 6661 756c 743d 5472 7565 290d 0a20 2023  fault=True)..  #
+00000d50: 20e9 a291 e981 93e6 80bb e5bc 80e5 85b3   ...............
+00000d60: 0d0a 2020 2020 7377 6974 6368 203d 2062  ..    switch = b
+00000d70: 6f6f 6c65 616e 2864 6566 6175 6c74 3d54  oolean(default=T
+00000d80: 7275 6529 0d0a 0d0a 5b70 7265 7365 745d  rue)....[preset]
+00000d90: 0d0a 2020 23e9 a284 e8ae bee6 b3a8 e586  ..  #...........
+00000da0: 8cef bc8c e586 b3e5 ae9a e4ba 86e5 8887  ................
+00000db0: e68d a2e9 a284 e8ae bee6 8c87 e4bb a4e7  ................
+00000dc0: 9a84 e9a2 84e8 aebe e590 8de7 a7b0 0d0a  ................
+00000dd0: 2020 7461 6720 3d20 7072 6573 6574 2864    tag = preset(d
+00000de0: 6566 6175 6c74 3d27 5072 6f6d 7074 4765  efault='PromptGe
+00000df0: 6e65 7261 746f 722e 7478 7427 290d 0a0d  nerator.txt')...
+00000e00: 0a5b 7275 6e74 696d 655d 0d0a 2020 23e8  .[runtime]..  #.
+00000e10: bf90 e8a1 8ce6 97b6 e985 8de7 bdae efbc  ................
+00000e20: 8ce9 809a e5b8 b8e4 b88d e99c 80e8 a681  ................
+00000e30: e4bf aee6 94b9 0d0a 2020 7072 6573 6574  ........  preset
+00000e40: 203d 2061 6e79 2864 6566 6175 6c74 3d27   = any(default='
+00000e50: 2729 0d0a 0d0a                           ')....
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,9 @@
 def check_id(value):
     return value
 
 def check_any(value):
     return value
 
 def check_preset(value):
-    return value
+    return value
+
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.1/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.1"
+version = "0.2.2"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
```

### Comparing `nonebot_plugin_sdgpt-0.2.1/README.md` & `nonebot_plugin_sdgpt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.1/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

