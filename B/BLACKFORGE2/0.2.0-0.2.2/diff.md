# Comparing `tmp/BLACKFORGE2-0.2.0.tar.gz` & `tmp/BLACKFORGE2-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.2.0.tar", last modified: Tue Jun 20 22:08:05 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.2.2.tar", last modified: Fri Jun 23 04:01:24 2023, max compression
```

## Comparing `BLACKFORGE2-0.2.0.tar` & `BLACKFORGE2-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.261164 BLACKFORGE2-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.242713 BLACKFORGE2-0.2.0/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14335 2023-06-20 22:06:51.000000 BLACKFORGE2-0.2.0/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.0/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.258172 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      312 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      312 2023-06-20 22:08:05.260165 BLACKFORGE2-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-20 22:08:05.261164 BLACKFORGE2-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-06-20 22:07:27.000000 BLACKFORGE2-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:01:24.207444 BLACKFORGE2-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-06-23 04:01:24.181962 BLACKFORGE2-0.2.2/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14534 2023-06-23 04:00:55.000000 BLACKFORGE2-0.2.2/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.2/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:01:24.203450 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-06-23 04:01:23.000000 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-23 04:01:23.000000 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 04:01:23.000000 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 04:01:23.000000 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-23 04:01:23.000000 BLACKFORGE2-0.2.2/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-06-23 04:01:24.206444 BLACKFORGE2-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-23 04:01:24.207444 BLACKFORGE2-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-06-23 04:01:03.000000 BLACKFORGE2-0.2.2/setup.py
```

### Comparing `BLACKFORGE2-0.2.0/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.2.2/BLACKFORGE2/FORGE.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,53 +15,58 @@
 #from settings import *
 
 """ PHYSICS """
 class Physics():
 
 	def __init__(self):
 		pass
-
+	
 	def apply_gravity(self, entity, gravity_value:float, delta_time:float):
 		entity.velocity.y += gravity_value * delta_time
 
-	def horizontal_movement_collision(self, entity, collision_tiles:pygame.sprite.Group):
-		entity = entity
-		for sprite in collision_tiles.sprites():
-			if sprite.rect.colliderect(entity.rect):
-				if entity.velocity.x < 0: 
-					entity.rect.left = sprite.rect.right
-					entity.collide_left = True
-					self.current_x = entity.rect.left
-				elif entity.velocity.x > 0:
-					entity.rect.right = sprite.rect.left
-					entity.collide_right = True
-					self.current_x = entity.rect.right
-
-		if entity.collide_left and (entity.rect.left < self.current_x or entity.velocity.x >= 0):
-			entity.collide_left = False
-		if entity.collide_right and (entity.rect.right > self.current_x or entity.velocity.x <= 0):
-			entity.collide_right = False
-
-	def vertical_movement_collision(self, entity, collision_tiles:pygame.sprite.Group):
-		entity = entity
-		for sprite in collision_tiles.sprites():
-			if sprite.rect.colliderect(entity.rect):
-				if entity.velocity.y > 0: 
-					entity.rect.bottom = sprite.rect.top
-					entity.velocity.y = 0
-					entity.collide_bottom = True
-				elif entity.velocity.y < 0:
-					entity.rect.top = sprite.rect.bottom
-					entity.velocity.y = 0
-					entity.collide_top = True
-
-		if entity.collide_bottom and entity.velocity.y < 0 or entity.velocity.y > 1:
-			entity.collide_bottom = False
-		if entity.collide_top and entity.velocity.y > 0.1:
-			entity.collide_top = False
+	def horizontal_movement_collision(self, entity, sprites_to_check:pygame.sprite.Group):
+		self.collision_area.center = self.rect.center
+		sprites_to_check = [sprite for sprite in sprites_to_check if sprite.rect.colliderect(self.collision_area)]
+
+		for sprite in sprites_to_check:
+			if sprite.rect.colliderect(self.rect):
+				if self.velocity.x < 0:
+					self.rect.left = sprite.rect.right
+					self.collide_left = True
+					self.current_x = self.rect.left
+
+				if self.velocity.x > 0:
+					self.rect.right = sprite.rect.left
+					self.collide_right = True
+					self.current_x = self.rect.right
+
+		if self.collide_left and (self.rect.left < self.current_x or self.velocity.x >= 0):
+			self.collide_left = False
+		if self.collide_right and (self.rect.right > self.current_x or self.velocity.x <= 0):
+			self.collide_right = False
+
+	def vertical_movement_collision(self, entity, sprites_to_check:pygame.sprite.Group):
+		self.collision_area.center = self.rect.center
+		sprites_to_check = [sprite for sprite in sprites_to_check if sprite.rect.colliderect(self.collision_area)]
+
+		for sprite in sprites_to_check:
+			if sprite.rect.colliderect(self.rect):
+				if self.velocity.y > 0:
+					self.rect.bottom = sprite.rect.top
+					self.velocity.y = 0
+					self.collide_bottom = True
+				if self.velocity.y < 0:
+					self.rect.top = sprite.rect.bottom
+					self.velocity.y = 0
+					self.collide_top = True
+
+		if self.collide_bottom and self.velocity.y < 0 or self.velocity.y > 1:
+			self.collide_bottom = False
+		if self.collide_top and self.velocity.y > 0.1:
+			self.collide_top = False
 
 """ GAME OBJECTS """
 class Entity(pygame.sprite.Sprite):
 
 	def __init__(self, size:int, position:tuple, speed:int, groups:list):
 		super().__init__(groups)
 		self.speed = speed
```

### Comparing `BLACKFORGE2-0.2.0/LICENSE` & `BLACKFORGE2-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.2.0/README.rst` & `BLACKFORGE2-0.2.2/README.rst`

 * *Files identical despite different names*

