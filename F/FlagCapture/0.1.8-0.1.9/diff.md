# Comparing `tmp/FlagCapture-0.1.8.tar.gz` & `tmp/FlagCapture-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlagCapture-0.1.8.tar", last modified: Wed Apr  5 02:26:46 2023, max compression
+gzip compressed data, was "FlagCapture-0.1.9.tar", last modified: Fri Apr 14 16:20:14 2023, max compression
```

## Comparing `FlagCapture-0.1.8.tar` & `FlagCapture-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 02:26:46.847298 FlagCapture-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-04-05 02:26:46.794422 FlagCapture-0.1.8/FlagCapture/
--rw-rw-rw-   0        0        0     3348 2023-04-05 02:24:36.000000 FlagCapture-0.1.8/FlagCapture/CaptureTheFlagServer.py
--rw-rw-rw-   0        0        0    19888 2023-04-05 02:24:22.000000 FlagCapture-0.1.8/FlagCapture/Game.py
--rw-rw-rw-   0        0        0     2742 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/Server.py
--rw-rw-rw-   0        0        0       52 2023-04-05 02:25:51.000000 FlagCapture-0.1.8/FlagCapture/__init__.py
--rw-rw-rw-   0        0        0    19903 2023-04-05 02:24:29.000000 FlagCapture-0.1.8/FlagCapture/_game.py
--rw-rw-rw-   0        0        0 14186642 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/build.py
--rw-rw-rw-   0        0        0    12815 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/entity.py
--rw-rw-rw-   0        0        0     1516 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/math.py
--rw-rw-rw-   0        0        0    41487 2023-04-05 02:23:23.000000 FlagCapture-0.1.8/FlagCapture/miniworld.py
--rw-rw-rw-   0        0        0     7741 2023-04-01 16:05:35.000000 FlagCapture-0.1.8/FlagCapture/objmesh.py
--rw-rw-rw-   0        0        0    15095 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/opengl.py
--rw-rw-rw-   0        0        0     4062 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/params.py
--rw-rw-rw-   0        0        0      901 2023-04-04 17:33:06.000000 FlagCapture-0.1.8/FlagCapture/utils.py
--rw-rw-rw-   0        0        0     1267 2023-03-30 23:37:11.000000 FlagCapture-0.1.8/FlagCapture/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-05 02:26:46.837912 FlagCapture-0.1.8/FlagCapture.egg-info/
--rw-rw-rw-   0        0        0      407 2023-04-05 02:26:46.000000 FlagCapture-0.1.8/FlagCapture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-04-05 02:26:46.000000 FlagCapture-0.1.8/FlagCapture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 02:26:46.000000 FlagCapture-0.1.8/FlagCapture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-05 02:26:46.000000 FlagCapture-0.1.8/FlagCapture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-05 02:26:46.000000 FlagCapture-0.1.8/FlagCapture.egg-info/zip-safe
--rw-rw-rw-   0        0        0      407 2023-04-05 02:26:46.845905 FlagCapture-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-05 02:26:46.850087 FlagCapture-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      524 2023-04-05 02:26:28.000000 FlagCapture-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:20:14.552058 FlagCapture-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-04-14 16:20:14.528122 FlagCapture-0.1.9/FlagCapture/
+-rw-rw-rw-   0        0        0     3348 2023-04-14 16:13:17.000000 FlagCapture-0.1.9/FlagCapture/CaptureTheFlagServer.py
+-rw-rw-rw-   0        0        0    19955 2023-04-14 16:14:04.000000 FlagCapture-0.1.9/FlagCapture/Game.py
+-rw-rw-rw-   0        0        0       52 2023-04-05 02:25:51.000000 FlagCapture-0.1.9/FlagCapture/__init__.py
+-rw-rw-rw-   0        0        0    19972 2023-04-14 16:13:12.000000 FlagCapture-0.1.9/FlagCapture/_game.py
+-rw-rw-rw-   0        0        0 14186642 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/build.py
+-rw-rw-rw-   0        0        0    12815 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/entity.py
+-rw-rw-rw-   0        0        0     1516 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/math.py
+-rw-rw-rw-   0        0        0    41487 2023-04-05 02:23:23.000000 FlagCapture-0.1.9/FlagCapture/miniworld.py
+-rw-rw-rw-   0        0        0     7741 2023-04-01 16:05:35.000000 FlagCapture-0.1.9/FlagCapture/objmesh.py
+-rw-rw-rw-   0        0        0    15095 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/opengl.py
+-rw-rw-rw-   0        0        0     4062 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/params.py
+-rw-rw-rw-   0        0        0      901 2023-04-04 17:33:06.000000 FlagCapture-0.1.9/FlagCapture/utils.py
+-rw-rw-rw-   0        0        0     1267 2023-03-30 23:37:11.000000 FlagCapture-0.1.9/FlagCapture/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:20:14.547071 FlagCapture-0.1.9/FlagCapture.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-04-14 16:20:14.000000 FlagCapture-0.1.9/FlagCapture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-14 16:20:14.000000 FlagCapture-0.1.9/FlagCapture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:20:14.000000 FlagCapture-0.1.9/FlagCapture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 16:20:14.000000 FlagCapture-0.1.9/FlagCapture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 16:20:14.000000 FlagCapture-0.1.9/FlagCapture.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      592 2023-04-14 16:20:14.550063 FlagCapture-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:20:14.552058 FlagCapture-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-14 16:18:52.000000 FlagCapture-0.1.9/setup.py
```

### Comparing `FlagCapture-0.1.8/FlagCapture/CaptureTheFlagServer.py` & `FlagCapture-0.1.9/FlagCapture/CaptureTheFlagServer.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/Game.py` & `FlagCapture-0.1.9/FlagCapture/Game.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,34 +105,32 @@
         self.add_rect_room(min_x=82, max_x=88, max_z=-49, min_z=-49.01, wall_tex='blueColor')
         self.add_rect_room(min_x=82, max_x=82.01, max_z=-49, min_z=-58, wall_tex='blueColor')
         self.redGate = self.place_entity(MeshEnt(mesh_name=f'gate', height=2.6), pos=[48, 0, 49], dir=-3.1)
         self.blueGate = self.place_entity(MeshEnt(mesh_name=f'gate', height=2.6), pos=[48, 0, -49], dir=6.3)
         self.redFlag = self.place_entity(MeshEnt(mesh_name=f'flagRed', height=2.5, static=False), pos=start_info['RedFlagPos'])
         self.blueFlag = self.place_entity(MeshEnt(mesh_name=f'flagBlue', height=2.5, static=False), pos=start_info['BlueFlagPos'])
         for person in start_info['Everything']:
