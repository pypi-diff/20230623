# Comparing `tmp/ephys_link-0.0.8.tar.gz` & `tmp/ephys_link-0.1.tar.gz`

## Comparing `ephys_link-0.0.8.tar` & `ephys_link-0.1.tar`

### file list

```diff
@@ -1,51 +1,56 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ephys_link-0.0.8/Dockerfile
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-0.0.8/MANIFEST.in
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ephys_link-0.0.8/docker-compose.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ephys_link-0.0.8/requirements.txt
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/auto-formatters.txt
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/pull_request_template.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/workflows/autoformat-and-lint.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/ephys-link.iml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/other.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/__main__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/common.py
--rw-r--r--   0        0        0    18899 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/platform_handler.py
--rw-r--r--   0        0        0    14165 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/server.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/platforms/__init__.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/platforms/new_scale_handler.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/platforms/sensapex_handler.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/platforms/sensapex_manipulator.py
--rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/resources/libum.dll
--rw-r--r--   0        0        0    69824 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/resources/libum.lib
--rw-r--r--   0        0        0    50104 2020-02-02 00:00:00.000000 ephys_link-0.0.8/ephys_link/resources/libum.so
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ephys_link-0.0.8/scripts/draw_demo.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ephys_link-0.0.8/scripts/probe_crash_test.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 ephys_link-0.0.8/scripts/read_to_file.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/calibration_test.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/can_write_test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/drive_to_depth_test.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/get_manipulators_test.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/get_pos_test.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/inside_brain_test.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/move_test.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/register_manipulator_test.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ephys_link-0.0.8/tests/stop_test.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 ephys_link-0.0.8/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-0.0.8/LICENSE
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 ephys_link-0.0.8/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 ephys_link-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 ephys_link-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ephys_link-0.1/Dockerfile
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-0.1/MANIFEST.in
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ephys_link-0.1/docker-compose.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ephys_link-0.1/requirements.txt
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/auto-formatters.txt
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/workflows/autoformat-and-lint.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 ephys_link-0.1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/ephys-link.iml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/other.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ephys_link-0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/__main__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/common.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/gui.py
+-rw-r--r--   0        0        0    19041 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platform_handler.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/server.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platforms/__init__.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platforms/new_scale_handler.py
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platforms/new_scale_manipulator.py
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platforms/sensapex_handler.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/platforms/sensapex_manipulator.py
+-rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/resources/CP210xManufacturing.dll
+-rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/resources/NstMotorCtrl.dll
+-rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/resources/SiUSBXp.dll
+-rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 ephys_link-0.1/ephys_link/resources/libum.dll
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ephys_link-0.1/scripts/draw_demo.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ephys_link-0.1/scripts/new_scale_move.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ephys_link-0.1/scripts/probe_crash_test.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ephys_link-0.1/scripts/read_to_file.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/calibration_test.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/can_write_test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/drive_to_depth_test.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/get_manipulators_test.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/get_pos_test.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/inside_brain_test.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/move_test.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/register_manipulator_test.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ephys_link-0.1/tests/stop_test.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 ephys_link-0.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-0.1/LICENSE
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 ephys_link-0.1/README.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 ephys_link-0.1/pyproject.toml
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 ephys_link-0.1/PKG-INFO
```

### Comparing `ephys_link-0.0.8/.github/CODE_OF_CONDUCT.md` & `ephys_link-0.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/.github/CONTRIBUTING.md` & `ephys_link-0.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/.github/dependabot.yml` & `ephys_link-0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `ephys_link-0.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/.github/workflows/codeql-analysis.yml` & `ephys_link-0.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/ephys_link/common.py` & `ephys_link-0.1/ephys_link/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,25 +66,27 @@
 
 # Output data dictionaries
 class GetManipulatorsOutputData(dict):
     """Output format for (manipulators)
 
     :param manipulators: Tuple of manipulator IDs (as strings)
     :type manipulators: list
+    :param type: Type of the output data (temporary solution until #165 is implemented)
+    :type type: str
     :param error: Error message
     :type error: str
 
     :example: Example generated dictionary
         :code:`{"manipulators": ["1", "2"], "error": ""}`
     """
 
-    def __init__(self, manipulators: list, error: str) -> None:
+    def __init__(self, manipulators: list, type: str, error: str) -> None:
         """Constructor"""
         super(GetManipulatorsOutputData, self).__init__(
-            manipulators=manipulators, error=error
+            manipulators=manipulators, type=type, error=error
         )
 
 
 class PositionalOutputData(dict):
     """Output format for (position, error)
 
     :param position: Position in mm (as a tuple, can be empty tuple)
```

### Comparing `ephys_link-0.0.8/ephys_link/platform_handler.py` & `ephys_link-0.1/ephys_link/platform_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def __init__(self):
         """Initialize the manipulator handler with a dictionary of manipulators."""
 
         # Registered manipulators are stored as a dictionary of IDs (string) to
         # manipulator objects
         self.manipulators = {}
+        self.type = "sensapex"  # Remove this after #165
 
     # Platform Handler Methods
 
     def reset(self) -> bool:
         """Reset handler
 
         :return: True if successful, False otherwise
@@ -68,15 +69,15 @@
         try:
             # noinspection PyUnresolvedReferences
             devices = self._get_manipulators()
             error = ""
         except Exception as e:
             print(f"[ERROR]\t\t Getting manipulators: {type(e)}: {e}\n")
         finally:
-            return com.GetManipulatorsOutputData(devices, error)
+            return com.GetManipulatorsOutputData(devices, self.type,  error)
 
     def register_manipulator(self, manipulator_id: str) -> str:
         """Register a manipulator
 
         :param manipulator_id: The ID of the manipulator to register.
         :type manipulator_id: str
         :return: Callback parameter (Error message (on error))
@@ -136,30 +137,30 @@
         :return: Callback parameters (manipulator ID, position in (x, y, z, w) (or an
             empty array on error), error message)
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         try:
             # Check calibration status
             if (
-                hasattr(self.manipulators[manipulator_id], "get_calibrated")
-                and not self.manipulators[manipulator_id].get_calibrated()
+                    hasattr(self.manipulators[manipulator_id], "get_calibrated")
+                    and not self.manipulators[manipulator_id].get_calibrated()
             ):
                 print(f"[ERROR]\t\t Calibration not complete: {manipulator_id}\n")
                 return com.PositionalOutputData([], "Manipulator not calibrated")
 
             # Get position
             return self._get_pos(manipulator_id)
 
         except KeyError:
             # Manipulator not found in registered manipulators
             print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}")
             return com.PositionalOutputData([], "Manipulator not registered")
 
     async def goto_pos(
-        self, manipulator_id: str, position: list[float], speed: int
+            self, manipulator_id: str, position: list[float], speed: int
     ) -> com.PositionalOutputData:
         """Move manipulator to position
 
         :param manipulator_id: The ID of the manipulator to move
         :type manipulator_id: str
         :param position: The position to move to
         :type position: list[float]
@@ -184,15 +185,15 @@
 
         except KeyError:
             # Manipulator not found in registered manipulators
             print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}\n")
             return com.PositionalOutputData([], "Manipulator not registered")
 
     async def drive_to_depth(
-        self, manipulator_id: str, depth: float, speed: int
+            self, manipulator_id: str, depth: float, speed: int
     ) -> com.DriveToDepthOutputData:
         """Drive manipulator to depth
 
         :param manipulator_id: The ID of the manipulator to drive
         :type manipulator_id: str
         :param depth: The depth to drive to
         :type depth: float
@@ -217,15 +218,15 @@
 
         except KeyError:
             # Manipulator not found in registered manipulators
             print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}\n")
             return com.DriveToDepthOutputData(0, "Manipulator " "not registered")
 
     def set_inside_brain(
-        self, manipulator_id: str, inside: bool
+            self, manipulator_id: str, inside: bool
     ) -> com.StateOutputData:
         """Set manipulator inside brain state (restricts motion)
 
         :param manipulator_id: The ID of the manipulator to set the state of
         :type manipulator_id: str
         :param inside: True if inside brain, False if outside
         :type inside: bool
@@ -302,19 +303,19 @@
         except Exception as e:
             # Other error
             print(f"[ERROR]\t\t Bypass calibration of manipulator {manipulator_id}")
             print(f"{e}\n")
             return "Error bypassing calibration"
 
     def set_can_write(
-        self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
+            self,
+            manipulator_id: str,
+            can_write: bool,
+            hours: float,
+            sio: socketio.AsyncServer,
     ) -> com.StateOutputData:
         """Set manipulator can_write state (enables/disabled moving manipulator)
 
         :param manipulator_id: The ID of the manipulator to set the state of
         :type manipulator_id: str
         :param can_write: True if allowed to move, False if outside
         :type can_write: bool
@@ -379,15 +380,15 @@
             empty array on error), error message)
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         pass
 
     @abstractmethod
     async def _goto_pos(
-        self, manipulator_id: str, position: list[float], speed: int
+            self, manipulator_id: str, position: list[float], speed: int
     ) -> com.PositionalOutputData:
         """Move manipulator to position
 
         :param manipulator_id: The ID of the manipulator to move
         :type manipulator_id: str
         :param position: The position to move to
         :type position: list[float]
@@ -397,15 +398,15 @@
                  empty array on error), error message)
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         pass
 
     @abstractmethod
     async def _drive_to_depth(
-        self, manipulator_id: str, depth: float, speed: int
+            self, manipulator_id: str, depth: float, speed: int
     ) -> com.DriveToDepthOutputData:
         """Drive manipulator to depth
 
         :param manipulator_id: The ID of the manipulator to drive
         :type manipulator_id: str
         :param depth: The depth to drive to
         :type depth: float
@@ -415,15 +416,15 @@
                  message)
         :rtype: :class:`ephys_link.common.DriveToDepthOutputData`
         """
         pass
 
     @abstractmethod
     def _set_inside_brain(
-        self, manipulator_id: str, inside: bool
+            self, manipulator_id: str, inside: bool
     ) -> com.StateOutputData:
         """Set manipulator inside brain state (restricts motion)
 
         :param manipulator_id: The ID of the manipulator to set the state of
         :type manipulator_id: str
         :param inside: True if inside brain, False if outside
         :type inside: bool
@@ -454,19 +455,19 @@
         :return: Callback parameters (manipulator ID, error message)
         :rtype: str
         """
         pass
 
     @abstractmethod
     def _set_can_write(
-        self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
+            self,
+            manipulator_id: str,
+            can_write: bool,
+            hours: float,
+            sio: socketio.AsyncServer,
     ) -> com.StateOutputData:
         """Set manipulator can_write state (enables/disabled moving manipulator)
 
         :param manipulator_id: The ID of the manipulator to set the state of
         :type manipulator_id: str
         :param can_write: True if allowed to move, False if outside
         :type can_write: bool
```

### Comparing `ephys_link-0.0.8/ephys_link/server.py` & `ephys_link-0.1/ephys_link/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,43 +8,48 @@
 3. Call the appropriate function in :mod:`ephys_link.sensapex_handler` with arguments
 4. Relay the response from :mod:`ephys_link.sensapex_handler` to the callback function
 """
 
 import argparse
 import importlib
 import signal
