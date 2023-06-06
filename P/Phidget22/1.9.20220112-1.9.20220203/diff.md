# Comparing `tmp/Phidget22-1.9.20220112.tar.gz` & `tmp/Phidget22-1.9.20220203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Phidget22-1.9.20220112.tar", last modified: Wed Jan 12 22:07:13 2022, max compression
+gzip compressed data, was "dist/Phidget22-1.9.20220203.tar", last modified: Fri Feb  4 00:25:26 2022, max compression
```

## Comparing `Phidget22-1.9.20220112.tar` & `Phidget22-1.9.20220203.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:07:13.000000 Phidget22-1.9.20220112/
-drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:07:12.000000 Phidget22-1.9.20220112/Phidget22/
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1212 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/Phidget22/Async.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      917 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/BridgeGain.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5177 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ChannelClass.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     2303 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ChannelSubclass.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3321 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/CodeInfo.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      488 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ControlMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3222 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/DeviceClass.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    15494 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/DeviceID.py
-drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:07:13.000000 Phidget22-1.9.20220112/Phidget22/Devices/
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6794 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Accelerometer.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    14164 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/BLDCMotor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     7530 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/CapacitiveTouch.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5757 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/CurrentInput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    15182 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/DCMotor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5726 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Dictionary.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3006 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/DigitalInput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     8111 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/DigitalOutput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     7721 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/DistanceSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6315 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Encoder.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     9082 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/FrequencyCounter.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6147 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/GPS.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5352 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Gyroscope.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      817 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Hub.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5203 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/HumiditySensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5584 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/IR.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    17652 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/LCD.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5329 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/LightSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3925 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Log.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     8164 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Magnetometer.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3224 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Manager.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    19204 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/MotorPositionController.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6221 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/PHSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     4112 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/PowerGuard.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5203 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/PressureSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    16504 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/RCServo.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5986 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/ResistanceInput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     4116 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/RFID.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6530 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/SoundSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     9574 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Spatial.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    14851 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/Stepper.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     7383 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/TemperatureSensor.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     9605 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/VoltageInput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     4607 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/VoltageOutput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     9970 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Devices/VoltageRatioInput.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/Phidget22/Devices/__init__.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1122 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/EncoderIOMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      888 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Encoding.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      344 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Endianness.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     7482 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ErrorCode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     3189 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ErrorEventCode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      450 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/FanMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      605 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/FilterType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      857 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/GPSDate.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1042 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/GPSTime.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      671 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/HandshakeMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      859 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/HubPortMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      359 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/InputMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      613 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/IOVoltage.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      894 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/IRCodeEncoding.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      553 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/IRCodeLength.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      554 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/LCDFont.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      443 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/LCDPixelState.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1686 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/LCDScreenSize.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1085 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/LEDForwardVoltage.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      547 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Length.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      732 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/LogLevel.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      354 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/MeshMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5054 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Net.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1144 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/PacketErrorCode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      419 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Parity.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)    17427 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Phidget.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1212 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/Phidget22/PhidgetException.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1737 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/PhidgetServer.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1990 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/PhidgetServerType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1039 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/Phidget22/PhidgetSupport.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      856 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/PortMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      499 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/PowerSupply.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1219 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Protocol.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      491 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/RCServoVoltage.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      445 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/RFIDProtocol.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      747 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/RTDType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      676 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/RTDWireSetup.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      608 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SpatialAlgorithm.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      842 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SpatialEulerAngles.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      606 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SpatialPrecision.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      866 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SpatialQuaternion.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      475 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SPIMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      312 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/SPLRange.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      495 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/StepperControlMode.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      307 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/StopBits.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      760 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/ThermocoupleType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1854 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/Unit.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      897 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/UnitInfo.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)      370 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/VoltageOutputRange.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     1402 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/VoltageRange.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     6706 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/VoltageRatioSensorType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)     5250 2022-01-12 22:06:57.000000 Phidget22-1.9.20220112/Phidget22/VoltageSensorType.py
--rwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/Phidget22/__init__.py
-drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-01-12 22:07:12.000000 Phidget22-1.9.20220112/Phidget22.egg-info/
--rw-r--r--   0 buildbot (197608) None     (197121)        1 2022-01-12 22:07:10.000000 Phidget22-1.9.20220112/Phidget22.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot (197608) None     (197121)      726 2022-01-12 22:07:10.000000 Phidget22-1.9.20220112/Phidget22.egg-info/PKG-INFO
--rw-r--r--   0 buildbot (197608) None     (197121)     2845 2022-01-12 22:07:10.000000 Phidget22-1.9.20220112/Phidget22.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot (197608) None     (197121)       10 2022-01-12 22:07:10.000000 Phidget22-1.9.20220112/Phidget22.egg-info/top_level.txt
--rw-r--r--   0 buildbot (197608) None     (197121)      726 2022-01-12 22:07:13.000000 Phidget22-1.9.20220112/PKG-INFO
--rwxr-xr-x   0 buildbot (197608) None     (197121)      198 2022-01-12 22:06:56.000000 Phidget22-1.9.20220112/README.md
--rw-r--r--   0 buildbot (197608) None     (197121)       38 2022-01-12 22:07:13.000000 Phidget22-1.9.20220112/setup.cfg
--rwxr-xr-x   0 buildbot (197608) None     (197121)      673 2022-01-12 22:07:00.000000 Phidget22-1.9.20220112/setup.py
+drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/
+drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/Phidget22/
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1212 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Async.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      917 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/BridgeGain.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     4545 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ChannelClass.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     2303 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ChannelSubclass.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     3321 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/CodeInfo.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      489 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ControlMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     2732 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/DeviceClass.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    12578 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/DeviceID.py
+drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/Phidget22/Devices/
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6794 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Accelerometer.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    14164 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/BLDCMotor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     7530 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/CapacitiveTouch.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5757 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/CurrentInput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    15182 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/DCMotor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5726 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/Dictionary.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     3006 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/DigitalInput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     8111 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/DigitalOutput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     7721 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/DistanceSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6315 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Encoder.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     9082 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/FrequencyCounter.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6147 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/GPS.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5352 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Gyroscope.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1133 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/Hub.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5203 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/HumiditySensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5584 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/IR.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    17652 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/LCD.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5329 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/LightSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     3925 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Log.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     8164 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Magnetometer.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     3224 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Manager.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    19204 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/MotorPositionController.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6221 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/PHSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     4112 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/PowerGuard.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5203 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/PressureSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    16504 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/RCServo.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5986 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/ResistanceInput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     4116 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/RFID.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6530 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Devices/SoundSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     9574 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Spatial.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    14851 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/Stepper.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     7383 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/TemperatureSensor.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     9605 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/VoltageInput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     4607 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/VoltageOutput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     9970 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Devices/VoltageRatioInput.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-02-04 00:25:07.000000 Phidget22-1.9.20220203/Phidget22/Devices/__init__.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1122 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/EncoderIOMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      888 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Encoding.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      344 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Endianness.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     7482 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ErrorCode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     3189 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ErrorEventCode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      450 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/FanMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      605 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/FilterType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      857 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/GPSDate.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1042 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/GPSTime.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      671 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/HandshakeMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      859 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/HubPortMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      359 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/InputMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      613 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/IOVoltage.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      894 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/IRCodeEncoding.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      553 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/IRCodeLength.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      554 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/LCDFont.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      443 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/LCDPixelState.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1686 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/LCDScreenSize.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1085 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/LEDForwardVoltage.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      547 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Length.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      732 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/LogLevel.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      354 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/MeshMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5054 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Net.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1144 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/PacketErrorCode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      419 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Parity.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)    19380 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/Phidget.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1212 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/Phidget22/PhidgetException.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1737 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/PhidgetServer.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1319 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/PhidgetServerType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1039 2022-02-04 00:25:07.000000 Phidget22-1.9.20220203/Phidget22/PhidgetSupport.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      856 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/PortMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      499 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/PowerSupply.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1219 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Protocol.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      491 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/RCServoVoltage.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      445 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/RFIDProtocol.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      747 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/RTDType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      676 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/RTDWireSetup.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      608 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SpatialAlgorithm.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      842 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SpatialEulerAngles.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      606 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SpatialPrecision.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      866 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SpatialQuaternion.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      475 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SPIMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      312 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/SPLRange.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      496 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/StepperControlMode.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      307 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/StopBits.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      760 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/ThermocoupleType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1854 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/Unit.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      897 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/UnitInfo.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      370 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/VoltageOutputRange.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     1402 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/VoltageRange.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     6706 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/VoltageRatioSensorType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)     5250 2022-02-04 00:25:09.000000 Phidget22-1.9.20220203/Phidget22/VoltageSensorType.py
+-rwxr-xr-x   0 buildbot (197608) None     (197121)       27 2022-02-04 00:25:12.000000 Phidget22-1.9.20220203/Phidget22/__init__.py
+drwxr-xr-x   0 buildbot (197608) None     (197121)        0 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/Phidget22.egg-info/
+-rw-r--r--   0 buildbot (197608) None     (197121)        1 2022-02-04 00:25:23.000000 Phidget22-1.9.20220203/Phidget22.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot (197608) None     (197121)      726 2022-02-04 00:25:23.000000 Phidget22-1.9.20220203/Phidget22.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot (197608) None     (197121)     2845 2022-02-04 00:25:23.000000 Phidget22-1.9.20220203/Phidget22.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot (197608) None     (197121)       10 2022-02-04 00:25:23.000000 Phidget22-1.9.20220203/Phidget22.egg-info/top_level.txt
+-rw-r--r--   0 buildbot (197608) None     (197121)      726 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/PKG-INFO
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      198 2022-02-04 00:25:08.000000 Phidget22-1.9.20220203/README.md
+-rw-r--r--   0 buildbot (197608) None     (197121)       38 2022-02-04 00:25:26.000000 Phidget22-1.9.20220203/setup.cfg
+-rwxr-xr-x   0 buildbot (197608) None     (197121)      673 2022-02-04 00:25:11.000000 Phidget22-1.9.20220203/setup.py
```

### Comparing `Phidget22-1.9.20220112/Phidget22/Async.py` & `Phidget22-1.9.20220203/Phidget22/Async.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/BridgeGain.py` & `Phidget22-1.9.20220203/Phidget22/BridgeGain.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/ChannelClass.py` & `Phidget22-1.9.20220203/Phidget22/ChannelClass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import sys
 import ctypes
 class ChannelClass:
