# Comparing `tmp/opensourceleg-1.2.4.tar.gz` & `tmp/opensourceleg-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.4.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.5.tar", max compression
```

## Comparing `opensourceleg-1.2.4.tar` & `opensourceleg-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.4/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.4/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.4/opensourceleg/__init__.py
--rw-r--r--   0        0        0    22445 2023-06-02 20:45:59.012884 opensourceleg-1.2.4/opensourceleg/actuators.py
--rw-r--r--   0        0        0     2283 2023-06-02 18:09:03.466245 opensourceleg-1.2.4/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.4/opensourceleg/control.py
--rw-r--r--   0        0        0     4259 2023-06-02 20:50:04.529275 opensourceleg-1.2.4/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.4/opensourceleg/example.py
--rw-r--r--   0        0        0    11210 2023-06-02 20:45:59.013945 opensourceleg-1.2.4/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.4/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8515 2023-06-02 20:45:59.014215 opensourceleg-1.2.4/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.4/opensourceleg/logger.py
--rw-r--r--   0        0        0    15026 2023-06-02 20:53:49.594477 opensourceleg-1.2.4/opensourceleg/osl.py
--rw-r--r--   0        0        0    10776 2023-06-02 20:50:04.631436 opensourceleg-1.2.4/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.4/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.4/opensourceleg/tui.py
--rw-r--r--   0        0        0     4331 2023-06-02 18:32:11.184018 opensourceleg-1.2.4/opensourceleg/units.py
--rw-r--r--   0        0        0    11590 2023-06-02 04:54:05.760995 opensourceleg-1.2.4/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-02 20:56:08.479891 opensourceleg-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.5/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.5/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.5/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.5/opensourceleg/actuators.py
+-rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.5/opensourceleg/ankle_encoder_map.npy
+-rw-r--r--   0        0        0     1156 2023-06-06 03:10:57.959424 opensourceleg-1.2.5/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-06-06 02:24:40.041165 opensourceleg-1.2.5/opensourceleg/control.py
+-rw-r--r--   0        0        0     6980 2023-06-06 02:08:02.414266 opensourceleg-1.2.5/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.5/opensourceleg/example.py
+-rw-r--r--   0        0        0    10678 2023-06-06 03:09:58.085513 opensourceleg-1.2.5/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.5/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.5/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.5/opensourceleg/logger.py
+-rw-r--r--   0        0        0    16449 2023-06-06 03:09:38.127246 opensourceleg-1.2.5/opensourceleg/osl.py
+-rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.5/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.5/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.5/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.5/opensourceleg/units.py
+-rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.5/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-06 03:12:38.602409 opensourceleg-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.5/PKG-INFO
```

### Comparing `opensourceleg-1.2.4/LICENSE` & `opensourceleg-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/README.md` & `opensourceleg-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/actuators.py` & `opensourceleg-1.2.5/opensourceleg/actuators.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 from ctypes import c_int
 from dataclasses import dataclass
 
 import flexsea.fx_enums as fxe
 import numpy as np
 from flexsea.device import Device
 
-from opensourceleg.constants import Constants
+import opensourceleg.constants as constants
 from opensourceleg.control import (
     DEFAULT_CURRENT_GAINS,
     DEFAULT_IMPEDANCE_GAINS,
     DEFAULT_POSITION_GAINS,
 )
 from opensourceleg.logger import Logger
 from opensourceleg.thermal import ThermalModel
 from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 
 
 @dataclass
 class ControlModes:
     """
-    Control modes for the Dephy Actpack
+    Control modes for the Dephy Actpack.
+
+    Available modes are Voltage, Current, Position, Impedance.
     """
 
     voltage: c_int = fxe.FX_VOLTAGE
     current: c_int = fxe.FX_CURRENT
     position: c_int = fxe.FX_POSITION
     impedance: c_int = fxe.FX_IMPEDANCE
 