-import sys
 import time
-from threading import Thread
+from threading import Event, Thread
+from tkinter import Tk
 from typing import Any
 
 import common as com
 
 # noinspection PyPackageRequirements
 import socketio
 from aiohttp import web
+from aiohttp.web_runner import GracefulExit
+from gui import GUI
 from platform_handler import PlatformHandler
+from pythonnet import load
 from serial import Serial
 from serial.tools.list_ports import comports
 
 # Setup server
+load("netfx")
 sio = socketio.AsyncServer()
 app = web.Application()
 sio.attach(app)
 is_connected = False
 
 # Declare platform handler
 platform: PlatformHandler
 
 # Setup argument parser
 parser = argparse.ArgumentParser(
     description="Electrophysiology Manipulator Link: a websocket interface for"
     " manipulators in electrophysiology experiments",
     prog="python -m ephys-link",
 )
+parser.add_argument("-g", "--gui", dest="gui", action="store_true", help="Launches GUI")
 parser.add_argument(
     "-t",
     "--type",
     type=str,
     dest="type",
     default="sensapex",
     help='Manipulator type (i.e. "sensapex" or "new_scale"). Default: "sensapex"',
@@ -57,44 +62,43 @@
     "--port",
     type=int,
     default=8081,
     dest="port",
     help="Port to serve on. Default: 8081 (avoids conflict with other HTTP servers)",
 )
 parser.add_argument(
-    "--new-scale-port",
-    type=int,
-    default=8080,
-    dest="new_scale_port",
-    help="Port to query New Scale HTTP server on. Default: 8080",
-)
-parser.add_argument(
     "-s",
     "--serial",
     type=str,
     default="no-e-stop",
     dest="serial",
     nargs="?",
     help="Emergency stop serial port (i.e. COM3). Default: disables emergency stop",
 )
 parser.add_argument(
     "--version",
     action="version",
-    version="Electrophysiology Manipulator Link v0.0.1",
+    version="Electrophysiology Manipulator Link v0.1",
     help="Print version and exit",
 )
 
+# Is the server running
+is_running = False
+
 # Setup Arduino serial port
 poll_rate = 0.05
-continue_polling = True
+kill_serial_event = Event()
+poll_serial_thread: Thread
 
 
-def poll_serial(serial_port: str) -> None:
+def poll_serial(kill_event: Event, serial_port: str) -> None:
     """Continuously poll serial port for data
 
+    :param kill_event: Event to stop polling
+    :type kill_event: Event
     :param serial_port: The serial port to poll
     :type serial_port: str
     :return: None
     """
     target_port = serial_port
     if serial_port is None:
         # Search for serial ports
@@ -103,22 +107,23 @@
                 target_port = port
                 break
     elif serial_port == "no-e-stop":
         # Stop polling if no-e-stop is specified
         return None
 
     ser = Serial(target_port, 9600, timeout=poll_rate)
-    while continue_polling:
+    while not kill_event.is_set():
         if ser.in_waiting > 0:
             ser.readline()
             # Cause a break
             com.dprint("[EMERGENCY STOP]\t\t Stopping all manipulators")
             platform.stop()
             ser.reset_input_buffer()
         time.sleep(poll_rate)
+    print("Close poll")
     ser.close()
 
 
 # Handle connection events
 
 
 @sio.event
@@ -385,15 +390,15 @@
         f'{"true" if can_write else "false"}'
     )
 
     return platform.set_can_write(manipulator_id, can_write, hours, sio)
 
 
 @sio.event
-async def stop(_) -> bool:
+def stop(_) -> bool:
     """Stop all manipulators
 
     :param _: Socket session ID (unused)
     :type _: str
     :return: True if successful, False otherwise
     :rtype: bool
     """
@@ -416,53 +421,100 @@
     """
     print(f"[UNKNOWN EVENT]:\t {data}")
 
 
 # Handle server start and end
 
 
-def launch() -> None:
+def launch_server(platform_type: str, server_port: int) -> None:
     """Launch the server
 
+    :param platform_type: Parsed argument for platform type
+    :type platform_type: str
+    :param server_port: HTTP port to serve the server
+    :type server_port: int
     :return: None
     """
-    # Parse arguments
-    args = parser.parse_args()
-    com.set_debug(args.debug)
 
     # Import correct manipulator handler
     global platform
-    if args.type == "sensapex":
-        platform = importlib.import_module(
-            "platforms.sensapex_handler"
-        ).SensapexHandler()
-    elif args.type == "new_scale":
-        platform = importlib.import_module(
-            "platforms.new_scale_handler"
-        ).NewScaleHandler(args.new_scale_port)
-    else:
-        exit(f"[ERROR]\t\t Invalid manipulator type: {args.type}")
-
-    # Start server
-    signal.signal(signal.SIGINT, close)
-    Thread(target=poll_serial, args=(args.serial,)).start()
-    web.run_app(app, port=args.port)
-
+    match platform_type:
+        case "sensapex":
+            platform = importlib.import_module(
+                "platforms.sensapex_handler"
+            ).SensapexHandler()
+        case "new_scale":
+            platform = importlib.import_module(
+                "platforms.new_scale_handler"
+            ).NewScaleHandler()
+        case unknown_type:
+            exit(f"[ERROR]\t\t Invalid manipulator type: {unknown_type}")
+
+    # List available manipulators
+    print("Available Manipulators:")
+    print(platform.get_manipulators()["manipulators"])
+
+    # Mark that server is running
+    global is_running
+    is_running = True
+    web.run_app(app, port=server_port)
 
-def close(_, __) -> None:
-    """Close the server
 