-	# Any channel
-	PHIDCHCLASS_NOTHING = 0
 	# Accelerometer channel
 	PHIDCHCLASS_ACCELEROMETER = 1
 	# Current input channel
 	PHIDCHCLASS_CURRENTINPUT = 2
-	# Data adapter channel
-	PHIDCHCLASS_DATAADAPTER = 3
 	# DC motor channel
 	PHIDCHCLASS_DCMOTOR = 4
 	# Digital input channel
 	PHIDCHCLASS_DIGITALINPUT = 5
 	# Digital output channel
 	PHIDCHCLASS_DIGITALOUTPUT = 6
 	# Distance sensor channel
@@ -35,16 +31,14 @@
 	PHIDCHCLASS_HUMIDITYSENSOR = 15
 	# IR channel
 	PHIDCHCLASS_IR = 16
 	# Light sensor channel
 	PHIDCHCLASS_LIGHTSENSOR = 17
 	# Magnetometer channel
 	PHIDCHCLASS_MAGNETOMETER = 18
-	# Mesh dongle channel
-	PHIDCHCLASS_MESHDONGLE = 19
 	# pH sensor channel
 	PHIDCHCLASS_PHSENSOR = 37
 	# Power guard channel
 	PHIDCHCLASS_POWERGUARD = 20
 	# Pressure sensor channel
 	PHIDCHCLASS_PRESSURESENSOR = 21
 	# RC Servo channel
