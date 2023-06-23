# Comparing `tmp/armaqdl-0.8.0.tar.gz` & `tmp/armaqdl-0.9.0.tar.gz`

## Comparing `armaqdl-0.8.0.tar` & `armaqdl-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.flake8
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/_version.py
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/armaqdl.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/config.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/const.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/update.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.8.0/config/settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/test_commands.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/test_config.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.8.0/LICENSE
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 armaqdl-0.8.0/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 armaqdl-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.flake8
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/_version.py
+-rw-r--r--   0        0        0    17627 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/armaqdl.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/config.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/const.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/update.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.9.0/config/settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/test_commands.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/test_config.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 armaqdl-0.9.0/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 armaqdl-0.9.0/PKG-INFO
```

### Comparing `armaqdl-0.8.0/armaqdl/armaqdl.py` & `armaqdl-0.9.0/armaqdl/armaqdl.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     if not mods or "none" in mods:
         return ""
 
     if VERBOSE:
         print(f"Process mods: {mods}")
 
     paths, skips = [], []
-    ignores = 0
+    ignores, opts = 0, 0
 
     for i, mod in enumerate(mods):
         location = "abs"  # Default if not specified
         marks = []
 
         # Path
         cli_mod = mod
@@ -140,41 +140,43 @@
         else:
             # Predefined path
             location_path = SETTINGS.get("locations", {}).get(location, {}).get('path')
             if location_path is None:
                 print(f"Invalid location: {location}")
                 continue
 
-        path = Path(location_path) / mod
-        path_build = path
+        path = Path(location_path)
 
         # Split wildcard (add to the end)
         if "*" in mod:
             mods_wildcard = [f"{location}:{str(mod_wildcard)[len(location_path) + 1:]}"
-                             for mod_wildcard in path.parent.glob("*") if mod_wildcard.is_dir()]
+                             for mod_wildcard in path.glob(mod) if mod_wildcard.is_dir()]
             mods.extend(mods_wildcard)
             ignores += 1
             continue
 
+        path = Path(location_path) / mod
+        path_build = path
+
         if not path.exists():
             print(f"Invalid mod path: {path}")
             continue
 
         # Skip mark (add to skip list)
         if "s" in marks or "skip" in marks:
             if VERBOSE:
-                print(f"{cli_mod}  [{path}]\n=> Skip in wildcards")
+                print(f"{location}:{mod}  [{path}]\n=> Skip in wildcards")
 
             skips.append(path)
             ignores += 1
             continue
 
         # Skip mod found in wildcard
         if path in skips:
-            print(f"(skip) {cli_mod}  [{path}]")
+            print(f"(skip) {location}:{mod}  [{path}]")
             ignores += 1
             continue
 
         # Get just identifiers (first letters) of each mark
         marks_identifiers = [x[0] for x in marks]
 
         # HEMTT launch type argument
@@ -202,33 +204,64 @@
             if not build_tool:
                 build_tool = "b"
 
         # Global build argument
         if not build_tool and build_dev_tool is not None and (location == "abs" or SETTINGS["locations"][location].get("build", False)):
             build_tool = build_dev_tool
 
-        print(f"{cli_mod}  [{path}]")
+        print(f"{location}:{mod}  [{path}]")
 
         # Build
         if build_tool:
             if not build_mod(path_build, build_tool, launch_type=launch_type):
                 continue
 
         # Check path existance after build, as HEMTT output does not exist if no build has been performed yet
         if not path.exists():
             print(f"Invalid mod path: {path}")
             continue
 
         paths.append(path)  # Marks success
 
+        # Optionals
+        if "o" in marks_identifiers:
+            optionals_index = marks_identifiers.index("o")
+            optionals = marks[optionals_index][2:]
+            optionals = optionals.split("@")
+
+            if VERBOSE:
+                print(f"  Process optionals: {optionals}")
+
+            for optional in optionals:
+                optionals_path = path / "optionals"
+                optional = f"@{optional}"
+
+                if "*" in optional:
+                    optionals_wildcard = [f"{optional_wildcard.name[1:]}"
+                                          for optional_wildcard in optionals_path.glob(optional) if optional_wildcard.is_dir()]
+                    optionals.extend(optionals_wildcard)
+                    ignores += 1
+                    continue
+
+                optional_path = optionals_path / optional
+
+                if not optional_path.exists():
+                    print(f"  Invalid optional path: {optional_path.relative_to(path)}")
+                    continue
+
+                print(f"  {optional_path.name}  [{optional_path.relative_to(path)}]")
+                paths.append(optional_path)
+
+            opts += len(optionals)
+
     # Some mods are invalid (return at the end to show all invalid locations/paths)
     if VERBOSE:
-        print(f"Paths: {len(paths)} processed vs. {len(mods) - ignores} input ({len(mods)} mods - {ignores} ignores)")
+        print(f"Paths: {len(paths)} processed vs. {len(mods) + opts - ignores} input ({len(mods) + opts} mods - {ignores} ignores)")
 
-    if len(paths) != len(mods) - ignores:
+    if len(paths) != len(mods) + opts - ignores:
         return None
 
     print(f"Total mods: {len(paths)}\n")
 
     return f"-mod={';'.join([str(x) for x in paths])}"
 
 
@@ -303,15 +336,15 @@
     else:
         print(f"Error! server.cfg not found! [{cfg_path}]")
 
     return ""
 
 
 def process_flags(args):
-    flags = ["-skipIntro", "-noSplash", "-hugePages"]
+    flags = ["-skipIntro", "-noSplash", "-noPause", "-hugePages"]
 
     profile = args.profile
     if args.headless:
         flags.append("-client")
 
         if not profile:
             profile = SETTINGS.get("headless", {}).get("profile", "headlessclient")
