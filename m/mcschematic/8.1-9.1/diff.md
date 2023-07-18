# Comparing `tmp/mcschematic-8.1.tar.gz` & `tmp/mcschematic-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcschematic-8.1.tar", last modified: Sun Sep 18 20:10:10 2022, max compression
+gzip compressed data, was "mcschematic-9.1.tar", last modified: Tue Sep 20 23:47:56 2022, max compression
```

## Comparing `mcschematic-8.1.tar` & `mcschematic-9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-09-18 20:10:10.496332 mcschematic-8.1/
--rw-rw-rw-   0        0        0     9180 2022-09-18 20:10:10.495836 mcschematic-8.1/PKG-INFO
--rw-rw-rw-   0        0        0     7739 2022-09-17 13:48:20.000000 mcschematic-8.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 20:10:10.490379 mcschematic-8.1/mcschematic/
--rw-rw-rw-   0        0        0       26 2022-08-10 07:33:20.000000 mcschematic-8.1/mcschematic/__init__.py
--rw-rw-rw-   0        0        0   123751 2022-09-18 18:58:14.000000 mcschematic-8.1/mcschematic/mcschematic.py
-drwxrwxrwx   0        0        0        0 2022-09-18 20:10:10.494844 mcschematic-8.1/mcschematic.egg-info/
--rw-rw-rw-   0        0        0     9180 2022-09-18 20:10:10.000000 mcschematic-8.1/mcschematic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2022-09-18 20:10:10.000000 mcschematic-8.1/mcschematic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 20:10:10.000000 mcschematic-8.1/mcschematic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-09-18 20:10:10.000000 mcschematic-8.1/mcschematic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-09-18 20:10:10.000000 mcschematic-8.1/mcschematic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-18 20:10:10.496332 mcschematic-8.1/setup.cfg
--rw-rw-rw-   0        0        0     1131 2022-09-18 20:09:32.000000 mcschematic-8.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-20 23:47:56.076406 mcschematic-9.1/
+-rw-rw-rw-   0        0        0     9180 2022-09-20 23:47:56.076406 mcschematic-9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7739 2022-09-17 13:48:20.000000 mcschematic-9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-09-20 23:47:56.070951 mcschematic-9.1/mcschematic/
+-rw-rw-rw-   0        0        0       26 2022-08-10 07:33:20.000000 mcschematic-9.1/mcschematic/__init__.py
+-rw-rw-rw-   0        0        0   139868 2022-09-20 23:44:28.000000 mcschematic-9.1/mcschematic/mcschematic.py
+drwxrwxrwx   0        0        0        0 2022-09-20 23:47:56.075415 mcschematic-9.1/mcschematic.egg-info/
+-rw-rw-rw-   0        0        0     9180 2022-09-20 23:47:56.000000 mcschematic-9.1/mcschematic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2022-09-20 23:47:56.000000 mcschematic-9.1/mcschematic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-20 23:47:56.000000 mcschematic-9.1/mcschematic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2022-09-20 23:47:56.000000 mcschematic-9.1/mcschematic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-09-20 23:47:56.000000 mcschematic-9.1/mcschematic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-09-20 23:47:56.076406 mcschematic-9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1150 2022-09-20 23:47:45.000000 mcschematic-9.1/setup.py
```

### Comparing `mcschematic-8.1/PKG-INFO` & `mcschematic-9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mcschematic
-Version: 8.1
-Summary: A Minecraft schematic creator library.
+Version: 9.1
+Summary: A Minecraft Schematic creator library.
 Home-page: UNKNOWN
 Author: Sloimay
 Author-email: <sloimayyy@gmail.com>
 License: Apache License 2.0
 Description: ### MCSchematic