@@ -63,37 +57,29 @@
 	PHIDCHCLASS_TEMPERATURESENSOR = 28
 	# Voltage input channel
 	PHIDCHCLASS_VOLTAGEINPUT = 29
 	# Voltage output channel
 	PHIDCHCLASS_VOLTAGEOUTPUT = 30
 	# Voltage ratio input channel
 	PHIDCHCLASS_VOLTAGERATIOINPUT = 31
-	# Firmware upgrade channel
-	PHIDCHCLASS_FIRMWAREUPGRADE = 32
-	# Generic channel
-	PHIDCHCLASS_GENERIC = 33
 	# Motor position control channel.
 	PHIDCHCLASS_MOTORPOSITIONCONTROLLER = 34
 	# BLDC motor channel
 	PHIDCHCLASS_BLDCMOTOR = 35
 	# Dictionary
 	PHIDCHCLASS_DICTIONARY = 36
 	# Current output channel
 	PHIDCHCLASS_CURRENTOUTPUT = 38
 
 	@classmethod
 	def getName(self, val):
-		if val == self.PHIDCHCLASS_NOTHING:
-			return "PHIDCHCLASS_NOTHING"
 		if val == self.PHIDCHCLASS_ACCELEROMETER:
 			return "PHIDCHCLASS_ACCELEROMETER"
 		if val == self.PHIDCHCLASS_CURRENTINPUT:
 			return "PHIDCHCLASS_CURRENTINPUT"
-		if val == self.PHIDCHCLASS_DATAADAPTER:
-			return "PHIDCHCLASS_DATAADAPTER"
 		if val == self.PHIDCHCLASS_DCMOTOR:
 			return "PHIDCHCLASS_DCMOTOR"
 		if val == self.PHIDCHCLASS_DIGITALINPUT:
 			return "PHIDCHCLASS_DIGITALINPUT"
 		if val == self.PHIDCHCLASS_DIGITALOUTPUT:
 			return "PHIDCHCLASS_DIGITALOUTPUT"
 		if val == self.PHIDCHCLASS_DISTANCESENSOR:
@@ -116,16 +102,14 @@
 			return "PHIDCHCLASS_HUMIDITYSENSOR"
 		if val == self.PHIDCHCLASS_IR:
 			return "PHIDCHCLASS_IR"
 		if val == self.PHIDCHCLASS_LIGHTSENSOR:
 			return "PHIDCHCLASS_LIGHTSENSOR"
 		if val == self.PHIDCHCLASS_MAGNETOMETER:
 			return "PHIDCHCLASS_MAGNETOMETER"
-		if val == self.PHIDCHCLASS_MESHDONGLE:
-			return "PHIDCHCLASS_MESHDONGLE"
 		if val == self.PHIDCHCLASS_PHSENSOR:
 			return "PHIDCHCLASS_PHSENSOR"
 		if val == self.PHIDCHCLASS_POWERGUARD:
 			return "PHIDCHCLASS_POWERGUARD"
 		if val == self.PHIDCHCLASS_PRESSURESENSOR:
 			return "PHIDCHCLASS_PRESSURESENSOR"
 		if val == self.PHIDCHCLASS_RCSERVO:
@@ -144,18 +128,14 @@
 			return "PHIDCHCLASS_TEMPERATURESENSOR"
 		if val == self.PHIDCHCLASS_VOLTAGEINPUT:
 			return "PHIDCHCLASS_VOLTAGEINPUT"
 		if val == self.PHIDCHCLASS_VOLTAGEOUTPUT:
 			return "PHIDCHCLASS_VOLTAGEOUTPUT"
 		if val == self.PHIDCHCLASS_VOLTAGERATIOINPUT:
 			return "PHIDCHCLASS_VOLTAGERATIOINPUT"
-		if val == self.PHIDCHCLASS_FIRMWAREUPGRADE:
-			return "PHIDCHCLASS_FIRMWAREUPGRADE"
-		if val == self.PHIDCHCLASS_GENERIC:
-			return "PHIDCHCLASS_GENERIC"
 		if val == self.PHIDCHCLASS_MOTORPOSITIONCONTROLLER:
 			return "PHIDCHCLASS_MOTORPOSITIONCONTROLLER"
 		if val == self.PHIDCHCLASS_BLDCMOTOR:
 			return "PHIDCHCLASS_BLDCMOTOR"
 		if val == self.PHIDCHCLASS_DICTIONARY:
 			return "PHIDCHCLASS_DICTIONARY"
 		if val == self.PHIDCHCLASS_CURRENTOUTPUT:
```

### Comparing `Phidget22-1.9.20220112/Phidget22/ChannelSubclass.py` & `Phidget22-1.9.20220203/Phidget22/ChannelSubclass.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/CodeInfo.py` & `Phidget22-1.9.20220203/Phidget22/CodeInfo.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/DeviceClass.py` & `Phidget22-1.9.20220203/Phidget22/DeviceClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import sys
 import ctypes
 class DeviceClass:
-	# Any device
-	PHIDCLASS_NOTHING = 0
 	# PhidgetAccelerometer device
 	PHIDCLASS_ACCELEROMETER = 1
 	# PhidgetAdvancedServo device
 	PHIDCLASS_ADVANCEDSERVO = 2
 	# PhidgetAnalog device
 	PHIDCLASS_ANALOG = 3
 	# PhidgetBridge device
@@ -21,16 +19,14 @@
 	PHIDCLASS_HUB = 8
 	# PhidgetInterfaceKit device
 	PHIDCLASS_INTERFACEKIT = 9
 	# PhidgetIR device
 	PHIDCLASS_IR = 10
 	# PhidgetLED device
 	PHIDCLASS_LED = 11
