# Comparing `tmp/python_omnilogic_local-0.8.1.tar.gz` & `tmp/python_omnilogic_local-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.8.1.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.9.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.8.1.tar` & `python_omnilogic_local-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1901 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0      164 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8416 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9968 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10194 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6338 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5297 2023-06-07 17:59:35.373135 python_omnilogic_local-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 python_omnilogic_local-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1901 2023-06-07 19:03:22.167353 python_omnilogic_local-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 19:03:22.167353 python_omnilogic_local-0.9.0/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    25487 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     9745 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9968 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10194 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6502 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-06-07 19:03:22.171353 python_omnilogic_local-0.9.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5297 2023-06-07 19:03:23.119355 python_omnilogic_local-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 python_omnilogic_local-0.9.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.8.1/README.md` & `python_omnilogic_local-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/api.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -410,7 +410,82 @@
         parameter = ET.SubElement(parameters_element, "Parameter", name="DaysActive", dataType="int")
         parameter.text = str(days_active)
         parameter = ET.SubElement(parameters_element, "Parameter", name="Recurring", dataType="bool")
         parameter.text = str(int(recurring))
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
         return await self.async_send_message(MessageType.SET_STANDALONE_LIGHT_SHOW, req_body, False)
+
+    async def async_set_chlorinator_enable(self, pool_id: int, enabled: int | bool) -> None:
+        body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
+
+        name_element = ET.SubElement(body_element, "Name")
+        name_element.text = "SetCHLOREnable"
+
+        parameters_element = ET.SubElement(body_element, "Parameters")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
+        parameter.text = str(pool_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="Enabled", dataType="bool", alias="Data")
+        parameter.text = str(int(enabled))
+
+        req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
+
+        return await self.async_send_message(MessageType.SET_CHLOR_ENABLED, req_body, False)
+
+    async def async_set_chlorinator_params(
+        self,
+        pool_id: int,
+        equipment_id: int,
+        cfg_state: int,
+        op_mode: int,
+        bow_type: int,
+        cell_type: int,
+        timed_percent: int,
+        sc_timeout: int,
+        orp_timeout: int,
+    ) -> None:
+        body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
+
+        name_element = ET.SubElement(body_element, "Name")
+        name_element.text = "SetCHLORParams"
+
+        parameters_element = ET.SubElement(body_element, "Parameters")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
+        parameter.text = str(pool_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="ChlorID", dataType="int", alias="EquipmentID")
+        parameter.text = str(equipment_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="CfgState", dataType="byte", alias="Data1")
+        parameter.text = str(cfg_state)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="OpMode", dataType="byte", alias="Data2")
+        parameter.text = str(op_mode)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="BOWType", dataType="byte", alias="Data3")
+        parameter.text = str(bow_type)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="CellType", dataType="byte", alias="Data4")
+        parameter.text = str(cell_type)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="TimedPercent", dataType="byte", alias="Data5")
+        parameter.text = str(timed_percent)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="SCTimeout", dataType="byte", unit="hour", alias="Data6")
+        parameter.text = str(sc_timeout)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="ORPTimout", dataType="byte", unit="hour", alias="Data7")
+        parameter.text = str(orp_timeout)
+
+        req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
+
+        return await self.async_send_message(MessageType.SET_CHLOR_PARAMS, req_body, False)
+
+    async def async_set_chlorinator_superchlorinate(self, pool_id: int, equipment_id: int, enabled: int | bool) -> None:
+        body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
+
+        name_element = ET.SubElement(body_element, "Name")
+        name_element.text = "SetUISuperCHLORCmd"
+
+        parameters_element = ET.SubElement(body_element, "Parameters")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
+        parameter.text = str(pool_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="ChlorID", dataType="int", alias="EquipmentID")
+        parameter.text = str(equipment_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="IsOn", dataType="byte", alias="Data1")
+        parameter.text = str(int(enabled))
+
+        req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
+
+        return await self.async_send_message(MessageType.SET_SUPERCHLORINATE, req_body, False)
```

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from pydantic import BaseModel, Field, ValidationError
 from xmltodict import parse as xml_parse
 
 from ..exceptions import OmniParsingException
 from ..types import (
     BodyOfWaterType,
+    ChlorinatorDispenserType,
     ColorLogicLightType,
     ColorLogicShow,
     FilterType,
     HeaterType,
     OmniType,
     PumpFunction,
     PumpType,
@@ -133,36 +134,61 @@
 
         # The heater equipment are nested down inside a list of "Operations", which also includes non Heater-Equipment items.  We need to
         # first filter down to just the heater equipment items, then populate our self.heater_equipment with parsed versions of those items.
         heater_equip_data = [op for op in data.get("Operation", {}) if OmniType.HEATER_EQUIP in op][0]
         self.heater_equipment = [MSPHeaterEquip.parse_obj(equip) for equip in heater_equip_data[OmniType.HEATER_EQUIP]]
 
 
+class MSPChlorinatorEquip(OmniBase):
+    omni_type: OmniType = OmniType.CHLORINATOR_EQUIP
+    enabled: Literal["yes", "no"] = Field(alias="Enabled")
+
+
+class MSPChlorinator(OmniBase):
+    _sub_devices = {"chlorinator_equipment"}
+
+    omni_type: OmniType = OmniType.CHLORINATOR
+    enabled: Literal["yes", "no"] = Field(alias="Enabled")
+    timed_percent: int = Field(alias="Timed-Percent")
+    superchlor_timeout: int = Field(alias="SuperChlor-Timeout")
+    dispenser_type: ChlorinatorDispenserType | str = Field(alias="Dispenser-Type")
+    chlorinator_equipment: list[MSPChlorinatorEquip] | None
+
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+        # The heater equipment are nested down inside a list of "Operations", which also includes non Heater-Equipment items.  We need to
+        # first filter down to just the heater equipment items, then populate our self.heater_equipment with parsed versions of those items.
+        chlorinator_equip_data = [op for op in data.get("Operation", {}) if OmniType.CHLORINATOR_EQUIP in op][0]
+        self.chlorinator_equipment = [MSPChlorinatorEquip.parse_obj(equip) for equip in chlorinator_equip_data[OmniType.CHLORINATOR_EQUIP]]
+
+
 class MSPColorLogicLight(OmniBase):
     omni_type: OmniType = OmniType.CL_LIGHT
     type: ColorLogicLightType | str = Field(alias="Type")
     v2_active: Literal["yes", "no"] | None = Field(alias="V2-Active")
     effects: list[ColorLogicShow] | None
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self.effects = list(ColorLogicShow) if self.v2_active == "yes" else [show for show in ColorLogicShow if show.value <= 16]
 
 
 class MSPBoW(OmniBase):
-    _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light", "pump"}
+    _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light", "pump", "chlorinator"}
 
     omni_type: OmniType = OmniType.BOW
     type: BodyOfWaterType | str = Field(alias="Type")
     filter: list[MSPFilter] | None = Field(alias="Filter")
     relay: list[MSPRelay] | None = Field(alias="Relay")
     heater: MSPVirtualHeater | None = Field(alias="Heater")
     sensor: list[MSPSensor] | None = Field(alias="Sensor")
     colorlogic_light: list[MSPColorLogicLight] | None = Field(alias="ColorLogic-Light")
     pump: list[MSPPump] | None = Field(alias="Pump")
+    chlorinator: MSPChlorinator | None = Field(alias="Chlorinator")
 
     # We override the __init__ here so that we can trigger the propagation of the bow_id down to all of it's sub devices after the bow
     # itself is initialized
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self.propagate_bow_id(self.system_id)
 
@@ -200,15 +226,15 @@
     def load_xml(xml: str) -> MSPConfig:
         data = xml_parse(
             xml,
             # Some things will be lists or not depending on if a pool has more than one of that piece of equipment.  Here we are coercing
             # everything that *could* be a list into a list to make the parsing more consistent.
             force_list=(
                 OmniType.BOW_MSP,
-                OmniType.CHLORINATOR,
+                OmniType.CHLORINATOR_EQUIP,
                 OmniType.CL_LIGHT,
                 OmniType.FAVORITES,
                 OmniType.FILTER,
                 OmniType.GROUPS,
                 OmniType.HEATER_EQUIP,
                 OmniType.PUMP,
                 OmniType.RELAY,
```

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.1/pyomnilogic_local/types.py` & `python_omnilogic_local-0.9.0/pyomnilogic_local/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 
 # OmniAPI Enums
 class MessageType(Enum):
     XML_ACK = 0000
     REQUEST_CONFIGURATION = 1
     SET_FILTER_SPEED = 9
     SET_HEATER_COMMAND = 11