@@ -326,17 +359,14 @@
 
     if not args.no_errors:
         flags.append("-showScriptErrors")
 
     if not args.no_debug:
         flags.append("-debug")
 
-    if args.no_pause:
-        flags.append("-noPause")
-
     if args.check_signatures:
         flags.append("-checkSignatures")
 
     if not args.fullscreen:
         flags.append("-window")
 
     # Headless always wants to connect
@@ -401,26 +431,25 @@
 
     # Parse arguments
     parser = argparse.ArgumentParser(
         prog=PACKAGE,
         description=f"Quick development Arma 3 launcher v{__version__}",
         formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip][:t[type]] ...", type=str, nargs="*", help="paths to mods or 'none' for no mods")
+    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip][:t[type]][:o[opts]] ...", type=str, nargs="*", help="paths to mods or 'none' for no mods")
     parser.add_argument("-m", "--mission", default="", type=str, help="mission to load")
 
     parser.add_argument("-s", "--server", action="store_true", help="start server")
     parser.add_argument("-j", "--join-server", nargs="?", const="", type=str, help="join server")
     parser.add_argument("-hc", "--headless", action="store_true", help="start headess client")
 
     parser.add_argument("-p", "--profile", default="", type=str, help="profile name")
     parser.add_argument("-nfp", "--no-filepatching", action="store_true", help="disable file patching")
     parser.add_argument("-ne", "--no-errors", action="store_true", help="hide script errors")
     parser.add_argument("-nd", "--no-debug", action="store_true", help="disable debug mode")
-    parser.add_argument("-np", "--no-pause", action="store_true", help="don't pause on focus loss")
     parser.add_argument("-c", "--check-signatures", action="store_true", help="check signatures")
     parser.add_argument("-f", "--fullscreen", action="store_true")
     parser.add_argument("-par", "--parameters", nargs="+", type=str,
                         help="other parameters to pass directly (use with '=' to pass '-<arg>')")
     parser.add_argument("-e", "--executable", default="arma3_x64", type=str,
                         help="Arma executable to launch (relative to Arma directory without .exe or absolute with .exe)")
```

### Comparing `armaqdl-0.8.0/armaqdl/config.py` & `armaqdl-0.9.0/armaqdl/config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/armaqdl/update.py` & `armaqdl-0.9.0/armaqdl/update.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/config/settings.toml` & `armaqdl-0.9.0/config/settings.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/tests/test_commands.py` & `armaqdl-0.9.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/tests/test_config.py` & `armaqdl-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/.gitignore` & `armaqdl-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/LICENSE` & `armaqdl-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/README.md` & `armaqdl-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
 
 Settings are in [TOML](https://toml.io/en/) format and can be edited with any text editor.
 
 ### Dedicated Server
 
-Loading a mission on dedicated server automatically requires `server.cfg` to be present next to `arma3_x64.exe` with at least the following entries mission and Headless Client entries.
+Loading a mission on dedicated server automatically requires `server.cfg` to be present next to `arma3_x64.exe` with at least the following mission and Headless Client entries.
 
 ```cpp
 // Automatically load the first mission in rotation
 class Missions {
     class Test {
         template = "mission.vr";
     };
@@ -156,14 +156,30 @@
 
 Build type for HEMTT can also be specified using the same flag in addition to build flag.
 
 ```sh
 $ armaqdl dev:cba:bhemtt:trelease dev:ace:b:tbuild
 ```
 
+**Example 5:** _(optionals)_
+
+_Note: Only optionals inside `optionals` folder in a full `@mod` folder structure (such as HEMTT produces) are supported._
+
+Launches Arma with Theseus Services from local development folder and its MELB Variants optional skipping the prefix using glob pattern matching. `@` must still be used for each optional (or pattern) specified.
+
+```sh
+$ armaqdl dev:TheseusServices:o@*variants_melb
+```
+
+Glob pattern matching may also be used to match multiple optionals.
+
+```sh
+$ armaqdl dev:TheseusServices:o@*variants*
+```
+
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
 
 ```sh
 $ pip install --user -e .
```

### Comparing `armaqdl-0.8.0/pyproject.toml` & `armaqdl-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.8.0/PKG-INFO` & `armaqdl-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArmaQDL
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
 Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
 Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
 Author-email: Jonpas <jonpas33@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Console
@@ -97,15 +97,15 @@
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
 
 Settings are in [TOML](https://toml.io/en/) format and can be edited with any text editor.
 
 ### Dedicated Server
 
-Loading a mission on dedicated server automatically requires `server.cfg` to be present next to `arma3_x64.exe` with at least the following entries mission and Headless Client entries.
+Loading a mission on dedicated server automatically requires `server.cfg` to be present next to `arma3_x64.exe` with at least the following mission and Headless Client entries.
 
 ```cpp
 // Automatically load the first mission in rotation
 class Missions {
     class Test {
         template = "mission.vr";
     };
@@ -180,14 +180,30 @@
 
 Build type for HEMTT can also be specified using the same flag in addition to build flag.
 
 ```sh
 $ armaqdl dev:cba:bhemtt:trelease dev:ace:b:tbuild
 ```
 
+**Example 5:** _(optionals)_
+
+_Note: Only optionals inside `optionals` folder in a full `@mod` folder structure (such as HEMTT produces) are supported._
+
+Launches Arma with Theseus Services from local development folder and its MELB Variants optional skipping the prefix using glob pattern matching. `@` must still be used for each optional (or pattern) specified.
+
+```sh
+$ armaqdl dev:TheseusServices:o@*variants_melb
+```
+
+Glob pattern matching may also be used to match multiple optionals.
+
+```sh
+$ armaqdl dev:TheseusServices:o@*variants*
+```
+
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
 
 ```sh
 $ pip install --user -e .
```