```

### Comparing `mcschematic-8.1/README.md` & `mcschematic-9.1/README.md`

 * *Files identical despite different names*

### Comparing `mcschematic-8.1/mcschematic/mcschematic.py` & `mcschematic-9.1/mcschematic/mcschematic.py`

 * *Files 16% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 '''
-import sys
 
 '''
 BY SLOIMAY 2022 :D
 Based on Fearless' implementation that he took from someone else
 that he doesn't remember the name of
 
 Versions (last is current):
@@ -227,133 +226,731 @@
     - New load feature :DDDDDDDDDDDDDDDDDDDD
     - Also new fancy BlockDataDB
     
 8 - 18/09/2022 
     - Made mcschematic 3 to 30 times faster while saving, 
       and 2 to 10 times faster while loading from a file!! :DDDD
     - Also BlockDataDB overhaul!!
+
+9 - 20/09/2022
+    - The editing update!!!
+    - Added a lot of getters
+    - Changed the internals of MCSchematic for the blocks and blockPalettes to be
+      in a form of a MCStructure class, for easier editing
+    - editing tools added:
+        - schematic pasting into another schematic
+        - translation
+        - xyz scaling
+        - naive rotation (no rotation of block states)
+        - flip
 '''
 from enum import Enum
 from typing import Union
 
 import nbtlib
 from nbtlib import File
 from nbtlib.tag import *
 
 import os
 
+from immutable_views import *
+
+import math
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 """
-Represents a minecraft schematic.
+Class representing a Minecraft structure, similar than a .schem format but is easier
+to modify. It's basically structure creator class that holds the blocks, but also
+have really neat tools such as translation, rotation etc..
+Used in the MCSchematic class.
 """
-class MCSchematic:
+class MCStructure:
 
     ### --- Fields
 
-    # The block palette used in this schematic
+    # The block palette used in this structure
     # The key is the block nbt representation and the content is the
     # id. Air is the first id in the palette, for convenience.
     _blockPalette: {Union[str, int]: Union[str, int]} = {'minecraft:air': 0, 0: 'minecraft:air'}
     _blockPaletteFreeId: int = 1
 
     # HashMap of all the blocks, with the key being their position,
     # and the content being the id of the block in the block palette.
     # We don't want to populate _blocks with strings otherwise it's going
     # to use an ungodly amount of RAM for nothing
     _blockStates: {tuple[int, int, int]: int} = {}
 
     # The HashMap of block entities in this schem. We store the string representation
     # for each of them instead of a fancy ID system.
-    # We know we have a block entity when the inputed blockNbt has a { or }.
+    # We know we have a block entity when the inputed blockData has a { or }.
     # The tuple key is the position in the schem, and the value is the blockData str.
     _blockEntities: {tuple[int, int, int]: str} = {}
 
     ### ---
 
 
 
     ### --- Init
 
-    def __init__(self, schematicToLoadPath: str = None):
-        if schematicToLoadPath is None:
-            self._defaultInit(); return
+    def __init__(self):
+        self._blockPalette = {'minecraft:air': 0, 0: 'minecraft:air'}
+        self._blockPaletteFreeId = 1
+        self._blockStates = {}
+        self._blockEntities = {}
+
+    ### ---
+
+
+
+    ### --- Public methods
+
+    '''
+    Sets a block in the schematic at the inputed position.
+    '''
+    def setBlock(self, position: tuple[int, int, int], blockData: str):
+        # We have a different treatment between block entities
+        # and normal blocks.
+        #if not self._isBlockDataBlockEntity(blockData):
+        if blockData[-1] != '}':
+            self._setBlockState(position, blockData)
+        else:
+            self._setBlockEntity(position, blockData)
+
+    '''
+    Returns the blockState at the inputed position, minecraft:air if there isn't.
+    '''
+    def getBlockStateAt(self, position: tuple[int, int, int]) -> str:
+        # If there isn't any blocks at that position, return none
+        if position in self._blockStates:
+            blockPaletteId = self._blockStates[position]
+            return self._blockPalette[blockPaletteId]
+        else:
+            return "minecraft:air"
+
+    '''
+    Return the block data at the inputted position, minecraft:air if there isn't anything.
+    '''
+    def getBlockDataAt(self, position: tuple[int, int, int]) -> str:
+        # The block datas are arranged in a way that blockEntities are a subset
+        # of blockStates with just NBT information. So we check for blockEntities first,
+        # then blockStates and then if nothing comes up we return minecraft:air!
+        if position in self._blockEntities:
+            return self._blockEntities[position]
+        if position in self._blockStates:
+            blockPaletteId = self._blockStates[position]
+            return self._blockPalette[blockPaletteId]
+        return "minecraft:air"
+
+    '''
+    Returns an unmodifiable view of this schematic's current internal block palette, which
+    is how the block palette is represented internally in the schematic object, not how
+    it really gets saved to the schematic file.
+
+    The unmodifiable view is in an attempt to heavily discourage trying to modify the block
+    palette yourself. Do not try to modify the block palette unless you know *exactly* what
+    you're doing.
+    '''
+    def getInternalBlockPalette(self) -> DictView:
+        return DictView(self._blockPalette)
+
+    '''
+    Returns the block palette of this schematic as how it would be saved in the schematic file.
+    Note that this method takes in the internal block palette, and then cleans it up manually
+    everytime it's called, so it can be computationally intensive if the palette is big
+    and it's called a lot.
+    '''
+    def getBlockPalette(self) -> DictView:
+        cleanBlockPalette = \
+            {
+                blockData: Int(blockPaletteId)
+                for blockData, blockPaletteId in self._blockPalette.items()
+                if type(blockData) == str
+            }
+        return DictView(cleanBlockPalette)
+
+    '''
+    Returns an unmodifiable view of the internal blockStates hashmap present in the schematic object.
+    The keys of this dict are the positions of the blockStates, and the values are their ID
+    in the hashmap.
+
+    The unmodifiable view is in an attempt to heavily discourage trying to modify the block
+    palette yourself. Do not try to modify the block palette unless you know *exactly* what
+    you're doing.
+    '''
+    def getBlockStates(self) -> DictView:
+        return DictView(self._blockStates)
+
+    '''
+    Returns an unmodifiable view of the internal blockEntities hashmap present in the schematic object.
+    The keys of this dict are the positions of the blockEntities, and the values are their blockData
+    in the hashmap.
+
+    The unmodifiable view is in an attempt to heavily discourage trying to modify the block
+    palette yourself. Do not try to modify the block palette unless you know *exactly* what
+    you're doing.
+    '''
+    def getBlockEntities(self) -> DictView:
+        return DictView(self._blockEntities)
+
+    '''
+    Computes the -X -Y -Z and +X +Y +Z corners of the structure.
+    Can be thought of as returning the 2 corners of the cuboid
+    containing the structure.
+    
+    Warning: this method can be very computationally intensive, use carefully.
+    '''
+    def getBounds(self) -> tuple[tuple[int, int, int], tuple[int, int, int]]:
+        xMin, yMin, zMin, xMax, yMax, zMax = 0, 0, 0, 0, 0, 0
+
+        keys = self._blockStates.keys()
+
+        for p in keys:
+            if p[0] < xMin:
+                xMin = p[0]
+            elif p[0] > xMax:
+                xMax = p[0]
+
+            if p[1] < yMin:
+                yMin = p[1]
+            elif p[1] > yMax:
+                yMax = p[1]
+
+            if p[2] < zMin:
+                zMin = p[2]
+            elif p[2] > zMax:
+                zMax = p[2]
+
+        return (xMin, yMin, zMin), (xMax, yMax, zMax)
+
+    '''
+    Returns the X, Y and Z length of the structure, from the bounds.
+    We need to input the bounds, because as they're really intensive
+    to calculate, it's the programmer's job
+    '''
+    def getStructureDimensions(self, structureBounds: tuple[tuple[int, int, int], tuple[int, int, int]]) -> tuple[
+        int, int, int]:
+        return structureBounds[1][0] - structureBounds[0][0] + 1, \
+               structureBounds[1][1] - structureBounds[0][1] + 1, \
+               structureBounds[1][2] - structureBounds[0][2] + 1
+
+
+    '''
+    Places the inputted structure inside of this structure, at the inputted position.
+    '''
+    def placeStructure(self, incomingStructure: 'MCStructure', placePosition: tuple[int, int, int]):
+
+        # Go through each block position of the incoming structure and get their block data, then
+        # setBlock in this structure. Not the cheapest way to do it, especially considering
+        # I have access to the internals so I shouldn't have to use setBlock, it's still
+        # easier to implement for now and will probably not be a problem anytime soon.
+        #
+        # Also going through the blockStates, as for each blockEntity, there is an
+        # associated blockState to it, so I don't need to loop over blockEntities too
+        # as I am sure I will loop over every coordinates.
+        for blockPosition, blockState in incomingStructure.getBlockStates().items():
+            # The block data from the incoming structure
+            blockDataHere = incomingStructure.getBlockDataAt(blockPosition)
+            # The position of this blockData but in this structure instead
+            blockPosInThisStructure = (blockPosition[0] + placePosition[0],
+                                       blockPosition[1] + placePosition[1],
+                                       blockPosition[2] + placePosition[2])
+            # Place!
+            self.setBlock(blockPosInThisStructure, blockDataHere)
+
+        # For chaining
+        return self
+
+    '''
+    Makes and returns a deep copy of this structure. So the returned structure
+    won't have its internals shared with the new one, it will have totally new
+    internals. And thus modifying this structure won't affect another one.
+    '''
+    def makeCopy(self) -> 'MCStructure':
+        # Instantiate new structure that we're gonna return
+        newStructure = MCStructure()
+        # Copy the data and put it inside the new structure using
+        # cheeky private member accessing
+        newStructure._blockPalette = self._blockPalette.copy()
+        newStructure._blockPaletteFreeId = self._blockPaletteFreeId
+        newStructure._blockStates = self._blockStates.copy()
+        newStructure._blockEntities = self._blockEntities.copy()
+        # retrun
+        return newStructure
+
+    '''
+    Translates every block in this structure 
+    
+    Can be computationally intensive.
+    '''
+    def translate(self, translationVector: tuple[int, int, int]):
+        # For translation, we create a new blockState and blockEntities hashmap
+        # with every block position translated.
+        # We do it this way because modifying the keys of the hashmap directly
+        # might overwrite already present blocks that have yet to be iterated upon
+
+        newBlockStates = {}
+        newBlockEntities = {}
+
+        # Iterating over states and then testing if this state is
+        # also a blockEntity
+        for blockPosition, blockState in self._blockStates.items():
+
+            # Translate the position and put the block state in the new hashmap
+            translatedPosition = (blockPosition[0] + translationVector[0],
+                                  blockPosition[1] + translationVector[1],
+                                  blockPosition[2] + translationVector[2])
+            newBlockStates[translatedPosition] = blockState
+
+            # See if this blockState is also a block entity, if so put it in
+            # the new BE hashmap
+            if blockPosition in self._blockEntities:
+                blockEntityData = self._blockEntities[blockPosition]
+                newBlockEntities[translatedPosition] = blockEntityData
+
+        # Set the new hashmaps
+        self._blockStates = newBlockStates
+        self._blockEntities = newBlockEntities
+
+        # For chaining
+        return self
+
+    '''
+    Scales the X, Y and Z components of every block's coordinates according to
+    an anchor point and a different scalar for each axis.
+    '''
+    def scaleXYZ(self, anchorPoint: tuple[int, int, int], scaleX: float, scaleY: float, scaleZ: float):
+        # Setup
+        newBlockStates = {}
+        newBlockEntities = {}
+
+
+        # Go through each block and scale their vertices and put them
+        # inside the new hashmaps
+        for blockPosition, blockState in self._blockStates.items():
+
+            # Firstly offset the position to the anchor point
+            blockPos = (blockPosition[0] - anchorPoint[0],
+                        blockPosition[1] - anchorPoint[1],
+                        blockPosition[2] - anchorPoint[2])
+
+            # Apply the scaling
+            blockPos = (blockPos[0] * scaleX,
+                        blockPos[1] * scaleY,
+                        blockPos[2] * scaleZ)
+
+            # Offset the positions again to put them where they would be originally
+            # but just scaled around the anchor point
+            # Also floor the block position so that we have integer coordinates
+            blockPos = (math.floor(blockPos[0] + anchorPoint[0]),
+                        math.floor(blockPos[1] + anchorPoint[1]),
+                        math.floor(blockPos[2] + anchorPoint[2]))
+
+            # Put the blockState in the new hashmap
+            newBlockStates[blockPos] = blockState
+            # See if this blockState is also a block entity, if so put it in
+            # the new BE hashmap
+            if blockPosition in self._blockEntities:
+                blockEntityData = self._blockEntities[blockPosition]
+                newBlockEntities[blockPos] = blockEntityData
+
+
+        # Set the new hashmaps
+        self._blockStates = newBlockStates
+        self._blockEntities = newBlockEntities
+
+        # For chaining
+        return self
+
+    '''
+    Scales the X, Y and Z components of every block's coordinates according to
+    an anchor point and a scalar.
+    '''
+    def scale(self, anchorPoint: tuple[int, int, int], scalar: float):
+        return self.scaleXYZ(anchorPoint, scalar, scalar, scalar)
+
+    '''
+    Rotates this schem's block positions by the inputted yaw, pitch and roll.
+    Note that it doesn't rotate the block states. So a comparator facing east rotated
+    pi/2 degrees will make the comparator face north.
+
+    Angles are assumed to be in a form where negative means CW, and positive angles are
+    CCW.
+
+    Rotations and how to determine which way is CCW and which way is CW:
+        - Yaw is a rotation around the Y axis, looking up (Y+) at the XZ plane.
+        - Pitch is a rotation around the X axis, looking east (X+) at the ZY plane.
+        - Roll is a rotation around the Z axis, looking south (Z+) at the XY plane. 
+    '''
+    def rotateRadians(self, anchorPoint: tuple[int, int, int], yaw:float =0.0, pitch:float =0.0, roll:float =0.0):
+
+        # Setup
+        newBlockStates = {}
+        newBlockEntities = {}
+        # The cos and sin values
+        # Yaw
+        # Negating the yaw because with the definition of this yaw
+        # and the rotation matrix definition the angles are
+        # actually going opposite ways
+        cosYaw = math.cos(-yaw)
+        sinYaw = math.sin(-yaw)
+        # Pitch
+        cosPitch = math.cos(pitch)
+        sinPitch = math.sin(pitch)
+        # Roll
+        # Negating the roll for the same reasons I negated the yaw
+        cosRoll = math.cos(-roll)
+        sinRoll = math.sin(-roll)
+
+
+        # Go through each block and rotate their vertices and put them
+        # inside the new hashmaps
+        for blockPosition, blockState in self._blockStates.items():
+
+            # Firstly offset the position to the anchor point
+            blockPos = (blockPosition[0] - anchorPoint[0],
+                        blockPosition[1] - anchorPoint[1],
+                        blockPosition[2] - anchorPoint[2])
+
+            # Apply rotations
+            if yaw != 0.0:
+                blockPos = (blockPos[2]*sinYaw + blockPos[0]*cosYaw,
+                            blockPos[1],
+                            blockPos[2]*cosYaw - blockPos[0]*sinYaw)
+
+            if pitch != 0.0:
+                blockPos = (blockPos[0],
+                            blockPos[2]*sinPitch + blockPos[1]*cosPitch,
+                            blockPos[2]*cosPitch - blockPos[1]*sinPitch)
+
+            if roll != 0.0:
+                blockPos = (blockPos[0]*cosRoll - blockPos[1]*sinRoll,
+                            blockPos[0]*sinRoll + blockPos[1]*cosRoll,
+                            blockPos[2])
+
+            # Offset the positions again to put them where they would be originally
+            # but just rotated around the anchor point
+            # Also floor the block position so that we have integer coordinates
+            blockPos = (math.floor( blockPos[0] + anchorPoint[0] ),
+                        math.floor( blockPos[1] + anchorPoint[1] ),
+                        math.floor( blockPos[2] + anchorPoint[2] ))
+
+            # Put the blockState in the new hashmap
+            newBlockStates[blockPos] = blockState
+            # See if this blockState is also a block entity, if so put it in
+            # the new BE hashmap
+            if blockPosition in self._blockEntities:
+                blockEntityData = self._blockEntities[blockPosition]
+                newBlockEntities[blockPos] = blockEntityData
+
+
+        # Set the new hashmaps
+        self._blockStates = newBlockStates
+        self._blockEntities = newBlockEntities
+
+        # For chaining
+        return self
+
+
+    '''
+    Rotates this schem's block positions by the inputted yaw, pitch and roll.
+    Note that it doesn't rotate the block states. So a comparator facing east rotated
+    90 degrees will make the comparator face north.
+    
+    Angles are assumed to be in a form where negative means CW, and positive angles are
+    CCW.
+    
+    Rotations and how to determine which way is CCW and which way is CW:
+        - Yaw is a rotation around the Y axis, looking up (Y+) at the XZ plane.
+        - Pitch is a rotation around the X axis, looking east (X+) at the ZY plane.
+        - Roll is a rotation around the Z axis, looking south (Z+) at the XY plane. 
+    '''
+    def rotateDegrees(self, anchorPoint: tuple[int, int, int], yaw: float, pitch: float, roll: float):
+        degreesToRadiansScalar = math.pi / 180
+        return self.rotateRadians(anchorPoint,
+                                  yaw * degreesToRadiansScalar,
+                                  pitch * degreesToRadiansScalar,
+                                  roll * degreesToRadiansScalar)
+
+    '''
+    Flips the structure by the inputted plane, which can be any combination of
+    2 axis out of "xyz". So "xy", "yz", "xz" is good. But "yx" is also good.
+    However "xx" and "yy" isn't good.
+    The inputted plane will also pass through the anchor point.
+    '''
+    def flip(self, anchorPoint: tuple[int, int, int], plane: str):
+
+        # Seeing if the plane is a valid one
+        # I don't exactly know why this algorithm I came up with works
+        # but it seems to work lmfao, just add 1 for each x, y, or z
+        # and if == to 2 then we have a combination of 2 different
+        # axis
+        xInPlane = 'x' in plane
+        yInPlane = 'y' in plane
+        zInPlane = 'z' in plane
+
+        if (xInPlane + yInPlane + zInPlane) != 2:
+            raise ValueError(
+                "Incorrect plane inputted. A plane should be the combination of 2 axis between x, y and z."
+            )
+
+        # Plane decoding so that I only have either
+        # "xy", "yz", or "xz"
+        flipPlane = ""
+        flipPlane += 'x' * xInPlane
+        flipPlane += 'y' * yInPlane
+        flipPlane += 'z' * zInPlane
+
+        # Setup for the new hashmaps
+        newBlockStates = {}
+        newBlockEntities = {}
+
+        # Go through each block and flip their vertices and put them
+        # inside the new hashmaps
+        for blockPosition, blockState in self._blockStates.items():
+            blockPos = None
+
+            # Flip
+            if   plane == "xy":
+                #blockPos = (blockPosition[0], blockPosition[1], -(blockPosition[2] - anchorPoint[2]) + anchorPoint[2])
+                blockPos = (blockPosition[0], blockPosition[1], -blockPosition[2] + 2*anchorPoint[2])
+            elif plane == "xz":
+                #blockPos = (blockPosition[0], -(blockPosition[1] - anchorPoint[1]) + anchorPoint[1], blockPosition[2])
+                blockPos = (blockPosition[0], -blockPosition[1] + 2*anchorPoint[1], blockPosition[2])
+            elif plane == "yz":
+                #blockPos = (-(blockPosition[0] - anchorPoint[0]) + anchorPoint[0], blockPosition[1], blockPosition[2])
+                blockPos = (-blockPosition[0] + 2*anchorPoint[0], blockPosition[1], blockPosition[2])
+
+            # Put the blockState in the new hashmap
+            newBlockStates[blockPos] = blockState
+            # See if this blockState is also a block entity, if so put it in
+            # the new BE hashmap
+            if blockPosition in self._blockEntities:
+                blockEntityData = self._blockEntities[blockPosition]
+                newBlockEntities[blockPos] = blockEntityData
+
+
+        # Set the new hashmaps
+        self._blockStates = newBlockStates
+        self._blockEntities = newBlockEntities
+
+        # For chaining
+        return self
+
+
+    ### ---
+
+
+
+    ### --- Private methods
+
+    '''
+    Returns a new ID for the block palette when called. Always returns an ID
+    that has never been used in the palette.
+    '''
+    def _getNewPaletteId(self) -> int:
+        newId = self._blockPaletteFreeId
+        self._blockPaletteFreeId += 1
+        return newId
+
+    '''
+    Removes the NBT part from a blockEntityString, for example, "barrel[]{}" would
+    then become "barrel[]". We assume that the blockNBT passed in has
+    NBTs.
+    '''
+    def _getBlockStateFromBlockEntityString(self, blockEntityString: str) -> str:
+        firstCurlyBracketIndex = blockEntityString.find('{')
+        return blockEntityString[:firstCurlyBracketIndex]
+
+    '''
+    Sets the block at the inputted position. The inputted block has to be a normal block state
+    '''
+    def _setBlockState(self, position: tuple[int, int, int], blockData: str):
+        # If the block is in the palette use its associated int, otherwise
+        # add a new entry in the palette
+        if blockData not in self._blockPalette:
+            newPaletteId = self._getNewPaletteId()
+            # Put the new block nbt in the palette
+            self._blockPalette[blockData] = newPaletteId
+            # Put the inverse in the palette as well when we want to
+            # access in O(1) the nbt of a block from its id
+            self._blockPalette[newPaletteId] = blockData
+
+        # Set the block in this schematic to the block we just inputted
+        self._blockStates[position] = self._blockPalette[blockData]
+
+    '''
+    Sets the block entity at the inputed position.
+    '''
+    def _setBlockEntity(self, position: tuple[int, int, int], blockEntityData: str):
+        # Get the block state of this blockEntity, because we still need to
+        # place the block state in the world
+        blockEntityState = self._getBlockStateFromBlockEntityString(blockEntityData)
+        # Set the block state in the world
+        self._setBlockState(position, blockEntityState)
+
+        # Add this block entity to the block entities hashmap
+        self._blockEntities[position] = blockEntityData
+
+    ###
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-        if not os.path.isfile(schematicToLoadPath):
-            self._defaultInit(); return
 
-        if not schematicToLoadPath.endswith(".schem"):
+
+
+
+
+
+
+
+
+
+
+
+"""
+Main class of mcschematic.
+It represents a Minecraft Schematic.
+"""
+class MCSchematic:
+
+    ### --- Fields
+
+    # The structure class holding all of our block and block entity data
+    _structure: MCStructure = None
+
+    ### ---
+
+
+
+    ### --- Init
+
+    def __init__(self, schematicToLoadPath_or_mcStructure: Union[str, MCStructure] = None):
+        if schematicToLoadPath_or_mcStructure is None:
             self._defaultInit(); return
 
-        self._initFromFile(schematicToLoadPath)
+        if type(schematicToLoadPath_or_mcStructure) == str:
+            schematicToLoadPath = schematicToLoadPath_or_mcStructure
+
+            if not os.path.isfile(schematicToLoadPath):
+                self._defaultInit(); return
+
+            if not schematicToLoadPath.endswith(".schem"):
+                self._defaultInit(); return
+
+            self._initFromFile(schematicToLoadPath)
+
+        if type(schematicToLoadPath_or_mcStructure) == MCStructure:
+            mcStructure = schematicToLoadPath_or_mcStructure
+
+            self._initFromMCStructure(mcStructure)
 
 
     '''
     The base class Init
     '''
     def _defaultInit(self):
-        self._blockPalette = {'minecraft:air': 0, 0: 'minecraft:air'}
-        self._blockPaletteFreeId = 1
-        self._blockStates = {}
-        self._blockEntities = {}
+        self._structure = MCStructure()
 
     '''
     Class init from existing schematic file
     '''
     def _initFromFile(self, schematicToLoadPath: str):
         # Get the schematic file as a nbt map
         schematicFile = nbtlib.load(schematicToLoadPath, gzipped=True)
         fileBase = schematicFile['Schematic'] if 'Schematic' in schematicFile else schematicFile
 
 
         ## Init the block palette
         filePalette = fileBase['Palette']
-        self._blockPalette = {}
+        structureBlockPalette = {}
 
         for blockState, idTagInPalette in filePalette.items():
             idInPalette = int(idTagInPalette)
-            self._blockPalette[blockState] = idInPalette
-            self._blockPalette[idInPalette] = blockState
+            structureBlockPalette[blockState] = idInPalette
+            structureBlockPalette[idInPalette] = blockState
         # Nothing has been put inside the block palette, so we default init it.
-        if len(self._blockPalette) == 0:
-            self._blockPalette = {'minecraft:air': 0, 0: 'minecraft:air'}
+        if len(structureBlockPalette) == 0:
+            structureBlockPalette = {'minecraft:air': 0, 0: 'minecraft:air'}
         # Set the free Id to the length of the block palette // 2 as each Id has 2 entries
-        self._blockPaletteFreeId = (len(self._blockPalette) // 2)
+        structureBlockPaletteFreeId = (len(structureBlockPalette) // 2)
 
         # -- Re process the block palette so that ID 0 is air
         # Put air inside the hashmap if it wasn't present yet.
         # used for future processing that's why it's not equal to 0
-        if 'minecraft:air' not in self._blockPalette:
-            self._blockPalette['minecraft:air'] = self._blockPaletteFreeId
-            self._blockPalette[self._blockPaletteFreeId] = 'minecraft:air'
-            self._blockPaletteFreeId += 1
+        if 'minecraft:air' not in structureBlockPalette:
+            structureBlockPalette['minecraft:air'] = structureBlockPaletteFreeId
+            structureBlockPalette[structureBlockPaletteFreeId] = 'minecraft:air'
+            structureBlockPaletteFreeId += 1
         # If the current air ID isn't 0, switch it up with the
         # current 0 id, example:
         #   palette{0: black_wool, 1: air} will get switched to:
         #   palette{0: air, 1: black_wool}
         # And the byte ids will get processed afterwards
-        beforeProcessingAirId = self._blockPalette['minecraft:air']
+        beforeProcessingAirId = structureBlockPalette['minecraft:air']
         airOldId = beforeProcessingAirId
         if beforeProcessingAirId != 0:
-            beforeProcessingId0State = self._blockPalette[0]
+            beforeProcessingId0State = structureBlockPalette[0]
             # Pop the 0 id
-            self._blockPalette.pop(0)
-            self._blockPalette.pop(beforeProcessingId0State)
+            structureBlockPalette.pop(0)
+            structureBlockPalette.pop(beforeProcessingId0State)
             # Pop the air id
-            self._blockPalette.pop(beforeProcessingAirId)
-            self._blockPalette.pop('minecraft:air')
+            structureBlockPalette.pop(beforeProcessingAirId)
+            structureBlockPalette.pop('minecraft:air')
 
             # Put the air at 0
-            self._blockPalette[0] = 'minecraft:air'
-            self._blockPalette['minecraft:air'] = 0
+            structureBlockPalette[0] = 'minecraft:air'
+            structureBlockPalette['minecraft:air'] = 0
             # Put the old currentId0State where air was
-            self._blockPalette[beforeProcessingAirId] = beforeProcessingId0State
-            self._blockPalette[beforeProcessingId0State] = beforeProcessingAirId
+            structureBlockPalette[beforeProcessingAirId] = beforeProcessingId0State
+            structureBlockPalette[beforeProcessingId0State] = beforeProcessingAirId
 
 
         ## Init the blockStates in _blocks
-        self._blockStates = {}
+        structureBlockStates: {tuple[int, int, int]: int} = {}
         if 'BlockData' in fileBase:
             # Get the necessary data
             fileBlockStatesIds = fileBase['BlockData']
             blockStatesIds = bytearray(fileBlockStatesIds)
             fileMetaData = fileBase['Metadata']
             schemOffset = ( int(fileMetaData['WEOffsetX']), int(fileMetaData['WEOffsetY']), int(fileMetaData['WEOffsetZ']) )
             schemHeight = int(fileBase['Height']) #y
@@ -386,19 +983,19 @@
 
                 # Shift the coordinates so that the blocks are back in their right position
                 realY = blockStateSchemY + schemOffset[1]
                 realZ = blockStateSchemZ + schemOffset[2]
                 realX = blockStateSchemX + schemOffset[0]
 
                 # Place the block
-                self._blockStates[(realX, realY, realZ)] = processedBlockStateId
+                structureBlockStates[(realX, realY, realZ)] = processedBlockStateId
 
 
         ## Block entities!
-        self._blockEntities = {}
+        structureBlockEntities = {}
         if 'BlockEntities' in fileBase:
             # Gather the necessary data
             fileBlockEntities = fileBase['BlockEntities']
             fileMetaData = fileBase['Metadata']
             schemOffset = ( int(fileMetaData['WEOffsetX']), int(fileMetaData['WEOffsetY']), int(fileMetaData['WEOffsetZ']) )
 
             # Iterate over every block entity
@@ -408,86 +1005,104 @@
 
                 # Get the position of this block entity
                 posCompound: IntArray = blockEntityCompound['Pos']
                 blockEntityPosX = int(posCompound[0]) + schemOffset[0]
                 blockEntityPosY = int(posCompound[1]) + schemOffset[1]
                 blockEntityPosZ = int(posCompound[2]) + schemOffset[2]
                 blockEntityPos = (blockEntityPosX, blockEntityPosY, blockEntityPosZ)
-                # Get its id
-                idCompound: String = blockEntityCompound['Id']
-                blockEntityState = str(idCompound)
+                # Get its id / blockState from the blockState hashmap
+                # (because the Id in the compound isn't complete)
+                blockEntityState: str = structureBlockPalette[structureBlockStates[blockEntityPos]]
 
                 # Create a compound without Pos and Id to serialize
                 pureCompound = Compound()
                 for k, v in blockEntityCompound.items():
                     if not (k == 'Pos' or k == 'Id'):
                         pureCompound.merge(Compound({k: v}))
 
                 # Create the blockEntity blockData string
                 blockData: str = blockEntityState + nbtlib.serialize_tag(pureCompound)
 
                 # Put it in _blockEntities
-                self._blockEntities[blockEntityPos] = blockData
+                structureBlockEntities[blockEntityPos] = blockData
+
+
+        ## Save the data gathered in a new structure class!
+        ## Using private member accessing shenanigans, do not recommend
+        ## using that anywhere else for whoever is looking at the code rn.
+        self._structure = MCStructure()
+        self._structure._blockPalette = structureBlockPalette
+        self._structure._blockPaletteFreeId = structureBlockPaletteFreeId
+        self._structure._blockStates = structureBlockStates
+        self._structure._blockEntities = structureBlockEntities
+
+    '''
+    Class init when a structure gets inputed. The inputted structure 
+    gets bound to the schematic.
+    '''
+    def _initFromMCStructure(self, mcStructure: MCStructure):
+        self._structure = mcStructure
 
     ### ---
 
 
 
     ### --- Public methods
 
     '''
     Saves this schematic to the inputed folder path.
+    
+    Some things to note:
+        If the schematic is more than 2 billion blocks in volume,
+        it will not save.
     '''
     def save(self, outputFolderPath: str, schemName: str, version: 'Version'):
-        # Setup
-        schemMinsAndMaxes = self._getSchematicMinAndMaxXYZ()
-        schemDims = self._getSchematicDimensions(schemMinsAndMaxes)
-        schemOffset = self._getSchematicOffsetFrom0XYZ(schemMinsAndMaxes)
-
+        ## Setup
+        schemBounds = self._structure.getBounds()
+        schemDims = self._structure.getStructureDimensions(schemBounds)
+        # The vector amount by which minBounds is offsetted from 0 0 0
+        schemOffset = schemBounds[0]
 
+        print(schemDims)
         ## BLOCK DATA
         # The block data encoded into the schematic, allocating every byte
         # for the schem, and setting them to 0 which conveniently is air
         encodedBlockData = bytearray(schemDims[1] * schemDims[2] * schemDims[0])
         schemYSliceArea = schemDims[0] * schemDims[2]
         schemXSliceLength = schemDims[0]
         # Loop over every block in our hashmap, deduce their placement in the bytearray
         # from their coordinates then replacing the byte there
-        for blockPosition, blockPaletteId in self._blockStates.items():
+        for blockPosition, blockPaletteId in self._structure.getBlockStates().items():
             # compute the position in the bytearray
             realX = blockPosition[0] - schemOffset[0]
             realY = blockPosition[1] - schemOffset[1]
             realZ = blockPosition[2] - schemOffset[2]
             byteArrayPos = realY * schemYSliceArea + realZ * schemXSliceLength + realX
             # Set the byte
             encodedBlockData[byteArrayPos] = blockPaletteId
 
 
         ## BLOCK ENTITIES
         blockEntitiesCompounds = \
             [
-                self._blockEntityStringToCompound(
+                self._blockEntityStringToSchemCompound(
                     (
                         position[0] - schemOffset[0],
                         position[1] - schemOffset[1],
                         position[2] - schemOffset[2]
                     ), blockEntityStr
                 )
-                for position, blockEntityStr in self._blockEntities.items()
+                for position, blockEntityStr in self._structure.getBlockEntities().items()
             ]
 
 
         # Get a cleaner version of the block palette, without the duplicates used
         # for back and forth O(1) access
-        cleanBlockPalette = \
-            {
-                blockData: Int(blockPaletteId)
-                for blockData, blockPaletteId in self._blockPalette.items()
-                if type(blockData) == str
-            }
+        self._structure.getBlockPalette()
+        cleanBlockPalette = self._structure.getBlockPalette()
 
 
         # Generate the schematic file from the byte array
         # From Fearless's code which was taken from someone else lOl
         schematic = File({
 
             'Version': Int(2),
@@ -530,199 +1145,74 @@
         # remove the "/", otherwise the name is gonna be "/<name>" which doesn't
         # work lOl
         schematicPath = \
             schemName + ".schem" if outputFolderPath == '' else \
             outputFolderPath + "/" + schemName + ".schem"
         schematic.save(schematicPath)
 
-
     '''
-    Sets a block in the schematic at the inputed position.
+    Returns the structure of this schematic, which is the class containing
+    every block and block entities.
+    '''
+    def getStructure(self):
+        return self._structure
+
     '''
+        Sets a block in the schematic at the inputed position.
+        '''
+
     def setBlock(self, position: tuple[int, int, int], blockData: str):
-        # We have a different treatment between block entities
-        # and normal blocks.
-        if not self._isBlockDataBlockEntity(blockData):
-            self._setBlockState(position, blockData)
-        else:
-            self._setBlockEntity(position, blockData)
+        return self._structure.setBlock(position, blockData)
 
     '''
     Returns the blockState at the inputed position, minecraft:air if there isn't.
     '''
+
     def getBlockStateAt(self, position: tuple[int, int, int]) -> str:
-        # If there isn't any blocks at that position, return none
-        if position in self._blockStates:
-            blockPaletteId = self._blockStates[position]
-            return self._blockPalette[blockPaletteId]
-        else:
-            return "minecraft:air"
+        return self._structure.getBlockStateAt(position)
 
     '''
     Return the block data at the inputted position, minecraft:air if there isn't anything.
     '''
     def getBlockDataAt(self, position: tuple[int, int, int]) -> str:
-        # The block datas are arranged in a way that blockEntities are a subset
-        # of blockStates with just NBT information. So we check for blockEntities first,
-        # then blockStates and then if nothing comes up we return minecraft:air!
-        if position in self._blockEntities:
-            return self._blockEntities[position]
-        if position in self._blockStates:
-            blockPaletteId = self._blockStates[position]
-            return self._blockPalette[blockPaletteId]
-        return "minecraft:air"
-
-    ### ---
-
-
-
-
-
-    ### --- Private methods
+        return self._structure.getBlockDataAt(position)
 
     '''
-    Returns a new ID for the block palette when called. Always returns an ID
-    that has never been used in the palette.
+    Places the inputted schematic inside this schematic at the inputted coordinates.
     '''
-    def _getNewPaletteId(self) -> int:
-        newId = self._blockPaletteFreeId
-        self._blockPaletteFreeId += 1
-        return newId
+    def placeSchematic(self, incomingSchematic: 'MCSchematic', placePosition: tuple[int, int, int]):
+        return self._structure.placeStructure(incomingSchematic.getStructure(), placePosition)
 
     '''
-    Computes the min and max XYZs of the schematic's block positions
+    Places the inputted structure inside this schematic at the inputted coordinates.
     '''
-    def _getSchematicMinAndMaxXYZ(self) -> tuple[int, int, int, int, int, int]:
-        xMin, yMin, zMin, xMax, yMax, zMax = 0, 0, 0, 0, 0, 0
-
-        keys = self._blockStates.keys()
-
-        for p in keys:
-            if p[0] < xMin:
-                xMin = p[0]
-            elif p[0] > xMax:
-                xMax = p[0]
-
-            if p[1] < yMin:
-                yMin = p[1]
-            elif p[1] > yMax:
-                yMax = p[1]
-
-            if p[2] < zMin:
-                zMin = p[2]
-            elif p[2] > zMax:
-                zMax = p[2]
-
-        return xMin, yMin, zMin, xMax, yMax, zMax
-
-
-        ### Keeping a catalogue of previously tried ways of computing mins and maxes lOl
-        #if optimisationType == 0:
-        #    # Slower but way less overhead
-        #    keys = self._blockStates.keys()
-        #    return (
-        #                min(pos[0] for pos in keys),
-        #                min(pos[1] for pos in keys),
-        #                min(pos[2] for pos in keys),
-        #                max(pos[0] for pos in keys),
-        #                max(pos[1] for pos in keys),
-        #                max(pos[2] for pos in keys)
-        #    )
-
-        #if optimisationType == 1:
-        #    # Faster but at the cost of more overhead
-        #    keys = self._blockStates.keys()
-        #
-        #    x = [p[0] for p in keys]
-        #    y = [p[1] for p in keys]
-        #    z = [p[2] for p in keys]
-        #
-        #    x.sort()
-        #    y.sort()
-        #    z.sort()
-        #
-        #    return x[0], y[0], z[0], x[-1], y[-1], z[-1]
+    def placeStructure(self, incomingStructure: MCStructure, placePosition: tuple[int, int, int]):
+        return self._structure.placeStructure(incomingStructure, placePosition)
 
-        #if optimisationType == 2:
-        #    # 1/3 the overhead of type 1 but same speed!
-        #    keys = self._blockStates.keys()
-        #
-        #    coordList = [p[0] for p in keys]
-        #    coordList.sort()
-        #    xMin, xMax = coordList[0], coordList[-1]
-        #
-        #    for i, p in enumerate(keys):
-        #        coordList[i] = p[1]
-        #    coordList.sort()
-        #    yMin, yMax = coordList[0], coordList[-1]
-        #
-        #    for i, p in enumerate(keys):
-        #       coordList[i] = p[2]
-        #    coordList.sort()
-        #    zMin, zMax = coordList[0], coordList[-1]
-        #
-        #    return xMin, yMin, zMin, xMax, yMax, zMax
-
-        #if optimisationType == 3:
-        #    xMin, yMin, zMin, xMax, yMax, zMax = 0, 0, 0, 0, 0, 0
-        #
-        #    keys = self._blockStates.keys()
-        #
-        #    for p in keys:
-        #        xMin = p[0] if p[0] < xMin else xMin
-        #        xMax = p[0] if p[0] > xMax else xMax
-        #
-        #        yMin = p[0] if p[0] < yMin else yMin
-        #        yMax = p[0] if p[0] > yMax else yMax
-        #
-        #        zMin = p[0] if p[0] < zMin else zMin
-        #        zMax = p[0] if p[0] > zMax else zMax
+    '''
+    Returns a deep copy of this schematic.
+    '''
+    def makeCopy(self):
+        return MCSchematic(self._structure.makeCopy())
 
-        #    return xMin, yMin, zMin, xMax, yMax, zMax
+    ### ---
 
 
 
-    '''
-    Gets the length in X, Y and Z of this schematic based on the mins and maxes of
-    the block positions in the schem.
-    '''
-    def _getSchematicDimensions(self, schematicMinsAndMaxes: tuple[int, int, int, int, int, int]) -> tuple[
-        int, int, int]:
-        return schematicMinsAndMaxes[3] - schematicMinsAndMaxes[0] + 1, \
-               schematicMinsAndMaxes[4] - schematicMinsAndMaxes[1] + 1, \
-               schematicMinsAndMaxes[5] - schematicMinsAndMaxes[2] + 1
 
-    '''
-    Gets the offset of the schematic from 0, 0, 0
-    Needed because we need to offset the schematic for its min XYZ to be at 0, 0, 0
-    '''
-    def _getSchematicOffsetFrom0XYZ(self, schematicMinsAndMaxes: tuple[int, int, int, int, int, int]) -> tuple[
-        int, int, int]:
-        return schematicMinsAndMaxes[0], schematicMinsAndMaxes[1], schematicMinsAndMaxes[2]
 
-    '''
-    Returns the blockData associated to the inputed ID in the palette.
-    Returns None if no blockData is attached to the inputed blockPaletteId
-    
-    Still in the code even though it's not used in case I remove the
-    duplicates in the hashmap of the block palette
-    '''
-    def _getNbtFromIdLinear(self, blockPaletteId: int) -> Union[str, None]:
-        # Using linear search as elements in a hashmap aren't ordered
-        for k, v in self._blockPalette.items():
-            if v == blockPaletteId:
-                return k
-        return None
+    ### --- Private methods
 
     '''
     Returns a Compound object from a blockEntity string, for example:
     "minecraft:barrel[]{CustomName:'{"italic":false,"text":"1"}',Items:[{Count:1b,Slot:0b,id:"minecraft:milk_bucket"}]}"
     Will get converted into a compound tag
     '''
-    def _blockEntityStringToCompound(self, blockEntityPosition: tuple[int, int, int], blockEntityString: str) -> Compound:
+    def _blockEntityStringToSchemCompound(self, blockEntityPosition: tuple[int, int, int],
+                                          blockEntityString: str) -> Compound:
         # The block entity nbt we are going to put in the schematic
         blockEntityNBTOut = Compound()
 
         # Get the NBT portion of the BEString, we know for sure that there is a '{'
         # in the string, as otherwise it would be a block iirc
         firstCurlyBracketIndex = blockEntityString.find('{')
         nbtPortion = blockEntityString[firstCurlyBracketIndex:]
@@ -748,95 +1238,40 @@
             # We have a "[]"
             idCompound = Compound({'Id': String(blockEntityString[:firstSquareBracketIndex])})
         blockEntityNBTOut.merge(idCompound)
 
         # We're finished pOG
         return blockEntityNBTOut
 
-    '''
-    Returns True if the inputed blockNbt is a blockEntity.
-    We check that by checking is there is at least a curly bracket in the string.
-    '''
-    def _isBlockDataBlockEntity(self, blockData: str) -> bool:
-        return '{' in blockData
+    ### ---
 
-    '''
-    Removes the NBT part from a blockEntityString, for example, "barrel[]{}" would
-    then become "barrel[]". We assume that the blockNBT passed in has
-    NBTs.
-    '''
-    def _getBlockStateFromBlockEntityString(self, blockEntityString: str) -> str:
-        firstCurlyBracketIndex = blockEntityString.find('{')
-        return blockEntityString[:firstCurlyBracketIndex]
 
-    '''
-    Returns a cleaned version of the block palette and some new mappings for it.
-    For example, if we have 2 block entities that have the same blockstate but not same NBT
-    such as: "barrel[]{CustomName:"a"}" and "barrel[]{CustomName:"b"}", one has the ID 0 and the
-    other has an ID of 1.
-    Yet in the cleaned palette, both are gonna get compiled to "barrel[]" which will have the same ID.
-    So the new mappings will map old IDs that are now unused to the new one. (So in this case, every 0
-    would be mapped to 1)
-    
-    Ended up not being implemented because I wanted to rewrite how block entities were handled  
-    '''
-    def _getCleanBlockPaletteAndReturnNewIdMappings(self):
-        pass
 
-    '''
-    Sets the block at the inputted position. The inputted block has to be a normal block state
-    '''
-    def _setBlockState(self, position: tuple[int, int, int], blockData: str):
-        # If the block is in the palette use its associated int, otherwise
-        # add a new entry in the palette
-        if blockData not in self._blockPalette:
-            newPaletteId = self._getNewPaletteId()
-            # Put the new block nbt in the palette
-            self._blockPalette[blockData] = newPaletteId
-            # Put the inverse in the palette as well when we want to
-            # access in O(1) the nbt of a block from its id
-            self._blockPalette[newPaletteId] = blockData
-
-        # Set the block in this schematic to the block we just inputted
-        self._blockStates[position] = self._blockPalette[blockData]
+    ### --- Defaults
 
     '''
-    Sets the block entity at the inputed position.
+    Really costly repr method, as everytime you call it, you have to recompute the
+    min and max XYZ of the schematic.
     '''
-    def _setBlockEntity(self, position: tuple[int, int, int], blockEntityData: str):
-        # Get the block state of this blockEntity, because we still need to
-        # place the block state in the world
-        blockEntityState = self._getBlockStateFromBlockEntityString(blockEntityData)
-        # Set the block state in the world
-        self._setBlockState(position, blockEntityState)
-
-        # Add this block entity to the block entities hashmap
-        self._blockEntities[position] = blockEntityData
+    #def __repr__(self):
+    #    ## Setup
+    #    dimensions = self._getSchematicDimensions(self._getSchematicMinAndMaxXYZ())
+    #    # The number of block states in the _blocks HashMap
+    #    blockStateCount = len(self._blockStates) // 2
+    #    # The number of block entities
+    #    blockEntityCount = len(self._blockEntities)
+    #
+    #    return f"[ Dimensions={dimensions}, BlockStateCount={blockStateCount}, BlockEntityCount={blockEntityCount} ]"
 
     ### ---
 
 
 
-    ### --- Defaults
 
-    '''
-    Really costly repr method, as everytime you call it, you have to recompute the
-    min and max XYZ of the schematic.
-    '''
-    def __repr__(self):
-        ## Setup
-        dimensions = self._getSchematicDimensions(self._getSchematicMinAndMaxXYZ())
-        # The number of block states in the _blocks HashMap
-        blockStateCount = len(self._blockStates) // 2
-        # The number of block entities
-        blockEntityCount = len(self._blockEntities)
-
-        return f"[ Dimensions={dimensions}, BlockStateCount={blockStateCount}, BlockEntityCount={blockEntityCount} ]"
 
-    ### ---
```

