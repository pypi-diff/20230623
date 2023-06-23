# Comparing `tmp/blizzardwarcraftapi-0.1.5.tar.gz` & `tmp/blizzardwarcraftapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blizzardwarcraftapi-0.1.5.tar", max compression
+gzip compressed data, was "blizzardwarcraftapi-0.2.0.tar", max compression
```

## Comparing `blizzardwarcraftapi-0.1.5.tar` & `blizzardwarcraftapi-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1003 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0        0        0      805 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0        0        0      139 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0        0        0      609 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/data.py
--rw-r--r--   0        0        0      292 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/exceptions.py
--rw-r--r--   0        0        0     1935 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
--rw-r--r--   0        0        0      639 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/__init__.py
--rw-r--r--   0        0        0     2195 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
--rw-r--r--   0        0        0     1694 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
--rw-r--r--   0        0        0     2056 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
--rw-r--r--   0        0        0        0 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/__init__.py
--rw-r--r--   0        0        0     1271 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
--rw-r--r--   0        0        0      683 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
--rw-r--r--   0        0        0     2965 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
--rw-r--r--   0        0        0     1766 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
--rw-r--r--   0        0        0      670 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
--rw-r--r--   0        0        0      746 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
--rw-r--r--   0        0        0        0 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/__init__.py
--rw-r--r--   0        0        0      421 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/urls.py
--rw-r--r--   0        0        0     1066 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/LICENSE
--rw-r--r--   0        0        0     2257 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/README.md
--rw-r--r--   0        0        0      916 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0        0        0     1581 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0        0        0      139 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0        0        0      609 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0        0        0      292 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/exceptions.py
+-rw-r--r--   0        0        0     1935 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0        0        0      685 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0        0        0     2195 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
+-rw-r--r--   0        0        0     1694 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
+-rw-r--r--   0        0        0     2056 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
+-rw-r--r--   0        0        0     3764 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
+-rw-r--r--   0        0        0      683 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
+-rw-r--r--   0        0        0     2965 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
+-rw-r--r--   0        0        0     1766 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
+-rw-r--r--   0        0        0      670 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
+-rw-r--r--   0        0        0      746 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/urls.py
+-rw-r--r--   0        0        0     1066 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2034 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/README.md
+-rw-r--r--   0        0        0      916 2023-06-23 13:26:18.604882 blizzardwarcraftapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.2.0/PKG-INFO
```

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardAuthToken.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/BlizzardAuthToken.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/data.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/__init__.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .gameData.AchievementAPI import AchievementAPI
 from .gameData.AuctionHouseAPI import AuctionHouseAPI
 from .gameData.ConnectedRealmAPI import ConnectedRealmAPI
+from .gameData.CreatureAPI import CreatureAPI
 
 from .profile.CharacterAchievementsAPI import CharacterAchievementsAPI
 from .profile.CharacterAppearanceAPI import CharacterAppearanceAPI
 from .profile.CharacterCollectionsAPI import CharacterCollectionsAPI
 from .profile.CharacterEncountersAPI import CharacterEncountersAPI
 from .profile.CharacterEquipmentAPI import CharacterEquipmentAPI
 from .profile.CharacterHunterPetsAPI import CharacterHunterPetsAPI
```

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py` & `blizzardwarcraftapi-0.2.0/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/LICENSE` & `blizzardwarcraftapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.1.5/README.md` & `blizzardwarcraftapi-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,32 +12,29 @@
 Install and update using <a href="https://pip.pypa.io/en/stable/getting-started/">pip</a>:
 ```shell
 pip install BlizzardWarcraftAPI
 ```
 
 # A Simple Example
 
-```python
-from BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken
+### Get Access Token
 
-token = BlizzardAuthToken("ClientID", "ClientSecret").get()
+````python
+from BlizzardWarcraftAPI import BlizzardAuthToken
 
-warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex
-```
+token = BlizzardAuthToken("ClientID", "ClientSecret")
+token.get()
+````
+
+### Get Achievement Category & Character Hunter Pets Summary
+
+````python
+from BlizzardWarcraftAPI import BlizzardWarcraftAPI
 
-# [APIs](https://develop.battle.net/documentation/world-of-warcraft)
+api = BlizzardWarcraftAPI("token", "region", "locale")
 
-## [Game Data](https://develop.battle.net/documentation/world-of-warcraft/game-data-apis)
+GameData = api.GameData()
+Profile = api.Profile()
 
-- [x] Achievement
-- [x] Auction House
-- [x] Connected Realm
-
-## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
-
-- [x] Character Achievements
-- [x] Character Appearance
-- [x] Character Collections
-- [x] Character Encounters
-- [x] Character Equipment
-- [x] Character Hunter Pets
+GameData.get_AchievementCategory(1)
+Profile.get_CharacterHunterPetsSummary("ravencrest", "bicmex")
+````
```

#### html2text {}

```diff
@@ -12,18 +12,15 @@
 developers to focus on building their applications or tools. By leveraging
 Blizzard's official API, BlizzardWarcraftAPI ensures that the data obtained is
 accurate and up-to-date. As the library continues to evolve, additional
 features and enhancements will be added to expand its capabilities and improve
 its usability. Developers interested in utilizing the vast resources offered by
 the World of Warcraft API will find BlizzardWarcraftAPI to be a valuable tool
 in their projects. # Installing Install and update using pip: ```shell pip
