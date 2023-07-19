# Comparing `tmp/sac_tello-0.0.9.tar.gz` & `tmp/sac_tello-0.1.0.tar.gz`

## Comparing `sac_tello-0.0.9.tar` & `sac_tello-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/SAC-Tello.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/vcs.xml
--rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/workspace.xml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/dictionaries/Michael.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/face_encoder.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_cmd.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_drive.py
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_drone.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_face_hud.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_hud.py
--rw-r--r--   0        0        0    11207 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_rc.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_remote.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_state.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_video.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.9/LICENSE
--rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 sac_tello-0.0.9/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    48264 2020-02-02 00:00:00.000000 sac_tello-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/SAC-Tello.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/__init__.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/face_encoder.py
+-rw-r--r--   0        0        0    18650 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_cmd.py
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_drone.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_face_hud.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_hud.py
+-rw-r--r--   0        0        0    16901 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_rc.py
+-rw-r--r--   0        0        0    10639 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_remote.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_state.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 sac_tello-0.1.0/SAC_Tello/tello_video.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.1.0/LICENSE
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 sac_tello-0.1.0/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 sac_tello-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    51363 2020-02-02 00:00:00.000000 sac_tello-0.1.0/PKG-INFO
```

### Comparing `sac_tello-0.0.9/sac_tello/face_encoder.py` & `sac_tello-0.1.0/SAC_Tello/face_encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,86 +4,91 @@
 # License: GNU GPLv3
 # Created On: 29 Jun 2023
 # Purpose:
 #   A simple face recognition suite.
 # Notes:
 
 import pickle
-import numpy as np
+from numpy import ones
 from face_recognition import face_encodings, face_locations, face_distance
 import cv2
 
 
 class FaceEncoder:
     # Precond:
     #   encode is a string containing a file name to load a set of encodings from.
     #
     # Postcond:
     #   Creates a new FaceEncoder object loaded with encodings from a given file.
     def __init__(self, load_file=None):
         self.encodings = {}
         # Speed upgrades
-        self.encode_scale = 1 / 4
+        self.encode_scale = 4
         if load_file is not None:
             self.load(load_file)
 
     # Precond:
     #   name is a string containing the name of the person whose face is being encoded.
     #   img_file is a string containing the name of a file containing an image of a single
     #       person's face.
     #
     # Postcond:
     #   Updates the encodings based on the image file.
     #   Returns False if no face was found.
     def encode_face(self, name, img_file):
-        img = cv2.imread(img_file)
-        img = cv2.resize(img, (640*self.encode_scale, 480*self.encode_scale))
+        img = self.__scale_image(cv2.imread(img_file))
         if name not in self.encodings:
             self.encodings[name] = []
-        location = face_locations(img)
-        if len(location) > 0:
-            location = location[0]
-            encoding = face_encodings(img, location)[0]
+        locations = face_locations(img)
+        if len(locations) > 0:
+            location = locations[0]
+            encoding = face_encodings(img, [location], model='large')[0]
             self.encodings[name].append(encoding)
             return True
         return False
     
     # Precond:
     #   img is a valid ndarray representing an image.
     #   min_dist is a floating point number indicating the minimal face distance (default: 0.6) for recognition.
     #
     # Postcond:
     #   Returns the most likely name of the faces in the image, paired with their locations.
     #   If no face matches within the specified distance, then it is labeled Unknown.
     #   Returned tuples are (name, location)
     def detect_faces(self, img, min_dist=0.6):
-        img = cv2.resize(img, (640 * self.encode_scale, 480 * self.encode_scale))
+        img = self.__scale_image(img)
         locations = face_locations(img)
+        if len(locations) == 0:
+            return []
+        if len(self.encodings.keys()) == 0:
+            idents = ['unknown' for i in range(len(locations))]
+            locations = list(map(self.__unscale_rect, locations))
+            return list(zip(idents, locations))
         encodings = face_encodings(img, locations)
         names = list(self.encodings.keys())
-        distances = np.ones(len(names))
+        distances = ones(len(names))
         idents = []
         for encoding in encodings:
             for idx, name in enumerate(names):
-                distances[idx] = face_distance(self.encodings[name], encoding).min()
-            if distances.min() > min_dist:
+                distances[idx] = face_distance(self.encodings[name], encoding).mean()
+            if distances.min(initial=1.0) > min_dist:
                 idents.append("unknown")
             else:
                 idents.append(names[distances.argmin()])
-        return zip(idents, locations)
+        locations = list(map(self.__unscale_rect, locations))
+        return list(zip(idents, locations))
 
     # Precond:
     #   filename is the path to a file which contains serialized face encodings.
     #
     # Postcond:
     #   Updates the recognizers encodings using the provided file.
     # Note:
     #   No exceptions handled by this method.
     def load(self, filename):
-        loaded = {}
         with open(filename, 'rb') as fin:
             loaded = pickle.load(fin)
         for person in loaded:
             if person not in self.encodings:
                 self.encodings[person] = []
             self.encodings[person].extend(loaded[person])
 
@@ -93,8 +98,26 @@
     # Postcond:
     #   Saves the known face encodings to the provided file.
     # Note:
     #   No exceptions handled by this method.
     def save(self, filename):
         with open(filename, 'wb') as fout:
             pickle.dump(self.encodings, fout)
-        
+        
+    # Precond:
+    #   location is a rectangle on the resized image.
+    #
+    # Postcond:
+    #   Returns a rectangle on the non-scaled image.
+    def __unscale_rect(self, location):
+        return tuple(map(lambda x: int(x * self.encode_scale), location))
+    
+    # Precond:
+    #   img is a numpy array representing an image.
+    #
+    # Postcond:
+    #   Returns a resized image by the encoder's scale factor.
+    def __scale_image(self, img):
+        height = 720 // self.encode_scale
+        width = 960 // self.encode_scale
+        return cv2.resize(img, (width, height))
+
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_cmd.py` & `sac_tello-0.1.0/SAC_Tello/tello_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 #       backward <dist>:  Moves the Tello backward <dist> cm.
 #       rotates [cw, ccw] <deg>: Rotates the Tello <deg> degrees [cw, ccw].
 #       flip [f, b, l, r]: Flips the drone in a direction ([f, b, l, r]).
 #       move <x> <y> <z> <spd>: Moves the Tello by the given (x, y, z) in cm at speed spd.
 #       stream [on, off]: Turns the Tello video stream [on, off].
 #       emergency: send command to shut down Tello (no confirmation).
 
-import multiprocessing as mp
+from multiprocessing import Queue
 from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
 from time import perf_counter
 from datetime import datetime
-import queue
+from queue import Empty
 import os
 
 
-def tello_command_loop(cmd_q: mp.Queue, conf_q: mp.Queue):
+def tello_command_loop(cmd_q: Queue, conf_q: Queue):
     # Create a management object
     manager = TelloCmd()
     res = manager.startup()
     conf_q.put((res, 'startup'))
     if not res:
         return
     running = True
@@ -94,37 +94,49 @@
                         res = manager.flip_forward()
                     elif cmd[1] == 'b':
                         res = manager.flip_backward()
                     elif cmd[1] == 'l':
                         res = manager.flip_left()
                     elif cmd[1] == 'r':
                         res = manager.flip_right()
-                elif cmd[0] == "move":
+                elif cmd[0] == "go":
                     res = manager.move(int(cmd[1]),
                                        int(cmd[2]),
                                        int(cmd[3]),
                                        int(cmd[4]))
                     conf_q.put((res, 'move'))
+                elif cmd[0] == "curve":
+                    res = manager.curve(int(cmd[1]),
+                                        int(cmd[2]),
+                                        int(cmd[3]),
+                                        int(cmd[4]),
+                                        int(cmd[5]),
+                                        int(cmd[6]),
+                                        int(cmd[7]))
+                    conf_q.put((res, 'curve'))
                 elif cmd[0] == "stream":
                     if cmd[1] == "on":
                         res = manager.stream_on()
                         conf_q.put((res, 'stream on'))
                     elif cmd[1] == "off":
                         res = manager.stream_on()
                         conf_q.put((res, 'stream off'))
                 elif cmd[0] == "emergency":
                     manager.emergency()
+                    conf_q.put((True, "Emergency"))
+                else:
+                    conf_q.put((False, "Unknown"))
             except ValueError:
                 conf_q.put((False, 'Invalid Argument'))