-	# Phidget Mesh Dongle
-	PHIDCLASS_MESHDONGLE = 12
 	# PhidgetMotorControl device
 	PHIDCLASS_MOTORCONTROL = 13
 	# PhidgetPHSensor device
 	PHIDCLASS_PHSENSOR = 14
 	# PhidgetRFID device
 	PHIDCLASS_RFID = 15
 	# PhidgetServo device
@@ -41,27 +37,21 @@
 	PHIDCLASS_STEPPER = 18
 	# PhidgetTemperatureSensor device
 	PHIDCLASS_TEMPERATURESENSOR = 19
 	# PhidgetTextLCD device
 	PHIDCLASS_TEXTLCD = 20
 	# Phidget VINT device
 	PHIDCLASS_VINT = 21
-	# Generic device
-	PHIDCLASS_GENERIC = 22
-	# Phidget device in Firmware Upgrade mode
-	PHIDCLASS_FIRMWAREUPGRADE = 23
 	# Dictionary device
 	PHIDCLASS_DICTIONARY = 24
 	# PhidgetDataAdapter device
 	PHIDCLASS_DATAADAPTER = 25
 
 	@classmethod
 	def getName(self, val):
-		if val == self.PHIDCLASS_NOTHING:
-			return "PHIDCLASS_NOTHING"
 		if val == self.PHIDCLASS_ACCELEROMETER:
 			return "PHIDCLASS_ACCELEROMETER"
 		if val == self.PHIDCLASS_ADVANCEDSERVO:
 			return "PHIDCLASS_ADVANCEDSERVO"
 		if val == self.PHIDCLASS_ANALOG:
 			return "PHIDCLASS_ANALOG"
 		if val == self.PHIDCLASS_BRIDGE:
@@ -76,16 +66,14 @@
 			return "PHIDCLASS_HUB"
 		if val == self.PHIDCLASS_INTERFACEKIT:
 			return "PHIDCLASS_INTERFACEKIT"
 		if val == self.PHIDCLASS_IR:
 			return "PHIDCLASS_IR"
 		if val == self.PHIDCLASS_LED:
 			return "PHIDCLASS_LED"
-		if val == self.PHIDCLASS_MESHDONGLE:
-			return "PHIDCLASS_MESHDONGLE"
 		if val == self.PHIDCLASS_MOTORCONTROL:
 			return "PHIDCLASS_MOTORCONTROL"
 		if val == self.PHIDCLASS_PHSENSOR:
 			return "PHIDCLASS_PHSENSOR"
 		if val == self.PHIDCLASS_RFID:
 			return "PHIDCLASS_RFID"
 		if val == self.PHIDCLASS_SERVO:
@@ -96,16 +84,12 @@
 			return "PHIDCLASS_STEPPER"
 		if val == self.PHIDCLASS_TEMPERATURESENSOR:
 			return "PHIDCLASS_TEMPERATURESENSOR"
 		if val == self.PHIDCLASS_TEXTLCD:
 			return "PHIDCLASS_TEXTLCD"
 		if val == self.PHIDCLASS_VINT:
 			return "PHIDCLASS_VINT"
-		if val == self.PHIDCLASS_GENERIC:
-			return "PHIDCLASS_GENERIC"
-		if val == self.PHIDCLASS_FIRMWAREUPGRADE:
-			return "PHIDCLASS_FIRMWAREUPGRADE"
 		if val == self.PHIDCLASS_DICTIONARY:
 			return "PHIDCLASS_DICTIONARY"
 		if val == self.PHIDCLASS_DATAADAPTER:
 			return "PHIDCLASS_DATAADAPTER"
 		return "<invalid enumeration value>"
```

### Comparing `Phidget22-1.9.20220112/Phidget22/DeviceID.py` & `Phidget22-1.9.20220203/Phidget22/DeviceID.py`

 * *Files 20% similar despite different names*

```diff
@@ -125,22 +125,16 @@
 	PHIDID_HIN1000 = 61
 	# Capacitive Scroll
 	PHIDID_HIN1001 = 62
 	# Joystick
 	PHIDID_HIN1100 = 63
 	# Phidget USB VINT Hub with 6 ports
 	PHIDID_HUB0000 = 64
-	# Phidget Mesh Hub with 4 ports
-	PHIDID_MESHHUB = 65
-	# Phidget Mesh Dongle
-	PHIDID_MESHDONGLE = 66
 	# Phidget SPI VINT Hub with 6 ports
 	PHIDID_HUB0004 = 67
-	# Phidget Lightning VINT Hub with 6 ports
-	PHIDID_LIGHTNINGHUB = 68
 	# Humidity Sensor
 	PHIDID_HUM1000 = 69
 	# LCD
 	PHIDID_LCD1100 = 70
 	# LED Driver 32
 	PHIDID_LED1000 = 71
 	# Light Sensor
@@ -177,106 +171,66 @@
 	PHIDID_TMP1000 = 87
 	# Thermocouple 1
 	PHIDID_TMP1100 = 88
 	# Thermocouple 4
 	PHIDID_TMP1101 = 89
 	# RTD
 	PHIDID_TMP1200 = 90
-	# Infrared Temperature Sensor
-	PHIDID_TMP1300 = 91
 	# Voltage Sensor High Precision
 	PHIDID_VCP1000 = 92
 	# Voltage Sensor Large
 	PHIDID_VCP1001 = 93
 	# Voltage Sensor Small
 	PHIDID_VCP1002 = 94
 	# Hub Port in Digital Input mode
 	PHIDID_DIGITALINPUT_PORT = 95
 	# Hub Port in Digital Output mode
 	PHIDID_DIGITALOUTPUT_PORT = 96
 	# Hub Port in Voltage Input mode
 	PHIDID_VOLTAGEINPUT_PORT = 97
 	# Hub Port in Voltage Ratio Input mode
 	PHIDID_VOLTAGERATIOINPUT_PORT = 98