-    :param _: Signal number (unused)
-    :type _: int
-    :param __: Frame (unused)
-    :type __: Any
-    :return: None
-    """
+def close_server(_, __) -> None:
+    """Close the server"""
     print("[INFO]\t\t Closing server")
-    global continue_polling
-    continue_polling = False
+
+    # Stop movement
     platform.stop()  # noqa
-    sys.exit(0)
+
+    # Exit
+    raise GracefulExit()
+
+
+def close_serial(_, __) -> None:
+    """Close the serial connection"""
+    print("[INFO]\t\t Closing serial")
+    kill_serial_event.set()
+    poll_serial_thread.join()
+
+
+def start() -> None:
+    """Starts everything"""
+
+    # Parse arguments
+    args = parser.parse_args()
+    com.set_debug(args.debug)
+
+    if args.gui:
+        # Start GUI (doesn't launch server yet)
+        root = Tk()
+        GUI(root, launch_server, stop, poll_serial, args)
+        root.mainloop()
+
+    else:
+        if args.serial != "no-e-stop":
+            # Register serial exit
+            signal.signal(signal.SIGTERM, close_serial)
+            signal.signal(signal.SIGINT, close_serial)
+
+            # Start emergency stop system if serial is provided
+            global poll_serial_thread
+            poll_serial_thread = Thread(
+                target=poll_serial,
+                args=(
+                    kill_serial_event,
+                    args.serial,
+                ),
+                daemon=True,
+            )
+            poll_serial_thread.start()
+
+        # Register server exit
+        signal.signal(signal.SIGTERM, close_server)
+        signal.signal(signal.SIGINT, close_server)
+
+        # Launch with parsed arguments on main thread
+        launch_server(args.type, args.port)
 
 
 if __name__ == "__main__":
-    launch()
+    start()
```

### Comparing `ephys_link-0.0.8/ephys_link/platforms/new_scale_handler.py` & `ephys_link-0.1/ephys_link/platforms/new_scale_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,119 @@
 """Handle communications with New Scale API
 
 Implements New Scale specific API calls.
 
 This is a subclass of :class:`ephys_link.platform_handler.PlatformHandler`.
 """
 
-from json import loads
-from urllib import request
+import importlib
+
+# noinspection PyPackageRequirements
+import clr
 
 # noinspection PyPackageRequirements
 import socketio
 
 from ephys_link import common as com
 from ephys_link.platform_handler import PlatformHandler
 
 
 class NewScaleHandler(PlatformHandler):
     """Handler for New Scale platform"""
 
-    # Valid New Scale manipulator IDs
-    VALID_MANIPULATOR_IDS = {
-        "A",
-        "B",
-        "C",
-        "D",
-        "E",
-        "F",
-        "G",
-        "H",
-        "I",
-        "J",
-        "K",
-        "L",
-        "M",
-        "N",
-        "O",
-        "P",
-        "Q",
-        "R",
-        "S",
-        "T",
-        "U",
-        "V",
-        "W",
-        "X",
-        "Y",
-        "Z",
-        "AA",
-        "AB",
-        "AC",
-        "AD",
-        "AE",
-        "AF",
-        "AG",
-        "AH",
-        "AI",
-        "AJ",
-        "AK",
-        "AL",
-        "AM",
-        "AN",
-    }
-
-    def __init__(self, port: int = 8080):
+    def __init__(self) -> None:
+        """Initialize New Scale handler"""
         super().__init__()
-        self.port = port
 
-        # Test connection to New Scale HTTP server
-        try:
-            request.urlopen(f"http://localhost:{self.port}")
-        except Exception as e:
-            raise ValueError(
-                f"New Scale HTTP server not online on port {self.port}"
-            ) from e
-
-    def query_data(self) -> dict:
-        """Query New Scale HTTP server for data and return as dict
-
-        :return: dict of data (originally in JSON)
-        """
-        try:
-            return loads(request.urlopen(f"http://localhost:{self.port}").read())
-        except Exception as e:
-            print(f"[ERROR]\t\t Unable to query for New Scale data: {type(e)} {e}\n")
-
-    def query_manipulator_data(self, manipulator_id: str) -> dict:
-        """Query New Scale HTTP server for data on a specific manipulator
-
-        :param manipulator_id: manipulator ID
-        :return: dict of data (originally in JSON)
-        :raises ValueError: if manipulator ID is not found in query
-        """
-        data_query = self.query_data()["ProbeArray"]
-        manipulator_data = data_query[self.manipulators[manipulator_id]]
-
-        # If the order of the manipulators switched (somehow)
-        if manipulator_data["Id"] != manipulator_id:
-            # Recalculate index and get data
-            (manipulator_index, manipulator_data) = next(
-                (
-                    (index, data)
-                    for index, data in enumerate(self.query_data()["ProbeArray"])
-                    if data["Id"] == manipulator_id
-                ),
-                (None, None),
-            )
-            # Update index in manipulators dict
-            if manipulator_index:
-                self.manipulators[manipulator_id] = manipulator_index
-
-        # If data query was unsuccessful
-        if not manipulator_data:
-            raise ValueError(f"Unable to find manipulator {manipulator_id}")
+        # FIXME: Remove after #165
+        self.type = "new_scale"
 
-        # Return data
-        return manipulator_data
+        # Load New Scale API
+        clr.AddReference("../resources/NstMotorCtrl")
+        # noinspection PyUnresolvedReferences
+        from NstMotorCtrl import NstCtrlHostIntf
+
+        self.ctrl = NstCtrlHostIntf()
+
+        # Connect manipulators and initialize
+        self.ctrl.ShowProperties()
+        self.ctrl.Initialize()
 
     def _get_manipulators(self) -> list:
-        return [probe["Id"] for probe in self.query_data()["ProbeArray"]]
+        return list(map(str, range(self.ctrl.PortCount)))
 
     def _register_manipulator(self, manipulator_id: str) -> None:
-        # Check if ID is a valid New Scale manipulator ID
-        if manipulator_id not in self.VALID_MANIPULATOR_IDS:
-            raise ValueError(f"Invalid manipulator ID {manipulator_id}")
+        # Check if ID is numeric
+        if not manipulator_id.isnumeric():
+            raise ValueError("Manipulator ID must be numeric")
 
         # Check if ID is connected
         if manipulator_id not in self._get_manipulators():
             raise ValueError(f"Manipulator {manipulator_id} not connected")
 
-        # Get index of the manipulator
-        manipulator_index = next(
-            (
-                index
-                for index, data in enumerate(self.query_data()["ProbeArray"])
-                if data["Id"] == manipulator_id
-            ),
-            None,
+        # Check if there are enough axes
+        if int(manipulator_id) * 3 + 2 >= self.ctrl.AxisCount:
+            raise ValueError(f"Manipulator {manipulator_id} has no axes")
+
+        # Register manipulator
+        first_axis_index = int(manipulator_id) * 3
+        self.manipulators[manipulator_id] = importlib.import_module(
+            "new_scale_manipulator"
+        ).NewScaleManipulator(
+            manipulator_id,
+            self.ctrl.GetAxis(first_axis_index),
+            self.ctrl.GetAxis(first_axis_index + 1),
+            self.ctrl.GetAxis(first_axis_index + 2),
         )
-        if manipulator_index is None:
-            raise ValueError(f"Unable to find manipulator {manipulator_id}")
-        self.manipulators[manipulator_id] = manipulator_index
 
     def _unregister_manipulator(self, manipulator_id: str) -> None:
         del self.manipulators[manipulator_id]
 
     def _get_pos(self, manipulator_id: str) -> com.PositionalOutputData:
-        manipulator_data = self.query_manipulator_data(manipulator_id)
-        return com.PositionalOutputData(
-            [
-                manipulator_data["Stage_X"],
-                manipulator_data["Stage_Y"],
-                manipulator_data["Stage_Z"],
-                0,
-            ],
-            "",
-        )
+        return self.manipulators[manipulator_id].get_pos()
 
     async def _goto_pos(
         self, manipulator_id: str, position: list[float], speed: int
     ) -> com.PositionalOutputData:
-        pass
+        return await self.manipulators[manipulator_id].goto_pos(position, speed)
 
     async def _drive_to_depth(
         self, manipulator_id: str, depth: float, speed: int
     ) -> com.DriveToDepthOutputData:
-        pass
+        return await self.manipulators[manipulator_id].drive_to_depth(depth, speed)
 
     def _set_inside_brain(
         self, manipulator_id: str, inside: bool
     ) -> com.StateOutputData:
-        pass
+        self.manipulators[manipulator_id].set_inside_brain(inside)
+        com.dprint(
+            f"[SUCCESS]\t Set inside brain state for manipulator:"
+            f" {manipulator_id}\n"
+        )
+        return com.StateOutputData(inside, "")
 
     async def _calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
-        pass
+        return (
+            ""
+            if self.manipulators[manipulator_id].calibrate()
+            else "Error calling calibrate"
+        )
 
     def _bypass_calibration(self, manipulator_id: str) -> str:
+        self.manipulators[manipulator_id].set_calibrated()
+        com.dprint(
+            f"[SUCCESS]\t Bypassed calibration for manipulator" f" {manipulator_id}\n"
+        )
         return ""
 
     def _set_can_write(
         self,
         manipulator_id: str,
         can_write: bool,
         hours: float,
         sio: socketio.AsyncServer,
     ) -> com.StateOutputData:
-        pass
+        self.manipulators[manipulator_id].set_can_write(can_write, hours, sio)
+        com.dprint(
+            f"[SUCCESS]\t Set can_write state for manipulator" f" {manipulator_id}\n"
+        )
+        return com.StateOutputData(can_write, "")
```

### Comparing `ephys_link-0.0.8/ephys_link/platforms/sensapex_handler.py` & `ephys_link-0.1/ephys_link/platforms/sensapex_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/ephys_link/platforms/sensapex_manipulator.py` & `ephys_link-0.1/ephys_link/platforms/sensapex_manipulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Sensapex manipulator API calls
+"""Sensapex Manipulator class
 
 Handles logic for calling Sensapex API functions. Also includes extra logic for safe
 function calls, error handling, managing per-manipulator attributes, and returning the
 appropriate callback parameters like in :mod:`ephys_link.sensapex_handler`.
 """
 
 import asyncio
@@ -20,42 +20,27 @@
 class SensapexManipulator:
     """Representation of a single Sensapex manipulator
 
     :param device: A Sensapex device
     :type device: :class: `sensapex.SensapexDevice`
     """
 
-    # How fast a manipulator is allowed to drive when inside the brain (in µm/s)
-    INSIDE_BRAIN_SPEED_LIMIT = 10
-
     def __init__(self, device: SensapexDevice) -> None:
-        """Construct a new Manipulator object"""
+        """Construct a new Manipulator object
+
+        :param device: A Sensapex device
+        """
         self._device = device
         self._id = device.dev_id
         self._calibrated = False
         self._inside_brain = False
         self._can_write = False
         self._reset_timer = None
         self._move_queue = deque()
 
-    class Movement:
-        """Movement data struct
-
-        :param event: An asyncio event
-        :type event: :class: `asyncio.Event`
-        :param position: A tuple of floats (x, y, z, w) representing the position to
-            move to in µm
-        :type position: list[float]
-        """
-
-        def __init__(self, event: asyncio.Event, position: list[float]) -> None:
-            """Construct a new Movement object"""
-            self.event = event
-            self.position = position
-
     # Device functions
     def get_pos(self) -> com.PositionalOutputData:
         """Get the current position of the manipulator and convert it into mm
 
         :return: Callback parameters (position in (x, y, z, w) (or an empty array on
             error), error message)
         :rtype: :class:`ephys_link.common.PositionalOutputData`
