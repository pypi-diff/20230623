# Comparing `tmp/pythonmc-1.0.3.tar.gz` & `tmp/pythonmc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmc-1.0.3.tar", last modified: Thu Jun 22 20:18:50 2023, max compression
+gzip compressed data, was "pythonmc-1.0.4.tar", last modified: Fri Jun 23 19:04:45 2023, max compression
```

## Comparing `pythonmc-1.0.3.tar` & `pythonmc-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.620172 pythonmc-1.0.3/
--rw-rw-rw-   0        0        0     4694 2023-06-22 20:18:50.620172 pythonmc-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4181 2023-06-22 18:13:59.000000 pythonmc-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-06-22 18:13:59.000000 pythonmc-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      675 2023-06-22 20:18:50.621168 pythonmc-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.614107 pythonmc-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.616167 pythonmc-1.0.3/src/pythonmc/
--rw-rw-rw-   0        0        0   155553 2023-06-22 19:37:55.000000 pythonmc-1.0.3/src/pythonmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.619167 pythonmc-1.0.3/src/pythonmc.egg-info/
--rw-rw-rw-   0        0        0     4694 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.561409 pythonmc-1.0.4/
+-rw-rw-rw-   0        0        0     5394 2023-06-23 19:04:45.560395 pythonmc-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-06-23 17:56:35.000000 pythonmc-1.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-20 00:42:26.000000 pythonmc-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:04:45.561409 pythonmc-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-06-23 19:04:36.000000 pythonmc-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.493425 pythonmc-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.501926 pythonmc-1.0.4/src/pythonmc/
+-rw-rw-rw-   0        0        0     2857 2023-06-23 19:01:34.000000 pythonmc-1.0.4/src/pythonmc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.510245 pythonmc-1.0.4/src/pythonmc/block/
+-rw-rw-rw-   0        0        0      120 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/block/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block.py
+-rw-rw-rw-   0        0        0       90 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block_pos.py
+-rw-rw-rw-   0        0        0      110 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block_state.py
+-rw-rw-rw-   0        0        0    25267 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/blocks.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.516799 pythonmc-1.0.4/src/pythonmc/entity/
+-rw-rw-rw-   0        0        0      251 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/entity/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/entity/arm.py
+-rw-rw-rw-   0        0        0      450 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/damage_sources.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.520954 pythonmc-1.0.4/src/pythonmc/entity/effects/
+-rw-rw-rw-   0        0        0       99 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/status_effect_instance.py
+-rw-rw-rw-   0        0        0      680 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/status_effects.py
+-rw-rw-rw-   0        0        0     2341 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/entity/entities.py
+-rw-rw-rw-   0        0        0     2388 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/entity.py
+-rw-rw-rw-   0        0        0       50 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/hand.py
+-rw-rw-rw-   0        0        0     2522 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/living_entity.py
+-rw-rw-rw-   0        0        0      142 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/removal_reasons.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.525417 pythonmc-1.0.4/src/pythonmc/item/
+-rw-rw-rw-   0        0        0      179 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/item/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.529423 pythonmc-1.0.4/src/pythonmc/item/enchantment/
+-rw-rw-rw-   0        0        0      126 2023-06-23 18:59:00.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/__init__.py
+-rw-rw-rw-   0        0        0       51 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantment.py
+-rw-rw-rw-   0        0        0       93 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantment_rarity.py
+-rw-rw-rw-   0        0        0      806 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantments.py
+-rw-rw-rw-   0        0        0      171 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/hide_flags.py
+-rw-rw-rw-   0        0        0       57 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/item.py
+-rw-rw-rw-   0        0        0       81 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/item_rarity.py
+-rw-rw-rw-   0        0        0     1365 2023-06-23 18:42:29.000000 pythonmc-1.0.4/src/pythonmc/item/item_stack.py
+-rw-rw-rw-   0        0        0    31019 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/items.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.533422 pythonmc-1.0.4/src/pythonmc/player/
+-rw-rw-rw-   0        0        0      183 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/player/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/ender_chest_inventory.py
+-rw-rw-rw-   0        0        0       86 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/player/hunger_manager.py
+-rw-rw-rw-   0        0        0     1063 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/player_entity.py
+-rw-rw-rw-   0        0        0      846 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/player_inventory.py
+-rw-rw-rw-   0        0        0      873 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/player/player_manager.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 17:56:35.000000 pythonmc-1.0.4/src/pythonmc/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.540094 pythonmc-1.0.4/src/pythonmc/scoreboard/
+-rw-rw-rw-   0        0        0      286 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/render_types.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.542598 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/
+-rw-rw-rw-   0        0        0       90 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/collision_rules.py
+-rw-rw-rw-   0        0        0      112 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/visibility_rules.py
+-rw-rw-rw-   0        0        0      907 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard.py
+-rw-rw-rw-   0        0        0     1156 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_criterions.py
+-rw-rw-rw-   0        0        0      262 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_objective.py
+-rw-rw-rw-   0        0        0      284 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_player_score.py
+-rw-rw-rw-   0        0        0      957 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/team.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.544606 pythonmc-1.0.4/src/pythonmc/server/
+-rw-rw-rw-   0        0        0       97 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.546606 pythonmc-1.0.4/src/pythonmc/server/difficulty/
+-rw-rw-rw-   0        0        0       74 2023-06-23 18:57:40.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/__init__.py
+-rw-rw-rw-   0        0        0       83 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/difficulties.py
+-rw-rw-rw-   0        0        0       59 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/difficulty.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.548872 pythonmc-1.0.4/src/pythonmc/server/gamemode/
+-rw-rw-rw-   0        0        0       66 2023-06-23 18:57:30.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/game_mode.py
+-rw-rw-rw-   0        0        0       92 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/game_modes.py
+-rw-rw-rw-   0        0        0      940 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/server.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.550872 pythonmc-1.0.4/src/pythonmc/server/text/
+-rw-rw-rw-   0        0        0       58 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/server/text/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/text/formatting.py
+-rw-rw-rw-   0        0        0      108 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/text/text.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.557395 pythonmc-1.0.4/src/pythonmc/world/
+-rw-rw-rw-   0        0        0      193 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/world/__init__.py
+-rw-rw-rw-   0        0        0      323 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/executor.py
+-rw-rw-rw-   0        0        0     1851 2023-06-23 18:40:37.000000 pythonmc-1.0.4/src/pythonmc/world/particles.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.559397 pythonmc-1.0.4/src/pythonmc/world/position/
+-rw-rw-rw-   0        0        0       50 2023-06-23 18:55:59.000000 pythonmc-1.0.4/src/pythonmc/world/position/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/position/vec2f.py
+-rw-rw-rw-   0        0        0       87 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/position/vec3d.py
+-rw-rw-rw-   0        0        0       73 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/time_.py
+-rw-rw-rw-   0        0        0       62 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/weather.py
+-rw-rw-rw-   0        0        0      780 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/world.py
+-rw-rw-rw-   0        0        0       63 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/worlds.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.506236 pythonmc-1.0.4/src/pythonmc.egg-info/
+-rw-rw-rw-   0        0        0     5394 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/top_level.txt
```

### Comparing `pythonmc-1.0.3/PKG-INFO` & `pythonmc-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.3
+Version: 1.0.4
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,37 +31,56 @@
   </a>
 
 <h3 align="center">PythonMC</h3>
 
   <p align="center">
     PythonMC is a Fabric mod that allows datapacks to be written in Python. Minecraft datapacks have some big limitations but, PythonMC has very little. Like for loops, functions, if statements, and modules. 
     <br />