-            animal = self.place_entity(MeshEnt(mesh_name=f''+start_info['Everything'][person]['team'], height=1.4, static=False), pos=start_info['Everything'][person]['pos'], dir=start_info['Everything'][person]['dir'])
-            people[person] = animal
-            if start_info['Everything'][person]['team'] == myTeam:
-                list_of_players_on_my_team.append(person)
-            else:
-                list_of_players_on_their_team.append(person)
+            if person != myId:
+                animal = self.place_entity(MeshEnt(mesh_name=f''+start_info['Everything'][person]['team'], height=1.4, static=False), pos=start_info['Everything'][person]['pos'], dir=start_info['Everything'][person]['dir'])
+                people[person] = animal
+                if not start_info['Everything'][person]['team'] == myTeam:
+                    list_of_players_on_their_team.append(person)
         self.leftRedButton = self.place_entity(MeshEnt(mesh_name=f'RedButton', height=1), pos=[82.5, 1, -44.749], dir=-1.5)
         self.rightRedButton = self.place_entity(MeshEnt(mesh_name=f'RedButton', height=1), pos=[9.5, 1, -44.749], dir=-1.5)
         self.rightBlueButton = self.place_entity(MeshEnt(mesh_name=f'BlueButton', height=1), pos=[9.5, 1, 44.749], dir=1.6)
         self.leftBlueButton = self.place_entity(MeshEnt(mesh_name=f'BlueButton', height=1), pos=[82.5, 1, 44.749], dir=1.6)
         self.place_agent()
 
 gym.envs.registration.register(id='Enviroment', entry_point=Scene)
 
 myinfo = start_info['MyInfo']
 
 myTeam = myinfo['team']
 myId = myinfo['id']
 