-	# Generic USB device
-	PHIDID_GENERICUSB = 99
-	# Generic VINT device
-	PHIDID_GENERICVINT = 100
-	# USB device in firmware upgrade mode
-	PHIDID_FIRMWARE_UPGRADE_USB = 101
-	# VINT Device in firmware upgrade mode, STM32F0 Proc.
-	PHIDID_FIRMWARE_UPGRADE_STM32F0 = 102
-	# VINT Device in firmware upgrade mode, STM8S Proc.
-	PHIDID_FIRMWARE_UPGRADE_STM8S = 103
-	# Phidget SPI device under firmware upgrade
-	PHIDID_FIRMWARE_UPGRADE_SPI = 104
 	# 30A Current Sensor
 	PHIDID_VCP1100 = 105
 	# BLDC Motor Controller
 	PHIDID_DCC1100 = 108
 	# Dial Encoder
 	PHIDID_HIN1101 = 109
 	# Small DC Motor Controller
 	PHIDID_DCC1001 = 110
 	# Dictionary
 	PHIDID_DICTIONARY = 111
 	# Bipolar Stepper Motor SmallController
 	PHIDID_STC1001 = 115
-	# OS Testing Fixture
-	PHIDID_USBSWITCH = 116
 	# 4A Small DC Motor Controller
 	PHIDID_DCC1002 = 117
 	# 8A Bipolar Stepper Motor Controller
 	PHIDID_STC1002 = 118
 	# 4A Bipolar Stepper Motor SmallController
 	PHIDID_STC1003 = 119
 	# 2 Channel DC Motor Controller
 	PHIDID_DCC1003 = 120
 	# 650mm distance sensor
 	PHIDID_DST1001 = 121
-	# 4-20mA Output
-	PHIDID_CURLOOP = 122
 	# Phidget Network Hub with 6 ports
 	PHIDID_HUB5000 = 123
 	# PhidgetAdvancedServo 8-Motor (RCC0004)
 	PHIDID_RCC0004 = 124
 	# Unknown device
 	PHIDID_UNKNOWN = 125
 	# 1200mm distance sensor
 	PHIDID_DST1002 = 126
 	# Humidity Sensor
 	PHIDID_HUM1001 = 127
-	# DC Motor Controller 12A
-	PHIDID_DCC1004 = 128
-	# DC Motor Controller High Current
-	PHIDID_DCC1005 = 129
-	# PhidgetSpatial 3/3/3
-	PHIDID_MOT0108 = 131
-	# RS232 Adapter
-	PHIDID_ADP1001 = 132
-	# RS485/422 Prototype
-	PHIDID_ADP_RS485_422 = 133
-	# Serial Prototype
-	PHIDID_ADP_SERIAL = 134
-	# VINT Moisture Sensor
-	PHIDID_HUM1100 = 136
 	# VINT Spatial Phidget AHRS
 	PHIDID_MOT1102 = 137
-	# VINT Accelerometer
-	PHIDID_VINTACCEL = 138
-	# Testpoint Diagnoser
-	PHIDID_TP_DIAGNOSER = 139
 	# PhidgetSpatial Precision 3/3/3
 	PHIDID_MOT0109 = 140
-	# PhidgetSpatial Precision 3/3/3
-	PHIDID_MOT0110 = 141
 	# Phidget USB VINT Hub with 6 ports
 	PHIDID_HUB0001 = 142
-	# VINT Device in firmware upgrade mode, STM32G0 Proc.
-	PHIDID_FIRMWARE_UPGRADE_STM32G0 = 143
 
 	@classmethod
 	def getName(self, val):
 		if val == self.PHIDID_NOTHING:
 			return "PHIDID_NOTHING"
 		if val == self.PHIDID_INTERFACEKIT_4_8_8:
 			return "PHIDID_INTERFACEKIT_4_8_8"
@@ -400,22 +354,16 @@
 			return "PHIDID_HIN1000"
 		if val == self.PHIDID_HIN1001:
 			return "PHIDID_HIN1001"
 		if val == self.PHIDID_HIN1100:
 			return "PHIDID_HIN1100"
 		if val == self.PHIDID_HUB0000:
 			return "PHIDID_HUB0000"
-		if val == self.PHIDID_MESHHUB:
-			return "PHIDID_MESHHUB"
-		if val == self.PHIDID_MESHDONGLE:
-			return "PHIDID_MESHDONGLE"
 		if val == self.PHIDID_HUB0004:
 			return "PHIDID_HUB0004"
-		if val == self.PHIDID_LIGHTNINGHUB:
-			return "PHIDID_LIGHTNINGHUB"
 		if val == self.PHIDID_HUM1000:
 			return "PHIDID_HUM1000"
 		if val == self.PHIDID_LCD1100:
 			return "PHIDID_LCD1100"
 		if val == self.PHIDID_LED1000:
 			return "PHIDID_LED1000"
 		if val == self.PHIDID_LUX1000:
@@ -452,100 +400,60 @@
 			return "PHIDID_TMP1000"
 		if val == self.PHIDID_TMP1100:
 			return "PHIDID_TMP1100"
 		if val == self.PHIDID_TMP1101:
 			return "PHIDID_TMP1101"
 		if val == self.PHIDID_TMP1200:
 			return "PHIDID_TMP1200"
-		if val == self.PHIDID_TMP1300:
-			return "PHIDID_TMP1300"
 		if val == self.PHIDID_VCP1000:
 			return "PHIDID_VCP1000"
 		if val == self.PHIDID_VCP1001:
 			return "PHIDID_VCP1001"
 		if val == self.PHIDID_VCP1002:
 			return "PHIDID_VCP1002"
 		if val == self.PHIDID_DIGITALINPUT_PORT:
 			return "PHIDID_DIGITALINPUT_PORT"
 		if val == self.PHIDID_DIGITALOUTPUT_PORT:
 			return "PHIDID_DIGITALOUTPUT_PORT"
 		if val == self.PHIDID_VOLTAGEINPUT_PORT:
 			return "PHIDID_VOLTAGEINPUT_PORT"
 		if val == self.PHIDID_VOLTAGERATIOINPUT_PORT:
 			return "PHIDID_VOLTAGERATIOINPUT_PORT"