@@ -186,15 +188,15 @@
             self._set_gains()
 
         self._set_motor_position(
             counts=int(
                 self._device._units.convert_to_default_units(
                     value=self._device.motor_position, attribute="position"
                 )
-                / Constants.RAD_PER_COUNT
+                / constants.RAD_PER_COUNT
             )
         )
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Position mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
         time.sleep(0.1)
@@ -239,15 +241,15 @@
             self._set_gains()
 
         self._set_motor_position(
             counts=int(
                 self._device._units.convert_to_default_units(
                     value=self._device.motor_position, attribute="position"
                 )
-                / Constants.RAD_PER_COUNT
+                / constants.RAD_PER_COUNT
             )
         )
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Impedance mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
         time.sleep(1 / self._device.frequency)
@@ -512,15 +514,15 @@
         if self._mode != self._modes["current"]:
             self._log.warning(msg=f"Cannot set motor_torque in mode {self._mode}")
             return
 
         self._mode._set_current(  # type: ignore
             int(
                 self._units.convert_to_default_units(value=torque, attribute="torque")
-                / Constants.NM_PER_MILLIAMP
+                / constants.NM_PER_MILLIAMP
             ),
         )
 
     def set_motor_position(self, position: float) -> None:
         """
         Sets the motor position
 
@@ -529,18 +531,21 @@
         """
         if self._mode not in [self._modes["position"], self._modes["impedance"]]:
             self._log.warning(msg=f"Cannot set motor position in mode {self._mode}")
             return
 
         self._mode._set_motor_position(  # type: ignore
             int(
-                self._units.convert_to_default_units(
-                    value=position, attribute="position"
+                (
+                    self._units.convert_to_default_units(
+                        value=position, attribute="position"
+                    )
+                    / constants.RAD_PER_COUNT
                 )
-                / Constants.RAD_PER_COUNT
+                + self.motor_zero_position
             ),
         )
 
     # Read only properties from the actpack
 
     @property
     def units(self) -> UnitsDefinition:
@@ -551,14 +556,18 @@
         return self._frequency
 
     @property
     def mode(self) -> ActpackMode:
         return self._mode
 
     @property
+    def modes(self) -> dict[str, ActpackMode]:
+        return self._modes
+
+    @property
     def motor_zero_position(self) -> float:
         return self._motor_zero_position
 
     @property
     def joint_zero_position(self) -> float:
         return self._joint_zero_position
 
@@ -602,35 +611,44 @@
         else:
             return 0.0
 
     @property
     def motor_torque(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.mot_cur * Constants.NM_PER_MILLIAMP,
+                value=self._data.mot_cur * constants.NM_PER_MILLIAMP,
                 attribute="torque",
             )
         else:
             return 0.0
 
     @property
     def motor_position(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
+                value=int(self._data.mot_ang - self.motor_zero_position)
+                * constants.RAD_PER_COUNT,
                 attribute="position",
             )
         else:
             return 0.0
 
     @property
+    def motor_encoder_counts(self):
+        return self._data.mot_ang
+
+    @property
+    def joint_encoder_counts(self):
+        return self._data.ank_ang
+
+    @property
     def motor_velocity(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=int(self._data.mot_vel) * Constants.RAD_PER_COUNT,
+                value=int(self._data.mot_vel) * constants.RAD_PER_COUNT,
                 attribute="velocity",
             )
         else:
             return 0.0
 
     @property
     def motor_acceleration(self) -> float:
@@ -642,25 +660,26 @@
         else:
             return 0.0
 
     @property
     def joint_position(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.ank_ang * Constants.RAD_PER_COUNT,
+                value=int(self._data.ank_ang - self._joint_zero_position)
+                * constants.RAD_PER_COUNT,
                 attribute="position",
             )
         else:
             return 0.0
 
     @property
     def joint_velocity(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.ank_vel * Constants.RAD_PER_COUNT,
+                value=self._data.ank_vel * constants.RAD_PER_COUNT,
                 attribute="velocity",
             )
         else:
             return 0.0
 
     @property
     def case_temperature(self) -> float:
@@ -698,62 +717,62 @@
         else:
             return np.zeros(shape=6)
 
     @property
     def accelx(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.accelx * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accelx * constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
             return 0.0
 
     @property
     def accely(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.accely * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accely * constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
             return 0.0
 
     @property
     def accelz(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.accelz * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accelz * constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
             return 0.0
 
     @property
     def gyrox(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyrox * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyrox * constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
             return 0.0
 
     @property
     def gyroy(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyroy * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyroy * constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
             return 0.0
 
     @property
     def gyroz(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyroz * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyroz * constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
             return 0.0
```

### Comparing `opensourceleg-1.2.4/opensourceleg/control.py` & `opensourceleg-1.2.5/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/joints.py` & `opensourceleg-1.2.5/opensourceleg/joints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 
 import numpy as np
 
+import opensourceleg.constants as constants
 from opensourceleg.actuators import DephyActpack
-from opensourceleg.constants import Constants
 from opensourceleg.logger import Logger
 from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 
 
 class Joint(DephyActpack):
     def __init__(
         self,
@@ -34,28 +34,27 @@
             dephy_log=dephy_log,
         )
 
         self._gear_ratio: float = gear_ratio
         self._is_homed: bool = False
         self._has_loadcell: bool = has_loadcell
         self._encoder_map = None
-        self._zero_pos = 0.0
 
         self._motor_zero_pos = 0.0
         self._joint_zero_pos = 0.0
 
         self._motor_voltage_sp = 0.0
         self._motor_current_sp = 0.0
         self._motor_position_sp = 0.0
 
         self._stiffness_sp: int = 200
         self._damping_sp: int = 400
         self._equilibrium_position_sp = 0.0
 
-        self._max_temperature: float = Constants.MAX_CASE_TEMPERATURE
+        self._max_temperature: float = constants.MAX_CASE_TEMPERATURE
 
         self._control_mode_sp: str = "voltage"
 
         if "knee" in name.lower() or "ankle" in name.lower():
             self._name: str = name
         else:
             self._log.warning(msg=f"Invalid joint name: {name}")
@@ -73,19 +72,27 @@
         self,
         homing_voltage: int = 2000,
         homing_frequency: int = 100,
     ) -> None:
 
         is_homing = True
 
-        CURRENT_THRESHOLD = 6000
+        CURRENT_THRESHOLD = 5000
         VELOCITY_THRESHOLD = 0.001
 
         self.set_mode(mode="voltage")
-        self.set_voltage(value=-1 * homing_voltage)  # mV, negative for counterclockwise
+
+        if "ankle" in self._name.lower():
+            homing_direction = 1.0
+        else:
+            homing_direction = -1.0
+
+        self.set_voltage(
+            value=homing_direction * homing_voltage
+        )  # mV, negative for counterclockwise
 
         _motor_encoder_array = []
         _joint_encoder_array = []
 
         time.sleep(0.1)
 
         try:
@@ -104,40 +111,26 @@
                     is_homing = False
 
         except KeyboardInterrupt:
             self.set_voltage(value=0)
             self._log.warning(msg="Homing interrupted.")
             return
 
-        _motor_zero_pos = self.motor_position
-        _joint_zero_pos = self.joint_position
+        _motor_zero_pos = self.motor_encoder_counts
+        _joint_zero_pos = self.joint_encoder_counts
 
         time.sleep(0.1)
 
-        if np.std(_motor_encoder_array) < 1e-6:
-            self._log.warning(
-                msg=f"[{self._name}] Motor encoder not working. Please check the wiring."
-            )
-            return
-
-        elif np.std(_joint_encoder_array) < 1e-6:
-            self._log.warning(
-                msg=f"[{self._name}] Joint encoder not working. Please check the wiring."
-            )
-            return
-
         if "ankle" in self._name.lower():
-            self._zero_pos = np.deg2rad(30)
-            self.set_motor_zero_position(position=_motor_zero_pos)
-            self.set_joint_zero_position(position=_joint_zero_pos)
-
+            _zero_pos: int = int(np.deg2rad(30) / constants.RAD_PER_COUNT)
         else:
-            self._zero_pos = 0.0
-            self.set_motor_zero_position(position=_motor_zero_pos)
-            self.set_joint_zero_position(position=_joint_zero_pos)
+            _zero_pos: int = 0
+
+        self.set_motor_zero_position(position=(_motor_zero_pos + _zero_pos))
+        self.set_joint_zero_position(position=(_joint_zero_pos + _zero_pos))
 
         self._is_homed = True
 
         if self.encoder_map is None:
             if (
                 input(f"[{self._name}] Would you like to make an encoder map? (y/n): ")
                 == "y"
@@ -158,15 +151,15 @@
         Author: Kevin Best, PhD
                 U-M Neurobionics Lab
                 Gitub: tkevinbest, https://github.com/tkevinbest
         """
 
         if not self.is_homed:
             self._log.warning(
-                msg=f"[{self._name}] Please home the joint before making the encoder map."
+                msg=f"[{self._name.capitalize}] Please home the joint before making the encoder map."
             )
             return
 
         self.set_mode(mode="current")
         self.set_current_gains()
         time.sleep(0.1)
         self.set_current_gains()
@@ -175,17 +168,15 @@
         time.sleep(0.1)
         self.set_output_torque(torque=0.0)
 
         _joint_position_array = []
         _output_position_array = []
 
         self._log.info(
-            msg=f"[{self._name}] Please manually move the joint numerous times \
-                through its full range of motion for 10 seconds.\
-                   \n Press any key to continue."
+            msg=f"[{self._name.capitalize}] Please manually move the joint numerous times through its full range of motion for 10 seconds. \nPress any key to continue."
         )
 
         _start_time: float = time.time()
 
         try:
             while time.time() - _start_time < 10:
                 self.update()
@@ -258,16 +249,16 @@
             K (float): Spring constant. Defaults to 0.08922 Nm/rad.
             B (float): Damping constant. Defaults to 0.0038070 Nm/rad/s.
             ff (int): Feedforward gain. Defaults to 128.
         """
         self.set_impedance_gains(
             kp=kp,
             ki=ki,
-            K=int(K * Constants.NM_PER_RAD_TO_K),
-            B=int(B * Constants.NM_S_PER_RAD_TO_B),
+            K=int(K * constants.NM_PER_RAD_TO_K),
+            B=int(B * constants.NM_S_PER_RAD_TO_B),
             ff=ff,
         )
 
     def set_joint_impedance(
         self,
         kp: int = 40,
         ki: int = 400,
@@ -297,22 +288,14 @@
             ff=ff,
         )
 
     def update_set_points(self) -> None:
         self.set_mode(mode=self.control_mode_sp)
 
     @property
-    def zero_position(self):
-        return self._zero_pos
-
-    @zero_position.setter
-    def zero_position(self, value):
-        self._zero_pos = value
-
-    @property
     def name(self) -> str:
         return self._name
 
     @property
     def gear_ratio(self) -> float:
         return self._gear_ratio
```

### Comparing `opensourceleg-1.2.4/opensourceleg/loadcell.py` & `opensourceleg-1.2.5/opensourceleg/loadcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 import numpy as np
 from smbus2 import SMBus
 
-from opensourceleg.constants import Constants
+import opensourceleg.constants as constants
 from opensourceleg.joints import Joint
 from opensourceleg.logger import Logger
 
 
 class StrainAmp:
     """
     A class to directly manage the 6ch strain gauge amplifier over I2C.
@@ -125,15 +125,15 @@
 class Loadcell:
     def __init__(
         self,
         dephy_mode: bool = False,
         joint: Joint = None,  # type: ignore
         amp_gain: float = 125.0,
         exc: float = 5.0,
-        loadcell_matrix: np.ndarray = Constants.LOADCELL_MATRIX,
+        loadcell_matrix: np.ndarray = constants.LOADCELL_MATRIX,
         logger: "Logger" = None,  # type: ignore
     ) -> None:
         self._is_dephy: bool = dephy_mode
         self._joint: Joint = joint
         self._amp_gain: float = amp_gain
         self._exc: float = exc
         self._adc_range: int = 2**12 - 1
```

### Comparing `opensourceleg-1.2.4/opensourceleg/logger.py` & `opensourceleg-1.2.5/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/osl.py` & `opensourceleg-1.2.5/opensourceleg/osl.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 import time
 
 import numpy as np
 
 sys.path.append("../")
 
+import opensourceleg.constants as constants
 import opensourceleg.utilities as utilities
-from opensourceleg.constants import Constants
 from opensourceleg.joints import Joint
 from opensourceleg.loadcell import Loadcell
 from opensourceleg.logger import Logger
 from opensourceleg.state_machine import State, StateMachine
 from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 from opensourceleg.utilities import SoftRealtimeLoop
 
@@ -84,22 +84,14 @@
 
         if self.has_loadcell:
             self._loadcell.initialize()
 
         if self.has_state_machine:
             self.state_machine.start()  # type: ignore
 
-            if self.has_knee:
-                self.knee.set_mode(mode="impedance")  # type: ignore
-                self.knee.set_impedance_gains()  # type: ignore
-
-            if self.has_ankle:
-                self.ankle.set_mode(mode="impedance")  # type: ignore
-                self.ankle.set_impedance_gains()  # type: ignore
-
     def __exit__(self, type, value, tb) -> None:
         if self.has_state_machine:
             self.state_machine.stop()  # type: ignore
 
         if self.has_knee:
             self._knee.stop()
 
@@ -114,14 +106,32 @@
         return f"OSL object. Frequency: {self._frequency} Hz"
 
     def add_tui(
         self,
         configuration: str = "state_machine",
         layout: str = "vertical",
     ) -> None:
+        """
+        Add a Terminal User Interface (TUI) to the OSL object. The TUI is used
+        to visualize the data from the OSL and to send commands to the OSL. Additionally,
+        the TUI also has a timer built-in to govern the frequency of the control loop, which is
+        less accurate than the "osl.clock" (SoftRealTimeLoop) object but is more convenient.
+
+        Note
+        ----
+        The timer/interface runs in a separate thread, so it does not affect the control loop.
+        This causes the code to not respond to keyboard interrupts (Ctrl+C) when the TUI is running.
+
+        Parameters
+        ----------
+        configuration : str, optional
+            The configuration of the TUI, by default "state_machine"
+        layout : str, optional
+            The layout of the TUI, by default "vertical"
+        """
         from opensourceleg.tui import TUI
 
         self._has_tui = True
         self.tui = TUI(
             title="www.opensourceleg.com", frequency=self._frequency, layout=layout
         )
 
@@ -160,31 +170,33 @@
         has_loadcell : bool, optional
             Whether the joint has a loadcell, by default False
         debug_level : int, optional
             The debug level of the joint, by default 0
         dephy_log : bool, optional
             Whether to log the joint data to the dephy log, by default False
         """
+        if port is None:
+            ports = utilities.get_active_ports()
 
-        if "knee" in name.lower():
-            self._has_knee = True
+            if len(ports) == 0:
+                self.log.warn(
+                    msg="No active ports found, please ensure that the joint is connected and powered on."
+                )
 
-            if port is None:
-                ports = utilities.get_active_ports()
+                exit()
 
-                if len(ports) == 0:
-                    self.log.warn(
-                        msg="No active ports found, please ensure that the joint is connected and powered on."
-                    )
+            elif len(ports) == 1:
+                port = ports[0]
 
-                else:
-                    if "knee" in name.lower():
-                        port = ports[0]
-                    else:
-                        port = ports[1]
+            else:
+                port = ports[0]
+                port_a = ports[1]
+
+        if "knee" in name.lower():
+            self._has_knee = True
 
             self._knee = Joint(
                 name=name,
                 port=port,
                 baud_rate=baud_rate,
                 frequency=self._frequency,
                 gear_ratio=gear_ratio,
@@ -193,14 +205,18 @@
                 units=self.units,
                 debug_level=debug_level,
                 dephy_log=dephy_log,
             )
 
         elif "ankle" in name.lower():
             self._has_ankle = True
+
+            if self.has_knee:
+                port = port_a
+
             self._ankle = Joint(
                 name=name,
                 port=port,
                 baud_rate=baud_rate,
                 frequency=self._frequency,
                 gear_ratio=gear_ratio,
                 has_loadcell=has_loadcell,
@@ -214,15 +230,15 @@
 
     def add_loadcell(
         self,
         dephy_mode: bool = False,
         joint: Joint = None,  # type: ignore
         amp_gain: float = 125.0,
         exc: float = 5.0,
-        loadcell_matrix=Constants.LOADCELL_MATRIX,
+        loadcell_matrix=constants.LOADCELL_MATRIX,
     ) -> None:
         """
         Add a loadcell to the OSL object.
 
         Parameters
         ----------
         dephy_mode : bool, optional
@@ -244,19 +260,28 @@
             exc=exc,
             loadcell_matrix=loadcell_matrix,  # type: ignore
             logger=self.log,
         )
 
     def add_state_machine(
         self,
+        spoof: bool = False,
     ) -> None:
         """
         Add a state machine to the OSL object.
+
+        Parameters
+        ----------
+        spoof : bool, optional
+            If True, the state machine will spoof the state transitions--ie, it will not
+            check the criteria for transitioning but will instead transition after the
+            minimum time spent in state has elapsed. This is useful for testing.
+            Defaults to False.
         """
-        self.state_machine = StateMachine(osl=self)
+        self.state_machine = StateMachine(osl=self, spoof=spoof)
         self._has_sm = True
 
     def update(
         self,
     ) -> None:
         if self.has_knee:
             self._knee.update()
@@ -282,24 +307,34 @@
             self._loadcell.update()
 
         if self.has_state_machine:
             self.state_machine.update()  # type: ignore
 
             if self._set_state_machine_parameters:
                 if self.has_knee and self.state_machine.current_state.is_knee_active:  # type: ignore
+
+                    if self.knee.mode != self.knee.modes["impedance"]:  # type: ignore
+                        self.knee.set_mode(mode="impedance")  # type: ignore
+                        self.knee.set_impedance_gains()  # type: ignore
+
                     self.knee.set_impedance_gains(  # type: ignore
                         K=self.state_machine.current_state.knee_stiffness,  # type: ignore
                         B=self.state_machine.current_state.knee_damping,  # type: ignore
                     )
 
                     self.knee.set_output_position(  # type: ignore
                         position=self.state_machine.current_state.knee_theta  # type: ignore
                     )
 
                 elif self.has_ankle and self.state_machine.current_state.is_ankle_active:  # type: ignore
+
+                    if self.ankle.mode != self.ankle.modes["impedance"]:  # type: ignore
+                        self.ankle.set_mode(mode="impedance")  # type: ignore
+                        self.ankle.set_impedance_gains()  # type: ignore
+
                     self.ankle.set_impedance_gains(  # type: ignore
                         K=self.state_machine.current_state.ankle_stiffness,  # type: ignore
                         B=self.state_machine.current_state.ankle_damping,  # type: ignore
                     )
 
                     self.ankle.set_output_position(  # type: ignore
                         position=self.state_machine.current_state.ankle_theta  # type: ignore
```

### Comparing `opensourceleg-1.2.4/opensourceleg/thermal.py` & `opensourceleg-1.2.5/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/tui.py` & `opensourceleg-1.2.5/opensourceleg/tui.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/units.py` & `opensourceleg-1.2.5/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.4/opensourceleg/utilities.py` & `opensourceleg-1.2.5/opensourceleg/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,8 +340,8 @@
         except (OSError, serial.SerialException):
             pass
 
     return serial_ports
 
 
 if __name__ == "__main__":
-    print(get_active_ports()[0])
+    print(get_active_ports())
```

### Comparing `opensourceleg-1.2.4/pyproject.toml` & `opensourceleg-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.4"
+version = "1.2.5"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.4/PKG-INFO` & `opensourceleg-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.4
+Version: 1.2.5
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