-list_of_players_on_my_team = []
 list_of_players_on_their_team = []
 people = {}
 
 creating = False
 
 board = key.KeyStateHandler()
 scene = gym.make("Enviroment", view='agent', render_mode='human')
@@ -168,45 +166,35 @@
     if intersection == True:
         x_pos = [x, 0, obj.pos[2]]
         if scene.intersect(obj, x_pos, obj.radius) == True:
             z_pos = [obj.pos[0], 0, z]
             if scene.intersect(obj, z_pos, obj.radius) == True:
                 return
             else:
-                obj.pos = [obj.pos[0], 0, z]
+                cl.send(str(['Updating pos', {'pos': z_pos}]).encode('utf-8'))
         else:
-            obj.pos = [x, 0, obj.pos[2]]
+            cl.send(str(['Updating pos', {'pos': x_pos}]).encode('utf-8'))
     else:
-        obj.pos = [x, 0, z]
-    if carrying == 'red' and z < 0:blue_wins()
-    if carrying == 'blue' and z > 0:red_wins()
+        cl.send(str(['Updating pos', {'pos': [x, 0, z]}]).encode('utf-8'))
 
 speed = 0.4
 
-def tell_pos_to_server(dt):
-    cl.send(str(['Updating pos', {'pos': scene.agent.pos}]).encode('utf-8'))
-
-def tell_dir_to_server(dt):
-    cl.send(str(['Updating dir', {'dir': scene.agent.dir}]).encode('utf-8'))
-
 def update(dt):
     global speed, carrying
     scene.unwrapped.fuel += 1
+    if carrying == 'red' and scene.agent.pos[2] < 0:blue_wins()
+    if carrying == 'blue' and scene.agent.pos[2] > 0:red_wins()
     if board[key.UP]:
         forward(scene.agent, speed)
-        pyglet.clock.schedule_once(tell_pos_to_server, 1.0/60)
     if board[key.LEFT]:
-        scene.agent.dir += speed/2
-        pyglet.clock.schedule_once(tell_dir_to_server, 1.0/60)
+        cl.send(str(['Updating dir', {'dir': scene.agent.dir + speed/2}]).encode('utf-8'))
     if board[key.RIGHT]:
-        scene.agent.dir -= speed/2
-        pyglet.clock.schedule_once(tell_dir_to_server, 1.0/60)
+        cl.send(str(['Updating dir', {'dir': scene.agent.dir - speed/2}]).encode('utf-8'))
     if board[key.DOWN]:
         forward(scene.agent, -speed)
-        pyglet.clock.schedule_once(tell_pos_to_server, 1.0/60)
     if board[key.P]:
         if scene.intersect(scene.agent, scene.agent.pos, scene.agent.radius) == scene.redFlag:
             carrying = 'red'
             scene.unwrapped.window.set_caption(f'{caption} [CARRYING A FLAG]')
             cl.send(str(['Updating carrying', {'carrying': 'red'}]).encode('utf-8'))
             scene.redFlag.pos = [30, -90, 0]
         if scene.intersect(scene.agent, scene.agent.pos, scene.agent.radius) == scene.blueFlag:
@@ -282,23 +270,22 @@
 
 def process_message(dt):
     global IAmPrisoner, message, creating
     try:
         message = eval(raw_message)
     except SyntaxError:
         return
+    
     for person in message:
         if person not in people and person != myId and not creating:#Some one joined
             creating = True
             animal = scene.place_entity(MeshEnt(mesh_name=message[person]['team'], height=1.4, static=False), pos=message[person]['pos'], dir=message[person]['dir'])
             print(message[person]['pos'])
             people[person] = animal
-            if message[person]['team'] == myTeam:
-                list_of_players_on_my_team.append(person)
-            else:
+            if not message[person]['team'] == myTeam:
                 list_of_players_on_their_team.append(person)
             creating = False
 
         elif person != myId: #Update the players
             people[person].pos = message[person]['pos']
             people[person].dir = message[person]['dir']
             if message[person]['carrying'] == 'red':
