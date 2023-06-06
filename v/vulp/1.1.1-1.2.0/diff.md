# Comparing `tmp/vulp-1.1.1.tar.gz` & `tmp/vulp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulp-1.1.1.tar", last modified: Mon Mar 13 11:06:13 2023, max compression
+gzip compressed data, was "vulp-1.2.0.tar", last modified: Tue Jun  6 14:06:26 2023, max compression
```

## Comparing `vulp-1.1.1.tar` & `vulp-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,43 @@
--rw-r--r--   0        0        0    10644 2023-03-13 11:06:13.787030 vulp-1.1.1/README.md
--rw-r--r--   0        0        0     1406 2023-03-13 11:06:13.779030 vulp-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      685 2023-03-13 11:06:13.783030 vulp-1.1.1/vulp/__init__.py
--rw-r--r--   0        0        0     3274 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/AgentInterface.cpp
--rw-r--r--   0        0        0     2957 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/AgentInterface.h
--rw-r--r--   0        0        0     2440 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/BUILD
--rw-r--r--   0        0        0      862 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/Request.h
--rw-r--r--   0        0        0     9081 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/Spine.cpp
--rw-r--r--   0        0        0     6184 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/Spine.h
--rw-r--r--   0        0        0     5110 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/StateMachine.cpp
--rw-r--r--   0        0        0     3944 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/StateMachine.h
--rw-r--r--   0        0        0      872 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/__init__.py
--rw-r--r--   0        0        0     4354 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/position_commands.h
--rw-r--r--   0        0        0     1011 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/request.py
--rw-r--r--   0        0        0      783 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/spine_error.py
--rw-r--r--   0        0        0     6305 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/spine_interface.py
--rw-r--r--   0        0        0     1200 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/stop_commands.h
--rw-r--r--   0        0        0      819 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/BUILD
--rw-r--r--   0        0        0    10158 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/SpineTest.cpp
--rw-r--r--   0        0        0     3799 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/StateMachineTest.cpp
--rw-r--r--   0        0        0     4671 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/position_commands_test.cpp
--rw-r--r--   0        0        0     6605 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/spine_interface_test.py
--rw-r--r--   0        0        0     1126 2023-03-13 11:06:13.763030 vulp-1.1.1/vulp/spine/tests/stop_commands_test.cpp
--rw-r--r--   0        0        0     1605 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/BUILD
--rw-r--r--   0        0        0     1716 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/Spinlock.h
--rw-r--r--   0        0        0     2604 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/SynchronousClock.cpp
--rw-r--r--   0        0        0     2987 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/SynchronousClock.h
--rw-r--r--   0        0        0     1091 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/datetime_now_string.h
--rw-r--r--   0        0        0     1193 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/handle_interrupts.cpp
--rw-r--r--   0        0        0     1121 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/handle_interrupts.h
--rw-r--r--   0        0        0     2025 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/low_pass_filter.h
--rw-r--r--   0        0        0     1003 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/math.h
--rw-r--r--   0        0        0     1302 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/random_string.h
--rw-r--r--   0        0        0     2106 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/realtime.h
--rw-r--r--   0        0        0     1416 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/serialize.py
--rw-r--r--   0        0        0      382 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/BUILD
--rw-r--r--   0        0        0     1502 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/SpinlockTest.cpp
--rw-r--r--   0        0        0     1356 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/SynchronousClockTest.cpp
--rw-r--r--   0        0        0      930 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     1234 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/low_pass_filter_test.cpp
--rw-r--r--   0        0        0      859 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/math_test.cpp
--rw-r--r--   0        0        0     1215 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/random_string_test.cpp
--rw-r--r--   0        0        0      920 2023-03-13 11:06:13.775030 vulp-1.1.1/vulp/utils/tests/realtime_test.cpp
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 vulp-1.1.1/setup.py
--rw-r--r--   0        0        0    11902 1970-01-01 00:00:00.000000 vulp-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10714 2023-06-06 14:06:26.335895 vulp-1.2.0/README.md
+-rw-r--r--   0        0        0     1406 2023-06-06 14:06:26.331895 vulp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/__init__.py
+-rw-r--r--   0        0        0     3444 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/AgentInterface.cpp
+-rw-r--r--   0        0        0     2957 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/AgentInterface.h
+-rw-r--r--   0        0        0     1991 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/BUILD
+-rw-r--r--   0        0        0      862 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/Request.h
+-rw-r--r--   0        0        0     9017 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/Spine.cpp
+-rw-r--r--   0        0        0     6184 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/Spine.h
+-rw-r--r--   0        0        0     5110 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/StateMachine.cpp
+-rw-r--r--   0        0        0     3944 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/StateMachine.h
+-rw-r--r--   0        0        0      872 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/position_commands.h
+-rw-r--r--   0        0        0     1011 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/request.py
+-rw-r--r--   0        0        0      783 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/spine_error.py
+-rw-r--r--   0        0        0     6305 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/spine_interface.py
+-rw-r--r--   0        0        0    20664 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tags
+-rw-r--r--   0        0        0     1638 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/AgentInterfaceTest.cpp
+-rw-r--r--   0        0        0      718 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/BUILD
+-rw-r--r--   0        0        0    10158 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/SpineTest.cpp
+-rw-r--r--   0        0        0     3799 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/StateMachineTest.cpp
+-rw-r--r--   0        0        0     6602 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/spine_interface_test.py
+-rw-r--r--   0        0        0     1574 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/BUILD
+-rw-r--r--   0        0        0     1716 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/Spinlock.h
+-rw-r--r--   0        0        0     2604 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/SynchronousClock.cpp
+-rw-r--r--   0        0        0     2987 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/SynchronousClock.h
+-rw-r--r--   0        0        0     1091 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/datetime_now_string.h
+-rw-r--r--   0        0        0     1193 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/handle_interrupts.cpp
+-rw-r--r--   0        0        0     1121 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/handle_interrupts.h
+-rw-r--r--   0        0        0     2025 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/low_pass_filter.h
+-rw-r--r--   0        0        0     1003 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/math.h
+-rw-r--r--   0        0        0     1302 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/random_string.h
+-rw-r--r--   0        0        0     2106 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/realtime.h
+-rw-r--r--   0        0        0     1416 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/serialize.py
+-rw-r--r--   0        0        0      351 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/tests/BUILD
+-rw-r--r--   0        0        0     1502 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/SpinlockTest.cpp
+-rw-r--r--   0        0        0     1356 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/SynchronousClockTest.cpp
+-rw-r--r--   0        0        0      930 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     1234 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/low_pass_filter_test.cpp
+-rw-r--r--   0        0        0      859 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/math_test.cpp
+-rw-r--r--   0        0        0     1215 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/random_string_test.cpp
+-rw-r--r--   0        0        0      920 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/realtime_test.cpp
+-rw-r--r--   0        0        0    11972 1970-01-01 00:00:00.000000 vulp-1.2.0/PKG-INFO
```

### Comparing `vulp-1.1.1/README.md` & `vulp-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 # Vulp — Real-time motion control for Python
 
 ![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/vulp/bazel.yml?branch=main)](https://github.com/tasts-robots/vulp/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/vulp/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/vulp/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/vulp?branch=main)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
-[![Example project](https://img.shields.io/badge/example-upkie_locomotion-green)](https://github.com/tasts-robots/upkie_locomotion)
+[![Example project](https://img.shields.io/badge/example-upkie-green)](https://github.com/tasts-robots/upkie)
+[![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Vulp provides a standard action-observation loop to control actuators/simulators from Python. It looks like this:
+Vulp provides an action-observation loop to control robots from Python, like this:
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/tasts-robots/vulp/main/doc/figures/action-observation-loop-full.svg" alt="Action-observation loop with Vulp" class="center"/>
 </p>
 
-More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
-
-In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
+Vulp works on Linux (desktop and Raspberry Pi) with [moteus](https://github.com/mjbots/moteus/) actuators and [Bullet](https://github.com/bulletphysics/bullet3) for simulation.
 
 ### Try it out!
 
 No installation required on Linux:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
-git clone https://github.com/tasts-robots/upkie_locomotion.git
-cd upkie_locomotion
-./tools/bazelisk run -c opt //agents/blue_balancer:bullet
+$ git clone https://github.com/tasts-robots/upkie.git
+$ cd upkie
+$ ./start_test_balancer.sh
 ```
 
 Connect a USB controller to move the robot around. 🎮
 
-The syntax is the same to deploy to the Raspberry Pi of a real robot like [Upkie](https://hackaday.io/project/185729-upkie-homemade-wheeled-biped-robot).
+Check out the [``upkie``](https://github.com/tasts-robots/upkie) repository for an example where Vulp is used with Upkie wheeled biped, including simulation environments, real-robot spines, state observers and locomotion agents.
+
+## Details
+
+More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
+
+In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
 
-## Features and non-features
+### Features and non-features
 
 All design decisions have their pros and cons. Take a look at the features and non-features below to decide if Vulp is a fit to your use case.
 
-### Features
+#### Features
 
 - Run the same Python code on simulated and real robots
 - Interfaces with to the [mjbots pi3hat](https://mjbots.com/products/mjbots-pi3hat-r4-4b) and mjbots actuators
 - Interfaces with to the [Bullet](http://bulletphysics.org/) simulator
 - Observer pipeline to extend observations
 - 🏗️ Controller pipeline to extend actions
 - Soft real-time: spine-agent loop interactions are predictable and repeatable
 - Unit tested, and not only with end-to-end tests
 
-### Non-features
+#### Non-features
 
 - Low frequency: Vulp is designed for tasks that run in the 1–400 Hz range (like balancing bipeds or quadrupeds)
 - Soft, not hard real-time guarantee: the code is empirically reliable by a large margin, that's it
 - Weakly-typed IPC: typing is used within agents and spines, but the interface between them is only checked at runtime
 
 ### Alternatives
 
@@ -64,25 +69,21 @@
 If your robot is built with some of the following open hardware components, you can also use their corresponding bindings directly:
 
 * [moteus](https://pypi.org/project/moteus/) - Python bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
 * [odri_control_interface](https://github.com/open-dynamic-robot-initiative/odri_control_interface) - interface to control robots built with the [ODRI](https://github.com/open-dynamic-robot-initiative) Master Board.
 
 Using control bindings directly is a simpler alternative if you don't need the action-observation loop and simulation/real-robot switch from Vulp.
 
-## Getting started
-
-Check out [``upkie_locomotion``](https://github.com/tasts-robots/upkie_locomotion) to get started with a simulation and real-robot spines, custom observers and locomotion agents.
-
 ## Q and A
 
 ### Performance
 
 #### How can motion control be real-time in Python, with garbage collection and all?
 
-Python agents talk with Vulp spines via the ``SpineInterface``, which can process both actions and observations in [about 0.7 ± 0.3 ms](doc/loop_cycles.md). This leaves plenty of room to implement other control components in a low-frequency loop. You may also be surprised at how Python performance has improved in recent years (most "tricks" that were popular ten years ago have been optimized away in CPython 3.8+). To consider one data point, here are the cycle periods measured in a complete Python agent for Upkie (the Pink balancer from [`upkie_locomotion`](https://github.com/tasts-robots/upkie_locomotion)) running on a Raspberry Pi 4 Model B (Quad core ARM Cortex-A72 @ 1.5GHz). It performs non-trivial tasks like balancing and whole-body inverse kinematics by quadratic programming:
+Python agents talk with Vulp spines via the ``SpineInterface``, which can process both actions and observations in [about 0.7 ± 0.3 ms](doc/loop_cycles.md). This leaves plenty of room to implement other control components in a low-frequency loop. You may also be surprised at how Python performance has improved in recent years (most "tricks" that were popular ten years ago have been optimized away in CPython 3.8+). To consider one data point, here are the cycle periods measured in a complete Python agent for Upkie (the Pink balancer from [`upkie`](https://github.com/tasts-robots/upkie)) running on a Raspberry Pi 4 Model B (Quad core ARM Cortex-A72 @ 1.5GHz). It performs non-trivial tasks like balancing and whole-body inverse kinematics by quadratic programming:
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/1189580/172820003-ade5aee1-fdca-41d7-958a-baf397a2caa3.png" width="800">
 </p>
 
 Note that the aforementioned 0.7 ± 0.3 ms processing time happens on the Python side, and is thus included in the 5.0 ms cycles represented by the orange curve. Meanwhile the spine is set to a reference frequency of 1.0 kHz and its corresponding cycle period was measured here at 1.0 ± 0.05 ms.
```

### Comparing `vulp-1.1.1/pyproject.toml` & `vulp-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/__init__.py` & `vulp-1.2.0/vulp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Real-time motion control for Python."""
 
-__version__ = "1.1.1"
+__version__ = "1.2.0"
```

### Comparing `vulp-1.1.1/vulp/spine/AgentInterface.cpp` & `vulp-1.2.0/vulp/spine/AgentInterface.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -23,27 +23,31 @@
 
 /*! Allocate file with some error handling.
  *
  * \param[in] file_descriptor File descriptor.
  * \param[in] bytes Number of bytes to allocate.
  */
 void allocate_file(int file_descriptor, int bytes) {
-  ::lseek(file_descriptor, bytes, SEEK_SET);
-  if (::write(file_descriptor, "", 1) < 1) {
-    throw std::runtime_error(
-        "Error allocating file (writing a single byte at the end)");
+  struct ::stat file_stats;
+  ::ftruncate(file_descriptor, bytes);
+  ::fstat(file_descriptor, &file_stats);
+  if (file_stats.st_size < bytes) {
+    throw std::runtime_error("Error allocating " + std::to_string(bytes) +
+                             " bytes in shared memory");
   }
-  ::lseek(file_descriptor, 0, SEEK_SET);
 }
 
 AgentInterface::AgentInterface(const std::string& name, size_t size)
     : name_(name), size_(size) {
   // Allocate shared memory
+  // About umask: see https://stackoverflow.com/a/11909753
+  mode_t existing_umask = ::umask(0);
   int file_descriptor =
       ::shm_open(name.c_str(), O_RDWR | O_CREAT | O_EXCL, 0666);
+  ::umask(existing_umask);
   if (file_descriptor < 0) {
     if (errno == EINVAL) {
       spdlog::error("Cannot open shared memory \"{}\": file name is invalid.",
                     name);
     } else if (errno == EEXIST) {
       spdlog::error(
           "Cannot open shared memory \"{}\": file already exists. Is the spine "
```

### Comparing `vulp-1.1.1/vulp/spine/AgentInterface.h` & `vulp-1.2.0/vulp/spine/AgentInterface.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/BUILD` & `vulp-1.2.0/vulp/spine/BUILD`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,18 @@
 
 load("//tools/lint:lint.bzl", "add_lint_tests")
 load("@pip_vulp//:requirements.bzl", "requirement")
 
 package(default_visibility = ["//visibility:public"])
 
 cc_library(
-    name = "stop_commands",
-    hdrs = [
-        "stop_commands.h",
-    ],
-    deps = [
-        "//actuation/moteus",
-    ],
-    include_prefix = "vulp/spine",
-)
-
-cc_library(
-    name = "position_commands",
-    hdrs = [
-        "position_commands.h",
-    ],
-    deps = [
-        "@palimpsest",
-        "//actuation/moteus",
-    ],
-    include_prefix = "vulp/spine",
-)
-
-cc_library(
     name = "request",
     hdrs = [
         "Request.h",
     ],
-    srcs = [
-    ],
-    deps = [
-    ],
     include_prefix = "vulp/spine",
 )
 
 cc_library(
     name = "agent_interface",
     hdrs = [
         "AgentInterface.h",
@@ -76,29 +49,28 @@
     name = "spine",
     hdrs = [
         "Spine.h",
     ],
     srcs = [
         "Spine.cpp",
     ],
-    linkopts = [
-        "-lrt",
-    ],
+    linkopts = select({
+        "//:linux": ["-lrt"],
+        "@//conditions:default": [],
+    }),
     deps = [
         "//actuation:imu_data",
         "//actuation:interface",
         "//observation:observe_imu",
         "//observation:observe_servos",
         "//observation:observe_time",
         "//observation:observer_pipeline",
         "//utils:realtime",
         "//utils:synchronous_clock",
-        ":position_commands",
         ":state_machine",
-        ":stop_commands",
         "@mpacklog",
     ],
     include_prefix = "vulp/spine",
 )
 
 py_library(
     name = "python",
@@ -118,8 +90,8 @@
         "__init__.py",
         "request.py",
         "spine_error.py",
         "spine_interface.py",
     ],
 )
 
-add_lint_tests(enable_clang_format_lint = True)
+add_lint_tests()
```

### Comparing `vulp-1.1.1/vulp/spine/Request.h` & `vulp-1.2.0/vulp/spine/Request.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/Spine.cpp` & `vulp-1.2.0/vulp/spine/Spine.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 #include "vulp/spine/Spine.h"
 
 #include <mpacklog/Logger.h>
 
 #include <limits>
 
 #include "vulp/observation/ObserverError.h"
-#include "vulp/spine/position_commands.h"
-#include "vulp/spine/stop_commands.h"
 
 namespace vulp::spine {
 
 using observation::ObserverError;
 using palimpsest::Dictionary;
 
 /*! Expect a timestamp in the action dictionary.
@@ -75,15 +73,15 @@
   dict_.insert<double>("time", observation.get<double>("time"));
 }
 
 void Spine::reset(const Dictionary& config) {
   actuation_.reset(config);
   dict_("action").clear();
   expect_timestamp(dict_("action"));
-  expect_position_commands(dict_("action"), actuation_.servo_joint_map());
+  actuation_.initialize_action(dict_("action"));
   observer_pipeline_.reset(config);
 }
 
 void Spine::log_dict() {
   Dictionary& spine = dict_("spine");
   spine("logger")("last_size") = logger_.last_size();
   spine("state")("cycle_beginning") =
@@ -185,33 +183,34 @@
                      e.key());
       }
     }
 
     // 2. Action
     if (state_machine_.state() == State::kSendStops ||
         state_machine_.state() == State::kShutdown) {
-      write_stop_commands(actuation_.commands());
+      actuation_.write_stop_commands();
     } else if (state_machine_.state() == State::kAct) {
       Dictionary& action = dict_("action");
-      write_position_commands(actuation_.commands(),
-                              actuation_.servo_joint_map(), action);
+      actuation_.write_position_commands(action);
+      // TODO(scaron): don't re-send actuation
+      // See https://github.com/tasts-robots/vulp/issues/2
+      // spdlog::info("[Spine::cycle_actuation] ok");
     } else {
-      // TODO(scaron): clear commands, otherwise the previous ones will be
-      // sent again!
+      // spdlog::warn("[Spine::cycle_actuation] re-sending previous commands");
     }
   } catch (const std::exception& e) {
     spdlog::error("[Spine::cycle_actuation] Caught an exception: {}", e.what());
     spdlog::error("[Spine::cycle_actuation] Sending stop commands...");
     state_machine_.process_event(Event::kInterrupt);
-    write_stop_commands(actuation_.commands());
+    actuation_.write_stop_commands();
   } catch (...) {
     spdlog::error("[Spine::cycle_actuation] Caught an unknown exception!");
     spdlog::error("[Spine::cycle_actuation] Sending stop commands...");
     state_machine_.process_event(Event::kInterrupt);
-    write_stop_commands(actuation_.commands());
+    actuation_.write_stop_commands();
   }
 
   // Whatever exceptions were thrown around, we caught them and at this
   // point every actuation command is either a stop or a position one.
 
   // 3. Wait for the result of the last query and copy it
   if (actuation_output_.valid()) {
```

### Comparing `vulp-1.1.1/vulp/spine/Spine.h` & `vulp-1.2.0/vulp/spine/Spine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/StateMachine.cpp` & `vulp-1.2.0/vulp/spine/StateMachine.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/StateMachine.h` & `vulp-1.2.0/vulp/spine/StateMachine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/__init__.py` & `vulp-1.2.0/vulp/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/request.py` & `vulp-1.2.0/vulp/spine/request.py`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/spine_error.py` & `vulp-1.2.0/vulp/spine/spine_error.py`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/spine_interface.py` & `vulp-1.2.0/vulp/spine/spine_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 import mmap
 import sys
 from time import perf_counter_ns
 
 import msgpack
 import posix_ipc
 
-from .request import Request
 from vulp.utils.serialize import serialize
+
+from .request import Request
 from .spine_error import SpineError
 
 
 class SpineInterface:
 
     """!
     Interface to interact with a spine from a Python agent.
@@ -39,15 +40,15 @@
         """!
         Connect to the spine shared memory.
 
         @param shm_name Name of the shared memory object.
         """
         try:
             shared_memory = posix_ipc.SharedMemory(
-                shm_name, posix_ipc.O_RDWR, size=0
+                shm_name, size=0, read_only=False
             )
         except posix_ipc.ExistentialError as exn:
             raise RuntimeError(f"spine {shm_name} is not running") from exn
         try:
             _mmap = mmap.mmap(
                 shared_memory.fd,
                 shared_memory.size,
```

### Comparing `vulp-1.1.1/vulp/spine/stop_commands.h` & `vulp-1.2.0/vulp/utils/math.h`

 * *Files 26% similar despite different names*

```diff
@@ -12,29 +12,27 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #pragma once
 
-#include <vector>
+#include <cstdint>
 
-#include "vulp/actuation/moteus/Mode.h"
-#include "vulp/actuation/moteus/ServoCommand.h"
+//! Utility functions.
+namespace vulp::utils {
 
-namespace vulp::spine {
+//! Mathematical functions.
+namespace math {
 
-/*! Stop all servos.
- *
- * \param[out] commands Servo commands to set to stop.
- *
- * This function does not and should not throw, as it will be called by default
- * if any exception is caught from the spine control loop.
- */
-inline void write_stop_commands(
-    std::vector<actuation::moteus::ServoCommand>& commands) noexcept {
-  for (auto& command : commands) {
-    command.mode = actuation::moteus::Mode::kStopped;
+//! True if and only if \p divisor divides \p number.
+inline bool divides(uint32_t number, uint32_t divisor) {
+  if (divisor == 0) {
+    return false;
   }
+  uint32_t k = number / divisor;
+  return (number == k * divisor);
 }
 
-}  // namespace vulp::spine
+}  // namespace math
+
+}  // namespace vulp::utils
```

### Comparing `vulp-1.1.1/vulp/spine/tests/BUILD` & `vulp-1.2.0/vulp/spine/tests/BUILD`

 * *Files 20% similar despite different names*

```diff
@@ -13,26 +13,24 @@
         "*.h",
     ]),
     deps = [
         "//actuation:mock_interface",
         "//observation/tests:observers",
         "//observation:observer_pipeline",
         "//spine:agent_interface",
-        "//spine:position_commands",
         "//spine:spine",
         "//spine:state_machine",
-        "//spine:stop_commands",
         "//utils:random_string",
         "@googletest//:main",
         "@palimpsest",
     ],
 )
 
 py_test(
     name = "spine_interface_test",
     srcs = ["spine_interface_test.py"],
     deps = [
         "//spine:python",
     ],
 )
 
-add_lint_tests(enable_clang_format_lint = True)
+add_lint_tests()
```

### Comparing `vulp-1.1.1/vulp/spine/tests/SpineTest.cpp` & `vulp-1.2.0/vulp/spine/tests/SpineTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/tests/StateMachineTest.cpp` & `vulp-1.2.0/vulp/spine/tests/StateMachineTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/spine/tests/spine_interface_test.py` & `vulp-1.2.0/vulp/spine/tests/spine_interface_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 import sys
 import unittest
 
 import msgpack
 import posix_ipc
 
 from vulp.spine.request import Request
-from vulp.utils.serialize import serialize
 from vulp.spine.spine_interface import SpineInterface
+from vulp.utils.serialize import serialize
 
 wait_pre_monkeypatch = SpineInterface._wait_for_spine
 
 
 class TestSpineInterface(unittest.TestCase):
-
     last_action: dict
     last_config: dict
     shm_name: str
     next_observation: dict
     spine: SpineInterface
 
     def setUp(self, shm_name="/vulp", size=1024):
@@ -46,15 +45,15 @@
         Initialize a new fixture instance.
 
         Args:
             shm_name: Name of shared memory file.
             size: Size of shared memory file in bytes.
         """
         shared_memory = posix_ipc.SharedMemory(
-            shm_name, posix_ipc.O_RDWR | posix_ipc.O_CREAT, size=size
+            shm_name, posix_ipc.O_CREAT, size=size, read_only=False
         )
         _mmap = mmap.mmap(
             shared_memory.fd,
             shared_memory.size,
             flags=mmap.MAP_SHARED,
             prot=mmap.PROT_READ | mmap.PROT_WRITE,
         )
```

### Comparing `vulp-1.1.1/vulp/utils/BUILD` & `vulp-1.2.0/vulp/utils/BUILD`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 py_library(
     name = "serialize",
     srcs = [
         "serialize.py",
     ],
 )
 
-add_lint_tests(enable_clang_format_lint = True)
+add_lint_tests()
```

### Comparing `vulp-1.1.1/vulp/utils/Spinlock.h` & `vulp-1.2.0/vulp/utils/Spinlock.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/SynchronousClock.cpp` & `vulp-1.2.0/vulp/utils/SynchronousClock.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/SynchronousClock.h` & `vulp-1.2.0/vulp/utils/SynchronousClock.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/datetime_now_string.h` & `vulp-1.2.0/vulp/utils/datetime_now_string.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/handle_interrupts.cpp` & `vulp-1.2.0/vulp/utils/handle_interrupts.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/handle_interrupts.h` & `vulp-1.2.0/vulp/utils/handle_interrupts.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/low_pass_filter.h` & `vulp-1.2.0/vulp/utils/low_pass_filter.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/random_string.h` & `vulp-1.2.0/vulp/utils/random_string.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/realtime.h` & `vulp-1.2.0/vulp/utils/realtime.h`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/serialize.py` & `vulp-1.2.0/vulp/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/SpinlockTest.cpp` & `vulp-1.2.0/vulp/utils/tests/SpinlockTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/SynchronousClockTest.cpp` & `vulp-1.2.0/vulp/utils/tests/SynchronousClockTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/datetime_now_string_test.cpp` & `vulp-1.2.0/vulp/utils/tests/datetime_now_string_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/low_pass_filter_test.cpp` & `vulp-1.2.0/vulp/utils/tests/low_pass_filter_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/math_test.cpp` & `vulp-1.2.0/vulp/utils/tests/math_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/random_string_test.cpp` & `vulp-1.2.0/vulp/utils/tests/random_string_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/vulp/utils/tests/realtime_test.cpp` & `vulp-1.2.0/vulp/utils/tests/realtime_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.1.1/PKG-INFO` & `vulp-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulp
-Version: 1.1.1
+Version: 1.2.0
 Summary: Real-time motion control for Python.
 Keywords: motion control,real time,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -29,57 +29,62 @@
 # Vulp — Real-time motion control for Python
 
 ![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/vulp/bazel.yml?branch=main)](https://github.com/tasts-robots/vulp/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/vulp/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/vulp/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/vulp?branch=main)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
-[![Example project](https://img.shields.io/badge/example-upkie_locomotion-green)](https://github.com/tasts-robots/upkie_locomotion)
+[![Example project](https://img.shields.io/badge/example-upkie-green)](https://github.com/tasts-robots/upkie)
+[![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Vulp provides a standard action-observation loop to control actuators/simulators from Python. It looks like this:
+Vulp provides an action-observation loop to control robots from Python, like this:
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/tasts-robots/vulp/main/doc/figures/action-observation-loop-full.svg" alt="Action-observation loop with Vulp" class="center"/>
 </p>
 
-More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
-
-In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
+Vulp works on Linux (desktop and Raspberry Pi) with [moteus](https://github.com/mjbots/moteus/) actuators and [Bullet](https://github.com/bulletphysics/bullet3) for simulation.
 
 ### Try it out!
 
 No installation required on Linux:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
-git clone https://github.com/tasts-robots/upkie_locomotion.git
-cd upkie_locomotion
-./tools/bazelisk run -c opt //agents/blue_balancer:bullet
+$ git clone https://github.com/tasts-robots/upkie.git
+$ cd upkie
+$ ./start_test_balancer.sh
 ```
 
 Connect a USB controller to move the robot around. 🎮
 
-The syntax is the same to deploy to the Raspberry Pi of a real robot like [Upkie](https://hackaday.io/project/185729-upkie-homemade-wheeled-biped-robot).
+Check out the [``upkie``](https://github.com/tasts-robots/upkie) repository for an example where Vulp is used with Upkie wheeled biped, including simulation environments, real-robot spines, state observers and locomotion agents.
+
+## Details
+
+More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
+
+In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
 
-## Features and non-features
+### Features and non-features
 
 All design decisions have their pros and cons. Take a look at the features and non-features below to decide if Vulp is a fit to your use case.
 
-### Features
+#### Features
 
 - Run the same Python code on simulated and real robots
 - Interfaces with to the [mjbots pi3hat](https://mjbots.com/products/mjbots-pi3hat-r4-4b) and mjbots actuators
 - Interfaces with to the [Bullet](http://bulletphysics.org/) simulator
 - Observer pipeline to extend observations
 - 🏗️ Controller pipeline to extend actions
 - Soft real-time: spine-agent loop interactions are predictable and repeatable
 - Unit tested, and not only with end-to-end tests
 
-### Non-features
+#### Non-features
 
 - Low frequency: Vulp is designed for tasks that run in the 1–400 Hz range (like balancing bipeds or quadrupeds)
 - Soft, not hard real-time guarantee: the code is empirically reliable by a large margin, that's it
 - Weakly-typed IPC: typing is used within agents and spines, but the interface between them is only checked at runtime
 
 ### Alternatives
 
@@ -92,25 +97,21 @@
 If your robot is built with some of the following open hardware components, you can also use their corresponding bindings directly:
 
 * [moteus](https://pypi.org/project/moteus/) - Python bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
 * [odri_control_interface](https://github.com/open-dynamic-robot-initiative/odri_control_interface) - interface to control robots built with the [ODRI](https://github.com/open-dynamic-robot-initiative) Master Board.
 
 Using control bindings directly is a simpler alternative if you don't need the action-observation loop and simulation/real-robot switch from Vulp.
 
-## Getting started
-
-Check out [``upkie_locomotion``](https://github.com/tasts-robots/upkie_locomotion) to get started with a simulation and real-robot spines, custom observers and locomotion agents.
-
 ## Q and A
 
 ### Performance
 
 #### How can motion control be real-time in Python, with garbage collection and all?
 
-Python agents talk with Vulp spines via the ``SpineInterface``, which can process both actions and observations in [about 0.7 ± 0.3 ms](doc/loop_cycles.md). This leaves plenty of room to implement other control components in a low-frequency loop. You may also be surprised at how Python performance has improved in recent years (most "tricks" that were popular ten years ago have been optimized away in CPython 3.8+). To consider one data point, here are the cycle periods measured in a complete Python agent for Upkie (the Pink balancer from [`upkie_locomotion`](https://github.com/tasts-robots/upkie_locomotion)) running on a Raspberry Pi 4 Model B (Quad core ARM Cortex-A72 @ 1.5GHz). It performs non-trivial tasks like balancing and whole-body inverse kinematics by quadratic programming:
+Python agents talk with Vulp spines via the ``SpineInterface``, which can process both actions and observations in [about 0.7 ± 0.3 ms](doc/loop_cycles.md). This leaves plenty of room to implement other control components in a low-frequency loop. You may also be surprised at how Python performance has improved in recent years (most "tricks" that were popular ten years ago have been optimized away in CPython 3.8+). To consider one data point, here are the cycle periods measured in a complete Python agent for Upkie (the Pink balancer from [`upkie`](https://github.com/tasts-robots/upkie)) running on a Raspberry Pi 4 Model B (Quad core ARM Cortex-A72 @ 1.5GHz). It performs non-trivial tasks like balancing and whole-body inverse kinematics by quadratic programming:
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/1189580/172820003-ade5aee1-fdca-41d7-958a-baf397a2caa3.png" width="800">
 </p>
 
 Note that the aforementioned 0.7 ± 0.3 ms processing time happens on the Python side, and is thus included in the 5.0 ms cycles represented by the orange curve. Meanwhile the spine is set to a reference frequency of 1.0 kHz and its corresponding cycle period was measured here at 1.0 ± 0.05 ms.
```