-		if val == self.PHIDID_GENERICUSB:
-			return "PHIDID_GENERICUSB"
-		if val == self.PHIDID_GENERICVINT:
-			return "PHIDID_GENERICVINT"
-		if val == self.PHIDID_FIRMWARE_UPGRADE_USB:
-			return "PHIDID_FIRMWARE_UPGRADE_USB"
-		if val == self.PHIDID_FIRMWARE_UPGRADE_STM32F0:
-			return "PHIDID_FIRMWARE_UPGRADE_STM32F0"
-		if val == self.PHIDID_FIRMWARE_UPGRADE_STM8S:
-			return "PHIDID_FIRMWARE_UPGRADE_STM8S"
-		if val == self.PHIDID_FIRMWARE_UPGRADE_SPI:
-			return "PHIDID_FIRMWARE_UPGRADE_SPI"
 		if val == self.PHIDID_VCP1100:
 			return "PHIDID_VCP1100"
 		if val == self.PHIDID_DCC1100:
 			return "PHIDID_DCC1100"
 		if val == self.PHIDID_HIN1101:
 			return "PHIDID_HIN1101"
 		if val == self.PHIDID_DCC1001:
 			return "PHIDID_DCC1001"
 		if val == self.PHIDID_DICTIONARY:
 			return "PHIDID_DICTIONARY"
 		if val == self.PHIDID_STC1001:
 			return "PHIDID_STC1001"
-		if val == self.PHIDID_USBSWITCH:
-			return "PHIDID_USBSWITCH"
 		if val == self.PHIDID_DCC1002:
 			return "PHIDID_DCC1002"
 		if val == self.PHIDID_STC1002:
 			return "PHIDID_STC1002"
 		if val == self.PHIDID_STC1003:
 			return "PHIDID_STC1003"
 		if val == self.PHIDID_DCC1003:
 			return "PHIDID_DCC1003"
 		if val == self.PHIDID_DST1001:
 			return "PHIDID_DST1001"
-		if val == self.PHIDID_CURLOOP:
-			return "PHIDID_CURLOOP"
 		if val == self.PHIDID_HUB5000:
 			return "PHIDID_HUB5000"
 		if val == self.PHIDID_RCC0004:
 			return "PHIDID_RCC0004"
 		if val == self.PHIDID_UNKNOWN:
 			return "PHIDID_UNKNOWN"
 		if val == self.PHIDID_DST1002:
 			return "PHIDID_DST1002"
 		if val == self.PHIDID_HUM1001:
 			return "PHIDID_HUM1001"
-		if val == self.PHIDID_DCC1004:
-			return "PHIDID_DCC1004"
-		if val == self.PHIDID_DCC1005:
-			return "PHIDID_DCC1005"
-		if val == self.PHIDID_MOT0108:
-			return "PHIDID_MOT0108"
-		if val == self.PHIDID_ADP1001:
-			return "PHIDID_ADP1001"
-		if val == self.PHIDID_ADP_RS485_422:
-			return "PHIDID_ADP_RS485_422"
-		if val == self.PHIDID_ADP_SERIAL:
-			return "PHIDID_ADP_SERIAL"
-		if val == self.PHIDID_HUM1100:
-			return "PHIDID_HUM1100"
 		if val == self.PHIDID_MOT1102:
 			return "PHIDID_MOT1102"
-		if val == self.PHIDID_VINTACCEL:
-			return "PHIDID_VINTACCEL"
-		if val == self.PHIDID_TP_DIAGNOSER:
-			return "PHIDID_TP_DIAGNOSER"
 		if val == self.PHIDID_MOT0109:
 			return "PHIDID_MOT0109"
-		if val == self.PHIDID_MOT0110:
-			return "PHIDID_MOT0110"
 		if val == self.PHIDID_HUB0001:
 			return "PHIDID_HUB0001"
-		if val == self.PHIDID_FIRMWARE_UPGRADE_STM32G0:
-			return "PHIDID_FIRMWARE_UPGRADE_STM32G0"
 		return "<invalid enumeration value>"
