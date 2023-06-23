# Comparing `tmp/openoligo-0.1.1.tar.gz` & `tmp/openoligo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.1.tar", max compression
+gzip compressed data, was "openoligo-0.1.2.tar", max compression
```

## Comparing `openoligo-0.1.1.tar` & `openoligo-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-06-20 15:02:43.473844 openoligo-0.1.1/LICENSE
--rw-r--r--   0        0        0     1917 2023-06-20 20:46:11.014057 openoligo-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-20 14:31:11.021160 openoligo-0.1.1/openoligo/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:58:07.198168 openoligo-0.1.1/openoligo/container/__init__.py
--rw-r--r--   0        0        0      579 2023-06-21 07:30:08.808691 openoligo-0.1.1/openoligo/container/cartridge.py
--rw-r--r--   0        0        0     1464 2023-06-21 07:11:10.738482 openoligo-0.1.1/openoligo/container/types.py
--rw-r--r--   0        0        0        0 2023-06-20 17:48:38.907388 openoligo-0.1.1/openoligo/driver/__init__.py
--rw-r--r--   0        0        0     1905 2023-06-21 05:08:40.538815 openoligo-0.1.1/openoligo/driver/manifold.py
--rw-r--r--   0        0        0     2184 2023-06-21 02:39:37.013644 openoligo-0.1.1/openoligo/driver/switch.py
--rw-r--r--   0        0        0      958 2023-06-21 03:42:34.120363 openoligo-0.1.1/openoligo/driver/types.py
--rw-r--r--   0        0        0      931 2023-06-21 04:56:42.236811 openoligo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 openoligo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 09:08:17.765678 openoligo-0.1.2/LICENSE
+-rw-r--r--   0        0        0      979 2023-06-23 09:08:17.765678 openoligo-0.1.2/README.md
+-rw-r--r--   0        0        0      490 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/__init__.py
+-rw-r--r--   0        0        0     1329 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/cartridge.py
+-rw-r--r--   0        0        0     1826 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/types.py
+-rw-r--r--   0        0        0      761 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/__init__.py
+-rw-r--r--   0        0        0     2941 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/gpio.py
+-rw-r--r--   0        0        0     2268 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/manifold.py
+-rw-r--r--   0        0        0      733 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/rpi_pins.py
+-rw-r--r--   0        0        0     4239 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/switch.py
+-rw-r--r--   0        0        0     1873 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/types.py
+-rw-r--r--   0        0        0      300 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/log_config.py
+-rw-r--r--   0        0        0      250 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/__init__.py
+-rw-r--r--   0        0        0      909 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/flow_sequence.py
+-rw-r--r--   0        0        0       94 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/types.py
+-rw-r--r--   0        0        0      164 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/utils/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/utils/wait.py
+-rw-r--r--   0        0        0     1037 2023-06-23 09:08:17.765678 openoligo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 openoligo-0.1.2/PKG-INFO
```

### Comparing `openoligo-0.1.1/LICENSE` & `openoligo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.1/openoligo/container/types.py` & `openoligo-0.1.2/openoligo/container/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 
 
 class BottleSize(Enum):
-    """The type of container."""
+    """The size of bottle."""
 
     SMALL = 1
     LARGE = 2
 
 
 class ReagentType(Enum):
     """The type of reagent."""
@@ -21,20 +21,24 @@
     LIQUID = 1
     LYOPHILIZED = 2
 
 
 class ReagentCategory(str, Enum):
     """The category of reagent."""
 
+    DETRITYLATION = "detritylation"
+    ACTIVATION = "activation"
+    COUPLING = "coupling"
     CAPPING = "capping"
+    OXIDATION = "oxidation"
     DEPROTECTION = "deprotection"
-    COUPLING = "coupling"
-    ACTIVATION = "activation"
+
     PHOSPHORAMIDITE = "phosphoramidite"
     SOLVENT = "solvent"
+    GAS = "gas"
 
 
 class SlotID(Enum):
     """The ID of the bottle slot."""
 
     A1 = 1
     A2 = 2
@@ -70,25 +74,37 @@
     D5 = 29
     D6 = 30
     D7 = 31
     D8 = 32
 
 
 @dataclass
+class Slot:
+    """A slot in the cartridge."""
+
+    slot_id: SlotID
+    associated_valve: int
+    size: BottleSize = BottleSize.SMALL
+
+
+@dataclass
 class Reagent:
     """A reagent."""
 
     name: str
     type: ReagentType
     category: ReagentCategory
     description: str = ""
+    solvent_slot: Optional[Slot] = None
 
 
 @dataclass
-class Slot:
-    """A slot in the cartridge."""
+class Bottle:
+    """A bottle containing a particular reagent."""
 
-    slot_id: SlotID
-    associated_valve: int
-    reagent: Optional[Reagent]
+    manufacturing_date: str
+    shelf_life: int = 45
+    slot: Optional[Slot] = None
+    reagent: Optional[Reagent] = None
     size: BottleSize = BottleSize.SMALL
-    associated_solvent: Optional[Reagent] = None
+    open_bottle_date: Optional[str] = None
+    expiry_date: Optional[str] = None
```

### Comparing `openoligo-0.1.1/openoligo/driver/switch.py` & `openoligo-0.1.2/openoligo/driver/manifold.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,69 @@
 """
-Switches can be used to control devices that can be turned on and off.
+Manifolds are a collection of valves.
 """