-install BlizzardWarcraftAPI ``` # A Simple Example ```python from
-BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken token =
-BlizzardAuthToken("ClientID", "ClientSecret").get() warcraft =
-BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
-develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
-develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
-Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
-develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
-Character Achievements - [x] Character Appearance - [x] Character Collections -
-[x] Character Encounters - [x] Character Equipment - [x] Character Hunter Pets
+install BlizzardWarcraftAPI ``` # A Simple Example ### Get Access Token
+````python from BlizzardWarcraftAPI import BlizzardAuthToken token =
+BlizzardAuthToken("ClientID", "ClientSecret") token.get() ```` ### Get
+Achievement Category & Character Hunter Pets Summary ````python from
+BlizzardWarcraftAPI import BlizzardWarcraftAPI api = BlizzardWarcraftAPI
+("token", "region", "locale") GameData = api.GameData() Profile = api.Profile()
+GameData.get_AchievementCategory(1) Profile.get_CharacterHunterPetsSummary
+("ravencrest", "bicmex") ````
```

### Comparing `blizzardwarcraftapi-0.1.5/pyproject.toml` & `blizzardwarcraftapi-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BlizzardWarcraftAPI"
-version = "0.1.5"
+version = "0.2.0"
 authors = ["Angeloffy <angeloffy.work@gmail.com>"]
 maintainers = [
     "Angeloffy <angeloffy.work@gmail.com>",
     "Kotorkovsciy <kotorkovsciy@gmail.com>"
 ]
 description = "Warcraft API"
 readme = "README.md"
```

### Comparing `blizzardwarcraftapi-0.1.5/PKG-INFO` & `blizzardwarcraftapi-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blizzardwarcraftapi
-Version: 0.1.5
+Version: 0.2.0
 Summary: Warcraft API
 Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
 License: MIT
 Author: Angeloffy
 Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy
 Maintainer-email: angeloffy.work@gmail.com
@@ -36,32 +36,29 @@
 Install and update using <a href="https://pip.pypa.io/en/stable/getting-started/">pip</a>:
 ```shell
 pip install BlizzardWarcraftAPI
 ```
 
 # A Simple Example
 
-```python
-from BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken
+### Get Access Token
 
-token = BlizzardAuthToken("ClientID", "ClientSecret").get()
+````python
+from BlizzardWarcraftAPI import BlizzardAuthToken
 
-warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex
-```
+token = BlizzardAuthToken("ClientID", "ClientSecret")
+token.get()
+````
+
+### Get Achievement Category & Character Hunter Pets Summary
+
+````python
+from BlizzardWarcraftAPI import BlizzardWarcraftAPI
 
-# [APIs](https://develop.battle.net/documentation/world-of-warcraft)
+api = BlizzardWarcraftAPI("token", "region", "locale")
 
-## [Game Data](https://develop.battle.net/documentation/world-of-warcraft/game-data-apis)
+GameData = api.GameData()
+Profile = api.Profile()
 
-- [x] Achievement
-- [x] Auction House
-- [x] Connected Realm
-
-## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
-
-- [x] Character Achievements
-- [x] Character Appearance
-- [x] Character Collections
-- [x] Character Encounters
-- [x] Character Equipment
-- [x] Character Hunter Pets
+GameData.get_AchievementCategory(1)
+Profile.get_CharacterHunterPetsSummary("ravencrest", "bicmex")
+````
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.2.0 Summary:
 Warcraft API Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/
 main License: MIT Author: Angeloffy Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy Maintainer-email: angeloffy.work@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -25,18 +25,15 @@
 developers to focus on building their applications or tools. By leveraging
 Blizzard's official API, BlizzardWarcraftAPI ensures that the data obtained is
 accurate and up-to-date. As the library continues to evolve, additional
 features and enhancements will be added to expand its capabilities and improve
 its usability. Developers interested in utilizing the vast resources offered by
 the World of Warcraft API will find BlizzardWarcraftAPI to be a valuable tool
 in their projects. # Installing Install and update using pip: ```shell pip
-install BlizzardWarcraftAPI ``` # A Simple Example ```python from
-BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken token =
-BlizzardAuthToken("ClientID", "ClientSecret").get() warcraft =
-BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
-develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
-develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
-Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
-develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
-Character Achievements - [x] Character Appearance - [x] Character Collections -
-[x] Character Encounters - [x] Character Equipment - [x] Character Hunter Pets
+install BlizzardWarcraftAPI ``` # A Simple Example ### Get Access Token
+````python from BlizzardWarcraftAPI import BlizzardAuthToken token =
+BlizzardAuthToken("ClientID", "ClientSecret") token.get() ```` ### Get
+Achievement Category & Character Hunter Pets Summary ````python from
+BlizzardWarcraftAPI import BlizzardWarcraftAPI api = BlizzardWarcraftAPI
+("token", "region", "locale") GameData = api.GameData() Profile = api.Profile()
+GameData.get_AchievementCategory(1) Profile.get_CharacterHunterPetsSummary
+("ravencrest", "bicmex") ````
```