+    SET_SUPERCHLORINATE = 15
     REQUEST_LOG_CONFIG = 31
     SET_SOLAR_SET_POINT_COMMAND = 40
     SET_HEATER_MODE_COMMAND = 42
+    SET_CHLOR_ENABLED = 121
     SET_HEATER_ENABLED = 147
+    SET_CHLOR_PARAMS = 155
     SET_EQUIPMENT = 164
     CREATE_SCHEDULE = 230
     DELETE_SCHEDULE = 231
     GET_TELEMETRY = 300
     GET_ALARM_LIST = 304
     SET_STANDALONE_LIGHT_SHOW = 308
     GET_FILTER_DIAGNOSTIC_INFO = 386
@@ -80,14 +83,18 @@
 # class ChlorinatorStatus(str,Enum):
 #     pass
 class ChlorinatorOperatingMode(PrettyEnum):
     TIMED = 1
     ORP = 2
 
 
+class ChlorinatorDispenserType(str, PrettyEnum):
+    SALT = "SALT_DISPENSING"
+
+
 class ColorLogicSpeed(PrettyEnum):
     ONE_SIXTEENTH = 0
     ONE_EIGHTH = 1
     ONE_QUARTER = 2
     ONE_HALF = 3
     ONE_TIMES = 4
     TWO_TIMES = 5
```

### Comparing `python_omnilogic_local-0.8.1/pyproject.toml` & `python_omnilogic_local-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.8.1"
+version = "0.9.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.8.1/PKG-INFO` & `python_omnilogic_local-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.8.1 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.9.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