-    <a href="https://RevolvingMadness.github.io/PythonMC"><strong>Explore the docs »</strong></a>
+    <a href="https://RevolvingMadness.github.io/PythonMC"><strong>Explore the docs Â»</strong></a>
     <br />
     <br />
     <a href="https://github.com/RevolvingMadness/PythonMC/issues">Report Bug</a>
-    ·
+    Â·
     <a href="https://github.com/RevolvingMadness/PythonMC/issues">Request Feature</a>
   </p>
 </div>
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
+## Getting Started
+
+### Prerequisites
+
+You need Python to use PythonMC, You can get it [here](https://www.python.org).  
+**MAKE SURE TO CHECK THIS BOX OTHERWISE PYTHONMC WON'T WORK:**  
+![](https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/addtoenvironmentvariables.png)
+
+### Installation
+
+1. Install Python packages
+   ```sh
+   pip install jep pythonmc
+   ```
+    - We need `jep` because that is how the mod interacts with Python.
+    - We need `pythonmc` because that provides syntax highlighting.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
 ## Usage
 
-If you want to know how to use PythonMC refer to the [documentation](https://RevolvingMadness.github.io/PythonMC)
+If you want to know how to use PythonMC, refer to the **[documentation](https://RevolvingMadness.github.io/PythonMC)**
 
-_For more examples, please refer to the **[Documentation](https://example.com)**_
+For examples, please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/examples)**
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Roadmap
 
-**???**
+Whatever you suggest.
 
 See the **[open issues](https://github.com/RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
 known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contributing
@@ -118,10 +137,12 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
+[product-screenshot]: ../images/screenshot.png
+
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -1,32 +1,42 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.3 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.4 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
 [license-shield]][license-url]
                                _[PythonMC_Logo]
                               **** PythonMC ****
     PythonMC is a Fabric mod that allows datapacks to be written in Python.
  Minecraft datapacks have some big limitations but, PythonMC has very little.
             Like for loops, functions, if statements, and modules.
-                             Explore_the_docs_Â»
+                            Explore_the_docs_ÃÂ»
 
-                         Report_Bug Â· Request_Feature
+                        Report_Bug ÃÂ· Request_Feature
                                                                   (back_to_top)
-## Usage If you want to know how to use PythonMC refer to the [documentation]
-(https://RevolvingMadness.github.io/PythonMC) _For more examples, please refer
-to the **[Documentation](https://example.com)**_
-                                                                  (back_to_top)
-## Roadmap **???** See the **[open issues](https://github.com/RevolvingMadness/
-PythonMC/issues)** for a full list of proposed features (and known issues).
+## Getting Started ### Prerequisites You need Python to use PythonMC, You can
+get it [here](https://www.python.org). **MAKE SURE TO CHECK THIS BOX OTHERWISE
+PYTHONMC WON'T WORK:** ![](https://raw.githubusercontent.com/RevolvingMadness/
+PythonMC/master/images/addtoenvironmentvariables.png) ### Installation 1.
+Install Python packages ```sh pip install jep pythonmc ``` - We need `jep`
+because that is how the mod interacts with Python. - We need `pythonmc` because
+that provides syntax highlighting.
+                                                                  (back_to_top)
+## Usage If you want to know how to use PythonMC, refer to the **
+[documentation](https://RevolvingMadness.github.io/PythonMC)** For examples,
+please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/
+examples)**
+                                                                  (back_to_top)
+## Roadmap Whatever you suggest. See the **[open issues](https://github.com/
+RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
@@ -50,9 +60,10 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
-Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [product-screenshot]: ../images/
+screenshot.png [fabricmc.net]: https://img.shields.io/badge/Fabric%20-
+1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

### Comparing `pythonmc-1.0.3/README.md` & `pythonmc-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -29,25 +29,44 @@
     <a href="https://github.com/RevolvingMadness/PythonMC/issues">Request Feature</a>
   </p>
 </div>
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
+## Getting Started
+
+### Prerequisites
+
+You need Python to use PythonMC, You can get it [here](https://www.python.org).  
+**MAKE SURE TO CHECK THIS BOX OTHERWISE PYTHONMC WON'T WORK:**  
+![](https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/addtoenvironmentvariables.png)
+
+### Installation
+
+1. Install Python packages
+   ```sh
+   pip install jep pythonmc
+   ```
+    - We need `jep` because that is how the mod interacts with Python.
+    - We need `pythonmc` because that provides syntax highlighting.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
 ## Usage
 
-If you want to know how to use PythonMC refer to the [documentation](https://RevolvingMadness.github.io/PythonMC)
+If you want to know how to use PythonMC, refer to the **[documentation](https://RevolvingMadness.github.io/PythonMC)**
 
-_For more examples, please refer to the **[Documentation](https://example.com)**_
+For examples, please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/examples)**
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Roadmap
 
-**???**
+Whatever you suggest.
 
 See the **[open issues](https://github.com/RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
 known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contributing
@@ -104,10 +123,12 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
+[product-screenshot]: ../images/screenshot.png
+
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -6,20 +6,30 @@
     PythonMC is a Fabric mod that allows datapacks to be written in Python.
  Minecraft datapacks have some big limitations but, PythonMC has very little.
             Like for loops, functions, if statements, and modules.
                              Explore_the_docs_Â»
 
                          Report_Bug Â· Request_Feature
                                                                   (back_to_top)
-## Usage If you want to know how to use PythonMC refer to the [documentation]
-(https://RevolvingMadness.github.io/PythonMC) _For more examples, please refer
-to the **[Documentation](https://example.com)**_
-                                                                  (back_to_top)
-## Roadmap **???** See the **[open issues](https://github.com/RevolvingMadness/
-PythonMC/issues)** for a full list of proposed features (and known issues).
+## Getting Started ### Prerequisites You need Python to use PythonMC, You can
+get it [here](https://www.python.org). **MAKE SURE TO CHECK THIS BOX OTHERWISE
+PYTHONMC WON'T WORK:** ![](https://raw.githubusercontent.com/RevolvingMadness/
+PythonMC/master/images/addtoenvironmentvariables.png) ### Installation 1.
+Install Python packages ```sh pip install jep pythonmc ``` - We need `jep`
+because that is how the mod interacts with Python. - We need `pythonmc` because
+that provides syntax highlighting.
+                                                                  (back_to_top)
+## Usage If you want to know how to use PythonMC, refer to the **
+[documentation](https://RevolvingMadness.github.io/PythonMC)** For examples,
+please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/
+examples)**
+                                                                  (back_to_top)
+## Roadmap Whatever you suggest. See the **[open issues](https://github.com/
+RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
@@ -43,9 +53,10 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
-Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [product-screenshot]: ../images/
+screenshot.png [fabricmc.net]: https://img.shields.io/badge/Fabric%20-
+1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

### Comparing `pythonmc-1.0.3/src/pythonmc.egg-info/PKG-INFO` & `pythonmc-1.0.4/src/pythonmc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.3
+Version: 1.0.4
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,37 +31,56 @@
   </a>
 
 <h3 align="center">PythonMC</h3>
 
   <p align="center">
     PythonMC is a Fabric mod that allows datapacks to be written in Python. Minecraft datapacks have some big limitations but, PythonMC has very little. Like for loops, functions, if statements, and modules. 
     <br />
-    <a href="https://RevolvingMadness.github.io/PythonMC"><strong>Explore the docs »</strong></a>
+    <a href="https://RevolvingMadness.github.io/PythonMC"><strong>Explore the docs Â»</strong></a>
     <br />
     <br />
     <a href="https://github.com/RevolvingMadness/PythonMC/issues">Report Bug</a>
-    ·
+    Â·
     <a href="https://github.com/RevolvingMadness/PythonMC/issues">Request Feature</a>
   </p>
 </div>
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
+## Getting Started
+
+### Prerequisites
+
+You need Python to use PythonMC, You can get it [here](https://www.python.org).  
+**MAKE SURE TO CHECK THIS BOX OTHERWISE PYTHONMC WON'T WORK:**  
+![](https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/addtoenvironmentvariables.png)
+
+### Installation
+
+1. Install Python packages
+   ```sh
+   pip install jep pythonmc
+   ```
+    - We need `jep` because that is how the mod interacts with Python.
+    - We need `pythonmc` because that provides syntax highlighting.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
 ## Usage
 
-If you want to know how to use PythonMC refer to the [documentation](https://RevolvingMadness.github.io/PythonMC)
+If you want to know how to use PythonMC, refer to the **[documentation](https://RevolvingMadness.github.io/PythonMC)**
 
-_For more examples, please refer to the **[Documentation](https://example.com)**_
+For examples, please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/examples)**
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Roadmap
 
-**???**
+Whatever you suggest.
 
 See the **[open issues](https://github.com/RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
 known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contributing
@@ -118,10 +137,12 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
+[product-screenshot]: ../images/screenshot.png
+
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -1,32 +1,42 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.3 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.4 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
 [license-shield]][license-url]
                                _[PythonMC_Logo]
                               **** PythonMC ****
     PythonMC is a Fabric mod that allows datapacks to be written in Python.
  Minecraft datapacks have some big limitations but, PythonMC has very little.
             Like for loops, functions, if statements, and modules.
-                             Explore_the_docs_Â»
+                            Explore_the_docs_ÃÂ»
 
-                         Report_Bug Â· Request_Feature
+                        Report_Bug ÃÂ· Request_Feature
                                                                   (back_to_top)
-## Usage If you want to know how to use PythonMC refer to the [documentation]
-(https://RevolvingMadness.github.io/PythonMC) _For more examples, please refer
-to the **[Documentation](https://example.com)**_
-                                                                  (back_to_top)
-## Roadmap **???** See the **[open issues](https://github.com/RevolvingMadness/
-PythonMC/issues)** for a full list of proposed features (and known issues).
+## Getting Started ### Prerequisites You need Python to use PythonMC, You can
+get it [here](https://www.python.org). **MAKE SURE TO CHECK THIS BOX OTHERWISE
+PYTHONMC WON'T WORK:** ![](https://raw.githubusercontent.com/RevolvingMadness/
+PythonMC/master/images/addtoenvironmentvariables.png) ### Installation 1.
+Install Python packages ```sh pip install jep pythonmc ``` - We need `jep`
+because that is how the mod interacts with Python. - We need `pythonmc` because
+that provides syntax highlighting.
+                                                                  (back_to_top)
+## Usage If you want to know how to use PythonMC, refer to the **
+[documentation](https://RevolvingMadness.github.io/PythonMC)** For examples,
+please refer to the **[examples](https://RevolvingMadness.github.io/PythonMC/
+examples)**
+                                                                  (back_to_top)
+## Roadmap Whatever you suggest. See the **[open issues](https://github.com/
+RevolvingMadness/PythonMC/issues)** for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
@@ -50,9 +60,10 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
-Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [product-screenshot]: ../images/
+screenshot.png [fabricmc.net]: https://img.shields.io/badge/Fabric%20-
+1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