### Comparing `mcschematic-8.1/mcschematic.egg-info/PKG-INFO` & `mcschematic-9.1/mcschematic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mcschematic
-Version: 8.1
-Summary: A Minecraft schematic creator library.
+Version: 9.1
+Summary: A Minecraft Schematic creator library.
 Home-page: UNKNOWN
 Author: Sloimay
 Author-email: <sloimayyy@gmail.com>
 License: Apache License 2.0
 Description: ### MCSchematic
```

### Comparing `mcschematic-8.1/setup.py` & `mcschematic-9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '8.1'
-DESCRIPTION = 'A Minecraft schematic creator library.'
+VERSION = '9.1'
+DESCRIPTION = 'A Minecraft Schematic creator library.'
 LONG_DESCRIPTION = 'Allows the creation of Minecraft schematic files directly through code. And soon the editing of schematics saved on drives too!'
 
 with open("README.md", "r") as readme:
     LONG_DESCRIPTION = readme.read()
 
 # Setting up
 setup(
@@ -18,15 +18,15 @@
     license="Apache License 2.0",
     description=DESCRIPTION,
     
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     
     packages=find_packages(),
-    install_requires=['nbtlib'],
+    install_requires=['nbtlib', 'immutable-views'],
     readme="README.md",
     keywords=['python', 'minecraft', 'schematic'],
     classifiers=[
         "Development Status :: 6 - Mature",
         "Intended Audience :: Other Audience",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

