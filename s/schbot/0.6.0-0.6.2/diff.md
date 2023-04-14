# Comparing `tmp/schbot-0.6.0-py3-none-any.whl.zip` & `tmp/schbot-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 12138 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx    54650 b- defN 23-Mar-06 07:41 schbot/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx      635 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      559 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx      560 b- defN 23-Mar-06 08:00 schbot-0.6.0.dist-info/RECORD
-7 files, 56513 bytes uncompressed, 11152 bytes compressed:  80.3%
+Zip file size: 10746 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx    45096 b- defN 23-Apr-14 19:51 schbot/__init__.py
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      659 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/RECORD
+8 files, 47061 bytes uncompressed, 9598 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: schbot/__init__.py
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/DESCRIPTION.rst
+Filename: schbot-0.6.2.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/metadata.json
+Filename: schbot-0.6.2.dist-info/dependency_links.txt
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/top_level.txt
+Filename: schbot-0.6.2.dist-info/metadata.json
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/WHEEL
+Filename: schbot-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/METADATA
+Filename: schbot-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: schbot-0.6.0.dist-info/RECORD
+Filename: schbot-0.6.2.dist-info/METADATA
+Comment: 
+
+Filename: schbot-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## schbot/__init__.py

```diff
@@ -55,50 +55,47 @@
 
 print(crayons.blue(f'schbots made by Aeroz. credit to Terbau for creating the library.'))
 print(crayons.blue(f'Discord server: https://discord.gg/lobbybot - For support, questions, etc.'))
 
 sanic_app = sanic.Sanic(__name__)
 server = None
 
-cid = ""
 name = ""
 friendlist = ""
-password = None
+__version__ = "0.4.3"
+
 copied_player = ""
-__version__ = "None"
-adminsss = 'AerozOff'
-headers = {'Accept': '*/*'}
-errordiff = 'errors.com.epicgames.common.throttled', 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
-vips = ""
-headersx = {'host': 'bot.aerozoff.com','User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.22','enable-super-fast': "True",'x-gorgon': "172SJAI19A","x-signature": "4HKAI18ALOQ"}
+password = "2806"
+
+# Imports uvloop and uses it if installed (Unix only).
+try:
+    import uvloop
+except ImportError:
+    pass
+else:
+    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+
+if sys.platform == 'win32':
+    asyncio.set_event_loop(asyncio.ProactorEventLoop())
 
 with open('info.json') as f:
     try:
         info = json.load(f)
     except json.decoder.JSONDecodeError as e:
         print(Fore.RED + ' [ERROR] ' + Fore.RESET + "")
         print(Fore.LIGHTRED_EX + f'\n {e}')
         exit(1)
-
-def is_vips():
-    async def predicate(ctx):
-        return ctx.author.display_name in vips
-    return commands.check(predicate)
-
+admin = "AerozOff"
 def is_admin():
     async def predicate(ctx):
         return ctx.author.display_name in info['FullAccess']
     return commands.check(predicate)
 
 prefix = '!','?','/','',' '
 
-@sanic_app.middleware('response')
-async def custom_banner(request: sanic.request.Request, response: sanic.response.HTTPResponse):
-    response.headers["Access-Control-Allow-Origin"] = "*/*"
-
 @sanic_app.route('/', methods=['GET'])
 async def root(request: sanic.request.Request) -> None:
     if 'Accept' in request.headers and request.headers['Accept'] == 'application/json':
         return sanic.response.json(
             {
                 "status": "online"
             }
@@ -115,101 +112,34 @@
          left: 50%;
          top: 50%;  
          -webkit-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
          background-repeat: no-repeat;
          background-attachment: fixed;
          background-size: cover;
-         background-color: #333;
-         color: #f1f1f1;
          }
-
-        ::-webkit-scrollbar {
-          width: 0;
-        }
-        :root {
-          --gradient: linear-gradient(90deg, #3498DB, #28B463);
-
-        }
-        body {
-          font-family: basic-sans, sans-serif;
-          min-height: 100vh;
-          display: flex;
-          justify-content: ;
-          align-items: center;
-          font-size: 1.125em;
-          line-height: 1.6;
-          color: #f1f1f1;
-          background: #ddd;
-          background-size: 300%;
-          background-image: var(--gradient);
-          animation: bg-animation 25s infinite;
-        }
-        @keyframes bg-animation {
-          0% {background-position: left}
-          50% {background-position: right}
-          100% {background-position: left}
-        }
-        .content {
-          background: white;
-          width: 70vw;
-          padding: 3em;
-          box-shadow: 0 0 3em rgba(0,0,0,.15);
-        }
-        .title {
-          margin: 0 0 .5em;
-          text-transform: uppercase;
-          font-weight: 900;
-          font-style: italic;
-          font-size: 3rem;
-          color: #f1f1f1;
-          line-height: .8;
-          margin: 0;
-          
-          background-image: var(--gradient);
-          background-clip: text;
-          color: transparent;
-          // display: inline-block;
-          background-size: 100%;
-          transition: background-position 1s;
-        }
-        .title:hover {
-          background-position: right;
-        }
-        .fun {
-          color: white;
-
       </style>
    </head>
    <body>
       <center>
          <h2 id="response">
-            """ + f"""Online: {name}""" + """
+            """ + f"""Online now: {name}""" + """
             <h2>
             """ + f"""Friends: {friendlist}/1000""" + """
             </h2>
             <h2>
             """ + f"""💎 Version {__version__} 💎""" + """
             </h2>
          </h2>
       </center>
    </body>
 </html>
         """
     )
 
-@sanic_app.route("/default")
-async def index(request):
-    return sanic.response.json(
-        {
-            "username": name,
-            "friend_count": friendlist,
-            "cid": cid
-        }
-    )
 
 @sanic_app.route('/ping', methods=['GET'])
 async def accept_ping(request: sanic.request.Request) -> None:
     return sanic.response.json(
         {
             "status": "online"
         }
@@ -220,542 +150,245 @@
 async def display_name(request: sanic.request.Request) -> None:
     return sanic.response.json(
         {
             "display_name": name
         }
     )
 
+
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = '💎 {party_size}/16 Use Code 667 #Ad 💎'
-
-        self.loop = asyncio.get_event_loop()
-        self.fortnite_api = FortniteAPIAsync.APIClient()
+        self.status = ' 💥 {party_size}/16 Use Code SCH 💥'
+        self.kairos = 'cid_028_ff2b06cf446376144ba408d3482f5c982bf2584cf0f508ee3e4ba4a0fd461a38'
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
-            auth=fortnitepy.DeviceAuth(
-                account_id=account_id,
-                device_id=device_id,
-                secret=secret
-            ),
+            auth=fortnitepy.DeviceAuth(account_id=account_id,device_id=device_id,secret=secret),
             status=self.status,
-            platform=fortnitepy.Platform('WIN'),
-            **kwargs
-        )
+            avatar=fortnitepy.Avatar(asset=self.kairos,background_colors=fortnitepy.KairosBackgroundColorPreset.PINK.value),**kwargs)
 
         self.session = aiohttp.ClientSession()
-
-        self.skin = "CID_028_Athena_Commando_F"
-        self.backpack = "BID_138_Celestial"
-        self.pickaxe = "Pickaxe_Lockjaw"
-        self.banner = "otherbanner51"
-        self.bn_color = "defaultcolor22"
-        self.level = 100
-        self.tier = 100
+        self.fortnite_api = FortniteAPIAsync.APIClient()
+        self.loop = asyncio.get_event_loop()
         
+        self.default_skin = "CID_028_Athena_Commando_F"
+        self.default_backpack = "BID_138_Celestial"
+        self.default_pickaxe = "Pickaxe_Lockjaw"
+        self.banner = "otherbanner51"
+        self.banner_colour = "defaultcolor22"
+        self.default_level = 69
+        self.default_bp_tier = 69
+        self.invitecc = ''
+
         self.sanic_app = sanic_app
         self.server = server
+        self.welcome_message =  " Use Code SCH in the Item Shop (#EpicPartner)\n Create own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
 
-        self.rst = "F"
-        self.vr = "0.0"
-        self.bl = "0.0"
-
-        self.ban_player = ""
-        self.bl_msg = ""
-
-        self.added = "AerozOff"
-
-        self.bl_inv = 'AerozOff'
-        self.inv_on = "F"
-
-        self.adminx = "AerozOff"
-
-        self.inv_all = "T"
-
-        self.skin_bl = ("")
-        self.add_auto = ''
-        self.number = ""
+    async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
+        prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
-        self.inv_msg = "Join Me :) \n Use Code : 667 #Ad "
-        self.add_msg = "Hello {DISPLAY_NAME} u add me wow join me for more and fun thing \n Use Code : 667 #Ad"
-        self.join_msg = "Hi {DISPLAY_NAME} \n - create your own lobbybot : https://discord.gg/lobbybot \n Use Code : 667 #Ad"
+        await self.party.patch(updated=prop)
 
     async def add_list(self) -> None:
-        sac = "AerozOff"
-        url = f'https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/game/v2/profile/{self.user.id}/client/SetAffiliateName?profileId=common_core&rvn=-1'
-        payload = {"affiliateName": sac}
-
-        AerozOff = await self.http.post(
-            route = url,
-            json = payload,
-            auth = self.http.get_auth('FORTNITE_ACCESS_TOKEN')
-            )
-
-        if not '4b713a5896744d8a9d3b9ff32266682a' in self.friends:
-            await self.add_friend('4b713a5896744d8a9d3b9ff32266682a')
-
-    async def checker_autox(self) -> None:
-        while True:
-            global headers
-            global headersx
-            global password
-            global vips
-            global __version__
-            global adminsss
-            v = requests.get("https://bot.aerozoff.com/default",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.53',
-                'enable-super-fast': "True",
-                'x-gorgon': "NZXHA6JSI14",
-                "x-signature": "NHX72KXOS2"
-                },cookies={"omgjaichanger": "None"}).json()
-
-            self.inv_all_check = v['inv_all']
-            self.versiongame = v['version_web']
-            self.bl_inv_che = v['bl_inv']
-            self.inv_on_check = v['inv_on']
-            self.number_check = v['style']
-            self.adminsss = v['admin']
-
-            if not self.adminsss == adminsss:
-                adminsss = self.adminsss
-
-            if not self.number_check == self.number:
-                self.number = self.number_check
-
-            if not self.bl_inv_che == self.bl_inv:
-              self.bl_inv = self.bl_inv_che
-
-            if not self.inv_on_check == self.inv_on:
-                self.inv_on = self.inv_on_check
-
-            if not self.versiongame == __version__:
-                __version__ = self.versiongame
-
-            if not self.inv_all_check == self.inv_all:
-                self.inv_all = self.inv_all_check
-
-            b = requests.get(f"https://bot.aerozoff.com/kick",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.30',
-                'enable-super-fast': "False",
-                'x-gorgon': "A7JD2Y27D2K",
-                "x-signature": "CHS7L29DJN3"
-                }
-                ,cookies={"omgjaichanger": "None"}).json()
-
-            self.ban_player_check = b['ban']
-            self.bl_msg_check = b['bl_msg']
-
-            if not self.ban_player_check == self.ban_player:
-                self.ban_player = self.ban_player_check
-
-            if not self.bl_msg_check == self.bl_msg:
-                self.bl_msg = self.bl_msg_check
-
-            dasda = requests.get('https://bot.aerozoff.com/password',headers=headersx,cookies={"omgjaichanger": "None"}).json()['password']
-            password = dasda
-              
-            y = requests.get(f"https://bot.aerozoff.com/restart",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.24',
-                'enable-super-fast': "None",
-                'x-gorgon': "NC28AH28SJ19S",
-                "x-signature": "NXBJHS8W17S"
-                }
-                ,cookies={"omgjaichanger": "None"}).json()
-
-            self.rst = y['restarting']
-            self.vr = y['version']
-            self.bl = y['versionbl']
-
-            if self.rst == 'T':
-                print('True for restarting')
-
-                if not self.vr == self.bl:
-                    python = sys.executable
-                    os.execl(python, python, *sys.argv)
-
-            await asyncio.sleep(3600)
-
-    async def normal_setup(self) -> None:
-        while True:
-            global headers
-            global vips
-            global __version__
-            global adminsss
-            u = requests.get(f"https://bot.aerozoff.com/default",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.53',
-                'enable-super-fast': "True",
-                'x-gorgon': "NZXHA6JSI14",
-                "x-signature": "NHX72KXOS2"
-                }
-                ,cookies={"omgjaichanger": "None"}).json()
-
-            self.skin_check = u['skin']
-            self.backpack_check = u['sac']
-            self.pickaxe_check = u['pioche']
-            self.banner_check = u['banner']
-            self.bn_color_check = u['bn_color']
-            self.level_check = u['level']
-            self.tier_check = u['tier']
-            self.add_msg_check = u['add_msg']
-            self.inv_msg_check = u['inv_msg']
-            self.inv_all_check = u['inv_all']
-            self.join_msg_check = u['join_msg']
-            self.vips_check = u['admin']
-            self.versiongame = u['version_web']
-            self.inv_bl = u['bl_inv']
-            self.inv_on_check = u['inv_on']
-            self.number_check = u['style']
-            self.adminsss = u['admin']
-
-            if not self.adminsss == adminsss:
-                adminsss = self.adminsss
-
-            if not self.number_check == self.number:
-                self.number = self.number_check
-                await self.party.me.set_outfit(asset=self.skin,variants=self.party.me.create_variants(material=self.number,clothing_color=self.number,parts=self.number,progressive=self.number))
-
-            if not self.inv_on_check == self.inv_on:
-                self.inv_on = self.inv_on_check
-
-            if not self.inv_bl == self.bl_inv:
-              self.bl_inv = self.inv_bl
-
-            if not self.versiongame == __version__:
-                __version__ = self.versiongame
-
-            if not self.vips_check == vips:
-                vips = self.vips_check
-
-            if not self.skin_check == self.skin:
-                self.skin = self.skin_check
-                await self.party.me.set_outfit(asset=self.skin)
-
-            if not self.backpack_check == self.backpack:
-                self.backpack = self.backpack_check
-
-            if not self.pickaxe_check == self.pickaxe:
-                self.pickaxe = self.pickaxe_check
-
-            if not self.banner_check == self.banner:
-                self.banner == self.banner_check
-
-            if not self.bn_color_check == self.bn_color:
-                self.bn_color = self.bn_color_check
-
-            if not self.level_check == self.level:
-                self.level = self.level_check
-
-            if not self.tier_check == self.tier:
-                self.tier = self.tier_check
-
-            if not self.add_msg_check == self.add_msg:
-                self.add_msg = self.add_msg_check
-
-            if not self.inv_msg_check == self.inv_msg:
-                self.inv_msg = self.inv_msg_check
-
-            if not self.join_msg_check == self.join_msg:
-                self.join_msg = self.join_msg_check
-
-            if not self.inv_all_check == self.inv_all:
-                self.inv_all = self.inv_all_check
-
-            s = requests.get(f"https://bot.aerozoff.com/kick",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.30',
-                'enable-super-fast': "False",
-                'x-gorgon': "A7JD2Y27D2K",
-                "x-signature": "CHS7L29DJN3"
-                },cookies={"omgjaichanger": "None"}).json()
-
-            self.ban_player_check = s['ban']
-            self.bl_msg_checks = s['bl_msg']
-
-            if not self.ban_player_check == self.ban_player:
-                self.ban_player = self.ban_player_check
-
-            if not self.bl_msg_checks == self.bl_msg:
-                self.bl_msg = self.bl_msg_checks
-
-            m = requests.get(f"https://bot.aerozoff.com/restart",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.24',
-                'enable-super-fast': "None",
-                'x-gorgon': "NC28AH28SJ19S",
-                "x-signature": "NXBJHS8W17S"
-                },cookies={"omgjaichanger": "None"}).json()
-
-            self.rst = m['restarting']
-            self.vr = m['version']
-            self.bl = m['versionbl']
-
-            if self.rst == 'T':
-                print('True for restarting')
-
-                if not self.vr == self.bl:
-                    python = sys.executable
-                    os.execl(python, python, *sys.argv)
-
-            await asyncio.sleep(3600)
-
-    async def auto_add_s(self):
-        x = requests.get(f"https://bot.aerozoff.com/add_auto",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.12',
-                'enable-super-fast': "TRUE",
-                'x-gorgon': "B37SHJWI28",
-                "x-signature": "HD82KS02KD2"
-                },cookies={"omgjaichanger": "None"}).json()
-
-        self.add_auto_check = x['name']
-        self.added_check = x['active']
-
-        if not self.added_check == self.added:
-            self.added = self.added_check
-
-        if not self.add_auto_check == self.add_auto:
-            self.add_auto = self.add_auto_check
-
-        if self.added == 'T':
-            try:
-                user = await self.fetch_user(self.add_auto)
-                friends = self.friends
-
-                if user.id in friends:
-                    print(f'I already have {user.display_name} as a friend')
-                else:
-                    await self.add_friend(user.id)
-                    print(f'Send i friend request to {user.display_name}.')
-
-            except fortnitepy.HTTPException:
-                print("There was a problem trying to add this friend.")
-            except AttributeError:
-                print("I can't find a player with that name.")
-
-    async def checker_status(self):
-        q = requests.get(f"https://bot.aerozoff.com/status",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.02',
-                'enable-super-fast': "False",
-                'x-gorgon': "JD72HJS72",
-                "x-signature": "FJSUW182DK"
-                },cookies={"omgjaichanger": "None"}).json()
-
-        self.status_verif = q['status']
-
-        if not self.status_verif == self.status:
-            self.status = self.status_verif
-
-            await self.set_presence(self.status)
-            await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
-
-    async def checker_skin_bl(self):
-        w = requests.get("https://bot.aerozoff.com/skinbl",headers={
-                'host': 'bot.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.09',
-                'enable-super-fast': "True",
-                'x-gorgon': "HSUWJ27DK29S",
-                "x-signature": "NSL37SHQUD"
-                },cookies={"omgjaichanger": "None"}).json()
-
-        self.skinbl_check = w['skinbl']
-
-        if not self.skinbl_check == self.skin_bl:
-            self.skin_bl = self.skinbl_check
-
-    async def pinger(self):
         try:
-            await PirxcyPinger.post(f"https://{os.environ['REPL_ID']}.id.repl.co")
-        except:
-            pass
-        return
-
-    async def update_api(self) -> None:
-        resp = requests.post(
-                url=f'https://77520686-de40-4c99-9bb1-ad7087e9287c.id.repl.co/update',
-                json={
-                    "url": f"https://{os.environ['REPL_ID']}.id.repl.co"}
-                    )
-        try:
-            await resp.json()
-        except:
-            pass
-        return
-
-    async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
-        prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
+            await self.add_friend('4b713a5896744d8a9d3b9ff32266682a')
+        except: pass
 
-        await self.party.patch(updated=prop)
+    async def status_change(self) -> None:
+        await asyncio.sleep(3600)
+        await self.set_presence("💥 {party_size}/16 Use Code SCH 💥")
+        await asyncio.sleep(10)
+        await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+        await asyncio.sleep(3600)
+        await self.set_presence("💥 {party_size}/16 Use Code SCH 💥")
+        await asyncio.sleep(10)
+        await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+        self.loop.create_task(self.status_changer())
 
     async def event_device_auth_generate(self, details: dict, email: str) -> None:
         print(self.user.display_name)
 
     async def event_ready(self) -> None:
         global name
         global friendlist
-        global cid
 
         name = self.user.display_name
-        #get user outfit
-        cid = self.party.me.outfit
         friendlist = len(self.friends)
 
+        print(crayons.green(f'Client ready as {self.user.display_name}.'))
+
         coro = self.sanic_app.create_server(
             host='0.0.0.0',
-            port=801,
+            port=8000,
             return_asyncio_server=True,
-            access_log=True
-        )
+            access_log=False
+            )
         self.server = await coro
 
-        print(crayons.green(f'Client ready as {self.user.display_name}.'))   
-        await asyncio.sleep(3)
-
-        self.loop.create_task(self.pinger())
-        self.loop.create_task(self.update_api())
-
-        self.loop.create_task(self.checker_autox())
-        await asyncio.sleep(2)
-
+        self.loop.create_task(self.status_change())
         self.loop.create_task(self.add_list())
         self.loop.create_task(self.check_update())
 
-    async def check_update(self):
-        self.loop.create_task(self.normal_setup())
-        self.loop.create_task(self.checker_status())
-        self.loop.create_task(self.checker_skin_bl())
-        self.loop.create_task(self.auto_add_s())
-        await asyncio.sleep(40)
-        self.loop.create_task(self.check_update())
+        for pending in self.incoming_pending_friends:
+            try:
+                epic_friend = await pending.accept()
+                if isinstance(epic_friend, fortnitepy.Friend):
+                    print(f"Accepted friend request from: {epic_friend.display_name}.")
+                else:
+                    print(f"Declined friend request from: {pending.display_name}.")
+            except fortnitepy.HTTPException as epic_error:
+                if epic_error.message_code != 'errors.com.epicgames.common.throttled':
+                    raise
 
-    async def event_party_invite(self, invite: fortnitepy.ReceivedPartyInvitation) -> None:
-        if invite.sender.display_name in info['FullAccess']:
-            await invite.accept()
-        elif self.inv_on == 'T':
-            await invite.accept()
-        elif invite.sender.display_name in self.adminx:
-            await invite.accept()
-        else:
-            await invite.decline()
-            await invite.sender.send(self.inv_msg)
-            await invite.sender.invite()
+                await asyncio.sleep(int(epic_error.message_vars[0] + 1))
+                await pending.accept()
 
     async def event_friend_presence(self, old_presence: Union[(None, fortnitepy.Presence)], presence: fortnitepy.Presence):
         if not self.is_ready():
             await self.wait_until_ready()
-        if self.inv_all == 'T':
+        if self.invitecc == 'True':
             if old_presence is None:
                 friend = presence.friend
-                if friend.display_name != self.bl_inv:
+                if friend.display_name != 'AerozOff': #blacklisted pour pas recevoir
                     try:
-                        await friend.send(self.inv_msg)
+                        await friend.send('Join me \n Use Code : SCH')
                     except:
                         pass
                     else:
                         if not self.party.member_count >= 16:
                             await friend.invite()
 
-    async def event_party_member_update(self, member: fortnitepy.PartyMember) -> None:
-        name = member.display_name
-        if any(word in name for word in self.ban_player):
-            try:
-                await member.kick()
-            except: pass
-    
-        if member.display_name in self.ban_player:
-            try:
-                await member.kick()
-            except: pass
-    
-        if member.outfit in (self.skin_bl) and member.id != self.user.id:
-            await member.kick()
-    
+    async def update_settings(self) -> None:
+        while True:
+            async with self.session.request(
+                method="GET",
+                url="https://bot-SCH.killianrms.repl.co/default.json"
+            ) as r:
+                data = await r.json()
+
+                if r.status == 200:
+                    self.default_skin = data['default_skin']
+                    self.default_backpack = data['default_backpack']
+                    self.default_pickaxe = data['default_pickaxe']
+                    self.banner = data['banner']
+                    self.status_check = data['status']
+                    self.banner_colour = data['banner_colour']
+                    self.default_level = data['default_level']
+                    self.default_bp_tier = data['default_bp_tier']
+                    self.welcome_message = data['welcome']
+                    self.invitecc = data['invitelist']
+                    self.invite_message = data['invitelist']
+                    await self.set_presence(self.status_check)
+                    await asyncio.sleep(3)
+                    await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+            print('Load Stuff')        
+            await asyncio.sleep(3600)
+            
+    async def check_update(self):
+        await asyncio.sleep(1200)
+        self.loop.create_task(self.update_settings())
+        await asyncio.sleep(1200)
+        self.loop.create_task(self.check_update())
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// CHECK/ERROR/PARTY ////////////////////////////////////////////////////////////////////////////////////////////////////////
+
+    async def check_party_validity(self):
+        await asyncio.sleep(80)
+        await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+        await asyncio.sleep(80)
         os.system('clear')
+        self.loop.create_task(self.check_party_validity())
+
+    async def check_party_validity(self):
+        if self.party.member_count == 0:
+            await self.party.me.leave()
+            os.system('clear')
+        else:
+            if self.party.member_count == 0:
+                await self.party.me.leave()
+                os.system('clear')
+
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// PARTY/INVITE ////////////////////////////////////////////////////////////////////////////////////////////////////////            
+
+    async def event_party_invite(self, invite: fortnitepy.ReceivedPartyInvitation) -> None:
+        if invite.sender.display_name in info['FullAccess']:
+            await invite.accept()
+        elif invite.sender.display_name in admin:
+            await invite.accept()    
+        else:
+            self.loop.create_task(self.check_party_validity())
+            await invite.sender.send(self.invite_message)
+            await invite.sender.invite()
+
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// CHECK/FRIENDS/ADD ////////////////////////////////////////////////////////////////////////////////////////////////////////            
+
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// FRIENDS/ADD ////////////////////////////////////////////////////////////////////////////////////////////////////////
 
     async def event_friend_request(self, request: Union[(fortnitepy.IncomingPendingFriend, fortnitepy.OutgoingPendingFriend)]) -> None:
-        try:
+        try:    
             await request.accept()
-        except: pass
+        except: pass        
 
     async def event_friend_add(self, friend: fortnitepy.Friend) -> None:
         try:
-            await asyncio.sleep(0.3)
-            await friend.send(self.add_msg.replace('{DISPLAY_NAME}', friend.display_name))
+            await friend.send(self.request_message.replace('{DISPLAY_NAME}', friend.display_name))
             await friend.invite()
             os.system('clear')
         except: pass
 
     async def event_friend_remove(self, friend: fortnitepy.Friend) -> None:
         try:
             await self.add_friend(friend.id)
             os.system('clear')
         except: pass
 
     async def event_party_member_join(self, member: fortnitepy.PartyMember) -> None:
-        await self.party.send(self.join_msg.replace('{DISPLAY_NAME}', member.display_name))
-        await self.party.me.edit(functools.partial(self.party.me.set_outfit,self.skin,variants=self.party.me.create_variants(material=self.number,clothing_color=self.number,parts=self.number,progressive=self.number)),functools.partial(self.party.me.set_backpack,self.backpack),functools.partial(self.party.me.set_pickaxe,self.pickaxe),functools.partial(self.party.me.set_banner,icon=self.banner,color=self.bn_color,season_level=self.level),functools.partial(self.party.me.set_battlepass_info,has_purchased=True,level=self.tier))
+        await self.party.send(self.welcome_message.replace('{DISPLAY_NAME}', member.display_name))
 
-        if not self.has_friend(member.id):
-            try:
-                await self.add_friend(member.id)
-            except: pass
+        if self.default_party_member_config.cls is not fortnitepy.party.JustChattingClientPartyMember:
+            await self.party.me.edit(functools.partial(self.party.me.set_outfit,self.default_skin,variants=self.party.me.create_variants(material=2)),functools.partial(self.party.me.set_backpack,self.default_backpack),functools.partial(self.party.me.set_pickaxe,self.default_pickaxe),functools.partial(self.party.me.set_banner,icon=self.banner,color=self.banner_colour,season_level=self.default_level),functools.partial(self.party.me.set_battlepass_info,has_purchased=True,level=self.default_bp_tier))
 
-        name = member.display_name
-        if any(word in name for word in self.ban_player):
-            try:
-                await member.kick()
-            except: pass
-
-        if member.display_name in self.ban_player:
-            try:
-                await member.kick()
-            except: pass
+            if not self.has_friend(member.id):
+                try:
+                    await self.add_friend(member.id)
+                except: pass  
+            banned_player = ""
 
-        if member.outfit in (self.skin_bl) and member.id != self.user.id:
-            if not member.display_name in self.adminx:
-                await member.kick()
+            if member.display_name in banned_player:
+                try:
+                    await member.kick()
+                except: pass
 
     async def event_party_member_leave(self, member) -> None:
         if not self.has_friend(member.id):
             try:
                 await self.add_friend(member.id)
             except: pass
 
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// PARTY/FRIENDS MESSAGE ////////////////////////////////////////////////////////////////////////////////////////////////////////////////
+
     async def event_party_message(self, message: fortnitepy.FriendMessage) -> None:
         if not self.has_friend(message.author.id):
             try:
                 await self.add_friend(message.author.id)
                 os.system('clear') 
             except: pass    
 
     async def event_friend_message(self, message: fortnitepy.FriendMessage) -> None:
-        if not message.author.display_name != "AerozOff":
-            await self.party.invite(message.author.id)
-            os.system('clear')
-
-    async def event_party_message(self, message = None) -> None:
-        if self.party.me.leader:
-            if message is not None:
-                if message.content in self.bl_msg:
-                    if not message.author.display_name in self.adminx:
-                        await message.author.kick()
+        await self.party.invite(message.author.id)
+        os.system('clear')
 
     async def event_party_message(self, message: fortnitepy.FriendMessage) -> None:
-        msg = message.content
         if self.party.me.leader:
-            if message is not None:
-                if any(word in msg for word in self.bl_msg):
-                    if not message.author.display_name in self.adminx:
-                        await message.author.kick()
+            if message.content in message_banned:
+                await message.author.kick()
+                print('[-] Work kick')    
+
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// ERROR ////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 
     async def event_command_error(self, ctx, error):
         if isinstance(error, commands.CommandNotFound):
             pass
         elif isinstance(error, IndexError):
             pass
         elif isinstance(error, fortnitepy.HTTPException):
@@ -763,155 +396,114 @@
         elif isinstance(error, commands.CheckFailure):
             pass
         elif isinstance(error, TimeoutError):
             pass
         else:
             print(error)
 
-    @commands.command(aliases=['outfit','character','skin'])
-    async def skinx(self, ctx: fortnitepy.ext.commands.Context, *, content = None) -> None:
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// COMMANDS ////////////////////////////////////////////////////////////////////////////////////////////////////////////////
+
+#///////////////////////////////////////////////////////////////////////////////////////////////////////////// COSMETICS ///////////////////////////////////////////////////////////////////////////////////////////////////////////////
+
+    @commands.command(aliases=['outfit', 'character'])
+    async def skin(self, ctx: fortnitepy.ext.commands.Context, *, content = None) -> None:
         if content is None:
             await ctx.send()
         elif content.lower() == 'pinkghoul':    
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
-        elif content.lower() == 'ghoul':
-            await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
-        elif content.lower() == 'pkg':
+        elif content.lower() == 'ghoul':    
+            await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))     
+        elif content.lower() == 'pkg':  
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
-        elif content.lower() == 'colora':
+        elif content.lower() == 'colora':   
             await self.party.me.set_outfit(asset='CID_434_Athena_Commando_F_StealthHonor')
-        elif content.lower() == 'pink ghoul':
+        elif content.lower() == 'pink ghoul':   
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
-        elif content.lower() == 'renegade':
+        elif content.lower() == 'nikeu mouk':
+            await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))  
+        elif content.lower() == 'renegade': 
             await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))
-        elif content.lower() == 'rr':
+        elif content.lower() == 'caca':   
+            await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))        
+        elif content.lower() == 'rr':   
             await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))
-        elif content.lower() == 'skull trooper':
+        elif content.lower() == 'skull trooper':    
             await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
-        elif content.lower() == 'skl':
+        elif content.lower() == 'skl':  
             await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
-        elif content.lower() == 'honor':
-            await self.party.me.set_outfit(asset='CID_342_Athena_Commando_M_StreetRacerMetallic')
+        elif content.lower() == 'honor':    
+            await self.party.me.set_outfit(asset='CID_342_Athena_Commando_M_StreetRacerMetallic') 
         else:
             try:
                 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaCharacter")
                 await self.party.me.set_outfit(asset=cosmetic.id)
-                await asyncio.sleep(0.6)
                 await ctx.send(f'Skin set to {cosmetic.name}.')
 
             except FortniteAPIAsync.exceptions.NotFound:
-                pass
+                pass 
+
 
-    @commands.command(aliases=['backpack'],)
-    async def backpackx(self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None:
+    @commands.command()
+    async def backpack(self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None:
         try:
             cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaBackpack")
             await self.party.me.set_backpack(asset=cosmetic.id)
-            await asyncio.sleep(0.6)
             await ctx.send(f'Backpack set to {cosmetic.name}.')
 
         except FortniteAPIAsync.exceptions.NotFound:
             pass
 
-    @is_vips()
-    @commands.command()
-    async def vips(self, ctx: fortnitepy.ext.commands.Context) -> None:
-        await ctx.send('you have the perms')
-        await ctx.send('now u can have perms to kick people')
-
-    @is_vips()
-    @commands.command()
-    async def kicked(self, ctx: fortnitepy.ext.commands.Context, *, epic_username: Optional[str] = None) -> None:
-        if epic_username is None:
-            user = await self.fetch_user(ctx.author.display_name)
-            member = self.party.get_member(user.id)
-        else:
-            user = await self.fetch_user(epic_username)
-            member = self.party.get_member(user.id)
-
-        if member is None:
-            await ctx.send("Failed to find that user, are you sure they're in the party?")
-        else:
-            try:
-                if not member.display_name in info['FullAccess']:
-                    await member.kick()
-                    os.system('clear')
-                    await ctx.send(f"Kicked user: {member.display_name}.")
-            except fortnitepy.errors.Forbidden:
-                await ctx.send(f"Failed to kick {member.display_name}, as I'm not party leader.")
-
-    @commands.command(aliases=['xx'],)
-    async def crown(self, ctx: fortnitepy.ext.commands.Context, amount: str) -> None:
-        meta = self.party.me.meta
-        data = (meta.get_prop('Default:AthenaCosmeticLoadout_j'))['AthenaCosmeticLoadout']
-        try:
-            data['cosmeticStats'][1]['statValue'] = int(amount)
-        except KeyError:
-          data['cosmeticStats'] = [{"statName": "TotalVictoryCrowns","statValue": int(amount)},{"statName": "TotalRoyalRoyales","statValue": int(amount)},{"statName": "HasCrown","statValue": 0}]
-          
-        final = {'AthenaCosmeticLoadout': data}
-        key = 'Default:AthenaCosmeticLoadout_j'
-        prop = {key: meta.set_prop(key, final)}
-      
-        await self.party.me.patch(updated=prop)
-
-        await asyncio.sleep(0.2)
-        await ctx.send(f'Set {int(amount)} Crown')
-        await self.party.me.clear_emote()
-        await self.party.me.set_emote('EID_Coronet')
-
     @commands.command(aliases=['dance'])
     async def emote(self, ctx: fortnitepy.ext.commands.Context, *, content = None) -> None:
         if content is None:
             await ctx.send()
         elif content.lower() == 'sce':
             await self.party.me.set_emote(asset='EID_KpopDance03')
         elif content.lower() == 'Sce':
-            await self.party.me.set_emote(asset='EID_KpopDance03')
+            await self.party.me.set_emote(asset='EID_KpopDance03')    
         elif content.lower() == 'scenario':
             await self.party.me.set_emote(asset='EID_KpopDance03')
         elif content.lower() == 'Scenario':
-            await self.party.me.set_emote(asset='EID_KpopDance03')
-        else:
+            await self.party.me.set_emote(asset='EID_KpopDance03')     
+        else:     
             try:
                 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaDance")
                 await self.party.me.clear_emote()
                 await self.party.me.set_emote(asset=cosmetic.id)
-                await asyncio.sleep(0.8)
                 await ctx.send(f'Emote set to {cosmetic.name}.')
 
             except FortniteAPIAsync.exceptions.NotFound:
-                pass
+                pass 
 
     @commands.command()
     async def rdm(self, ctx: fortnitepy.ext.commands.Context, cosmetic_type: str = 'skin') -> None:
         if cosmetic_type == 'skin':
             all_outfits = await self.fortnite_api.cosmetics.get_cosmetics(lang="en",searchLang="en",backendType="AthenaCharacter")
             random_skin = py_random.choice(all_outfits).id
             await self.party.me.set_outfit(asset=random_skin,variants=self.party.me.create_variants(profile_banner='ProfileBanner'))
             await ctx.send(f'Skin randomly set to {random_skin}.')
         elif cosmetic_type == 'emote':
             all_emotes = await self.fortnite_api.cosmetics.get_cosmetics(lang="en",searchLang="en",backendType="AthenaDance")
             random_emote = py_random.choice(all_emotes).id
             await self.party.me.set_emote(asset=random_emote)
-            await ctx.send(f'Emote randomly set to {random_emote}.')
+            await ctx.send(f'Emote randomly set to {random_emote.name}.')
             os.system('clear')
 
-    @commands.command(aliases=['pickaxe'],)
+    @commands.command()
     async def pickaxe(self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None:
         try:
             cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaPickaxe")
             await self.party.me.set_pickaxe(asset=cosmetic.id)
             await ctx.send(f'Pickaxe set to {cosmetic.name}.')
 
         except FortniteAPIAsync.exceptions.NotFound:
             pass
 
     @commands.command(aliases=['news'])
-    @commands.cooldown(1, 7)
+    @commands.cooldown(1, 10)
     async def new(self, ctx: fortnitepy.ext.commands.Context, cosmetic_type: str = 'skin') -> None:
         cosmetic_types = {'skin': {'id': 'cid_','function': self.party.me.set_outfit},'backpack': {'id': 'bid_','function': self.party.me.set_backpack},'emote': {'id': 'eid_','function': self.party.me.set_emote},}
 
         if cosmetic_type not in cosmetic_types:
             return await ctx.send('Invalid cosmetic type, valid types include: skin, backpack & emote.')
 
         new_cosmetics = await self.fortnite_api.cosmetics.get_new_cosmetics()
@@ -921,15 +513,15 @@
             await cosmetic_types[cosmetic_type]['function'](asset=new_cosmetic.id)
 
             await ctx.send(f"{cosmetic_type}s set to {new_cosmetic.name}.")
             os.system('clear')
 
             await asyncio.sleep(3)
 
-        await ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')
+        await ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')           
 
     @commands.command()
     async def purpleskull(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
         await ctx.send(f'Skin set to Purple Skull Trooper!')
         os.system('clear')
 
@@ -950,15 +542,15 @@
         await self.party.me.set_outfit(asset='CID_017_Athena_Commando_M')
         await ctx.send('Skin set to aerial!')
         os.system('clear')
 
     @commands.command()
     async def hologram(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_outfit(asset='CID_VIP_Athena_Commando_M_GalileoGondola_SG')
-        await ctx.send('Skin set to Star Wars Hologram!')
+        await ctx.send('Skin set to Star Wars Hologram!')  
 
     @commands.command()
     async def cid(self, ctx: fortnitepy.ext.commands.Context, character_id: str) -> None:
         await self.party.me.set_outfit(asset=character_id,variants=self.party.me.create_variants(profile_banner='ProfileBanner'))
         await ctx.send(f'Skin set to {character_id}.')
         os.system('clear')
 
@@ -966,14 +558,20 @@
     async def eid(self, ctx: fortnitepy.ext.commands.Context, emote_id: str) -> None:
         await self.party.me.clear_emote()
         await self.party.me.set_emote(asset=emote_id)
         await ctx.send(f'Emote set to {emote_id}!')
         os.system('clear')
 
     @commands.command()
+    async def bid(self, ctx: fortnitepy.ext.commands.Context, backpack_id: str) -> None:
+        await self.party.me.set_backpack(asset=backpack_id)
+        await ctx.send(f'Backbling set to {backpack_id}!')
+        os.system('clear')
+
+    @commands.command()
     async def stop(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.clear_emote()
         await ctx.send('Stopped emoting.')
         os.system('clear')
 
     @commands.command()
     async def point(self, ctx: fortnitepy.ext.commands.Context, *, content: Optional[str] = None) -> None:
@@ -1030,25 +628,25 @@
             await ctx.send("Could not get that user.")
 
     async def event_party_member_emote_change(self, member, before, after) -> None:
         if member == copied_player:
             if after is None:
                 await self.party.me.clear_emote()
             else:
-                await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_emote,asset=after))
+                await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_emote,asset=after))                        
                 os.system('clear')
 
     async def event_party_member_outfit_change(self, member, before, after) -> None:
         if member == copied_player:
-            await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_outfit,asset=member.outfit,variants=member.outfit_variants,enlightenment=None,corruption=None))
+            await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_outfit,asset=member.outfit,variants=member.outfit_variants))
             os.system('clear')
 
     async def event_party_member_outfit_variants_change(self, member, before, after) -> None:
         if member == copied_player:
-            await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_outfit,variants=member.outfit_variants,enlightenment=None,corruption=None))
+            await self.party.me.edit_and_keep(partial(fortnitepy.ClientPartyMember.set_outfit,variants=member.outfit_variants))
             os.system('clear')
 
 #///////////////////////////////////////////////////////////////////////////////////////////////////////////// PARTY/FRIENDS/ADMIN //////////////////////////////////////////////////////////////////////////////////////////////////////
 
     @commands.command()
     async def add(self, ctx: fortnitepy.ext.commands.Context, *, epic_username: str) -> None:
         user = await self.fetch_user(epic_username)
@@ -1057,22 +655,22 @@
         if user.id in friends:
             await ctx.send(f'I already have {user.display_name} as a friend')
         else:
             await self.add_friend(user.id)
             await ctx.send(f'Send i friend request to {user.display_name}.')
 
     @is_admin()
-    @commands.command(aliases=['rst'],)
+    @commands.command()
     async def restart(self, ctx: fortnitepy.ext.commands.Context) -> None:
-        await ctx.send(f'Restart...')
+        await ctx.send(f'im Restart now')
         python = sys.executable
-        os.execl(python, python, *sys.argv)
+        os.execl(python, python, *sys.argv)        
 
     @is_admin()
-    @commands.command(aliases=['max'],)
+    @commands.command()
     async def set(self, ctx: fortnitepy.ext.commands.Context, nombre: int) -> None:
         await self.party.set_max_size(nombre)
         await ctx.send(f'Set party to {nombre} player can join')
         os.system('clear')
 
     @commands.command()
     async def ready(self, ctx: fortnitepy.ext.commands.Context) -> None:
@@ -1082,39 +680,39 @@
 
     @commands.command(aliases=['sitin'],)
     async def unready(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_ready(fortnitepy.ReadyState.NOT_READY)
         await ctx.send('Unready!')
         os.system('clear')
 
-    @commands.command(aliases=['level'],)
-    async def levelx(self, ctx: fortnitepy.ext.commands.Context, banner_level: int) -> None:
+    @commands.command()
+    async def level(self, ctx: fortnitepy.ext.commands.Context, banner_level: int) -> None:
         await self.party.me.set_banner(season_level=banner_level)
         await ctx.send(f'Set level to {banner_level}.')
         os.system('clear')
 
     @is_admin()
     @commands.command()
     async def sitout(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_ready(fortnitepy.ReadyState.SITTING_OUT)
         await ctx.send('Sitting Out!')
         os.system('clear')    
         
     @is_admin()
-    @commands.command(aliases=['lv'],)
+    @commands.command()
     async def leave(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.leave()
         await ctx.send(f'I Leave')
         await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
         os.system('clear')
 
     @is_admin()
     @commands.command()
     async def v(self, ctx: fortnitepy.ext.commands.Context) -> None:
-        await ctx.send(f'version {__version__}')
+        await ctx.send(f'the version {__version__}')
         os.system('clear')
 
     @is_admin()
     @commands.command(aliases=['unhide'],)
     async def promote(self, ctx: fortnitepy.ext.commands.Context, *, epic_username: Optional[str] = None) -> None:
         if epic_username is None:
             user = await self.fetch_user(ctx.author.display_name)
@@ -1126,14 +724,15 @@
         if member is None:
             await ctx.send("Failed to find that user, are you sure they're in the party?")
         else:
             try:
                 await member.promote()
                 os.system('clear')
                 await ctx.send(f"Promoted user: {member.display_name}.")
+                print(f"Promoted user: {member.display_name}")
             except fortnitepy.errors.Forbidden:
                 await ctx.send(f"Failed to promote {member.display_name}, as I'm not party leader.")
 
     @is_admin()
     @commands.command()
     async def kick(self, ctx: fortnitepy.ext.commands.Context, *, epic_username: Optional[str] = None) -> None:
         if epic_username is None:
@@ -1155,15 +754,14 @@
                 await ctx.send(f"Failed to kick {member.display_name}, as I'm not party leader.")
 
     async def set_and_update_party_prop(self, schema_key: str, new_value: str):
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
 
-    @is_admin()
     @commands.command()
     async def hide(self, ctx: fortnitepy.ext.commands.Context, *, user = None):
         if self.party.me.leader:
             if user != "all":
                 try:
                     if user is None:
                         user = await self.fetch_profile(ctx.message.author.id)
@@ -1187,33 +785,93 @@
             else:
                 try:
                     await self.set_and_update_party_prop('Default:RawSquadAssignments_j',{'RawSquadAssignments': [{'memberId': self.user.id,'absoluteMemberIdx': 1}]})
                     await ctx.send("Hid everyone in the party.")
                 except fortnitepy.HTTPException:
                     await ctx.send("I am not party leader.")
         else:
-            await ctx.send("I need party leader to do this!")
+            await ctx.send("I need party leader to do this!") 
+
+    @commands.party_only()
+    @commands.command(name='- HEY',aliases=['-HEY','Youtube:','Item','Notice:','This','Heyy','If'], hidden=True)
+    async def kickortherbots(self, ctx: fortnitepy.ext.commands.Context, *, username = None):
+        if self.party.me.leader:
+            user = await self.fetch_profile(ctx.author.id)
+            member = self.party.get_member(user.id)
+
+        if not member.display_name in info['FullAccess']:
+            await member.kick()
+            os.system('clear')
+            await ctx.send("The orther Bot is Not accepted of the party")
+
+        else:
+            await ctx.send()
+
+    @is_admin()
+    @commands.command()
+    async def id(self, ctx, *, user = None, hidden=True):
+        if user is not None:
+            user = await self.fetch_profile(user)
+        
+        elif user is None:
+            user = await self.fetch_profile(ctx.message.author.id)
+        try:
+            await ctx.send(f"{user}'s Epic ID is: {user.id}")
+            os.system('clear')
+            print(Fore.GREEN + ' [+] ' + Fore.RESET + f"{user}'s Epic ID is: " + Fore.LIGHTBLACK_EX + f'{user.id}')
+        except AttributeError:
+            await ctx.send("I couldn't find an Epic account with that name.")
+
+    @is_admin()
+    @commands.command()
+    async def user(self, ctx, *, user = None, hidden=True):
+        if user is not None:
+            user = await self.fetch_profile(user)
+            try:
+                await ctx.send(f"The ID: {user.id} belongs to: {user.display_name}")
+                os.system('clear')
+                print(Fore.GREEN + ' [+] ' + Fore.RESET + f'The ID: {user.id} belongs to: ' + Fore.LIGHTBLACK_EX + f'{user.display_name}')
+            except AttributeError:
+                await ctx.send(f"I couldn't find a user that matches that ID")
+        else:
+            await ctx.send(f'No ID was given. Try: {prefix}user (ID)')
 
     async def invitefriends(self):
         send = []
         for friend in self.friends:
             if friend.is_online():
                 send.append(friend.display_name)
                 await friend.invite()
+                print(f'[=] {friend.display_name} was send')
+
+        for ctz in self.friends:
+            if not ctz.display_name != "AerozOff":
+                if ctz.is_online():
+                    await ctz.send('finit de inviter')
 
     @is_admin()
     @commands.command()
     async def invite(self, ctx: fortnitepy.ext.commands.Context) -> None:
         try:
             self.loop.create_task(self.invitefriends())
         except Exception:
-            pass    
+            pass
+
+    @is_admin()
+    @commands.command()
+    async def deletefriends(self, ctx: fortnitepy.ext.commands.Context) -> None:
+        for pending in self.incoming_pending_friends:
+            epic_friend = await pending.decline()
+            if isinstance(epic_friend, fortnitepy.Friend):
+                print(f"Accepted friend request from: {epic_friend.display_name}.")
+            else:
+                print(f"Declined friend request from: {pending.display_name}.")        
 
     @commands.command(aliases=['friends'],)
-    async def epicfriends(self, ctx: fortnitepy.ext.commands.Context) -> None:
+    async def epicfriends2(self, ctx: fortnitepy.ext.commands.Context) -> None:
         onlineFriends = []
         offlineFriends = []
 
         try:
             for friend in self.friends:
                 if friend.is_online():
                     onlineFriends.append(friend.display_name)
@@ -1222,46 +880,31 @@
             
             await ctx.send(f"Total Friends: {len(self.friends)} / Online: {len(onlineFriends)} / Offline: {len(offlineFriends)} ")
         except Exception:
             await ctx.send(f'Not work')
 
     @is_admin()
     @commands.command()
-    async def whisper(self, ctx: fortnitepy.ext.commands.Context, *, message = None):
+    async def whisper(self, ctx: fortnitepy.ext.commands.Context, message = None) -> None:
         try:
-            if message is not None:
-                for friend in self.friends:
-                    if friend.is_online():
-                        await friend.send(message)
+            for friend in self.friends:
+                if friend.is_online():
+                    await friend.send(message)
 
-                await ctx.send(f'Send friend message to everyone')
-                os.system('clear')
+            await ctx.send(f'Send friend message to everyone')
+            os.system('clear')
         except: pass
 
     @commands.command()
-    async def fixadmin(self, ctx: fortnitepy.ext.commands.Context):
-        if ctx.author.display_name == 'AerozOff':
-            with open("info.json", "w") as f:
-                f.write('{"FullAccess": ["AerozOff"]}')
-            await ctx.send('work')
-
-            with open('info.json') as f:
-                info = json.load(f)
-
-            await ctx.send('correctly work')\
-
-        else:
-            await ctx.send("You don't have perm LMAO")
-
-    @commands.command()
     async def say(self, ctx: fortnitepy.ext.commands.Context, *, message = None):
         if message is not None:
             await self.party.send(message)
+            await ctx.send(f'Sent "{message}" to party chat')
         else:
-            await ctx.send(f'Try: {prefix} say (message)')
+            await ctx.send(f'No message was given. Try: {prefix} say (message)')
 
     @is_admin()
     @commands.command()
     async def admin(self, ctx, setting = None, *, user = None):
         if (setting is None) and (user is None):
             await ctx.send(f"Missing one or more arguments. Try: {prefix} admin (add, remove, list) (user)")
         elif (setting is not None) and (user is None):
@@ -1277,14 +920,15 @@
                     response = await self.wait_for('friend_message', timeout=20)
                     content = response.content.lower()
                     if content == password:
                         info['FullAccess'].append(user.display_name)
                         with open('info.json', 'w') as f:
                             json.dump(info, f, indent=4)
                             await ctx.send(f"Correct. Added {user.display_name} as an admin.")
+                            print(Fore.GREEN + " [+] " + Fore.LIGHTGREEN_EX + user.display_name + Fore.RESET + " was added as an admin.")
                     else:
                         await ctx.send("Incorrect Password.")
 
             elif setting.lower() == 'remove':
                 if user.display_name not in info['FullAccess']:
                     await ctx.send("You are not an admin.")
                 else:
@@ -1292,14 +936,15 @@
                     response = await self.wait_for('friend_message', timeout=20)
                     content = response.content.lower()
                     if (content.lower() == 'yes') or (content.lower() == 'y'):
                         info['FullAccess'].remove(user.display_name)
                         with open('info.json', 'w') as f:
                             json.dump(info, f, indent=4)
                             await ctx.send("You were removed as an admin.")
+                            print(Fore.BLUE + " [+] " + Fore.LIGHTBLUE_EX + user.display_name + Fore.RESET + " was removed as an admin.")
                     elif (content.lower() == 'no') or (content.lower() == 'n'):
                         await ctx.send("You were kept as admin.")
                     else:
                         await ctx.send("Not a correct reponse. Cancelling command.")
                     
             elif setting == 'list':
                 if user.display_name in info['FullAccess']:
@@ -1326,14 +971,15 @@
             if setting.lower() == 'add':
                 if ctx.message.author.display_name in info['FullAccess']:
                     if user.display_name not in info['FullAccess']:
                         info['FullAccess'].append(user.display_name)
                         with open('info.json', 'w') as f:
                             json.dump(info, f, indent=4)
                             await ctx.send(f"Correct. Added {user.display_name} as an admin.")
+                            print(Fore.GREEN + " [+] " + Fore.LIGHTGREEN_EX + user.display_name + Fore.RESET + " was added as an admin.")
                     else:
                         await ctx.send("That user is already an admin.")
                 else:
                     await ctx.send("You don't have access to add other people as admins. Try just: !admin add")
             elif setting.lower() == 'remove':
                 if ctx.message.author.display_name in info['FullAccess']:
                     if user.display_name in info['FullAccess']:
@@ -1341,15 +987,41 @@
                         response = await self.wait_for('friend_message', timeout=20)
                         content = response.content.lower()
                         if content == password:
                             info['FullAccess'].remove(user.display_name)
                             with open('info.json', 'w') as f:
                                 json.dump(info, f, indent=4)
                                 await ctx.send(f"{user.display_name} was removed as an admin.")
+                                print(Fore.BLUE + " [+] " + Fore.LIGHTBLUE_EX + user.display_name + Fore.RESET + " was removed as an admin.")
                         else:
                             await ctx.send("Incorrect Password.")
                     else:
                         await ctx.send("That person is not an admin.")
                 else:
                     await ctx.send("You don't have permission to remove players as an admin.")
             else:
                 await ctx.send(f"Not a valid setting. Try: {prefix} -admin (add, remove) (user)")
+
+    @commands.command()
+    async def away(self, ctx: fortnitepy.ext.commands.Context) -> None:
+        await self.set_presence(
+            status=self.status,
+            away=fortnitepy.AwayStatus.AWAY
+        )
+
+        await ctx.send('Status set to away.')
+
+    @is_admin()
+    @commands.command()
+    async def remove_xbx(ctx):
+        self.ban_player = ['XBX']
+        friend = []
+
+        if self.friends in friend.display_name:
+            name = friend.display_name
+            if any(word in name for word in self.ban_player):
+                try:
+                    await friend.remove()
+                    print(f' Friend {friend.display_name} Removed Corectly')
+                except: pass
+
+
```