@@ -306,26 +293,31 @@
                 if scene.redFlag.pos[2] < 0:blue_wins()
                 scene.redFlag.dir = math.radians(math.degrees(message[person]['dir'])+180)
             if message[person]['carrying'] == 'blue':
                 scene.blueFlag.pos = [message[person]['pos'][0], 0, message[person]['pos'][2]]
                 if scene.blueFlag.pos[2] > 0:red_wins()
                 scene.blueFlag.dir = math.radians(math.degrees(message[person]['dir'])+180)
 
-            check_for_capture_and_touching_button()
-
-            if person in list_of_players_on_my_team and IAmPrisoner and message[person]['touching']:#Check to see if someone is freeing you
+            if message[person]['team'] == myTeam and IAmPrisoner and message[person]['touching']:#Check to see if someone is freeing you
                     IAmPrisoner=False
                     alert(get_file_path("images", "release", "png"), 2.5)
+
+        elif person == myId:
+            scene.agent.pos = message[person]['pos']
+            scene.agent.dir = message[person]['dir']
+            if message[person]['touching'] == True:
+                alert(get_file_path("images", "release", "png"), 2.5)
+                forward(scene.agent, -10)
+        
     for person in people:
         if person not in message:#Some one left
             scene.unwrapped.entities.remove(people[person])
             del people[person]
-            try: list_of_players_on_my_team.remove(person)
-            except ValueError: list_of_players_on_their_team.remove(person)
             break
+    check_for_capture_and_touching_button()
 
 @scene.unwrapped.window.event
 def on_close():
     cl.close()
 
 touching = False
 
@@ -342,49 +334,52 @@
         if myTeam == 'lynx':
             if intersection != scene.leftRedButton or intersection == scene.rightRedButton:
                 cl.send(str(['Updating touching', {'touching': False}]).encode('utf-8'))
                 touching = False
 
     #Check for touching enemy and in enemy territory
     for person in list_of_players_on_their_team:
-        if intersection == people[person] and scene.agent.pos[2] < 0:
-            if myTeam == 'wolf':
-                if carrying:
-                    drop_flag()
-                    scene.agent.pos = [48, 0, -55]
-                    scene.agent.dir = 4.754
-                    IAmPrisoner = True
-                    cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                    cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
-            if myTeam == 'lynx':
-                if message[person]['carrying']: return
-                if message[person]['prisoner']: return
-                drop_flag()
-                scene.agent.pos = [48, 0, 55]
-                scene.agent.dir = 1.654
-                IAmPrisoner = True
-                cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
-        if intersection == people[person] and scene.agent.pos[2] > 0:
-            if myTeam == 'lynx':
-                if carrying:
+        try:
+            if intersection == people[person] and scene.agent.pos[2] < 0:
+                if myTeam == 'wolf':
+                    if carrying:
+                        drop_flag()
+                        scene.agent.pos = [48, 0, -55]
+                        scene.agent.dir = 4.754
+                        IAmPrisoner = True
+                        cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                        cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+                if myTeam == 'lynx':
+                    if message[person]['carrying']: return
+                    if message[person]['prisoner']: return
                     drop_flag()
                     scene.agent.pos = [48, 0, 55]
                     scene.agent.dir = 1.654
                     IAmPrisoner = True
                     cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
                     cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
-            if myTeam == 'wolf':
-                if message[person]['carrying']:return
-                if message[person]['prisoner']: return
-                drop_flag()
-                scene.agent.pos = [48, 0, -55]
-                scene.agent.dir = 4.754
-                IAmPrisoner = True
-                cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+            if intersection == people[person] and scene.agent.pos[2] > 0:
+                if myTeam == 'lynx':
+                    if carrying:
+                        drop_flag()
+                        scene.agent.pos = [48, 0, 55]
+                        scene.agent.dir = 1.654
+                        IAmPrisoner = True
+                        cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                        cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
+                if myTeam == 'wolf':
+                    if message[person]['carrying']:return
+                    if message[person]['prisoner']: return
+                    drop_flag()
+                    scene.agent.pos = [48, 0, -55]
+                    scene.agent.dir = 4.754
+                    IAmPrisoner = True
+                    cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                    cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+        except KeyError:
+            list_of_players_on_their_team.remove(person)
 
 
 T(target=recv).start()
 
 pyglet.clock.schedule_interval(update, 1.0/30)