@@ -78,50 +63,49 @@
         :type position: list[float]
         :param speed: The speed to move at (in µm/s)
         :type speed: float
         :return: Callback parameters (position in (x, y, z, w) (or an empty array on
             error), error message)
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
+        # Check if able to write
+        if not self._can_write:
+            print(f"[ERROR]\t\t Manipulator {self._id} movement " f"canceled")
+            return com.PositionalOutputData([], "Manipulator " "movement canceled")
+
         # Convert position to µm
-        position = [axis * 1000 for axis in position]
+        position_um = [axis * 1000 for axis in position]
 
-        # Add movement to queue
-        self._move_queue.appendleft(self.Movement(asyncio.Event(), position))
+        # Push movement intent to queue
+        self._move_queue.appendleft(asyncio.Event())
 
         # Wait for preceding movement to finish
         if len(self._move_queue) > 1:
-            await self._move_queue[1].event.wait()
-
-        if not self._can_write:
-            print(f"[ERROR]\t\t Manipulator {self._id} movement " f"canceled")
-            return com.PositionalOutputData([], "Manipulator " "movement canceled")
+            await self._move_queue[1].wait()
 
         try:
-            target_position = position
-            target_speed = speed
+            target_position = position_um
 
-            # Alter target position if inside brain
+            # Restrict target position to just depth-axis if inside brain
             if self._inside_brain:
                 target_position = self._device.get_pos()