```

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Accelerometer.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Accelerometer.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/BLDCMotor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/BLDCMotor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/CapacitiveTouch.py` & `Phidget22-1.9.20220203/Phidget22/Devices/CapacitiveTouch.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/CurrentInput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/CurrentInput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/DCMotor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/DCMotor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Dictionary.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Dictionary.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/DigitalInput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/DigitalInput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/DigitalOutput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/DigitalOutput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/DistanceSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/DistanceSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Encoder.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Encoder.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/FrequencyCounter.py` & `Phidget22-1.9.20220203/Phidget22/Devices/FrequencyCounter.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/GPS.py` & `Phidget22-1.9.20220203/Phidget22/Devices/GPS.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Gyroscope.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Gyroscope.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/HumiditySensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/HumiditySensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/IR.py` & `Phidget22-1.9.20220203/Phidget22/Devices/IR.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/LCD.py` & `Phidget22-1.9.20220203/Phidget22/Devices/LCD.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/LightSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/LightSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Log.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Log.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Magnetometer.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Magnetometer.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Manager.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Manager.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/MotorPositionController.py` & `Phidget22-1.9.20220203/Phidget22/Devices/MotorPositionController.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/PHSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/PHSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/PowerGuard.py` & `Phidget22-1.9.20220203/Phidget22/Devices/PowerGuard.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/PressureSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/PressureSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/RCServo.py` & `Phidget22-1.9.20220203/Phidget22/Devices/RCServo.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/ResistanceInput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/ResistanceInput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/RFID.py` & `Phidget22-1.9.20220203/Phidget22/Devices/RFID.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/SoundSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/SoundSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Spatial.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Spatial.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/Stepper.py` & `Phidget22-1.9.20220203/Phidget22/Devices/Stepper.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/TemperatureSensor.py` & `Phidget22-1.9.20220203/Phidget22/Devices/TemperatureSensor.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/VoltageInput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/VoltageInput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/VoltageOutput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/VoltageOutput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Devices/VoltageRatioInput.py` & `Phidget22-1.9.20220203/Phidget22/Devices/VoltageRatioInput.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/EncoderIOMode.py` & `Phidget22-1.9.20220203/Phidget22/EncoderIOMode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Encoding.py` & `Phidget22-1.9.20220203/Phidget22/Encoding.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/ErrorCode.py` & `Phidget22-1.9.20220203/Phidget22/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/ErrorEventCode.py` & `Phidget22-1.9.20220203/Phidget22/ErrorEventCode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/FilterType.py` & `Phidget22-1.9.20220203/Phidget22/FilterType.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/GPSDate.py` & `Phidget22-1.9.20220203/Phidget22/GPSDate.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/GPSTime.py` & `Phidget22-1.9.20220203/Phidget22/GPSTime.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/HandshakeMode.py` & `Phidget22-1.9.20220203/Phidget22/HandshakeMode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/HubPortMode.py` & `Phidget22-1.9.20220203/Phidget22/HubPortMode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/IOVoltage.py` & `Phidget22-1.9.20220203/Phidget22/IOVoltage.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/IRCodeEncoding.py` & `Phidget22-1.9.20220203/Phidget22/IRCodeEncoding.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/IRCodeLength.py` & `Phidget22-1.9.20220203/Phidget22/IRCodeLength.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/LCDFont.py` & `Phidget22-1.9.20220203/Phidget22/LCDFont.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/LCDScreenSize.py` & `Phidget22-1.9.20220203/Phidget22/LCDScreenSize.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/LEDForwardVoltage.py` & `Phidget22-1.9.20220203/Phidget22/LEDForwardVoltage.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Length.py` & `Phidget22-1.9.20220203/Phidget22/Length.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/LogLevel.py` & `Phidget22-1.9.20220203/Phidget22/LogLevel.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Net.py` & `Phidget22-1.9.20220203/Phidget22/Net.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/PacketErrorCode.py` & `Phidget22-1.9.20220203/Phidget22/PacketErrorCode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Phidget.py` & `Phidget22-1.9.20220203/Phidget22/Phidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -469,14 +469,61 @@
 		result = __func(self.handle, ctypes.byref(_HubPortCount))
 
 		if result > 0:
 			raise PhidgetException(result)
 
 		return _HubPortCount.value
 
+	def getHubPortSpeed(self):
+		_HubPortSpeed = ctypes.c_uint32()
+
+		__func = PhidgetSupport.getDll().Phidget_getHubPortSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, ctypes.byref(_HubPortSpeed))
+
+		if result > 0:
+			raise PhidgetException(result)
+
+		return _HubPortSpeed.value
+
+	def setHubPortSpeed(self, HubPortSpeed):
+		_HubPortSpeed = ctypes.c_uint32(HubPortSpeed)
+
+		__func = PhidgetSupport.getDll().Phidget_setHubPortSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, _HubPortSpeed)
+
+		if result > 0:
+			raise PhidgetException(result)
+
+
+	def getMaxHubPortSpeed(self):
+		_MaxHubPortSpeed = ctypes.c_uint32()
+
+		__func = PhidgetSupport.getDll().Phidget_getMaxHubPortSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, ctypes.byref(_MaxHubPortSpeed))
+
+		if result > 0:
+			raise PhidgetException(result)
+
+		return _MaxHubPortSpeed.value
+
+	def getHubPortSupportsSetSpeed(self):
+		_HubPortSupportsSetSpeed = ctypes.c_int()
+
+		__func = PhidgetSupport.getDll().Phidget_getHubPortSupportsSetSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, ctypes.byref(_HubPortSupportsSetSpeed))
+
+		if result > 0:
+			raise PhidgetException(result)
+
+		return _HubPortSupportsSetSpeed.value
+
 	def getIsChannel(self):
 		_IsChannel = ctypes.c_int()
 
 		__func = PhidgetSupport.getDll().Phidget_getIsChannel
 		__func.restype = ctypes.c_int32
 		result = __func(self.handle, ctypes.byref(_IsChannel))
 
@@ -643,14 +690,38 @@
 		result = __func(self.handle, ctypes.byref(_ServerUniqueName))
 
 		if result > 0:
 			raise PhidgetException(result)
 
 		return _ServerUniqueName.value.decode('utf-8')
 
+	def getMaxVINTDeviceSpeed(self):
+		_MaxVINTDeviceSpeed = ctypes.c_uint32()
+
+		__func = PhidgetSupport.getDll().Phidget_getMaxVINTDeviceSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, ctypes.byref(_MaxVINTDeviceSpeed))
+
+		if result > 0:
+			raise PhidgetException(result)
+
+		return _MaxVINTDeviceSpeed.value
+
+	def getVINTDeviceSupportsSetSpeed(self):
+		_VINTDeviceSupportsSetSpeed = ctypes.c_int()
+
+		__func = PhidgetSupport.getDll().Phidget_getVINTDeviceSupportsSetSpeed
+		__func.restype = ctypes.c_int32
+		result = __func(self.handle, ctypes.byref(_VINTDeviceSupportsSetSpeed))
+
+		if result > 0:
+			raise PhidgetException(result)
+
+		return _VINTDeviceSupportsSetSpeed.value
+
 	def writeDeviceLabel(self, deviceLabel):
 		_deviceLabel = ctypes.create_string_buffer(deviceLabel.encode('utf-8'))
 
 		__func = PhidgetSupport.getDll().Phidget_writeDeviceLabel
 		__func.restype = ctypes.c_int32
 		result = __func(self.handle, ctypes.byref(_deviceLabel))
```

