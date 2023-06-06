# Comparing `tmp/opensourceleg-1.2.5.tar.gz` & `tmp/opensourceleg-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.5.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.6.tar", max compression
```

## Comparing `opensourceleg-1.2.5.tar` & `opensourceleg-1.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.5/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.5/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.5/opensourceleg/__init__.py
--rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.5/opensourceleg/actuators.py
--rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.5/opensourceleg/ankle_encoder_map.npy
--rw-r--r--   0        0        0     1156 2023-06-06 03:10:57.959424 opensourceleg-1.2.5/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-06-06 02:24:40.041165 opensourceleg-1.2.5/opensourceleg/control.py
--rw-r--r--   0        0        0     6980 2023-06-06 02:08:02.414266 opensourceleg-1.2.5/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.5/opensourceleg/example.py
--rw-r--r--   0        0        0    10678 2023-06-06 03:09:58.085513 opensourceleg-1.2.5/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.5/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.5/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.5/opensourceleg/logger.py
--rw-r--r--   0        0        0    16449 2023-06-06 03:09:38.127246 opensourceleg-1.2.5/opensourceleg/osl.py
--rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.5/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.5/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.5/opensourceleg/tui.py
--rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.5/opensourceleg/units.py
--rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.5/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-06 03:12:38.602409 opensourceleg-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.6/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.6/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.6/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.6/opensourceleg/actuators.py
+-rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.6/opensourceleg/ankle_encoder_map.npy
+-rw-r--r--   0        0        0     1156 2023-06-06 13:48:00.772459 opensourceleg-1.2.6/opensourceleg/constants.py
+-rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.6/opensourceleg/control.py
+-rw-r--r--   0        0        0     6550 2023-06-06 14:57:46.304774 opensourceleg-1.2.6/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.6/opensourceleg/example.py
+-rw-r--r--   0        0        0    10820 2023-06-06 14:59:16.262812 opensourceleg-1.2.6/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.6/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.6/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.6/opensourceleg/logger.py
+-rw-r--r--   0        0        0    17217 2023-06-06 15:00:18.710389 opensourceleg-1.2.6/opensourceleg/osl.py
+-rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.6/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.6/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21242 2023-06-06 15:01:15.079436 opensourceleg-1.2.6/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.6/opensourceleg/units.py
+-rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.6/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-06 15:01:21.796614 opensourceleg-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.6/PKG-INFO
```

### Comparing `opensourceleg-1.2.5/LICENSE` & `opensourceleg-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/README.md` & `opensourceleg-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/actuators.py` & `opensourceleg-1.2.6/opensourceleg/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/constants.py` & `opensourceleg-1.2.6/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/control.py` & `opensourceleg-1.2.6/opensourceleg/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 @dataclass
 class Gains:
     """
     Dataclass for controller gains
 
-    Attributes:
+    Args:
         kp (int): Proportional gain
         ki (int): Integral gain
         kd (int): Derivative gain
         K (int): Stiffness of the impedance controller
         B (int): Damping of the impedance controller
         ff (int): Feedforward gain
     """
```

### Comparing `opensourceleg-1.2.5/opensourceleg/demo.py` & `opensourceleg-1.2.6/opensourceleg/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,56 +13,56 @@
 KNEE_B_ESTANCE = 0
 KNEE_THETA_ESTANCE = 5
 
 LOAD_LSTANCE: float = -1.0 * BODY_WEIGHT * 0.3 * 4.4
 
 ANKLE_K_ESTANCE = 50
 ANKLE_B_ESTANCE = 0
-ANKLE_THETA_ESTANCE = 20
+ANKLE_THETA_ESTANCE = 0
 
 # --------------------------------------------- #
 # STATE 2: LATE STANCE
 
 KNEE_K_LSTANCE = 150
 KNEE_B_LSTANCE = 0
 KNEE_THETA_LSTANCE = 5
 
 LOAD_ESWING: float = -1.0 * BODY_WEIGHT * 0.2 * 4.4
 
 ANKLE_K_LSTANCE = 90
 ANKLE_B_LSTANCE = 0
-ANKLE_THETA_LSTANCE = 0
+ANKLE_THETA_LSTANCE = 15
 
 # --------------------------------------------- #
 # STATE 3: EARLY SWING
 
 KNEE_K_ESWING = 30
 KNEE_B_ESWING = 40
 KNEE_THETA_ESWING = 85
 
 KNEE_THETA_ESWING_TO_LSWING = 60
 KNEE_DTHETA_ESWING_TO_LSWING = 3
 
 ANKLE_K_ESWING = 20
 ANKLE_B_ESWING = 0