-                target_position[3] = position[3]
-                target_speed = min(speed, self.INSIDE_BRAIN_SPEED_LIMIT)
+                target_position[3] = position_um[3]
 
-            # Move manipulator
-            movement = self._device.goto_pos(target_position, target_speed)
+            # Send move command
+            movement = self._device.goto_pos(target_position, speed)
 
             # Wait for movement to finish
             while not movement.finished:
                 await asyncio.sleep(0.1)
 
             # Get position
             manipulator_final_position = self._device.get_pos()
 
             # Remove event from queue and mark as completed
-            self._move_queue.pop().event.set()
+            self._move_queue.pop().set()
 
             com.dprint(
                 f"[SUCCESS]\t Moved manipulator {self._id} to position"
                 f" {manipulator_final_position}\n"
             )
             return com.PositionalOutputData(manipulator_final_position, "")
         except Exception as e:
```

### Comparing `ephys_link-0.0.8/ephys_link/resources/libum.dll` & `ephys_link-0.1/ephys_link/resources/libum.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/scripts/draw_demo.py` & `ephys_link-0.1/scripts/draw_demo.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/scripts/probe_crash_test.py` & `ephys_link-0.1/scripts/probe_crash_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/scripts/read_to_file.py` & `ephys_link-0.1/scripts/read_to_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 def cleanup(_, __):
     print("Cleaning up")
     global running
     running = False
 
     for manipulator in manipulators:
         manipulator.file.flush()
-        manipulator.file.close()
+        manipulator.file.close_server()
 
     sio.disconnect()
 
 
 print("Begin recording")
 for manipulator_id in manipulators.keys():
     sio.emit("get_pos", manipulator_id, callback=record)
```

### Comparing `ephys_link-0.0.8/tests/calibration_test.py` & `ephys_link-0.1/tests/calibration_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/tests/can_write_test.py` & `ephys_link-0.1/tests/can_write_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/tests/drive_to_depth_test.py` & `ephys_link-0.1/tests/drive_to_depth_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/tests/get_manipulators_test.py` & `ephys_link-0.1/tests/get_manipulators_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/tests/get_pos_test.py` & `ephys_link-0.1/tests/get_pos_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     """Tests get_pos event"""
 
     def setUp(self):
         """Setup test case"""
         self.sio = socketio.Client()
         self.mock = Mock()
 
-        self.sio.connect("http://localhost:8080")
+        self.sio.connect("http://localhost:8081")
 
     def test_get_pos_unregistered(self):
         """Test get_pos event with unregistered manipulator"""
-        self.sio.emit("get_pos", 1, callback=self.mock)
-        self.sio.emit("bypass_calibration", 1)
+        self.sio.emit("get_pos", "1", callback=self.mock)
+        self.sio.emit("bypass_calibration", "1")
         self.wait_for_callback()
 
         self.mock.assert_called_with(
             PositionalOutputData([], "Manipulator not registered")
         )
 
     def test_get_pos_registered(self):
         """Test get_pos event with registered manipulator"""
-        self.sio.emit("register_manipulator", 1)
-        self.sio.emit("bypass_calibration", 1)
-        self.sio.emit("get_pos", 1, callback=self.mock)
+        self.sio.emit("register_manipulator", "1")
+        self.sio.emit("bypass_calibration", "1")
+        self.sio.emit("get_pos", "1", callback=self.mock)
         self.wait_for_callback()
 
         args = self.mock.call_args.args[0]
         self.assertEqual(len(args["position"]), 4)
         self.assertEqual(args["error"], "")
 
     def tearDown(self) -> None:
```

### Comparing `ephys_link-0.0.8/tests/inside_brain_test.py` & `ephys_link-0.1/tests/inside_brain_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/tests/move_test.py` & `ephys_link-0.1/tests/stop_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from unittest import TestCase
 from unittest.mock import Mock
 
 # noinspection PyPackageRequirements
 import socketio
 