-pyglet.app.run()
+pyglet.app.run()
```

### Comparing `FlagCapture-0.1.8/FlagCapture/_game.py` & `FlagCapture-0.1.9/FlagCapture/_game.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,34 +105,32 @@
         self.add_rect_room(min_x=82, max_x=88, max_z=-49, min_z=-49.01, wall_tex='blueColor')
         self.add_rect_room(min_x=82, max_x=82.01, max_z=-49, min_z=-58, wall_tex='blueColor')
         self.redGate = self.place_entity(MeshEnt(mesh_name=f'gate', height=2.6), pos=[48, 0, 49], dir=-3.1)
         self.blueGate = self.place_entity(MeshEnt(mesh_name=f'gate', height=2.6), pos=[48, 0, -49], dir=6.3)
         self.redFlag = self.place_entity(MeshEnt(mesh_name=f'flagRed', height=2.5, static=False), pos=start_info['RedFlagPos'])
         self.blueFlag = self.place_entity(MeshEnt(mesh_name=f'flagBlue', height=2.5, static=False), pos=start_info['BlueFlagPos'])
         for person in start_info['Everything']:
-            animal = self.place_entity(MeshEnt(mesh_name=f''+start_info['Everything'][person]['team'], height=1.4, static=False), pos=start_info['Everything'][person]['pos'], dir=start_info['Everything'][person]['dir'])
-            people[person] = animal
-            if start_info['Everything'][person]['team'] == myTeam:
-                list_of_players_on_my_team.append(person)
-            else:
-                list_of_players_on_their_team.append(person)
+            if person != myId:
+                animal = self.place_entity(MeshEnt(mesh_name=f''+start_info['Everything'][person]['team'], height=1.4, static=False), pos=start_info['Everything'][person]['pos'], dir=start_info['Everything'][person]['dir'])
+                people[person] = animal
+                if not start_info['Everything'][person]['team'] == myTeam:
+                    list_of_players_on_their_team.append(person)
         self.leftRedButton = self.place_entity(MeshEnt(mesh_name=f'RedButton', height=1), pos=[82.5, 1, -44.749], dir=-1.5)
         self.rightRedButton = self.place_entity(MeshEnt(mesh_name=f'RedButton', height=1), pos=[9.5, 1, -44.749], dir=-1.5)
         self.rightBlueButton = self.place_entity(MeshEnt(mesh_name=f'BlueButton', height=1), pos=[9.5, 1, 44.749], dir=1.6)
         self.leftBlueButton = self.place_entity(MeshEnt(mesh_name=f'BlueButton', height=1), pos=[82.5, 1, 44.749], dir=1.6)
         self.place_agent()
 
 gym.envs.registration.register(id='Enviroment', entry_point=Scene)
 
 myinfo = start_info['MyInfo']
 
 myTeam = myinfo['team']
 myId = myinfo['id']
 
-list_of_players_on_my_team = []
 list_of_players_on_their_team = []
 people = {}
 
 creating = False
 
 board = key.KeyStateHandler()
 scene = gym.make("Enviroment", view='agent', render_mode='human')
@@ -168,45 +166,35 @@
     if intersection == True:
         x_pos = [x, 0, obj.pos[2]]
         if scene.intersect(obj, x_pos, obj.radius) == True:
             z_pos = [obj.pos[0], 0, z]
             if scene.intersect(obj, z_pos, obj.radius) == True:
                 return
             else:
-                obj.pos = [obj.pos[0], 0, z]
+                cl.send(str(['Updating pos', {'pos': z_pos}]).encode('utf-8'))
         else:
-            obj.pos = [x, 0, obj.pos[2]]
+            cl.send(str(['Updating pos', {'pos': x_pos}]).encode('utf-8'))
     else:
-        obj.pos = [x, 0, z]
-    if carrying == 'red' and z < 0:blue_wins()
-    if carrying == 'blue' and z > 0:red_wins()
+        cl.send(str(['Updating pos', {'pos': [x, 0, z]}]).encode('utf-8'))
 
 speed = 0.4
 