-        except queue.Empty:
+        except Empty:
             pass
     try:
         while not cmd_q.empty():
             cmd_q.get_nowait()
-    except queue.Empty:
+    except Empty:
         pass
     cmd_q.close()
     manager.close()
     
 
 # Class for handling sending Tello commands and logging data.
 class TelloCmd:
@@ -340,21 +352,50 @@
     #   spd is the speed of movement
     #
     # Postcond:
     #   Moves the drone by the given x, y, and z values.
     #   Returns False if the command could not be sent or executed for any
     #       reason.
     def move(self, x, y, z, spd):
-        if not self.connected or not (20 < max(abs(x), abs(y), abs(z)) < 500) or spd not in range(10, 101):
+        if (not self.connected) or (not (20 < max(abs(x), abs(y), abs(z)) < 500)) or (spd not in range(10, 101)):
             return False
-        coord_str = ' '.join([str(x), str(y), str(z)])
+        coord_str = ' '.join([str(x), str(y), str(z), str(spd)])
         res = self.__send("go " + coord_str)
         return res is not None and res == 'ok'
 
     # Precond:
+    #   x1 the x coordinate of the point to curve through.
+    #   y1 the y coordinate of the point to curve through.
+    #   z1 the z coordinate of the point to curve through.
+    #   x2 the final amount to move in the x-axis.
+    #   y2 the final amount to move in the y-axis.
+    #   z2 the final amount to move in the z-axis.
+    #   spd is the speed of movement
+    #
+    # Postcond:
+    #   Moves the drone in a curve defined by the current and two given
+    #   coordinates.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
+    def curve(self, x1, y1, z1, x2, y2, z2, spd):
+        p1 = (x1, y1, z1)
+        p2 = (x2, y2, z2)
+        in_range = True
+        for coord in p1:
+            in_range = in_range and (20 <= abs(coord) <= 500)
+        for coord in p2:
+            in_range = in_range and (20 <= abs(coord) <= 500)
+        if (not self.connected) or not in_range or (spd not in range(10, 61)):
+            return False
+        coord_str = list(map(str, p1)) + list(map(str, p2)) + [str(spd)]
+        coord_str = ' '.join(coord_str)
+        res = self.__send("curve " + coord_str)
+        return res is not None and res == 'ok'
+
+    # Precond:
     #   None.
     #
     # Postcond:
     #   Sends the emergency command, in triplicate. Does not wait for response.
     def emergency(self):
         for _ in range(3):
             self.__send_nowait("emergency")
@@ -458,8 +499,12 @@
         while not self.stop:
             try:
                 response, ip = self.send_channel.recvfrom(1024)
                 response = response.decode('utf-8')
                 self.log[-1][1] = response.strip()
             except OSError as exc:
                 if not self.stop:
-                    print("Caught exception socket.error : %s" % exc)
+                    print("Caught exception socket.error : %s" % exc)
+            except UnicodeDecodeError as dec:
+                if not self.stop:
+                    self.log[-1][1] = "Decode Error"
+                    print("Caught exception Unicode 0xcc error.")
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_drone.py` & `sac_tello-0.1.0/SAC_Tello/tello_drone.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 # Purpose:
 #   A basic method of controlling a Tello Drone and allowing a video feed.
 #
 # Notes:
 #   Some code inspired/borrowed from: github.com/dji-sdk/Tello-Python/
 
 
-import multiprocessing as mp
-import queue
+# import multiprocessing as mp
+from multiprocessing import Process, Queue
+from queue import Empty
 from time import sleep
-import sys
+from sys import stderr
 from threading import Thread
 
 from .tello_cmd import tello_command_loop
 from .tello_state import tello_state_loop
 from .tello_video import tello_video_loop
 
 
@@ -26,40 +27,34 @@
     # Precond:
     #   The computer creating the TelloDrone instance is connected to the Tello's Wi-Fi.
     #
     # Postcond:
     #   Sets up a connection with the Tello Drone.
     def __init__(self):
         # Setup command process
-        self.cmdQ = mp.Queue()
-        self.cmd_confQ = mp.Queue()
-        self.cmd_process = mp.Process(target=tello_command_loop, args=(self.cmdQ, self.cmd_confQ))
-        self.cmd_process.daemon = True
+        self.cmdQ = Queue(2)
+        self.cmd_confQ = Queue(2)
+        self.cmd_process = Process(target=tello_command_loop, args=(self.cmdQ, self.cmd_confQ))
         self.cmd_thread = Thread(target=self.__cmd_thread)
-        self.cmd_thread.daemon = True
         
         # Setup state process
-        self.state_haltQ = mp.Queue()
-        self.state_recQ = mp.Queue()
-        self.state_process = mp.Process(target=tello_state_loop, args=(self.state_haltQ, self.state_recQ))
-        self.state_process.daemon = True
+        self.state_haltQ = Queue(2)
+        self.state_recQ = Queue(2)
+        self.state_process = Process(target=tello_state_loop, args=(self.state_haltQ, self.state_recQ))
         self.state_thread = Thread(target=self.__state_thread)
-        self.state_thread.daemon = True
 
         # Setup video process
-        self.video_haltQ = mp.Queue()
-        self.video_recQ = mp.Queue()
-        self.video_process = mp.Process(target=tello_video_loop, args=(self.video_haltQ, self.video_recQ))
-        self.video_process.daemon = True
+        self.video_haltQ = Queue(2)
+        self.video_recQ = Queue(2)
+        self.video_process = Process(target=tello_video_loop, args=(self.video_haltQ, self.video_recQ))
         self.video_thread = Thread(target=self.__video_thread)
-        self.video_thread.daemon = True
         
         # Internal variables
         self.commandQ = []
-        self.commandQ_limit = 10
+        self.commandQ_limit = 100
         self.last_state = None
         self.last_frame = None
         self.running = False
 
     # ==========================
     #   MANAGEMENT METHODS
     # ==========================
@@ -78,24 +73,24 @@
         self.cmd_thread.start()
         self.cmd_process.start()
         # Check to see if connection worked.
         try:
             conf = self.cmd_confQ.get(block=True, timeout=5)
             if not conf[0]:
                 return False
-        except queue.Empty:
+        except Empty:
             return False
 
         # Start the video stream
         self.cmdQ.put("stream on")
         try:
             conf = self.cmd_confQ.get(block=True, timeout=5)
             if not conf[0]:
                 return False
-        except queue.Empty:
+        except Empty:
             return False
         self.state_thread.start()
         self.state_process.start()
         self.video_thread.start()
         self.video_process.start()
         return True
 
@@ -321,14 +316,45 @@
             return False
         coord_str = ' '.join([str(x), str(y), str(z), str(spd)])
         if len(self.commandQ) < self.commandQ_limit:
             self.commandQ.append("go " + coord_str)
             return True
         return False
 
+    # Precond:
+    #   x1 the x coordinate of the point to curve through.
+    #   y1 the y coordinate of the point to curve through.
+    #   z1 the z coordinate of the point to curve through.
+    #   x2 the final amount to move in the x-axis.
+    #   y2 the final amount to move in the y-axis.
+    #   z2 the final amount to move in the z-axis.
+    #   spd is the speed of movement
+    #
+    # Postcond:
+    #   Moves the drone in a curve defined by the current and two given
+    #   coordinates.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
+    def curve(self, x1, y1, z1, x2, y2, z2, spd):
+        p1 = (x1, y1, z1)
+        p2 = (x2, y2, z2)
+        in_range = True
+        for coord in p1:
+            in_range = in_range and (20 <= abs(coord) <= 500)
+        for coord in p2:
+            in_range = in_range and (20 <= abs(coord) <= 500)
+        if not in_range or (spd not in range(10, 61)):
+            return False
+        coord_str = list(map(str, p1)) + list(map(str, p2)) + [str(spd)]
+        coord_str = ' '.join(coord_str)
+        if len(self.commandQ) < self.commandQ_limit:
+            self.commandQ.append("curve " + coord_str)
+            return True
+        return False
+
     # ======================================
     # Info METHODS
     # ======================================
     
     # Precond:
     #   None.
     #
@@ -366,15 +392,15 @@
     #   Thread handling command execution.
     def __cmd_thread(self):
         while self.running:
             if len(self.commandQ) > 0 and self.cmdQ.empty():
                 self.cmdQ.put(self.commandQ.pop(0))
                 conf = self.cmd_confQ.get()
                 if not conf[0]:
-                    print("Problem executing command ", conf[1], file=sys.stderr)
+                    print("Problem executing command ", conf[1], file=stderr)
 
     # Precond:
     #   None.
     #
     # Postcond:
     #   Thread handling state extraction..
     def __state_thread(self):
@@ -391,15 +417,15 @@
             self.last_frame = self.video_recQ.get()
         
     # Precond:
     #   q is a valid mp.Queue object.
     #
     # Postcond:
     #   Clears the q and closes it.
-    def __clear_q(q: mp.Queue):
+    @staticmethod
+    def __clear_q(q: Queue):
         try:
             while not q.empty():
                 q.get_nowait()
-        except queue.Empty:
+        except Empty:
             pass
-        q.close()
-        
+        q.close()
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_face_hud.py` & `sac_tello-0.1.0/SAC_Tello/tello_face_hud.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 # Purpose:
 # Notes:
 
 from .tello_drone import TelloDrone
 from .tello_rc import TelloRC
 from .face_encoder import FaceEncoder
 from time import perf_counter
-import pygame as pg
+from pygame import display, draw, event, Rect, DOUBLEBUF, OPENGLBLIT, QUIT
+from pygame.font import Font, get_default_font
+from pygame.image import frombuffer
 from threading import Thread
 
 
 class TelloFaceHud:
     def __init__(self, drone: TelloDrone | TelloRC, faces: FaceEncoder):
         self.drone = drone
         self.encoder = faces
         self.running = False
         self.hud_thread = Thread(target=self.__hud_stream)
         self.hud_thread.daemon = True
         
         #pg reqs
-        self.font = pg.font.Font(pg.font.get_default_font(), 16)
+        self.font = Font(get_default_font(), 16)
     
     def activate_hud(self):
         if self.running:
             return
         self.running = True
         self.hud_thread.start()
     
@@ -40,39 +42,39 @@
         self.hud_thread.join()
     
     def is_active(self):
         return self.running
     
     def __hud_stream(self):
         # Setup Pygame
-        pg.display.init()
-        screen = pg.display.set_mode((640, 480))
-        pg.font.init()
-        hud_font = pg.font.Font(pg.font.get_default_font(), 20)
+        screen = display.set_mode((960, 720))
+        display.set_caption("Tello HUD")
         # Setup video loop basics
         frame_timer = perf_counter()
-        frame_delta = 1 / 24
+        frame_delta = 1 / 30
         while self.running:
             if (perf_counter() - frame_timer) > frame_delta:
                 frame_timer = perf_counter()
-                frame = self.drone.get_frame()
-                if frame is not None:
-                    frame = frame[0]
-                    frame = pg.image.frombuffer(frame.tobytes(), frame.shape[1::-1], "BGR")
+                drone_frame = self.drone.get_frame()
+                if drone_frame is not None:
+                    frame = frombuffer(drone_frame.tobytes(), drone_frame.shape[1::-1], "BGR")
                     screen.blit(frame, (0, 0))
                     # Detect Faces
-                    faces = self.encoder.detect_faces(frame)
+                    faces = self.encoder.detect_faces(drone_frame)
                     for name, location in faces:
                         rect = TelloFaceHud.__convert_rect(location)
-                        pg.draw.rect(frame, (0, 200, 0), rect, 1)
+                        draw.rect(screen, (0, 200, 0), rect, 5)
                         name_text = self.font.render(name, True, (0, 200, 0))
-                        frame.blit(name_text, (rect.x, rect.y-name_text.get_height()-1))
-                pg.display.flip()
-                for event in pg.event.get(pg.QUIT):
+                        screen.blit(name_text, (rect.x, rect.y-name_text.get_height()-1))
+                display.flip()
+                for _ in event.get(QUIT):
                     self.running = False
-        pg.display.quit()
+        display.quit()
     
     @staticmethod
     def __convert_rect(rect):
-        top_left = rect[3], rect[0]
-        width_height = rect[1]-rect[2], rect[2]-rect[0]
-        return pg.Rect(top_left, width_height)
+        left = rect[3]
+        top = rect[0]
+        width = rect[1]-rect[3]
+        height = rect[2]-rect[0]
+        return Rect(left, top, width, height)
+
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_hud.py` & `sac_tello-0.1.0/SAC_Tello/tello_hud.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,128 +6,155 @@
 # Purpose:
 #   A simple hud program that can be run on a separate thread.
 # Notes:
 
 from .tello_drone import TelloDrone
 from .tello_rc import TelloRC
 from time import perf_counter, sleep
-import pygame as pg
+from pygame import display, draw, event, Surface, Vector2, QUIT, SRCALPHA, KEYDOWN, K_p
+from pygame.font import Font, get_default_font
+from pygame.image import frombuffer
 from math import sin, cos, radians
 from threading import Thread
+import uuid
+from cv2 import imwrite
 
 
 class TelloHud:
     def __init__(self, drone: TelloDrone | TelloRC):
         self.drone = drone
         self.running = False
         self.hud_thread = Thread(target=self.__hud_stream)
         self.hud_thread.daemon = True
+        self.hud_font = Font(get_default_font(), 20)
+        # self.hud_thread.daemon = True
         # Create base visuals for hud
         self.hud_rad = 50