-from ephys_link.common import PositionalOutputData
-
 
 # noinspection DuplicatedCode
-class MoveTest(TestCase):
-    """Tests movement event"""
+class StopTest(TestCase):
+    """Tests stop event"""
 
     DRIVE_SPEED = 8000
 
     def setUp(self) -> None:
         """Setup test case"""
         self.sio = socketio.Client()
         self.mock = Mock()
 
         self.sio.connect("http://localhost:8080")
 
-    def test_move_no_asserts(self):
-        """Test movement without asserts"""
+    def test_stop_event(self):
+        """Test stopping movement with event"""
         self.sio.emit("register_manipulator", 1)
         self.sio.emit("register_manipulator", 2)
         self.sio.emit("bypass_calibration", 1)
         self.sio.emit("bypass_calibration", 2)
         self.sio.emit(
             "set_can_write", {"manipulator_id": 1, "can_write": True, "hours": 1}
         )
@@ -47,88 +45,80 @@
         self.sio.emit(
             "goto_pos",
             {
                 "manipulator_id": 1,
                 "pos": [10000, 10000, 10000, 10000],
                 "speed": self.DRIVE_SPEED,
             },
-            callback=self.mock,
         )
         self.sio.emit(
             "goto_pos",
             {
                 "manipulator_id": 2,
                 "pos": [10000, 10000, 10000, 10000],
                 "speed": self.DRIVE_SPEED,
             },
-            callback=self.mock,
         )
 
-        while self.mock.call_count != 4:
+        while self.mock.call_count != 2:
             pass
 
-    def test_move_with_asserts(self):
-        """Test movement with asserts"""
-        self.sio.emit("register_manipulator", 1)
-        self.sio.emit("register_manipulator", 2)
-        self.sio.emit("bypass_calibration", 1)
-        self.sio.emit("bypass_calibration", 2)
-        self.sio.emit(
-            "set_can_write", {"manipulator_id": 1, "can_write": True, "hours": 1}
-        )
-        self.sio.emit(
-            "set_can_write", {"manipulator_id": 2, "can_write": True, "hours": 1}
-        )
+        self.sio.sleep(1)
+
+        # Test stop
+        self.mock.called = False
+        self.sio.emit("stop", callback=self.mock)
+        self.wait_for_callback()
+        stop_arg = self.mock.call_args.args[0]
 
+        # Test no calibration
         self.sio.emit(
             "goto_pos",
             {"manipulator_id": 1, "pos": [0, 0, 0, 0], "speed": self.DRIVE_SPEED},
             callback=self.mock,
         )
         self.wait_for_callback()
         args = self.mock.call_args.args[0]
-        self.assertEqual(args["error"], "")
-        self.assertEqual(len(args["position"]), 4)
 
+        # Bring back to home
+        self.mock.call_count = 0
+        self.sio.emit("bypass_calibration", 1)
+        self.sio.emit("bypass_calibration", 2)
+        self.sio.emit(
+            "set_can_write", {"manipulator_id": 1, "can_write": True, "hours": 1}
+        )
+        self.sio.emit(
+            "set_can_write", {"manipulator_id": 2, "can_write": True, "hours": 1}
+        )
         self.sio.emit(
             "goto_pos",
             {
                 "manipulator_id": 1,
                 "pos": [10000, 10000, 10000, 10000],
                 "speed": self.DRIVE_SPEED,
             },
             callback=self.mock,
         )
-        self.wait_for_callback()
-
-    def test_move_unregistered(self):
-        """Test movement with unregistered manipulator"""
         self.sio.emit(
             "goto_pos",
-            {"manipulator_id": 1, "pos": [0, 0, 0, 0], "speed": self.DRIVE_SPEED},
+            {
+                "manipulator_id": 2,
+                "pos": [10000, 10000, 10000, 10000],
+                "speed": self.DRIVE_SPEED,
+            },
             callback=self.mock,
         )
-        self.wait_for_callback()
-        self.mock.assert_called_with(
-            PositionalOutputData([], "Manipulator not registered")
-        )
 
-    def test_move_no_write(self):
-        """Test movement with no write"""
-        self.sio.emit("register_manipulator", 1)
-        self.sio.emit("bypass_calibration", 1)
-        self.sio.emit(
-            "goto_pos",
-            {"manipulator_id": 1, "pos": [0, 0, 0, 0], "speed": self.DRIVE_SPEED},
-            callback=self.mock,
-        )
-        self.wait_for_callback()
-        self.mock.assert_called_with(
-            PositionalOutputData([], "Cannot write to manipulator")
-        )
+        while self.mock.call_count != 2:
+            pass
+
+        # Asserts
+        self.assertTrue(stop_arg)
+        self.assertEqual(len(args), 2)
+        self.assertEqual(args["error"], "Cannot write to manipulator")
 
     def tearDown(self) -> None:
         """Cleanup test case"""
         self.sio.disconnect()
 
     def wait_for_callback(self):
         """Wait for callback to be called"""
```

### Comparing `ephys_link-0.0.8/tests/register_manipulator_test.py` & `ephys_link-0.1/tests/register_manipulator_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,34 +9,34 @@
     """Tests manipulator registration"""
 
     def setUp(self) -> None:
         """Setup test case"""
         self.sio = socketio.Client()
         self.mock = Mock()
 
-        self.sio.connect("http://localhost:8080")
+        self.sio.connect("http://localhost:8081")
 
     def test_register_manipulator(self):
         """Tests registering a manipulator"""