-def tell_pos_to_server(dt):
-    cl.send(str(['Updating pos', {'pos': scene.agent.pos}]).encode('utf-8'))
-
-def tell_dir_to_server(dt):
-    cl.send(str(['Updating dir', {'dir': scene.agent.dir}]).encode('utf-8'))
-
 def update(dt):
     global speed, carrying
     scene.unwrapped.fuel += 1
+    if carrying == 'red' and scene.agent.pos[2] < 0:blue_wins()
+    if carrying == 'blue' and scene.agent.pos[2] > 0:red_wins()
     if board[key.UP]:
         forward(scene.agent, speed)
-        pyglet.clock.schedule_once(tell_pos_to_server, 1.0/60)
     if board[key.LEFT]:
-        scene.agent.dir += speed/2
-        pyglet.clock.schedule_once(tell_dir_to_server, 1.0/60)
+        cl.send(str(['Updating dir', {'dir': scene.agent.dir + speed/2}]).encode('utf-8'))
     if board[key.RIGHT]:
-        scene.agent.dir -= speed/2
-        pyglet.clock.schedule_once(tell_dir_to_server, 1.0/60)
+        cl.send(str(['Updating dir', {'dir': scene.agent.dir - speed/2}]).encode('utf-8'))
     if board[key.DOWN]:
         forward(scene.agent, -speed)
-        pyglet.clock.schedule_once(tell_pos_to_server, 1.0/60)
     if board[key.P]:
         if scene.intersect(scene.agent, scene.agent.pos, scene.agent.radius) == scene.redFlag:
             carrying = 'red'
             scene.unwrapped.window.set_caption(f'{caption} [CARRYING A FLAG]')
             cl.send(str(['Updating carrying', {'carrying': 'red'}]).encode('utf-8'))
             scene.redFlag.pos = [30, -90, 0]
         if scene.intersect(scene.agent, scene.agent.pos, scene.agent.radius) == scene.blueFlag:
@@ -282,23 +270,22 @@
 
 def process_message(dt):
     global IAmPrisoner, message, creating
     try:
         message = eval(raw_message)
     except SyntaxError:
         return
+    
     for person in message:
         if person not in people and person != myId and not creating:#Some one joined
             creating = True
             animal = scene.place_entity(MeshEnt(mesh_name=message[person]['team'], height=1.4, static=False), pos=message[person]['pos'], dir=message[person]['dir'])
             print(message[person]['pos'])
             people[person] = animal
-            if message[person]['team'] == myTeam:
-                list_of_players_on_my_team.append(person)
-            else:
+            if not message[person]['team'] == myTeam:
                 list_of_players_on_their_team.append(person)
             creating = False
 
         elif person != myId: #Update the players
             people[person].pos = message[person]['pos']
             people[person].dir = message[person]['dir']
             if message[person]['carrying'] == 'red':
@@ -306,26 +293,31 @@
                 if scene.redFlag.pos[2] < 0:blue_wins()
                 scene.redFlag.dir = math.radians(math.degrees(message[person]['dir'])+180)
             if message[person]['carrying'] == 'blue':
                 scene.blueFlag.pos = [message[person]['pos'][0], 0, message[person]['pos'][2]]
                 if scene.blueFlag.pos[2] > 0:red_wins()
                 scene.blueFlag.dir = math.radians(math.degrees(message[person]['dir'])+180)
 
-            check_for_capture_and_touching_button()
-
-            if person in list_of_players_on_my_team and IAmPrisoner and message[person]['touching']:#Check to see if someone is freeing you
+            if message[person]['team'] == myTeam and IAmPrisoner and message[person]['touching']:#Check to see if someone is freeing you
                     IAmPrisoner=False
                     alert(get_file_path("images", "release", "png"), 2.5)
+
+        elif person == myId:
+            scene.agent.pos = message[person]['pos']
+            scene.agent.dir = message[person]['dir']
+            if message[person]['touching'] == True:
+                alert(get_file_path("images", "release", "png"), 2.5)
+                forward(scene.agent, -10)
+        
     for person in people:
         if person not in message:#Some one left
             scene.unwrapped.entities.remove(people[person])
             del people[person]
-            try: list_of_players_on_my_team.remove(person)
-            except ValueError: list_of_players_on_their_team.remove(person)
             break