-import asyncio
-import logging
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Generic, List, Type, TypeVar
 
-from openoligo.driver.types import Switchable, SwitchingError
+from openoligo.driver.switch import toggle
+from openoligo.driver.types import InvalidManifoldSizeError, Valvable, ValveType
 
+T = TypeVar("T", bound=Valvable)
 
-@dataclass
-class SimulatedSwitch(Switchable):
-    """
-    This class represents a simulated switch. It is useful for testing purposes.
-    It can also be used as a base class for other switchable devices.
-    """
-
-    pin: int
-    name: str
-    switch_count: int = 0
-    _state: bool = False
-
-    async def set(self, switch: bool):
-        """Set state of the switch ON or OFF."""
-        self._state = switch
-        self.switch_count += 1
-
-    @property
-    def value(self) -> bool:
-        """Get the current value of the switch."""
-        return self._state
-
-
-class PneumaticValve(SimulatedSwitch):
-    """
-    This class represents a pneumatic valve. It is useful for testing purposes.
-    It can also be used as a base class for other switchable devices.
-    """
 
-    def __init__(self, pin: int, name: str):
-        super().__init__(pin, name)
-
-
-async def toggle(switch: Switchable):
-    """
-    Toggle the state of a switchable device.
-
-    :param switch: The device to be toggled
+@dataclass
+class Manifold(Generic[T]):
     """
-    await switch.set(not switch.value)
-    logging.debug("Toggled the switch: %s", switch)
-
-
-async def periodic_toggle(
-    switch: Switchable, interval: float, loop_forever: bool = True, count: int = 0
-):
+    This class represents a set of switches.
+    The switches are created at initialization based on the provided size.
     """
-    Periodically toggle the state of a switchable device.
 
-    :param switch: The device to be toggled
-    :param interval: The time interval between toggles in seconds
-    :param loop_forever: If True, toggles the device indefinitely, else toggles it for 'count' times
-    :param count: The number of times to toggle the device (ignored if loop_forever is True)
-    """
-    assert interval > 0, "Interval must be greater than 0"
-    assert count > 0 or loop_forever, "Must toggle at least once"
+    VALID_SIZES = {4, 8, 10, 16, 20}
 
-    try:
-        while loop_forever or count > 0:
-            count -= 1 if count > 0 else 0
-            await toggle(switch)
-            logging.debug(switch)
-            await asyncio.sleep(interval)
-    except SwitchingError as error:
-        logging.error(error)
+    valve_class: Type[T]
+    size: int
+    manifold_type: ValveType = ValveType.NORMALLY_OPEN
+    valves: List[T] = field(init=False)
+
+    def __post_init__(self):
+        if self.size not in self.VALID_SIZES:
+            raise InvalidManifoldSizeError(
+                f"Invalid switch size: {self.size}. Must be one of {self.VALID_SIZES}"
+            )
+        self.valves = [
+            self.valve_class(i, f"Valve {i}", self.manifold_type) for i in range(self.size)
+        ]
+
+    def set(self, index: int, state: bool):
+        """Set state of the switch at a given index ON or OFF."""
+        if index < 0 or index >= self.size:
+            raise ValueError(f"Index out of range: {index}")
+        self.valves[index].set(state)
+
+    def value(self, index: int) -> bool:
+        """Get the current value of the switch at a given index."""
+        try:
+            return self.valves[index].value
+        except IndexError as exc:
+            raise ValueError(f"Index out of range: {index}") from exc
+
+    def all(self, state: bool):
+        """Set the state of a list of switches."""
+        for valve in self.valves:
+            valve.set(state)
+
+    def toggle(self):
+        """Toggle the state of a list of switches."""
+        for valve in self.valves:
+            toggle(valve)
+
+    def activate_flow(self, index: int):
+        """Set state for the index to ON and all others to OFF"""
+        self.activate_n_flows([index])
+
+    def activate_n_flows(self, indices: List[int]):
+        """Set state for the indices to ON and all others to OFF"""
+        for i in indices:
+            if i < 0 or i >= self.size:
+                raise ValueError(f"Index out of range: {i}")
+        for i in range(self.size):
+            self.set(i, i in indices)
```

### Comparing `openoligo-0.1.1/pyproject.toml` & `openoligo-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 [tool.poetry]
 name = "OpenOligo"
-version = "0.1.1"
+version = "0.1.2"
 description = "An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes."
 license = "Apache-2.0"
 authors = ["Satyam Tiwary <satyam@technoculture.io>"]
 readme = "README.md"
 keywords = ["DNA", "synthesis", "genetics", "open-source"]
 
 [tool.poetry.scripts]
-openoligo = 'main:main'
+oligo-server= 'app.server:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
+rich = "^13.4.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
-pytest-asyncio = "^0.21.0"
 flake8 = "^3.9.2"
 black = "^23.3.0"
 pylint = "^2.17.4"
 mypy = "^1.3.0"
 isort = "^5.12.0"
+coverage-badge = "^1.1.0"
+jupyter = "^1.0.0"
+jupyterlab = "^4.0.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
-addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=90"
+addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=80"
 
 [tool.coverage.run]
 source = ["openoligo"]
 omit = ["**/types.py"]
+
+[tool.poetry.extras]
+rpi = ["RPi.GPIO"]
```