### Comparing `Phidget22-1.9.20220112/Phidget22/PhidgetException.py` & `Phidget22-1.9.20220203/Phidget22/PhidgetException.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/PhidgetServer.py` & `Phidget22-1.9.20220203/Phidget22/PhidgetServer.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/PhidgetServerType.py` & `Phidget22-1.9.20220203/Phidget22/PhidgetServerType.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,19 @@
 import sys
 import ctypes
 class PhidgetServerType:
-	# Unknown or unspecified server type
-	PHIDGETSERVER_NONE = 0
-	# Phidget22 Server listener
-	PHIDGETSERVER_DEVICELISTENER = 1
-	# Phidget22 Server connection
-	PHIDGETSERVER_DEVICE = 2
 	# Phidget22 Server<br/>Server discovery with this server type allows discovery of servers hosting Phidget devices. Enabling server discovery with this server type allows automated connection to these servers, and the Phidgets connected to them. Enabling server discovery with this server type will also enable ServerAdded and ServerRemoved events for this server type.
 	PHIDGETSERVER_DEVICEREMOTE = 3
-	# Phidget22 Web Server
-	PHIDGETSERVER_WWWLISTENER = 4
-	# Phidget22 Web Server connection
-	PHIDGETSERVER_WWW = 5
 	# Phidget22 Web server<br/>Server discovery with this server type detects the presence of Phidget web servers used to communicate with in-browser JavaScript. Enabling server discovery with this server type will enable ServerAdded and ServerRemoved events for this server type.
 	PHIDGETSERVER_WWWREMOTE = 6
 	# Phidget SBC<br/>Server discovery with this server type detects the presence of Phidget SBCs on the network. Enabling server discovery with this server type will enable ServerAdded and ServerRemoved events for this server type.
 	PHIDGETSERVER_SBC = 7
 
 	@classmethod
 	def getName(self, val):
-		if val == self.PHIDGETSERVER_NONE:
-			return "PHIDGETSERVER_NONE"
-		if val == self.PHIDGETSERVER_DEVICELISTENER:
-			return "PHIDGETSERVER_DEVICELISTENER"
-		if val == self.PHIDGETSERVER_DEVICE:
-			return "PHIDGETSERVER_DEVICE"
 		if val == self.PHIDGETSERVER_DEVICEREMOTE:
 			return "PHIDGETSERVER_DEVICEREMOTE"
-		if val == self.PHIDGETSERVER_WWWLISTENER:
-			return "PHIDGETSERVER_WWWLISTENER"
-		if val == self.PHIDGETSERVER_WWW:
-			return "PHIDGETSERVER_WWW"
 		if val == self.PHIDGETSERVER_WWWREMOTE:
 			return "PHIDGETSERVER_WWWREMOTE"
 		if val == self.PHIDGETSERVER_SBC:
 			return "PHIDGETSERVER_SBC"
 		return "<invalid enumeration value>"
```

### Comparing `Phidget22-1.9.20220112/Phidget22/PhidgetSupport.py` & `Phidget22-1.9.20220203/Phidget22/PhidgetSupport.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/PortMode.py` & `Phidget22-1.9.20220203/Phidget22/PortMode.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Protocol.py` & `Phidget22-1.9.20220203/Phidget22/Protocol.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/RTDType.py` & `Phidget22-1.9.20220203/Phidget22/RTDType.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/RTDWireSetup.py` & `Phidget22-1.9.20220203/Phidget22/RTDWireSetup.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/SpatialAlgorithm.py` & `Phidget22-1.9.20220203/Phidget22/SpatialAlgorithm.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/SpatialEulerAngles.py` & `Phidget22-1.9.20220203/Phidget22/SpatialEulerAngles.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/SpatialPrecision.py` & `Phidget22-1.9.20220203/Phidget22/SpatialPrecision.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/SpatialQuaternion.py` & `Phidget22-1.9.20220203/Phidget22/SpatialQuaternion.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/ThermocoupleType.py` & `Phidget22-1.9.20220203/Phidget22/ThermocoupleType.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/Unit.py` & `Phidget22-1.9.20220203/Phidget22/Unit.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/UnitInfo.py` & `Phidget22-1.9.20220203/Phidget22/UnitInfo.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/VoltageRange.py` & `Phidget22-1.9.20220203/Phidget22/VoltageRange.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/VoltageRatioSensorType.py` & `Phidget22-1.9.20220203/Phidget22/VoltageRatioSensorType.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22/VoltageSensorType.py` & `Phidget22-1.9.20220203/Phidget22/VoltageSensorType.py`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/Phidget22.egg-info/PKG-INFO` & `Phidget22-1.9.20220203/Phidget22.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phidget22
-Version: 1.9.20220112
+Version: 1.9.20220203
 Summary: Phidget22 Python wrapper library
 Home-page: http://www.phidgets.com
 Author: Phidgets Inc
 Author-email: support@phidgets.com
 License: MIT
 Description: # Phidget22 Python Package
```

### Comparing `Phidget22-1.9.20220112/Phidget22.egg-info/SOURCES.txt` & `Phidget22-1.9.20220203/Phidget22.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Phidget22-1.9.20220112/PKG-INFO` & `Phidget22-1.9.20220203/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phidget22
-Version: 1.9.20220112
+Version: 1.9.20220203
 Summary: Phidget22 Python wrapper library
 Home-page: http://www.phidgets.com
 Author: Phidgets Inc
 Author-email: support@phidgets.com
 License: MIT
 Description: # Phidget22 Python Package
```

### Comparing `Phidget22-1.9.20220112/setup.py` & `Phidget22-1.9.20220203/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="Phidget22",
-    version='1.9.20220112',
+    version='1.9.20220203',
     author="Phidgets Inc",
     author_email="support@phidgets.com",
     description="Phidget22 Python wrapper library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.phidgets.com",
     packages=setuptools.find_packages(),
```