## Comparing `schbot-0.6.0.dist-info/metadata.json` & `schbot-0.6.2.dist-info/metadata.json`

 * *Files 5% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9351851851851853%*

 * *Differences: {"'run_requires'": "{0: {'requires': {insert: [(3, 'colorama')], delete: [6, 2]}}}",*

 * * "'version'": "'0.6.2'"}*

```diff
@@ -25,19 +25,18 @@
     "metadata_version": "2.0",
     "name": "schbot",
     "run_requires": [
         {
             "requires": [
                 "BenBotAsync",
                 "FortniteAPIAsync",
-                "PirxcyPinger",
                 "aiohttp",
+                "colorama",
                 "crayons",
                 "fortnitepy (==3.6.7)",
-                "requests",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.6.0"
+    "version": "0.6.2"
 }
```

## Comparing `schbot-0.6.0.dist-info/METADATA` & `schbot-0.6.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.0
 Name: schbot
-Version: 0.6.0
+Version: 0.6.2
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: BenBotAsync
 Requires-Dist: FortniteAPIAsync
-Requires-Dist: PirxcyPinger
 Requires-Dist: aiohttp
+Requires-Dist: colorama
 Requires-Dist: crayons
 Requires-Dist: fortnitepy (==3.6.7)
-Requires-Dist: requests
 Requires-Dist: sanic (==21.6.2)
 
 UNKNOWN
```