-        self.sio.emit("register_manipulator", 1, callback=self.mock)
+        self.sio.emit("register_manipulator", "1", callback=self.mock)
         self.wait_for_callback()
 
         self.mock.assert_called_with("")
 
     def test_re_register_manipulator(self):
         """Test re-registering a manipulator"""
         self.sio.emit("register_manipulator", 1)
         self.sio.emit("register_manipulator", 1, callback=self.mock)
         self.wait_for_callback()
 
         self.mock.assert_called_with("Manipulator already registered")
 
     def test_register_unknown_manipulator(self):
         """Test registering an unknown manipulator"""
-        self.sio.emit("register_manipulator", 3, callback=self.mock)
+        self.sio.emit("register_manipulator", 99, callback=self.mock)
         self.wait_for_callback()
 
         self.mock.assert_called_with("Manipulator not found")
 
     def tearDown(self) -> None:
         """Cleanup test case"""
         self.sio.disconnect()
```

### Comparing `ephys_link-0.0.8/.gitignore` & `ephys_link-0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/LICENSE` & `ephys_link-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ephys_link-0.0.8/README.md` & `ephys_link-0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,21 @@
        system (macOS users should virtualize Linux).
 2. For Sensapex devices, the controller unit must be connected to the PC via an
    ethernet cable. A USB-to-ethernet adapter is acceptable as well.
 3. To use the emergency stop feature, ensure an Arduino with
    the [StopSignal][StopSignal] sketch is connected to the computer. Follow
    the instructions on that repo for how to set up the Arduino.
 
+**NOTE:** Ephys Link is an HTTP server without cross-origin support. The server is currently designed to interface with local/desktop instances of Pinpoint. It will not work with the web browser versions of Pinpoint at this time.
+
 ## Installation
 
-1. Ensure Python 3.8+ and pip are installed
-2. `pip install ephys-link`
+1. Ensure Python 3.10+ and pip are installed
+2. `pip install ephys-link --use-pep517`
+    1. PEP 517 is needed to allow the Sensapex Manipulator API to be installed
 3. Run `python -m ephys_link` to start the server
     1. To view available command-line arguments,
        run `python -m ephys_link --help`
     2. Note: all arguments are optional and none are needed to use the server
        normally
 
 # Usage and more
```

### Comparing `ephys_link-0.0.8/pyproject.toml` & `ephys_link-0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ephys-link"
-version = "0.0.8"
+version = "0.1"
 authors = [{ name = "Kenneth Yang", email = "kjy5@uw.edu" }]
 description = "A Python WebSocket server that allows any WebSocket compliant application to communicate with manipulators used in electrophysiology experiments."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 keywords = ["websocket", "manipulator", "electrophysiology", "ephys", "sensapex", "neuroscience", "vbl", "brain"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Healthcare Industry",
@@ -21,14 +21,15 @@
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 dependencies = [
     "aiohttp ~= 3.8",
     "pyserial ~= 3.5",
     "python-socketio ~= 5.7",
+    "pythonnet ~= 3.0",
     "sensapex ~= 1.22",
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/VirtualBrainLab/ephys-link"
 Documentation = "https://virtualbrainlab.org/05_misc/03_ephys_link.html"
 "Issue Tracker" = "https://github.com/VirtualBrainLab/ephys-link/issues"
```

### Comparing `ephys_link-0.0.8/PKG-INFO` & `ephys_link-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephys-link
-Version: 0.0.8
+Version: 0.1
 Summary: A Python WebSocket server that allows any WebSocket compliant application to communicate with manipulators used in electrophysiology experiments.
 Project-URL: GitHub, https://github.com/VirtualBrainLab/ephys-link
 Project-URL: Documentation, https://virtualbrainlab.org/05_misc/03_ephys_link.html
 Project-URL: Issue Tracker, https://github.com/VirtualBrainLab/ephys-link/issues
 Author-email: Kenneth Yang <kjy5@uw.edu>
 License-File: LICENSE
 Keywords: brain,electrophysiology,ephys,manipulator,neuroscience,sensapex,vbl,websocket
@@ -13,18 +13,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: aiohttp~=3.8
 Requires-Dist: pyserial~=3.5
 Requires-Dist: python-socketio~=5.7
+Requires-Dist: pythonnet~=3.0
 Requires-Dist: sensapex~=1.22
 Description-Content-Type: text/markdown
 
 # Electrophysiology Manipulator Link
 
 The Electrophysiology Manipulator Link (or Ephys Link for short) is a Python
 WebSocket server that allows any WebSocket-compliant application (such
@@ -46,18 +47,21 @@
        system (macOS users should virtualize Linux).
 2. For Sensapex devices, the controller unit must be connected to the PC via an
    ethernet cable. A USB-to-ethernet adapter is acceptable as well.
 3. To use the emergency stop feature, ensure an Arduino with
    the [StopSignal][StopSignal] sketch is connected to the computer. Follow
    the instructions on that repo for how to set up the Arduino.
 
+**NOTE:** Ephys Link is an HTTP server without cross-origin support. The server is currently designed to interface with local/desktop instances of Pinpoint. It will not work with the web browser versions of Pinpoint at this time.
+
 ## Installation
 
-1. Ensure Python 3.8+ and pip are installed
-2. `pip install ephys-link`
+1. Ensure Python 3.10+ and pip are installed
+2. `pip install ephys-link --use-pep517`
+    1. PEP 517 is needed to allow the Sensapex Manipulator API to be installed
 3. Run `python -m ephys_link` to start the server
     1. To view available command-line arguments,
        run `python -m ephys_link --help`
     2. Note: all arguments are optional and none are needed to use the server
        normally
 
 # Usage and more
```