+    check_for_capture_and_touching_button()
 
 @scene.unwrapped.window.event
 def on_close():
     cl.close()
 
 touching = False
 
@@ -342,49 +334,52 @@
         if myTeam == 'lynx':
             if intersection != scene.leftRedButton or intersection == scene.rightRedButton:
                 cl.send(str(['Updating touching', {'touching': False}]).encode('utf-8'))
                 touching = False
 
     #Check for touching enemy and in enemy territory
     for person in list_of_players_on_their_team:
-        if intersection == people[person] and scene.agent.pos[2] < 0:
-            if myTeam == 'wolf':
-                if carrying:
-                    drop_flag()
-                    scene.agent.pos = [48, 0, -55]
-                    scene.agent.dir = 4.754
-                    IAmPrisoner = True
-                    cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                    cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
-            if myTeam == 'lynx':
-                if message[person]['carrying']: return
-                if message[person]['prisoner']: return
-                drop_flag()
-                scene.agent.pos = [48, 0, 55]
-                scene.agent.dir = 1.654
-                IAmPrisoner = True
-                cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
-        if intersection == people[person] and scene.agent.pos[2] > 0:
-            if myTeam == 'lynx':
-                if carrying:
+        try:
+            if intersection == people[person] and scene.agent.pos[2] < 0:
+                if myTeam == 'wolf':
+                    if carrying:
+                        drop_flag()
+                        scene.agent.pos = [48, 0, -55]
+                        scene.agent.dir = 4.754
+                        IAmPrisoner = True
+                        cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                        cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+                if myTeam == 'lynx':
+                    if message[person]['carrying']: return
+                    if message[person]['prisoner']: return
                     drop_flag()
                     scene.agent.pos = [48, 0, 55]
                     scene.agent.dir = 1.654
                     IAmPrisoner = True
                     cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
                     cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
-            if myTeam == 'wolf':
-                if message[person]['carrying']:return
-                if message[person]['prisoner']: return
-                drop_flag()
-                scene.agent.pos = [48, 0, -55]
-                scene.agent.dir = 4.754
-                IAmPrisoner = True
-                cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
-                cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+            if intersection == people[person] and scene.agent.pos[2] > 0:
+                if myTeam == 'lynx':
+                    if carrying:
+                        drop_flag()
+                        scene.agent.pos = [48, 0, 55]
+                        scene.agent.dir = 1.654
+                        IAmPrisoner = True
+                        cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                        cl.send(str(['Updating pos', {'pos': [48, 0, 55]}]).encode('utf-8'))
+                if myTeam == 'wolf':
+                    if message[person]['carrying']:return
+                    if message[person]['prisoner']: return
+                    drop_flag()
+                    scene.agent.pos = [48, 0, -55]
+                    scene.agent.dir = 4.754
+                    IAmPrisoner = True
+                    cl.send(str(['Updating prisoner', {'prisoner': [48, 0, -55]}]).encode('utf-8'))
+                    cl.send(str(['Updating pos', {'pos': [48, 0, -55]}]).encode('utf-8'))
+        except KeyError:
+            list_of_players_on_their_team.remove(person)
 
 
 T(target=recv).start()
 
 pyglet.clock.schedule_interval(update, 1.0/30)
 pyglet.app.run()
```

### Comparing `FlagCapture-0.1.8/FlagCapture/build.py` & `FlagCapture-0.1.9/FlagCapture/build.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/entity.py` & `FlagCapture-0.1.9/FlagCapture/entity.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/math.py` & `FlagCapture-0.1.9/FlagCapture/math.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/miniworld.py` & `FlagCapture-0.1.9/FlagCapture/miniworld.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/objmesh.py` & `FlagCapture-0.1.9/FlagCapture/objmesh.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/opengl.py` & `FlagCapture-0.1.9/FlagCapture/opengl.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/params.py` & `FlagCapture-0.1.9/FlagCapture/params.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/utils.py` & `FlagCapture-0.1.9/FlagCapture/utils.py`

 * *Files identical despite different names*

### Comparing `FlagCapture-0.1.8/FlagCapture/wrappers.py` & `FlagCapture-0.1.9/FlagCapture/wrappers.py`

 * *Files identical despite different names*