-ANKLE_THETA_ESWING = 30
+ANKLE_THETA_ESWING = -25
 
 # --------------------------------------------- #
 # STATE 4: LATE SWING
 
 KNEE_K_LSWING = 20
 KNEE_B_LSWING = 60
 KNEE_THETA_LSWING = 5
 
 LOAD_ESTANCE: float = -1.0 * BODY_WEIGHT * 0.3 * 4.4
 KNEE_THETA_LSWING_TO_ESTANCE = 20
 
 ANKLE_K_LSWING = 20
 ANKLE_B_LSWING = 0
-ANKLE_THETA_LSWING = 30
+ANKLE_THETA_LSWING = -25
 
 # ------------- FSM TRANSITIONS --------------- #
 
 
 def estance_to_lstance(osl: OpenSourceLeg) -> bool:
     """
     Transition from early stance to late stance when the loadcell
@@ -127,20 +127,25 @@
         or osl.knee.output_position > KNEE_THETA_LSWING_TO_ESTANCE
     ):
         return True
     else:
         return False
 
 
-def main():
+def state_machine_controller():
     osl = OpenSourceLeg(frequency=200)
     osl.units["position"] = "deg"  # type: ignore
     osl.units["velocity"] = "deg/s"  # type: ignore
 
     osl.add_joint(
+        name="knee",
+        gear_ratio=41.4999,
+    )
+
+    osl.add_joint(
         name="ankle",
         gear_ratio=41.4999,
     )
 
     osl.add_loadcell(
         dephy_mode=False,
     )
@@ -235,35 +240,16 @@
     osl.state_machine.add_transition(
         source=late_swing,
         destination=early_stance,
         event=heel_strike,
         callback=lswing_to_estance,
     )
 
-    # osl.add_tui()
+    osl.add_tui()
 
     with osl:
-        # osl.home()
-        osl.log.info(osl.ankle.motor_position)
-        osl.log.info(osl.ankle.output_position)
-        time.sleep(1)
         osl.home()
-        osl.log.info(osl.ankle.motor_position)
-        osl.log.info(osl.ankle.output_position)
-        time.sleep(1)
-
-        # osl.knee.set_mode(mode="impedance")
-        # osl.knee.set_impedance_gains()
-        # osl.knee.set_output_position(position=10)
-
-        # time.sleep(2)
-
-        # osl.update()
-
-        # osl.log.info(osl.knee.motor_position)
-        # osl.log.info(osl.knee.output_position)
-
-        # osl.run(set_state_machine_parameters=True)
+        osl.run(set_state_machine_parameters=True)
 
 
 if __name__ == "__main__":
-    main()
+    state_machine_controller()
```

### Comparing `opensourceleg-1.2.5/opensourceleg/joints.py` & `opensourceleg-1.2.6/opensourceleg/joints.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Joint(DephyActpack):
     def __init__(
         self,
         name: str = "knee",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
-        gear_ratio: float = 1.0,
+        gear_ratio: float = 41.4999,
         has_loadcell: bool = False,
         logger: Logger = Logger(),
         units: UnitsDefinition = DEFAULT_UNITS,
         debug_level: int = 0,
         dephy_log: bool = False,
     ) -> None:
 
@@ -76,19 +76,15 @@
 
         is_homing = True
 
         CURRENT_THRESHOLD = 5000
         VELOCITY_THRESHOLD = 0.001
 
         self.set_mode(mode="voltage")
-
-        if "ankle" in self._name.lower():
-            homing_direction = 1.0
-        else:
-            homing_direction = -1.0
+        homing_direction = -1.0
 
         self.set_voltage(
             value=homing_direction * homing_voltage
         )  # mV, negative for counterclockwise
 
         _motor_encoder_array = []
         _joint_encoder_array = []
@@ -117,30 +113,36 @@
 
         _motor_zero_pos = self.motor_encoder_counts
         _joint_zero_pos = self.joint_encoder_counts
 
         time.sleep(0.1)
 
         if "ankle" in self._name.lower():
-            _zero_pos: int = int(np.deg2rad(30) / constants.RAD_PER_COUNT)
+            _zero_pos: int = int(
+                (np.deg2rad(30) * self.gear_ratio) / constants.RAD_PER_COUNT
+            )
+            _zero_pos_joint: int = int(np.deg2rad(30) / constants.RAD_PER_COUNT)
         else:
             _zero_pos: int = 0
+            _zero_pos_joint: int = 0
 
         self.set_motor_zero_position(position=(_motor_zero_pos + _zero_pos))
-        self.set_joint_zero_position(position=(_joint_zero_pos + _zero_pos))
+        self.set_joint_zero_position(position=(_joint_zero_pos + _zero_pos_joint))
 
         self._is_homed = True
 
         if self.encoder_map is None:
             if (
                 input(f"[{self._name}] Would you like to make an encoder map? (y/n): ")
                 == "y"
             ):
                 self.make_encoder_map()
 
+        self._log.info(f"[{self._name}] Homing complete.")
+
     def make_encoder_map(self) -> None:
         """
         This method makes a lookup table to calculate the position measured by the joint encoder.
         This is necessary because the magnetic output encoders are nonlinear.
         By making the map while the joint is unloaded, joint position calculated by motor position * gear ratio
         should be the same as the true joint position.