-        self.hud_base = pg.Surface((4*self.hud_rad, 4*self.hud_rad), pg.SRCALPHA, 32)
-        hud_center = pg.Vector2(self.hud_base.get_width() // 2, self.hud_base.get_height() // 2)
-        pg.draw.circle(self.hud_base, (0, 0, 0, 100), hud_center, 2*self.hud_rad)
+        self.hud_base = Surface((4 * self.hud_rad, 4 * self.hud_rad), SRCALPHA, 32)
+        hud_center = Vector2(self.hud_base.get_width() // 2, self.hud_base.get_height() // 2)
+        draw.circle(self.hud_base, (0, 0, 0, 100), hud_center, 2 * self.hud_rad)
         # Draw baselines
-        pg.draw.circle(self.hud_base, (0, 200, 0), hud_center, self.hud_rad, self.hud_rad // 10)
+        draw.circle(self.hud_base, (0, 200, 0), hud_center, self.hud_rad, self.hud_rad // 10)
         # Roll baseline
-        roll_baseline = pg.Vector2(cos(0), sin(0))
+        roll_baseline = Vector2(cos(0), sin(0))
         roll_start = (roll_baseline * self.hud_rad) + hud_center
         roll_end = (roll_baseline * (2 * self.hud_rad)) + hud_center
-        pg.draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
+        draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
         roll_baseline - -roll_baseline
         roll_start = (roll_baseline * self.hud_rad) + hud_center
         roll_end = (roll_baseline * (2 * self.hud_rad)) + hud_center
-        pg.draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
+        draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
+        # Pitch indicator
+        draw.line(self.hud_base, (0, 0, 220),
+                  (hud_center.x - self.hud_rad + (self.hud_rad // 10), hud_center.y),
+                  (hud_center.x - (self.hud_rad // 2), hud_center.y), 6)
+        draw.line(self.hud_base, (0, 0, 220),
+                  (hud_center.x + (self.hud_rad // 2), hud_center.y),
+                  (hud_center.x + self.hud_rad - (self.hud_rad // 10), hud_center.y), 6)
     
     def activate_hud(self):
         if self.running:
             return
         self.running = True
         self.hud_thread.start()
-        
+        while self.drone.get_frame() is None:
+            sleep(1)
+    
     def deactivate_hud(self):
         if not self.running:
             if self.hud_thread.is_alive():
                 self.hud_thread.join()
             return
         self.running = False
         self.hud_thread.join()
-        
+    
     def is_active(self):
         return self.running
     
     def __hud_stream(self):
         # Setup Pygame
-        pg.display.init()
-        screen = pg.display.set_mode((640, 480))
-        pg.font.init()
-        hud_font = pg.font.Font(pg.font.get_default_font(), 20)
+        screen = display.set_mode((960, 720))
+        display.set_caption("Tello HUD")
         # Setup video loop basics
         frame_timer = perf_counter()
-        frame_delta = 1/30
+        frame_delta = 1 / 30
+        event.set_allowed([QUIT, KEYDOWN])
+        horizon_rad = 50
+        horizon_size = 4 * horizon_rad
+        horizon_placement = ((screen.get_width() - horizon_size) // 2, (screen.get_height() - horizon_size) // 2)
         while self.running:
-            if (perf_counter() - frame_timer) > frame_delta:
+            delta = perf_counter() - frame_timer
+            if delta >= frame_delta:
                 frame_timer = perf_counter()
+                screen.fill((0, 0, 0, 255))
                 frame = self.drone.get_frame()
                 if frame is not None:
-                    frame = frame[0]
-                    frame = pg.image.frombuffer(frame.tobytes(), frame.shape[1::-1], "BGR")
-                    screen.blit(frame, (0, 0))
-                state = self.drone.get_state()
-                if state is not None:
-                    state = state[0]
-                    bat_text = hud_font.render(f"Battery: {state['bat']:4}", True, (0, 200, 0), (0, 0, 0))
-                    screen.blit(bat_text, (0, 0))
-                    height_text = hud_font.render(f"ToF: {state['tof']:4}", True, (0, 200, 0), (0, 0, 0))
-                    screen.blit(height_text, (0, bat_text.get_height()))
-                    horizon = self.__artificial_horizon(50, int(state['pitch']), int(state['roll']))
-                    horizon_pos = (screen.get_width() - horizon.get_width())//2, (screen.get_height() - horizon.get_height())//2
-                    screen.blit(horizon, horizon_pos)
-                pg.display.flip()
-                for event in pg.event.get(pg.QUIT):
+                    screen.blit(frombuffer(frame.tobytes(), frame.shape[1::-1], "BGR"), (0, 0))
+                    state = self.drone.get_state()
+                    if state is not None:
+                        fps_text = self.hud_font.render(f"FPS: {int(1 / delta):4}", True, (0, 200, 0), (0, 0, 0))
+                        bat_text = self.hud_font.render(f"Battery: {state['bat']:4}", True, (0, 200, 0), (0, 0, 0))
+                        height_text = self.hud_font.render(f"ToF: {state['tof']:4}", True, (0, 200, 0), (0, 0, 0))
+                        horizon = self.__artificial_horizon(horizon_rad, int(state['pitch']), int(state['roll']))
+                        screen.blits([
+                            (fps_text, (0, 0)),
+                            (bat_text, (0, fps_text.get_height())),
+                            (height_text, (bat_text.get_width(), fps_text.get_height())),
+                            (horizon, horizon_placement)
+                        ])
+                else:
+                    init_text = self.hud_font.render("Initializing...", True, (0, 200, 0), (9, 0, 0))
+                    x = (screen.get_width() - init_text.get_width()) // 2
+                    y = (screen.get_height() - init_text.get_height()) // 2
+                    screen.blit(init_text, (x, y))
+                display.flip()
+                for _ in event.get(QUIT):
                     self.running = False
-        pg.display.quit()
-        
+                for evt in event.get(KEYDOWN):
+                    if evt.key == K_p:
+                        filename = str(uuid.uuid4()) + '.jpg'
+                        imwrite(filename, frame)
+                        
+    
     def __artificial_horizon(self, rad: int, pitch: int, roll: int):
-        result = pg.surface.Surface((4*rad, 4*rad), pg.SRCALPHA, 32)
+        result = Surface((4 * rad, 4 * rad), SRCALPHA, 32)
         result.blit(self.hud_base, (0, 0))
-        center = pg.Vector2(result.get_width() // 2, result.get_height() // 2)
-        # Draw roll lines]
+        center = Vector2(result.get_width() // 2, result.get_height() // 2)
+        # Draw roll lines
         left_ang = radians(180 + roll)
-        left_vec = pg.Vector2(cos(left_ang), sin(left_ang))
+        left_vec = Vector2(cos(left_ang), sin(left_ang))
         left_start = left_vec * rad
-        left_end = left_vec * (rad*2)
+        left_end = left_vec * (rad * 2)
         left_start = left_start + center
         left_end = left_end + center
-        pg.draw.line(result, (0, 200, 0), left_start, left_end, 3)
+        draw.line(result, (0, 200, 0), left_start, left_end, 3)
         right_ang = radians(roll)
-        right_vec = pg.Vector2(cos(right_ang), sin(right_ang))
+        right_vec = Vector2(cos(right_ang), sin(right_ang))
         right_start = right_vec * rad
         right_end = right_vec * rad * 2
         right_start = right_start + center
         right_end = right_end + center
-        pg.draw.line(result, (0, 200, 0), right_start, right_end, 3)
+        draw.line(result, (0, 200, 0), right_start, right_end, 3)
         # Draw Pitch lines
-        pitch = -pitch # Line direction adjustment
+        pitch = -pitch  # Line direction adjustment
         pitch_line_deg = 10
-        pitch_lines = pg.Surface((rad, rad), pg.SRCALPHA)
+        pitch_lines = Surface((rad, rad), SRCALPHA)
         pixels_per_ang = 2
-        start_angle = pitch - ((pitch_lines.get_height()//2)//pixels_per_ang)
+        start_angle = pitch - ((pitch_lines.get_height() // 2) // pixels_per_ang)
         pixel_start = pitch_line_deg - (start_angle % pitch_line_deg)
         pixel_start = pixel_start * pixels_per_ang
         angles = []
-        for i in range(pixel_start, pitch_lines.get_height(), pitch_line_deg*pixels_per_ang):
+        for i in range(pixel_start, pitch_lines.get_height(), pitch_line_deg * pixels_per_ang):
             ang = start_angle + (i // pixels_per_ang)
             angles.append(ang)
             if ang % pitch_line_deg == 0:
                 if ang != 0:
-                    pg.draw.line(pitch_lines, (0, 200, 0), (0, i), (pitch_lines.get_width(), i), 3)
+                    draw.line(pitch_lines, (0, 200, 0), (0, i), (pitch_lines.get_width(), i), 3)
                 else:
-                    pg.draw.line(pitch_lines, (200, 0, 0), (0, i), (pitch_lines.get_width(), i), 3)
-        line_adj = pg.Vector2(-(pitch_lines.get_width()//2), -(pitch_lines.get_height()//2))
+                    draw.line(pitch_lines, (200, 0, 0), (0, i), (pitch_lines.get_width(), i), 3)
+        line_adj = Vector2(-(pitch_lines.get_width() // 2), -(pitch_lines.get_height() // 2))
         center_pitch = center + line_adj
         # Current Pitch indicator
-        indicator_height = pitch_lines.get_height()//2
-        pg.draw.line(pitch_lines, (0, 0, 200), (0, indicator_height), (pitch_lines.get_width(), indicator_height), 3)
+        indicator_height = pitch_lines.get_height() // 2
+        draw.line(pitch_lines, (0, 0, 200), (0, indicator_height), (pitch_lines.get_width(), indicator_height), 3)
         result.blit(pitch_lines, center_pitch)
         return result
-
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_rc.py` & `sac_tello-0.1.0/SAC_Tello/tello_remote.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,344 +1,347 @@
-# File: tello_rc.py
+# File: tello_remote.py
 # Author: Michael Huelsman
 # Copyright: Dr. Michael Andrew Huelsman 2023
 # License: GNU GPLv3
 # Created On: 29 Jun 2023
 # Purpose:
-#   A class for handling a multi-processed tello drone using keyboard controls.
+#   A class and function for handling a multi-processed rc tello controller.
 # Notes:
 
-
-import multiprocessing as mp
-import queue
-from time import perf_counter
-from math import log1p
-import pygame as pg
-import sys
+from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
+from time import perf_counter, sleep
+from multiprocessing import Queue
+from queue import Empty
+
+
+def tello_remote_loop(rc_q: Queue, conf_q: Queue):
+    # Create a management object
+    manager = TelloRemote()
+    res = manager.startup()
+    conf_q.put((res, 'startup'))
+    if not res:
+        return
+    running = True
+    while running:
+        # Grab from the rcQ
+        if not rc_q.empty():
+            current = rc_q.get()
+            if type(current) == str:
+                if current == "halt":
+                    running = False
+                elif current == "takeoff":
+                    conf_q.put((manager.takeoff(), 'takeoff'))
+                elif current == "land":
+                    conf_q.put((manager.land(), 'land'))
+                elif current == "emergency":
+                    conf_q.put((manager.emergency(), 'emergency'))
+                elif current == "flip f":
+                    conf_q.put((manager.flip_forward(), 'flip f'))
+                elif current == "flip b":
+                    conf_q.put((manager.flip_backward(), 'flip b'))
+                elif current == "flip r":
+                    conf_q.put((manager.flip_right(), 'flip r'))
+                elif current == "flip l":
+                    conf_q.put((manager.flip_left(), 'flip l'))
+            elif type(current) == tuple:
+                manager.set_rc(*current)
+    try:
+        while not rc_q.empty():
+            rc_q.get_nowait()
+    except Empty:
+        pass
+    rc_q.close()
+    manager.close()
+    
 
-from .tello_remote import tello_remote_loop
-from .tello_state import tello_state_loop
-from .tello_video import tello_video_loop
+class TelloRemote:
+    def __init__(self):
+        # Addresses
+        self.local_addr = ('', 8889)
+        self.tello_addr = ('192.168.10.1', 8889)
+    
+        # Setup channels
+        self.send_channel = socket(AF_INET, SOCK_DGRAM)
+        self.send_channel.bind(self.local_addr)
+    
+        self.stop = True
+        self.connected = False
+    
+        # Setup receiving thread
+        self.receive_thread = Thread(target=self.__receive)
+        self.receive_thread.daemon = True
+    
+        # Setup logs
+        self.log = []
+        self.rc = [0, 0, 0, 0]
+        self.MAX_TIME_OUT = 10  # measured in seconds
+        self.rc_tick = 10
+        self.waiting = False
+        self.last_beat = perf_counter()
+    
+    def startup(self):
+        self.stop = False
+        self.receive_thread.start()
+        # self.rc_beat_thread.start()
+        if self.__connect(5):
+            self.stream_on()
+            return True
+        return False
+    
+    # ======================================
+    # COMMAND METHODS
+    # ======================================
 
+    # Precond:
+    #   The value to set the forward throttle to.
+    #
+    # Postcond:
+    #   Set forward throttle.
+    def set_x(self, val):
+        nv = min(max(-100, int(val)), 100)
+        if nv != self.rc[1]:
+            self.rc[1] = nv
+            self.__send_rc()
 
-class TelloRC:
     # Precond:
-    #   The computer creating the TelloDrone instance is connected to the Tello's Wi-Fi.
+    #   The value to set the right throttle to.
     #
     # Postcond:
-    #   Sets up a connection with the Tello Drone.
-    def __init__(self):
-        # Setup command process
-        self.rcQ = mp.Queue()
-        self.rc_confQ = mp.Queue()
-        self.rc_process = mp.Process(target=tello_remote_loop, args=(self.rcQ, self.rc_confQ))
-        self.rc_process.daemon = True
-        
-        # Setup state process
-        self.state_haltQ = mp.Queue()
-        self.state_recQ = mp.Queue()
-        self.state_process = mp.Process(target=tello_state_loop, args=(self.state_haltQ, self.state_recQ))
-        self.state_process.daemon = True
-        self.state_thread = Thread(target=self.__state_thread)
-        self.state_thread.daemon = True
-        
-        # Setup video process
-        self.video_haltQ = mp.Queue()
-        self.video_recQ = mp.Queue()
-        self.video_process = mp.Process(target=tello_video_loop, args=(self.video_haltQ, self.video_recQ))
-        self.video_process.daemon = True
-        self.video_thread = Thread(target=self.__video_thread)
-        self.video_thread.daemon = True
-        
-        # Internal variables
-        self.current_rc = [0, 0, 0, 0]
-        self.last_state = None
-        self.last_frame = None
-        self.running = False
-        self.vel_timing = 10
-
-    # ==========================
-    #   MANAGEMENT METHODS
-    # ==========================
+    #   Set right throttle.
+    def set_y(self, val):
+        nv = min(max(-100, int(val)), 100)
+        if nv != self.rc[1]:
+            self.rc[0] = nv
+            self.__send_rc()
 
     # Precond:
-    #   None.
+    #   The value to set the vertical throttle to.
     #
     # Postcond:
-    #   Starts the TelloRC object.
-    #   Connects to the Tello.
-    #   Connects to all streams and begins all processes.
-    #   Returns True if all processes have been started.
-    def start(self):
-        self.running = True
-        self.rc_process.start()
-        self.state_thread.start()
-        self.state_process.start()
-        self.video_thread.start()
-        self.video_process.start()
-        return True
-    
-    def control(self):
-        # Setup
-        key_holds = {'w': 0, 's': 0, 'd': 0, 'a': 0, 'q': 0, 'e': 0, 'r': 0, 'f': 0}
-        poll_timer = perf_counter()
-        poll_delta = 1/30
-        # Main Loop
-        control_running = True
-        pg.init()
-        while control_running:
-            delta = perf_counter() - poll_timer
-            if delta >= poll_delta:
-                # Check for events
-                command_sent = False
-                for event in pg.event.get(pg.KEYDOWN):
-                    if event.key == pg.K_t:
-                        command_sent = True
-                        if not self.takeoff():
-                            print("Problem with takeoff!")
-                    elif event.key == pg.K_l:
-                        command_sent = True
-                        if not self.land():
-                            print("Problem with landing!")
-                    elif event.key == pg.K_ESCAPE:
-                        command_sent = True
-                        if not self.emergency():
-                            print("Problem with emergency shutdown!")
-                    elif event.key == pg.K_BACKSPACE:
-                        control_running = False
-                    elif event.key == pg.K_DELETE:
-                        self.rcQ.put((0, 0, 0, 0))
-                    elif event.key == pg.K_UP:
-                        command_sent = True
-                        if not self.flip_forward():
-                            print("Problem with forward flip!")
-                    elif event.key == pg.K_DOWN:
-                        command_sent = True
-                        if not self.flip_backward():
-                            print("Problem with backward flip!")
-                    elif event.key == pg.K_RIGHT:
-                        command_sent = True
-                        if not self.flip_right():
-                            print("Problem with right flip!")
-                    elif event.key == pg.K_LEFT:
-                        command_sent = True
-                        if not self.flip_left():
-                            print("Problem with left flip!")
-                if command_sent:
-                    poll_timer = perf_counter()
-                    continue
-                # Deal with held keys
-                key_state = pg.key.get_pressed()
-                for key in key_holds:
-                    if key_state[pg.key.key_code(key)]:
-                        key_holds[key] += delta
-                    else:
-                        key_holds[key] -= delta
-                    key_holds[key] = max(0, min(self.vel_timing, key_holds[key]))
-                y = self.__vel_curve(key_holds['w']) - self.__vel_curve(key_holds['s'])
-                x = self.__vel_curve(key_holds['d']) - self.__vel_curve(key_holds['a'])
-                z = self.__vel_curve(key_holds['r']) - self.__vel_curve(key_holds['f'])
-                rot = self.__vel_curve(key_holds['e']) - self.__vel_curve(key_holds['q'])
-                if self.rcQ.empty():
-                    self.rcQ.put((int(x), int(y), int(z), int(rot)))
-    
+    #   Set vertical throttle.
+    def set_z(self, val):
+        nv = min(max(-100, int(val)), 100)
+        if nv != self.rc[1]:
+            self.rc[2] = nv
+            self.__send_rc()
+
     # Precond:
-    #   None.
+    #   The value to set the rotation throttle to.
     #
     # Postcond:
-    #   Closes down communication with the drone and writes the log to a file.
-    def close(self):
-        self.running = False
-        if self.state_thread.is_alive():
-            self.state_thread.join()
-        if self.video_thread.is_alive():
-            self.video_thread.join()
-        if self.video_process.is_alive():
-            self.video_haltQ.put("halt")
-            TelloRC.__clear_q(self.video_recQ)
-            self.video_process.join()
-        if self.state_process.is_alive():
-            self.state_haltQ.put("halt")
-            TelloRC.__clear_q(self.state_recQ)
-            self.state_process.join()
-        if self.rc_process.is_alive():
-            self.rcQ.put("halt")
-            TelloRC.__clear_q(self.rc_confQ)
-            self.rc_process.join()
+    #   Set rotation throttle.
+    def set_rot(self, val):
+        nv = min(max(-100, int(val)), 100)
+        if nv != self.rc[1]:
+            self.rc[3] = nv
+            self.__send_rc()
 
-    # ======================================
-    # COMMAND METHODS
-    # ======================================
-    # Section Notes:
-    #   All commands check to see if the drone has been connected and put into SDK mode before sending commands.
+    # Precond:
+    #   x, y, z, and rot are numberic calues indicating the rc settings.
+    #
+    # Postcond:
+    #   Updates the rc and sends the command if anything has changed.
+    def set_rc(self, x, y, z, rot):
+        nx = min(max(-100, int(x)), 100)
+        ny = min(max(-100, int(y)), 100)
+        nz = min(max(-100, int(z)), 100)
+        nrot = min(max(-100, int(rot)), 100)
+        if [nx, ny, nz, nrot] != self.rc:
+            self.rc = [nx, ny, nz, nrot]
+            self.__send_rc()
 
     # Precond:
     #   None.
     #
     # Postcond
     #   Sends the takeoff command.
     #   If a non-okay response is given returns False, otherwise returns true.
     def takeoff(self):
-        self.rcQ.put("takeoff")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
+        res = self.__send("takeoff")
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond
     #   Sends the land command.
     #   If a non-okay response is given returns False, otherwise returns true.
     def land(self):
-        self.rcQ.put("land")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
+        res = self.__send("land")
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Sends the emergency command, in triplicate. Does not wait for response.
-    def emergency(self):
-        self.rcQ.put("emergency")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
-            return False
-        return True
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Adds flip l command to the command queue.
+    #   Flips the drone left.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
     def flip_left(self):
-        self.rcQ.put("flip l")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
+        res = self.__send("flip l")
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Adds flip r command to the command queue.
+    #   Flips the drone right.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
     def flip_right(self):
-        self.rcQ.put("flip r")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
+        res = self.__send("flip r")
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Adds flip f command to the command queue.
+    #   Flips the drone forward.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
     def flip_forward(self):
-        self.rcQ.put("flip f")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
+        res = self.__send("flip f")
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Adds flip b command to the command queue.
+    #   Flips the drone backward.
+    #   Returns False if the command could not be sent or executed for any
+    #       reason.
     def flip_backward(self):
-        self.rcQ.put("flip b")
-        try:
-            conf = self.rc_confQ.get(block=True, timeout=5)
-            if not conf[0]:
-                return False
-        except queue.Empty:
+        if not self.connected:
             return False
-        return True
-
-    # ======================================
-    # Info METHODS
-    # ======================================
-
+        res = self.__send("flip b")
+        return res is not None and res == 'ok'
+    
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Returns the last frame taken by the Tello.
-    #   Returns None if the stream is off.
-    def get_frame(self):
-        return self.last_frame
-
+    #   Sends the emergency command, in triplicate. Does not wait for response.
+    def emergency(self):
+        for _ in range(3):
+            self.__send_nowait("emergency")
+    
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Returns the last state received from the Tello as a dictionary.
-    def get_state(self):
-        return self.last_state
-
+    #   Sends a command to the Tello turning its video stream on.
+    def stream_on(self):
+        res = self.__send("streamon")
+        return res is not None and res == 'ok'
+    
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Sends a command to the Tello turing its video stream off.
+    def stream_off(self):
+        res = self.__send("streamoff")
+        return res is not None and res == 'ok'
+    
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Closes down communication with the drone and writes the log to a file.
+    def close(self):
+        self.stop = True
+        self.send_channel.close()
+        if self.receive_thread.is_alive():
+            self.receive_thread.join()
+    
     # ======================================
     # PRIVATE METHODS
     # ======================================
-
+    
     # Precond:
-    #   None.
+    #   attempts is the number of times to try and connect.
     #
     # Postcond:
-    #   Thread handling state extraction..
-    def __state_thread(self):
-        while self.running:
-            self.last_state = self.state_recQ.get()
-
+    #   Checks connection to the drone by sending a message to
+    #     switch the drone into SDK mode.
+    #   Returns true if the connection was made.
+    #   Returns false if there was a problem connecting and attempts were
+    #       exceeded.
+    def __connect(self, attempts=5):
+        for _ in range(attempts):
+            res = self.__send("command")
+            if res is not None and res == 'ok':
+                self.connected = True
+                return True
+        return False
+    
     # Precond:
-    #   None.
+    #   mess is a string containing the message to send.
     #
     # Postcond:
-    #   Thread handling video extraction.
-    def __video_thread(self):
-        while self.running:
-            self.last_frame = self.video_recQ.get()
-
+    #   Sends the given message to the Tello.
+    #   Returns the response string if the message was received.
+    #   Returns None if the message failed.
+    def __send(self, msg):
+        self.log.append([msg, None])
+        self.send_channel.sendto(msg.encode('utf-8'), self.tello_addr)
+        # Response wait loop
+        start = perf_counter()
+        self.waiting = True
+        while self.log[-1][1] is None:
+            if (perf_counter() - start) > self.MAX_TIME_OUT:
+                self.log[-1][1] = "TIMED OUT"
+                self.waiting = False
+                return None
+        self.waiting = False
+        return self.log[-1][1]
+    
     # Precond:
-    #   q is a valid mp.Queue object.
+    #   mess is a string containing the message to send.
     #
     # Postcond:
-    #   Clears the q and closes it.
-    def __clear_q(q: mp.Queue):
-        try:
-            while not q.empty():
-                q.get_nowait()
-        except queue.Empty:
-            pass
-        q.close()
+    #   Sends the given message to the Tello.
+    #   Does not wait for a response.
+    #   Used (internally) only for sending the emergency signal (which is sent
+    #       in triplicate.)
+    def __send_nowait(self, msg):
+        self.send_channel.sendto(msg.encode('utf-8'), self.tello_addr)
+        return None
     
     # Precond:
-    #   t is a valid floating point value.
+    #   None.
+    #
+    # Postcond:
+    #   Receives messages from the Tello and logs them.
+    def __receive(self):
+        while not self.stop:
+            try:
+                response, ip = self.send_channel.recvfrom(1024)
+                response = response.decode('utf-8')
+                self.log[-1][1] = response.strip()
+            except OSError as exc:
+                if not self.stop:
+                    print("Caught exception socket.error : %s" % exc)
+            except UnicodeDecodeError as dec:
+                if not self.stop:
+                    print("Caught exception Unicode 0xcc error.")
+
+    # Precond:
+    #   None.
     #
     # Postcond:
-    #   Returns the current velocity based on how long a key has  been pressed.
-    def __vel_curve(self, t):
-        return 100 * (log1p(t) / log1p(self.vel_timing))
+    #   Sends RC messages to the tello based on internal throttle numbers.
+    def __send_rc(self):
+        cmd = 'rc ' + ' '.join(map(str, self.rc))
+        self.last_beat = perf_counter()
+        self.__send_nowait(cmd)
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_state.py` & `sac_tello-0.1.0/SAC_Tello/tello_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,61 +17,60 @@
 #   Commands (case insensitive) accepted:
 #       halt: Stops the process and closes the management object.
 
 from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
 from time import perf_counter
 from datetime import datetime
-import multiprocessing as mp
-import queue
+from multiprocessing import Queue
+from queue import Empty
 import os
 
 
-def tello_state_loop(halt_q: mp.Queue, state_q: mp.Queue):
+def tello_state_loop(halt_q: Queue, state_q: Queue):
     # Create a management object.
     manager = TelloState()
     manager.start()
     running = True
     while running:
         try:
-            halt = str(halt_q.get(False))
-            if halt.lower() == 'halt':
-                break
-        except queue.Empty:
+            if not halt_q.empty():
+                halt = str(halt_q.get(False))
+                if halt.lower() == 'halt':
+                    break
+        except Empty:
             pass
         if state_q.empty():
             state = manager.get()
             if state is not None:
                 state_q.put(state)
     try:
         while not state_q.empty():
             state_q.get_nowait()
-    except queue.Empty:
+    except Empty:
         pass
     state_q.close()
     manager.close()
     
 
 # Class for handling receiving the state information from a Tello.
 class TelloState:
     def __init__(self):
         # Running info
         self.stop = False
-        self.last_grab = -1
         self.mission_start = perf_counter()
 
         # Connecting to current state information
         self.state_addr = ('192.168.10.1', 8890)
         self.local_state_addr = ('', 8890)
         self.state_channel = socket(AF_INET, SOCK_DGRAM)
         self.state_channel.bind(self.local_state_addr)
-        self.state_log = []
+        self.state_log = [[None]]
     
         self.receive_state_thread = Thread(target=self.__receive)
-        self.receive_state_thread.daemon = True
 
     # Precond:
     #   None.
     #
     # Postcond:
     #   Starts the state receiving thread.
     def start(self):
@@ -82,18 +81,15 @@
     #   None.
     #
     # Postcond:
     #   Non-blocking function.
     #   Returns the next state
     #   If no new state has been received then None is returned.
     def get(self):
-        if self.last_grab + 1 < len(self.state_log):
-            self.last_grab += 1
-            return self.state_log[self.last_grab]
-        return None
+        return self.state_log[-1][0]
     
     # Precond:
     #   fldr is a string containing the path to the folder to place the log file..
     #
     # Postcond:
     #   Closes the threads and various channel.
     #   Writes out log data.
@@ -103,14 +99,16 @@
         self.receive_state_thread.join()
         t = datetime.now()
         log_name = os.path.join(fldr, t.strftime("%Y-%m-%d_%H-%M-%S") + '-state.log')
         if not os.path.exists(fldr):
             os.mkdir(fldr)
         with open(log_name, 'w') as fout:
             for entry in self.state_log:
+                if entry[0] is None:
+                    continue
                 print("Mission Time(s):", round(entry[1], 3), file=fout)
                 print("State:", entry[0], file=fout)
 
     # Precond:
     #   None.
     #
     # Postcond:
@@ -129,12 +127,8 @@
                     label, val = item.split(':')
                     state[label] = val
                 state_time = perf_counter() - self.mission_start
                 self.state_log.append((state, state_time))
             except OSError as exc:
                 if not self.stop:
                     print("Caught exception socket.error : %s" % exc)
-                    
-                    
-if __name__ == '__main__':
-    mp.freeze_support()
-    
+
```

### Comparing `sac_tello-0.0.9/sac_tello/tello_video.py` & `sac_tello-0.1.0/SAC_Tello/tello_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,42 @@
 #       halt_q: Used by the parent to send commands to the state gatherer.
 #               Commands should be sent as a single string.
 #       conf_q: Used by the child to send the next frame gathered from the Tello.
 #
 #   Commands (case insensitive) accepted:
 #       halt: Stops the process and closes the management object.
 
+
 from threading import Thread
-import multiprocessing as mp
-import cv2
-import queue
+from multiprocessing import Queue
+from queue import Empty
+from cv2 import VideoCapture
+from cv2 import CAP_PROP_FRAME_WIDTH, CAP_PROP_FRAME_HEIGHT, CAP_ANY
+from math import ceil
 
 
-def tello_video_loop(halt_q: mp.Queue, frame_q: mp.Queue):
+def tello_video_loop(halt_q: Queue, frame_q: Queue):
     # Create a management object.
     manager = TelloVideo()
     manager.start()
     running = True
     while running:
         try:
-            halt = str(halt_q.get(False))
-            if halt.lower() == 'halt':
-                break
-        except queue.Empty:
+            if not halt_q.empty():
+                halt = str(halt_q.get(False))
+                if halt.lower() == 'halt':
+                    break
+        except Empty:
             pass
         if frame_q.empty():
-            frame = manager.get()
-            if frame is not None:
-                frame_q.put(frame)
+            frame_q.put( manager.get())
     try:
         while not frame_q.empty():
             frame_q.get_nowait()
-    except queue.Empty:
+    except Empty:
         pass
     frame_q.close()
     manager.close()
 
 
 # Class for handling receiving video frames from a Tello.
 class TelloVideo:
@@ -69,33 +71,29 @@
     #   None.
     #
     # Postcond:
     #   Starts the state receiving thread.
     def start(self):
         # Set up the video stream
         self.stream_active = True
-        self.video_stream = cv2.VideoCapture(self.video_connect_str)
-        self.video_stream.set(cv2.CAP_PROP_BUFFERSIZE, 2)
-        self.frame_width = self.video_stream.get(cv2.CAP_PROP_FRAME_WIDTH)
-        self.frame_height = self.video_stream.get(cv2.CAP_PROP_FRAME_HEIGHT)
+        self.video_stream = VideoCapture(self.video_connect_str, CAP_ANY)
+        self.frame_width = self.video_stream.get(CAP_PROP_FRAME_WIDTH)
+        self.frame_height = self.video_stream.get(CAP_PROP_FRAME_HEIGHT)
         self.video_thread.start()
         self.frame_update = False
     
     # Precond:
     #   None.
     #
     # Postcond:
     #   Non-blocking function.
     #   Returns the most recent frame.
     #   If no new frame has been received then None is returned.
     def get(self):
-        if self.frame_update:
-            self.frame_update = False
-            return self.last_frame
-        return None
+        return self.last_frame
     
     # Precond:
     #   None.
     #
     # Postcond:
     #   Closes the threads and various channels.
     def close(self):
@@ -108,16 +106,9 @@
     #
     # Postcond:
     #   Receives video messages from the Tello.
     def __receive(self):
         while self.stream_active:
             ret, img = self.video_stream.read()
             if ret:
-                self.last_frame = (img, self.frame_width, self.frame_height)
-                self.frame_update = True
-        self.video_stream.release()
-        cv2.destroyAllWindows()
-        
-        
-if __name__ == '__main__':
-    mp.freeze_support()
-    
+                self.last_frame = img
+        self.video_stream.release()
```

### Comparing `sac_tello-0.0.9/.gitignore` & `sac_tello-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.9/LICENSE` & `sac_tello-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.9/pyproject.toml` & `sac_tello-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
+[tool.hatch.build]
+exclude = [
+    "tello_drive.py",
+]
 [project]
 name = "SAC-Tello"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Michael Huelsman", email="michael.huelsman@gmail.com" },
 ]
-description = "A Python-based DJI Tello interface which utilizes parallel processing."
+description = "A Python-based DJI Tello interface which utilizes parallel processing. Created primaily for educational use."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy>=1.23.4",
     "opencv-python>=4.6.0.66",
     "face_recognition>=1.3.0",
-    "pygame>=2.2.0",
+    "pygame>=2.5.0",
 ]
 [project.urls]
 "Homepage" = "https://github.com/xLeachimx/SAC-Tello"
 "Bug Tracker" = "https://github.com/xLeachimx/SAC-Tello/issues"
```

### Comparing `sac_tello-0.0.9/PKG-INFO` & `sac_tello-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SAC-Tello
-Version: 0.0.9
-Summary: A Python-based DJI Tello interface which utilizes parallel processing.
+Version: 0.1.0
+Summary: A Python-based DJI Tello interface which utilizes parallel processing. Created primaily for educational use.
 Project-URL: Homepage, https://github.com/xLeachimx/SAC-Tello
 Project-URL: Bug Tracker, https://github.com/xLeachimx/SAC-Tello/issues
 Author-email: Michael Huelsman <michael.huelsman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,72 +682,84 @@
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: face-recognition>=1.3.0
 Requires-Dist: numpy>=1.23.4
 Requires-Dist: opencv-python>=4.6.0.66
-Requires-Dist: pygame>=2.2.0
+Requires-Dist: pygame>=2.5.0
 Description-Content-Type: text/markdown
 
 # SAC-Tello
 A simple library for controlling a DJI Tello Drone. Built for educational use.
 
 # Dependencies
 
 > numpy>=1.23.4
 > 
 > opencv-python>=4.6.0.66
 > 
 > face_recognition>=1.3.0
 > 
-> pygame>=2.2.0
+> pygame>=2.5.0
 
 ### Install
 SAC-Tello can be installed by running the following command:
 ```commandline
 python3 -m pip install SAC-Tello
 ```
 for MacOS/Linux
 
 Or
 ```commandline
 python -m pip install SAC-Tello
 ```
 for Windows
 
+Note: Some users may have problems installing dependencies such as `opencv-python`
+or `face_recognition` or dependencies of `SAC-Tello` dependencies. We find that
+often this due to external non-python build tools being needed, for example
+`opency-python` needs C++ build tools from Visual Studio to properly install on
+Windows.
+
 # How To Use
 
+Since this package spawns multiple child processes any use of the package must originate from
+a protected starting point (i.e. `if __name__ == __main__:`) or else a Runtime Error **will**
+occur.
+
 ## Tello Drone
 
 The primary interface for the drone is the TelloDrone class.
 
 Creating a TelloDrone object is a simple as the following:
 ```python
 from SAC_Tello import TelloDrone
-drone = TelloDrone()
+if __name__ == '__main__':
+    drone = TelloDrone()
 ``` 
 
 A created drone object does **not** connect to the tello drone. This merely
 sets up everything that needs to be in place **before** a connection is made.
 
 To connect to the Tello, the TelloDrone class has a method called `start()`
 once the Tello is connected **remember** to call the `close()` method when
 done. The `start()` method returns `True` if the connection worked and `False`
 if not.
 
 For example a simple takeoff and land program looks like this:
 ```python
 from SAC_Tello import TelloDrone
-drone = TelloDrone()
-drone.start()
-drone.takeoff()
-drone.land()
-drone.complete()
-drone.close()
+if __name__ == '__main__':
+    drone = TelloDrone()
+    drone.start()
+    drone.takeoff()
+    drone.land()
+    drone.complete()
+    drone.close()
 ```
 
 The following are all commands that can be sent to the Tello:
 
 | Command       | Method        | Arguments                        |
 |---------------|---------------|----------------------------------| 
 | takeoff       | takeoff       | None                             |
@@ -780,114 +792,167 @@
 - Current Time-of-Flight sensor reading
 - Artificial Horizon indicating changes in pitch and roll
 
 To use the HUD simply import and create a `TelloDrone` object and link it
 with a `TelloHud` object:
 ```python
 from SAC_Tello import TelloDrone, TelloHud
-drone = TelloDrone()
-hud = TelloHud(drone)
-drone.start()
-hud.activate_hud()
-hud.deactivate_hud()
-drone.close()
+if __name__ == '__main__':
+    drone = TelloDrone()
+    hud = TelloHud(drone)
+    drone.start()
+    hud.activate_hud()
+    hud.deactivate_hud()
+    drone.close()
 ```
 
 The HUD will launch a separate window when activated. This window can be
 closed at anytime by pressing the `X` in the upper right-hand corner.
 
+Pressing the `P` key while the hud is active and streaming from the Tello will
+save the current frame from the Tello (this will remove all HUD elements.) The
+file will be saved, as a jpeg, in the current working directory using a
+UUID as its name.
+
 Note: Before the HUD is activated nothing will happen. Once the HUD is
 active you will need to deactivate before your program ends.
 
 ## Tello Face Detection
 
 Another feature provided by SAC-Tello is access to face recognition via the
 tello's camera. In order to access the face recognition we must first make
 a `FaceEncoder` object. `FaceEncoder` objects take images and names and log
 a person's facial characteristics for later comparison. To register a face
 with the encoder we need to call the `encode_face` method and give it a name
 and the filename of a image containing that person's face. For example:
 
 ```python
 from SAC_Tello import FaceEncoder
-face_encoder = FaceEncoder()
-face_encoder.encode_face("Jim", "jim_selfie.jpg")
+if __name__ == '__main__':
+    face_encoder = FaceEncoder()
+    face_encoder.encode_face("Jim", "jim_selfie.jpg")
 ```
 
 Once we have given all the faces we want to recognize to the `FaceEncoder`
 object we can pass in the current camera frame from the tello drone. The
 example below simply lists out the names of all people detected by the drone.
 ```python
 from SAC_Tello import FaceEncoder
 from SAC_Tello import TelloDrone
-face_encoder = FaceEncoder()
-face_encoder.encode_face("Jim", "jim_selfie.jpg")
-drone = TelloDrone()
-drone.start()
-while drone.get_frame() is None:
-    pass
-faces = face_encoder.detect_faces(drone.get_frame())
-for name, frame_location in faces:
-    print(name, "is in the frame.")
-drone.close()
+if __name__ == '__main__':
+    face_encoder = FaceEncoder()
+    face_encoder.encode_face("Jim", "jim_selfie.jpg")
+    drone = TelloDrone()
+    drone.start()
+    while drone.get_frame() is None:
+        pass
+    faces = face_encoder.detect_faces(drone.get_frame())
+    for name, frame_location in faces:
+        print(name, "is in the frame.")
+    drone.close()
 ```
 
 Of course this only looks at the first frame from the camera. To make it easier
 to see the face recognition in action SAC-Tello provides a face recognition
 version of the heads-up display. This is contained in the `TelloFaceHud` class
 and works similarly to the `TelloHud` class. For example the following code
-will allow for RC control of the Tello while streaming video that recognizes
-faces and displays names:
+will allow for commands based control of the Tello while streaming video that
+recognizes faces and displays names:
 
 ```python
 from SAC_Tello import FaceEncoder
-from SAC_Tello import TelloRC
+from SAC_Tello import TelloDrone
 from SAC_Tello import TelloFaceHud
-face_encoder = FaceEncoder()
-face_encoder.encode_face("Jim", "jim_selfie.jpg")
-drone = TelloRC()
-hud = TelloFaceHud(drone, face_encoder)
-hud.activate_hud()
-drone.control()
-hud.deactivate_hud()
-drone.close()
+if __name__ == '__main__':
+    face_encoder = FaceEncoder()
+    face_encoder.encode_face("Jim", "jim_selfie.jpg")
+    drone = TelloDrone()
+    hud = TelloFaceHud(drone, face_encoder)
+    hud.activate_hud()
+    drone.takeoff()
+    # insert drone flight commands here
+    drone.land()
+    hud.deactivate_hud()
+    drone.close()
+```
+
+Since encoding faces can take a long time the `FaceEncoder` class gives the
+ability to save and load a set of encodings. Consider the following block of
+code:
+
+```python
+from SAC_Tello import FaceEncoder
+if __name__ == '__main__':
+    face_encoder = FaceEncoder()
+    face_encoder.encode_face("Jim", "jim_selfie.jpg")
+    # Saves the encodings.
+    face_encoder.save("my_encodings.enc")
+    another_encoder = FaceEncoder()
+    another_encoder.load("my_encodings.enc")
 ```
 
-Note: It may take a long time to encode all faces and so you should encode
-faces first, then use them. If a `FaceEncoder` object detects a face it does
-not recognize it will attribute the name `unknown` to it. Face recongition
-in this package not entirely reliable and results may vary.
+This code saves the encodings computed in the first `FaceEndocer` object to the
+file `my_encodings.enc` and then loads them into another `FaceEncoder` object.
+
+If you are going to encode many faces for use with the Tello we suggest you write
+a separate program which encodes all the faces you desire and saves that
+information to a file, then when using the Tello you load that file. This ensures
+the Tello will not automatically shutdown while face encoding is happening.
+
+Notes:
+- It is best to use photos taken by the Tello itself. This helps to reduce the
+potential difference in distortion, resolution, and sapect ratio from affecting
+the accuracy of face recognition.
+- It is possible to assign multiple images to a single name. This will increase
+accuracy of face detection.
+- It may take a long time to encode all faces and so you should encode
+faces first, then use them.
+- As encoding faces takes a long time, it is recommended to encode first, then
+connect to the drone as encoding time may exceed the drone's autoshutoff limit.
+- If a `FaceEncoder` object detects a face it does not recognize it will
+attribute the name `unknown` to it.
+- Detection is not a fast algorithm and while the HUD will attempt 30 frames
+per second, actual refresh rate varies with a number of factors.
+- Face recongition in this package not entirely reliable and results may vary.
 
 ## Tello Remote Control
 
 SAC-Tello also comes with a class for using a ground station computer as
 a remote control for the tello. This remote control can be combined with
 the `TelloHud` class just like the `TelloDrone` class, but we will skip that
 here.
 
 To create and use the remote control simply include the following in your
 program:
 ```python
 from SAC_Tello import TelloRC
-drone = TelloRC()
-drone.start()
-drone.control()
-drone.close()
+if __name__ == '__main__':
+    drone = TelloRC()
+    drone.start()
+    drone.control()
+    drone.close()
 ```
 
+The `TelloRC` class has it's own integrated hud system and does **not** require
+creaton and activation of a separate hud.
+
 The `control()` method begins polling loop for keyboard input. The controls
 are as follows:
 
-| Key Press | Effect                |
-|-----------|-----------------------|
-| T         | Takeoff               |
-| L         | Land                  |
-| ESCAPE    | Emergency Kill Switch | 
-| BACKSPACE | End Remote Control    |
-| DELETE    | Zero Velocity         |
+| Key Press   | Effect                  |
+|-------------|-------------------------|
+| T           | Takeoff                 |
+| L           | Land                    |
+| ESCAPE      | Emergency Kill Switch   | 
+| BACKSPACE   | End Remote Control      |
+| DELETE      | Zero Velocity           |
+| LEFT ARROW  | Flip Drone to the Left  |
+| RIGHT ARROW | Flip Drone to the Right |
+| UP ARROW    | Flip Drone Forward      |
+| DOWN ARROW  | Flip Drone Backeard     |
 
 | Key Held | Effect                      |
 |----------|-----------------------------|
 | W        | Increase Forward Velocity   |
 | A        | Increase Leftward Velocity  |
 | S        | Increase Backward Velocity  |
 | D        | Increase Rightward Velocity |
```