```

### Comparing `opensourceleg-1.2.5/opensourceleg/loadcell.py` & `opensourceleg-1.2.6/opensourceleg/loadcell.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/logger.py` & `opensourceleg-1.2.6/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/osl.py` & `opensourceleg-1.2.6/opensourceleg/osl.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 
         self._has_knee: bool = False
         self._has_ankle: bool = False
         self._has_loadcell: bool = False
         self._has_tui: bool = False
         self._has_sm: bool = False
 
-        self._set_state_machine_parameters: bool = False
+        self._is_sm_running: bool = False
+        self._is_homed: bool = False
 
         self._knee: Joint = None  # type: ignore
         self._ankle: Joint = None  # type: ignore
         self._loadcell: Loadcell = None  # type: ignore
 
         self.log = Logger(
             file_path=file_name, log_format="[%(asctime)s] %(levelname)s: %(message)s"
@@ -81,19 +82,16 @@
 
         if self.has_ankle:
             self._ankle.start()
 
         if self.has_loadcell:
             self._loadcell.initialize()
 
-        if self.has_state_machine:
-            self.state_machine.start()  # type: ignore
-
     def __exit__(self, type, value, tb) -> None:
-        if self.has_state_machine:
+        if self.has_state_machine and self.is_sm_running:
             self.state_machine.stop()  # type: ignore
 
         if self.has_knee:
             self._knee.stop()
 
         if self.has_ankle:
             self._ankle.stop()
@@ -181,19 +179,19 @@
                 self.log.warn(
                     msg="No active ports found, please ensure that the joint is connected and powered on."
                 )
 
                 exit()
 
             elif len(ports) == 1:
-                port = ports[0]
+                port = ports[-1]
 
             else:
-                port = ports[0]
-                port_a = ports[1]
+                port = ports[-1]
+                port_a = ports[-2]
 
         if "knee" in name.lower():
             self._has_knee = True
 
             self._knee = Joint(
                 name=name,
                 port=port,
@@ -278,14 +276,15 @@
             Defaults to False.
         """
         self.state_machine = StateMachine(osl=self, spoof=spoof)
         self._has_sm = True
 
     def update(
         self,
+        set_state_machine_parameters: bool = False,
     ) -> None:
         if self.has_knee:
             self._knee.update()
 
             if self.knee.case_temperature > self.knee.max_temperature:  # type: ignore
                 self.log.warn(
                     msg="[KNEE] Thermal limit {self.knee.max_temperature} reached. Stopping motor."
@@ -303,17 +302,22 @@
                 self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_loadcell:
             self._loadcell.update()
 
         if self.has_state_machine:
+
+            if self.is_homed and not self.is_sm_running:
+                self.state_machine.start()
+                self._is_sm_running = True
+
             self.state_machine.update()  # type: ignore
 
-            if self._set_state_machine_parameters:
+            if set_state_machine_parameters:
                 if self.has_knee and self.state_machine.current_state.is_knee_active:  # type: ignore
 
                     if self.knee.mode != self.knee.modes["impedance"]:  # type: ignore
                         self.knee.set_mode(mode="impedance")  # type: ignore
                         self.knee.set_impedance_gains()  # type: ignore
 
                     self.knee.set_impedance_gains(  # type: ignore
@@ -321,15 +325,15 @@
                         B=self.state_machine.current_state.knee_damping,  # type: ignore
                     )
 
                     self.knee.set_output_position(  # type: ignore
                         position=self.state_machine.current_state.knee_theta  # type: ignore
                     )
 
-                elif self.has_ankle and self.state_machine.current_state.is_ankle_active:  # type: ignore
+                if self.has_ankle and self.state_machine.current_state.is_ankle_active:  # type: ignore
 
                     if self.ankle.mode != self.ankle.modes["impedance"]:  # type: ignore
                         self.ankle.set_mode(mode="impedance")  # type: ignore
                         self.ankle.set_impedance_gains()  # type: ignore
 
                     self.ankle.set_impedance_gains(  # type: ignore
                         K=self.state_machine.current_state.ankle_stiffness,  # type: ignore
@@ -349,24 +353,32 @@
 
         Parameters
         ----------
         set_state_machine_parameters : bool, optional
             Whether to set the joint impedance gains and equilibrium angles to the current state's values, by default False
         """
 
-        self._set_state_machine_parameters = set_state_machine_parameters
-        self.update()
+        if self.is_homed:
+            if not self.is_sm_running:
+                self.state_machine.start()
+                self._is_sm_running = True
+        else:
+            osl.log.warn(
+                f"[OSL] Please run the homing routine by calling `osl.home()` before starting the state-machine."
+            )
+            exit()
 
-        time.sleep(0.1)
+        self.update(set_state_machine_parameters=set_state_machine_parameters)
 
         if not self.has_tui:
-            self.update()
+            self.update(set_state_machine_parameters=set_state_machine_parameters)
 
         else:
-            self.tui.add_update_callback(callback=self.update)  # type: ignore
+            time.sleep(0.1)
+            self.tui.add_update_callback(callback=self.update, args=set_state_machine_parameters)  # type: ignore
             self.tui.run()  # type: ignore
 
     def initialize_sm_tui(self) -> None:
 
         from opensourceleg.tui import COLORS
 
         assert self.tui is not None
@@ -385,30 +397,30 @@
         self.tui.add_panel(
             name="fz",
             parent="top",
             show_title=True,
         )
 
         self.tui.add_panel(
-            name="joint_position",
+            name="knee_joint_position",
             parent="top",
             show_title=True,
         )
 
         self.tui.add_plot(
             name="fz_plot",
             parent="fz",
             object=self.loadcell,
             attribute="fz",
             color=COLORS.cyan,
         )
 
         self.tui.add_plot(
             name="joint_position_plot",
-            parent="joint_position",
+            parent="knee_joint_position",
             object=self.knee,
             attribute="output_position",
             color=COLORS.yellow,
         )
 
         self.tui.add_state_visualizer(
             name="state_machine",
@@ -438,14 +450,16 @@
             self.log.debug(msg="[OSL] Homing knee joint.")
             self.knee.home()  # type: ignore
 
         if self.has_ankle:
             self.log.debug(msg="[OSL] Homing ankle joint.")
             self.ankle.home()  # type: ignore
 
+        self._is_homed = True
+
     def calibrate_loadcell(self) -> None:
         self.log.debug(msg="[OSL] Calibrating loadcell.")
         if self.has_loadcell:
             self.loadcell.reset()  # type: ignore
 
     def calibrate_encoders(self) -> None:
         self.log.debug(msg="[OSL] Calibrating encoders.")
@@ -512,14 +526,22 @@
     def has_state_machine(self) -> bool:
         return self._has_sm
 
     @property
     def has_tui(self) -> bool:
         return self._has_tui
 
+    @property
+    def is_homed(self) -> bool:
+        return self._is_homed
+
+    @property
+    def is_sm_running(self) -> bool:
+        return self._is_sm_running
+
 
 if __name__ == "__main__":
     osl = OpenSourceLeg(frequency=200)
 
     osl.units["position"] = "deg"  # type: ignore
 
     osl.add_joint(
```

### Comparing `opensourceleg-1.2.5/opensourceleg/state_machine.py` & `opensourceleg-1.2.6/opensourceleg/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/thermal.py` & `opensourceleg-1.2.6/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/tui.py` & `opensourceleg-1.2.6/opensourceleg/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             titleColor=ttk.TTkColor.BOLD + ttk.TTkColor.fg(COLORS.cyan),
         )
 
         self.frame.setLayout(self._layouts[layout]())
         self._panels["root"] = self.frame
 
         self._update_callbacks: list[Callable] = []  # type: ignore
+        self._update_args: list = []  # type: ignore
 
         self.timer.timeout.connect(self.update)
         self.timer.start(1)
 
     @ttk.pyTTkSlot()
     def update(self):
         if self._plots:
@@ -133,21 +134,23 @@
                     ):
                         self._state_vizualisers[_sv].states[
                             self._state_vizualisers[_sv].previous_state
                         ].setDisabled(True)
 
                     self._state_vizualisers[_sv].previous_state = _current_state
 
-        for callback in self._update_callbacks:
-            callback()
+        for i, callback in enumerate(self._update_callbacks):
+            if self._update_args[i]:
+                callback(self._update_args[i])
 
         self.timer.start(self.dt)
 
-    def add_update_callback(self, callback: Callable = lambda: None):  # type: ignore
+    def add_update_callback(self, callback: Callable = lambda: None, args: Any = None):  # type: ignore
         self._update_callbacks.append(callback)
+        self._update_args.append(args)
 
     def set_active_attribute(self, attribute: str):
         self._attribute = attribute
 
     def set_plot_value(self, value: float):
         self._pvalue = [value]
```

### Comparing `opensourceleg-1.2.5/opensourceleg/units.py` & `opensourceleg-1.2.6/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/opensourceleg/utilities.py` & `opensourceleg-1.2.6/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.5/pyproject.toml` & `opensourceleg-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.5"
+version = "1.2.6"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.5/PKG-INFO` & `opensourceleg-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.5
+Version: 1.2.6
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

