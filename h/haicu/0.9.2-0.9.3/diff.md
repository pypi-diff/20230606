# Comparing `tmp/haicu-0.9.2.tar.gz` & `tmp/haicu-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.9.2.tar", last modified: Wed May 10 21:01:38 2023, max compression
+gzip compressed data, was "haicu-0.9.3.tar", last modified: Tue Jun  6 18:27:18 2023, max compression
```

## Comparing `haicu-0.9.2.tar` & `haicu-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.9.2/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 21:01:38.537605 haicu-0.9.2/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2619 2023-05-09 22:37:20.000000 haicu-0.9.2/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/haicu/
--rwxrwxr-x   0 bry       (1000) bry       (1000)    27557 2023-05-10 20:58:28.000000 haicu-0.9.2/haicu/__haicu_ctl.py
--rw-rw-r--   0 bry       (1000) bry       (1000)       43 2023-05-10 21:01:34.000000 haicu-0.9.2/haicu/__init__.py
--rw-rw-r--   0 bry       (1000) bry       (1000)       80 2023-05-10 17:49:55.000000 haicu-0.9.2/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    22343 2023-05-10 20:04:34.000000 haicu-0.9.2/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    15631 2023-05-10 19:56:51.000000 haicu-0.9.2/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      295 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       53 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      832 2023-05-10 17:49:32.000000 haicu-0.9.2/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-05-10 21:01:38.537605 haicu-0.9.2/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-06-06 18:27:18.983725 haicu-0.9.3/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-06-05 17:03:47.000000 haicu-0.9.3/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-06-06 18:27:18.983725 haicu-0.9.3/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2619 2023-06-05 17:03:47.000000 haicu-0.9.3/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-06-06 18:27:18.983725 haicu-0.9.3/haicu/
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    27767 2023-06-05 17:18:37.000000 haicu-0.9.3/haicu/__haicu_ctl.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)       43 2023-06-06 18:14:25.000000 haicu-0.9.3/haicu/__init__.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)       80 2023-06-05 17:03:47.000000 haicu-0.9.3/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    23302 2023-06-06 18:17:43.000000 haicu-0.9.3/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    15631 2023-06-05 17:03:47.000000 haicu-0.9.3/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-06-06 18:27:18.983725 haicu-0.9.3/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      295 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       53 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-06-06 18:27:18.000000 haicu-0.9.3/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      832 2023-06-05 17:03:47.000000 haicu-0.9.3/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-06-06 18:27:18.983725 haicu-0.9.3/setup.cfg
```

### Comparing `haicu-0.9.2/LICENSE` & `haicu-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.9.2/PKG-INFO` & `haicu-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.9.2
+Version: 0.9.3
 Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.9.2/README.md` & `haicu-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.9.2/haicu/__haicu_ctl.py` & `haicu-0.9.3/haicu/__haicu_ctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,25 @@
 def handle_set(name, ftdi_dev, addr, mask, offset, data, json):
         if(data == None):
             result = read_masked_register(ftdi_dev, addr, mask, offset)
             print("0x" + '{:02X}'.format(result)) if(not json) else  print("{\"" + name + "\": 0x" + '{:02X}'.format(result) + "}")
         else:
             rmr_register(ftdi_dev, addr, mask, offset, int(data, 0))
 
+def get_mld1200(args):
+    try:
+        ftdi_dev = haicu_ftdi.init(args.serial)
+    except:
+        print("Device '" + str(args.serial) + "' not found!")
+        print()
+        arg_list(args, None)
+        sys.exit(-1)
+
+    return ftdi_dev
+
 def main():
     prog='haicu_ctl'
     parser = argparse.ArgumentParser(prog=prog)
     parser.add_argument('--version', action='version', version='%(prog)s ' + str(VERSION))
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase logging verbosity, can be repeated')
     parser.add_argument('-l', '--log', metavar='file', help='Log to output file')
     parser.add_argument('-s', '--serial', type=str, default='', help='MLD1200 serial of device to connect')
@@ -162,38 +173,33 @@
     memtest_parser.set_defaults(func=arg_memtest)
 
     stop_parser = cmd_parser.add_parser("stop")
     stop_parser.set_defaults(func=arg_stop)
 
     args = parser.parse_args()
 
-    try:
-        ftdi_dev = haicu_ftdi.init(args.serial)
-    except:
-        print("Device '" + str(args.serial) + "' not found!")
-        print()
-        arg_list(args, None)
-        sys.exit(-1)
-
     if(args.command == None):
         parser.print_usage()
         sys.exit(0)
 
-    args.func(args, ftdi_dev)
+    args.func(args)
 
-def arg_list(args, ftdi_dev):
+def arg_list(args):
     print("Available devices:")
     result = haicu_ftdi.list_devices()
     for n, r in enumerate(result):
         print(str(n+1) + "\t" + str(r))
 
     if(len(result) == 0):
         print("No devices found")
 
-def arg_memtest(args, ftdi_dev):
+def arg_memtest(args):
+
+    ftdi_dev = get_mld1200(args)
+
     # Generate random data of 'tlen' length
     tlen = 1048576 # number of 32-bit words to transfer
     tlen_in_bytes = tlen * 4
     print("Test transfer size: " + str(tlen_in_bytes) + " bytes")
     test_data = []
     for n in range(0, tlen):
         test_data.append(random.randrange(100))
@@ -222,19 +228,22 @@
         if(result[n] != test_data[n]):
             print("Mismatch at " + str(n) + "\tExpected: " + str(test_data[n]) + " Result: " + str(result[n]))
             sys.exit(-1)
 
     print("Verification Successful")
 
 
-def arg_stop(args, ftdi_dev):
+def arg_stop(args):
+    ftdi_dev = get_mld1200(args)
     haicu_ftdi.write_register(ftdi_dev, 0, 0)
 
 ## Converts status values into human read-able format
-def arg_info(args, ftdi_dev):
+def arg_info(args):
+    ftdi_dev = get_mld1200(args)
+
     status_resp = haicu_ftdi.gather_status_registers(ftdi_dev)
     control_resp = haicu_ftdi.gather_control_registers(ftdi_dev)
 
     if(not args.json):
         print("Status:")
         print("\tFrontpanel Bits: 0x" + f"{(status_resp['fp_status']):02X}")
         print("\tProgram Load: " + str(status_resp['program_load']))
@@ -288,15 +297,17 @@
         print("\tInvert Frontpanel: 0x" + f"{(control_resp['invert_frontpanel']):02X}")
         print("\tInvert Left Address: 0x" + f"{(control_resp['invert_left_address']):03X}")
         print("\tInvert Right Address: 0x" + f"{(control_resp['invert_right_address']):03X}")
     else:
         print("{\"status\":" + dumps(status_resp) + ",\"control\":" + dumps(control_resp) + "}")
 
 ## Converts register values into human read-able format
-def arg_set(args, ftdi_dev):
+def arg_set(args):
+    ftdi_dev = get_mld1200(args)
+
     addr = args.regname
     if(addr == GET_REG_TABLE["trigger_invert"]):
         handle_set("trigger_invert", ftdi_dev, 2, 0x40000000, 30, args.data, args.json)
 
     if(addr == GET_REG_TABLE["trigger_delay"]):
         handle_set("trigger_delay", ftdi_dev, 2, 0x000000FF, 0, args.data, args.json)
 
@@ -379,15 +390,17 @@
             print("0x" + '{:02X}'.format(result)) if(not args.json) else print("{\"invert_frontpanel\": 0x" + '{:02X}'.format(result) + "}")
         else:
             value = int(args.data, 0) & 0xFF
             rmr_register(ftdi_dev, 8, 0xF0000000, 28, (value & 0xF0) >> 4)
             rmr_register(ftdi_dev, 8, 0x0000F000, 12, value & 0x0F)
 
 ## Low level status register read
-def arg_status(args, ftdi_dev):
+def arg_status(args):
+    ftdi_dev = get_mld1200(args)
+
     addr = int(args.addr, 0)
     val = haicu_ftdi.read_status(ftdi_dev, addr)
     if(not args.json):
         if(val != None):
             if(args.verbose > 0):
                 print("[" + "0x{:02x}".format(addr) + "] " + '0x{:08x}'.format(val) + " (" + str(val) + ")")
             else:
@@ -400,15 +413,17 @@
             print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": " + '{:d}'.format(val) + "}")
         else:
             print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": null}")
 
 
 ## Read/Write a register
 # if no data is passed 'read' is assumed
-def arg_reg(args, ftdi_dev):
+def arg_reg(args):
+    ftdi_dev = get_mld1200(args)
+
     addr = int(args.addr, 0)
     if(not args.data == None):
         haicu_ftdi.write_register(ftdi_dev, addr, int(args.data, 0))
     else:
         val = haicu_ftdi.read_register(ftdi_dev, addr)
         if(not args.json):
             if(val != None):
@@ -421,15 +436,17 @@
                 sys.exit(-1)
         else:
             if(val != None):
                 print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": " + '{:d}'.format(val) + "}")
             else:
                 print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": null}")
 
-def arg_mem(args, ftdi_dev):
+def arg_mem(args):
+    ftdi_dev = get_mld1200(args)
+
     addr = int(args.addr, 0)
     if(not args.data == None):
         haicu_ftdi.write_memory(ftdi_dev, addr, int(args.data, 0))
     else:
         val = haicu_ftdi.read_memory(ftdi_dev, addr, 1)
         if(not args.json):
             if(len(val) > 0):
@@ -442,15 +459,17 @@
                 sys.exit(-1)
         else:
             if(len(val) > 0):
                 print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": " + '{:d}'.format(val[0]) + "}")
             else:
                 print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": null}")
 
-def arg_block(args, ftdi_dev):
+def arg_block(args):
+    ftdi_dev = get_mld1200(args)
+
     addr = int(args.addr, 0)
     count = int(args.count, 0)
     response = haicu_ftdi.read_memory(ftdi_dev, addr, count)
     if(not args.json):
         if(len(response) > 0):
             for idx, val in enumerate(response):
                 if(args.verbose > 0):
@@ -469,15 +488,17 @@
                 else:
                     result_str = result_str + '{:d}'.format(val) + ","
             print(result_str)
         else:
             print("{\"address\": " + "{:d}".format(addr)  + ", \"value\": null}")
 
 
-def arg_upload(args, ftdi_dev):
+def arg_upload(args):
+    ftdi_dev = get_mld1200(args)
+
     if(not os.path.exists(args.file)):
         print("File " + args.file + " does not exist")
         sys.exit(-1)
 
     in_name, in_ext = os.path.splitext(args.file)
 
     try:
@@ -496,15 +517,15 @@
         else:
             print("File not found: " + args.file)
             sys.exit(-1)
 
     upload(ftdi_dev, rle, args.section, args.verbose)
 
 
-def arg_program(args, ftdi_dev):
+def arg_program(args):
     if(not os.path.exists(args.config_file)):
         if(args.verbose > 0):
             print("Config file " + args.config_file + " not found")
         sys.exit(-1)
 
     config = configparser.ConfigParser()
     config.read(args.config_file)
@@ -569,15 +590,15 @@
             if(args.verbose > 0):
                 print("No device specified for " + section_name + " section. Ignoring section in file")
 
         if(args.verbose > 0):
             print()
 
 
-def arg_convert(args, ftdi_dev):
+def arg_convert(args):
     if(args.verbose > 0):
         print("Converting " + args.infile + " to RLE")
 
     in_name, in_ext = os.path.splitext(args.infile)
     if(in_ext != ".txt"):
         print("Invalid extension, input file must be .txt")
         sys.exit(-1)
@@ -594,15 +615,15 @@
     if(args.verbose > 0):
         print("Creating RLE file " + args.outfile)
 
     with open(args.outfile, "wb+") as f:
         for n in range(len(rle)):
             f.write(rle[n])
 
-def arg_compare(args, ftdi_dev):
+def arg_compare(args):
     # Verification
     if(haicu_format.match(args.dfile, args.rfile)):
         if(args.verbose > 0):
             print("RLE and Derived files match")
     else:
         if(args.verbose > 0):
             print("RLE and Derived files do not match!")
```

### Comparing `haicu-0.9.2/haicu/format.py` & `haicu-0.9.3/haicu/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,205 +1,205 @@
 import struct
 from simplejson import dumps
 
 NUM_RUN_BITS = 13  # 13-bit maximum in run-length encoding 'run' field
 MAX_RUN_ALLOWED_RLE = pow(2, NUM_RUN_BITS)
 
 def convert_derived_absolute2rle(derived_file_name: str) -> list[list[bytearray]]:
-    """Convert absolute timing derived file to RLE format suitable for upload to device
+     """Convert absolute timing derived file to RLE format suitable for upload to device
 
-    Args:
-        derived_file_name(str): File to convert to RLE format
-
-    Returns:
-        A list containing each section found in derived file. Each section is given as an array of bytes
-
-    """
-    initial = []
-    final = []
-
-    with open(derived_file_name, 'r') as fp:
-        for num_lines, line in enumerate(fp):
-            pass
-    num_sections = int((num_lines) / 21)
-
-    for n in range(num_sections):
-        initial.append([])
-        final.append(bytearray())
-
-    with open(derived_file_name, "r") as f:
-
-        # 1 Timing, 8 Tune, 1 Address per MLD, two MLDs
-        for section in range(num_sections):
-            section_bitstream = bytearray()
-            section_word_count = 0
-
-            # First line is discarded
-            f.readline()
-            for n in range(20):
-                # 0 - Tunebox 1 Timing
-                # 1 - Tunebox 1 Value
-                # 2 - Tunebox 2 Timing
-                # 3 - Tunebox 2 Value
-                # 4 - Tunebox 3 Timing
-                # 5 - Tunebox 3 Value
-                # 6 - Tunebox 4 Timing
-                # 7 - Tunebox 4 Value
-                # 8 - Tunebox 5 Timing
-                # 9 - Tunebox 5 Value
-                # 10 - Tunebox 6 Timing
-                # 11 - Tunebox 6 Value
-                # 12 - Tunebox 7 Timing
-                # 13 - Tunebox 7 Value
-                # 14 - Tunebox 8 Timing
-                # 15 - Tunebox 8 Value
-                # 16 - Address timing
-                # 17 - Left
-                # 18 - Right
-                # 19 - Output bits?
-                initial[section].append(f.readline().strip().split())
-
-            tunebox_timing = []
-            tunebox_value = []
-            for n in range(8):
-                tunebox_timing.append(initial[section][n*2][0:-8])
-                tunebox_value.append(initial[section][(n*2)+1][0:-8])
-
-            # Convert
-            for n in range(len(tunebox_timing)):
-                for entry in tunebox_timing[n]:
-                    entry = int(entry)
-
-            address_timing = initial[section][16][0:-8]
-            address_left = initial[section][17][0:-8]
-            address_right = initial[section][18][0:-8]
-            address_front = initial[section][19][0:-8]
-
-            # Now we will run through in time, a given tunebox or address can get 'ahead' of this, if if when we parse it,
-            # it has a steady-state that extends beyond our current time, we'll catch up to it later...
-            current_time = 0
-            time_length = int(tunebox_timing[0][-1])
-            pos_time = [0, 0, 0, 0, 0, 0]
-            pos_index = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
-
-            while(current_time <= time_length):
-                for n in range(6):
-                    if(n < 4):
-                        pos_index1 = pos_index[(n * 2)]
-                        pos_index2 = pos_index[(n * 2)+1]
-
-                        if(pos_time[n] <= current_time):
-                            # Behind, so generate RLE word
-
-                            # TODO: Check here if we are done with this tunebox
-
-                            time_diff1 = MAX_RUN_ALLOWED_RLE if (time_diff1 > MAX_RUN_ALLOWED_RLE) else tunebox_timing[n][pos_index1] - pos_time[n]
-                            time_diff2 = MAX_RUN_ALLOWED_RLE if (time_diff2 > MAX_RUN_ALLOWED_RLE) else tunebox_timing[n][pos_index2] - pos_time[n]
-
-                            time_diff = time_diff1 if(time_diff1 < time_diff2) else time_diff2
-                            value1 = tunebox_value[n][pos_index1]
-                            value2 = tunebox_value[n][pos_index2]
-
-                            pos_and_time = ((n & 0x7) << 13) | (time_diff & 0x1FFF)
-                            value = (value1 << 16) | (value2)
-
-                            # Write word to bitstream
-                            section_bitstream.extend(struct.pack(">HH", pos_and_time, value))
-                            section_word_count = section_word_count + 1
-
-                            pos_time[n] = pos_time[n] + time_diff
-                            pos_index1 = pos_index1 + 1 if(pos_time[n] == tunebox_timing[n][pos_index1]) else pos_index1
-                            pos_index2 = pos_index2 + 1 if(pos_time[n] == tunebox_timing[n][pos_index2]) else pos_index2
-
-                            pos_index[(n * 2)] = pos_index1
-                            pos_index[(n * 2)+1] = pos_index2
-
-
-                # There is a better way to hop, but for now use this
-                current_time = current_time + 1
-
-
-    for section in range(num_sections):
-
-        # Technically its 8 tuneboxes, 1 address, but functionally it is the same for us here
-        rle = []
-        tunebox = []
-        for n in range(6):
-            rle.append([])
-
-
-
-
-    # Now we iterate thru using the 'time' in the first array position
-    for time_div in range(1, len(initial[section][0])):
-        time_jump = int(initial[section][0][time_div])
-        # For each Tune and Address line (9 lines total)
-        for n in range(6):
-            if(n<4):
-                pos_value = int(initial[section][1+(n*2)][time_div])
-                pos_value2 = int(initial[section][2+(n*2)][time_div])
-            elif(n==4):
-                pos_value = (int(initial[section][1+(n*2)][time_div]) & 0x0000_0FFF) | ((int(initial[section][1+(n*2)][time_div]) & 0x0F00_0000) >> 12)
-                pos_value2 = 0
-            elif(n==5):
-                pos_value = ((int(initial[section][1+((n-1)*2)][time_div]) & 0x00FF_F000) >> 12) | ((int(initial[section][1+((n-1)*2)][time_div]) & 0xF000_0000) >> 16)
-                pos_value2 = 0
-            else:
-                raise Exception
-            # Check if the value has changed for this position
-            # This means we will write out its length and old value to the file
-            # Then restart the 'run' count on the new value
-            # If a count is greater than MAX_RUN_ALLOWED_RLE, may have to write multiple times
-            if(tunebox[n][1] == pos_value) and (tunebox[n][2] == pos_value2):
-                tunebox[n][0] = tunebox[n][0] + time_jump
-            else:
-                # Value changed, dump previous value to rle array
-                rle[tunebox[n][3]] = (n, tunebox[n][0] - 1 ,tunebox[n][1], tunebox[n][2])
-                rle.append([])
-                # Update to new values
-                tunebox[n][0] = time_jump
-                tunebox[n][1] = pos_value
-                tunebox[n][2] = pos_value2
-                tunebox[n][3] = len(rle)-1
-        # Check to make sure no position will starve out before this time jump is over
-        # Iterate thru so in a long jump we don't fill one FIFO before starting on the next
-        check_overrun = True
-        while(check_overrun):
-            check_overrun = False
-            for n in range(6):
-                if(tunebox[n][0] > MAX_RUN_ALLOWED_RLE):
-                    rle[tunebox[n][3]] = (n, MAX_RUN_ALLOWED_RLE-1, tunebox[n][1], tunebox[n][2])
-                    rle.append([])
-                    tunebox[n][0] = tunebox[n][0] - MAX_RUN_ALLOWED_RLE
-                    tunebox[n][3] = len(rle)-1
-                    check_overrun = True
-        # Write any outstanding final
-        for n in range(6):
-            if(time_div == len(initial[section][0]) - 1):
-                rle[tunebox[n][3]] = (n, tunebox[n][0] - 1, tunebox[n][1], tunebox[n][2])
-
-        # Dump RLE to bitstream
-        final[section].extend(struct.pack(">I", len(rle)))
-        for pos in rle:
-            pos_and_time = ((pos[0] & 0x7) << 13) | (pos[1] & 0x1FFF)
+     Args:
+         derived_file_name(str): File to convert to RLE format
 
-            if(pos[0] == 4) or (pos[0] == 5):
-                value = pos[2] & 0xFFFF
-            else:
-                value = (pos[2] & 0xFF) << 8 | (pos[3] & 0xFF)
+     Returns:
+         A list containing each section found in derived file. Each section is given as an array of bytes
 
-            final[section].extend(struct.pack(">HH", pos_and_time, value))
+     """
+     initial = []
+     final = []
+
+     with open(derived_file_name, 'r') as fp:
+         for num_lines, line in enumerate(fp):
+             pass
+     num_sections = int((num_lines) / 21)
+
+     for n in range(num_sections):
+         initial.append([])
+         final.append(bytearray())
+
+     with open(derived_file_name, "r") as f:
+
+         # 1 Timing, 8 Tune, 1 Address per MLD, two MLDs
+         for section in range(num_sections):
+             section_bitstream = bytearray()
+             section_word_count = 0
+
+             # First line is discarded
+             f.readline()
+             for n in range(20):
+                 # 0 - Tunebox 1 Timing
+                 # 1 - Tunebox 1 Value
+                 # 2 - Tunebox 2 Timing
+                 # 3 - Tunebox 2 Value
+                 # 4 - Tunebox 3 Timing
+                 # 5 - Tunebox 3 Value
+                 # 6 - Tunebox 4 Timing
+                 # 7 - Tunebox 4 Value
+                 # 8 - Tunebox 5 Timing
+                 # 9 - Tunebox 5 Value
+                 # 10 - Tunebox 6 Timing
+                 # 11 - Tunebox 6 Value
+                 # 12 - Tunebox 7 Timing
+                 # 13 - Tunebox 7 Value
+                 # 14 - Tunebox 8 Timing
+                 # 15 - Tunebox 8 Value
+                 # 16 - Address timing
+                 # 17 - Left
+                 # 18 - Right
+                 # 19 - Output bits?
+                 initial[section].append(f.readline().strip().split())
+
+             tunebox_timing = []
+             tunebox_value = []
+             for n in range(8):
+                 tunebox_timing.append(initial[section][n*2][0:-8])
+                 tunebox_value.append(initial[section][(n*2)+1][0:-8])
+
+             # Convert
+             for n in range(len(tunebox_timing)):
+                 for entry in tunebox_timing[n]:
+                     entry = int(entry)
+
+             address_timing = initial[section][16][0:-8]
+             address_left = initial[section][17][0:-8]
+             address_right = initial[section][18][0:-8]
+             address_front = initial[section][19][0:-8]
+
+             # Now we will run through in time, a given tunebox or address can get 'ahead' of this, if if when we parse it,
+             # it has a steady-state that extends beyond our current time, we'll catch up to it later...
+             current_time = 0
+             time_length = int(tunebox_timing[0][-1])
+             pos_time = [0, 0, 0, 0, 0, 0]
+             pos_index = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
+
+             while(current_time <= time_length):
+                 for n in range(6):
+                     if(n < 4):
+                         pos_index1 = pos_index[(n * 2)]
+                         pos_index2 = pos_index[(n * 2)+1]
+
+                         if(pos_time[n] <= current_time):
+                             # Behind, so generate RLE word
+
+                             # TODO: Check here if we are done with this tunebox
+
+                             time_diff1 = MAX_RUN_ALLOWED_RLE if (time_diff1 > MAX_RUN_ALLOWED_RLE) else tunebox_timing[n][pos_index1] - pos_time[n]
+                             time_diff2 = MAX_RUN_ALLOWED_RLE if (time_diff2 > MAX_RUN_ALLOWED_RLE) else tunebox_timing[n][pos_index2] - pos_time[n]
+
+                             time_diff = time_diff1 if(time_diff1 < time_diff2) else time_diff2
+                             value1 = tunebox_value[n][pos_index1]
+                             value2 = tunebox_value[n][pos_index2]
+
+                             pos_and_time = ((n & 0x7) << 13) | (time_diff & 0x1FFF)
+                             value = (value1 << 16) | (value2)
+
+                             # Write word to bitstream
+                             section_bitstream.extend(struct.pack(">HH", pos_and_time, value))
+                             section_word_count = section_word_count + 1
+
+                             pos_time[n] = pos_time[n] + time_diff
+                             pos_index1 = pos_index1 + 1 if(pos_time[n] == tunebox_timing[n][pos_index1]) else pos_index1
+                             pos_index2 = pos_index2 + 1 if(pos_time[n] == tunebox_timing[n][pos_index2]) else pos_index2
+
+                             pos_index[(n * 2)] = pos_index1
+                             pos_index[(n * 2)+1] = pos_index2
+
+
+                 # There is a better way to hop, but for now use this
+                 current_time = current_time + 1
+
+
+     for section in range(num_sections):
+
+         # Technically its 8 tuneboxes, 1 address, but functionally it is the same for us here
+         rle = []
+         tunebox = []
+         for n in range(6):
+             rle.append([])
+
+
+
+
+     # Now we iterate thru using the 'time' in the first array position
+     for time_div in range(1, len(initial[section][0])):
+         time_jump = int(initial[section][0][time_div])
+         # For each Tune and Address line (9 lines total)
+         for n in range(6):
+             if(n<4):
+                 pos_value = int(initial[section][1+(n*2)][time_div])
+                 pos_value2 = int(initial[section][2+(n*2)][time_div])
+             elif(n==4):
+                 pos_value = (int(initial[section][1+(n*2)][time_div]) & 0x0000_0FFF) | ((int(initial[section][1+(n*2)][time_div]) & 0x0F00_0000) >> 12)
+                 pos_value2 = 0
+             elif(n==5):
+                 pos_value = ((int(initial[section][1+((n-1)*2)][time_div]) & 0x00FF_F000) >> 12) | ((int(initial[section][1+((n-1)*2)][time_div]) & 0xF000_0000) >> 16)
+                 pos_value2 = 0
+             else:
+                 raise Exception
+             # Check if the value has changed for this position
+             # This means we will write out its length and old value to the file
+             # Then restart the 'run' count on the new value
+             # If a count is greater than MAX_RUN_ALLOWED_RLE, may have to write multiple times
+             if(tunebox[n][1] == pos_value) and (tunebox[n][2] == pos_value2):
+                 tunebox[n][0] = tunebox[n][0] + time_jump
+             else:
+                 # Value changed, dump previous value to rle array
+                 rle[tunebox[n][3]] = (n, tunebox[n][0] - 1 ,tunebox[n][1], tunebox[n][2])
+                 rle.append([])
+                 # Update to new values
+                 tunebox[n][0] = time_jump
+                 tunebox[n][1] = pos_value
+                 tunebox[n][2] = pos_value2
+                 tunebox[n][3] = len(rle)-1
+         # Check to make sure no position will starve out before this time jump is over
+         # Iterate thru so in a long jump we don't fill one FIFO before starting on the next
+         check_overrun = True
+         while(check_overrun):
+             check_overrun = False
+             for n in range(6):
+                 if(tunebox[n][0] > MAX_RUN_ALLOWED_RLE):
+                     rle[tunebox[n][3]] = (n, MAX_RUN_ALLOWED_RLE-1, tunebox[n][1], tunebox[n][2])
+                     rle.append([])
+                     tunebox[n][0] = tunebox[n][0] - MAX_RUN_ALLOWED_RLE
+                     tunebox[n][3] = len(rle)-1
+                     check_overrun = True
+         # Write any outstanding final
+         for n in range(6):
+             if(time_div == len(initial[section][0]) - 1):
+                 rle[tunebox[n][3]] = (n, tunebox[n][0] - 1, tunebox[n][1], tunebox[n][2])
+
+         # Dump RLE to bitstream
+         final[section].extend(struct.pack(">I", len(rle)))
+         for pos in rle:
+             pos_and_time = ((pos[0] & 0x7) << 13) | (pos[1] & 0x1FFF)
+
+             if(pos[0] == 4) or (pos[0] == 5):
+                 value = pos[2] & 0xFFFF
+             else:
+                 value = (pos[2] & 0xFF) << 8 | (pos[3] & 0xFF)
+
+             final[section].extend(struct.pack(">HH", pos_and_time, value))
+
+         time_required = 0
+         for time_div in range(len(initial[section][0])):
+             time_required = time_required + int(initial[section][0][time_div])
 
-        time_required = 0
-        for time_div in range(len(initial[section][0])):
-            time_required = time_required + int(initial[section][0][time_div])
+         # print("Time required for section " + str(section) + ":" + str(time_required * 10) + "ns (" + str(time_required * 10 / 1000000) + "ms)")
 
-        # print("Time required for section " + str(section) + ":" + str(time_required * 10) + "ns (" + str(time_required * 10 / 1000000) + "ms)")
-
-    return final
+     return final
 
 def convert_derived2rle(derived_file_name: str) -> list[list[bytearray]]:
     """Convert derived file to RLE format suitable for upload to device
 
     Args:
         derived_file_name(str): File to convert to RLE format
 
@@ -237,49 +237,64 @@
             rle.append([])
 
             # Address line is... complicated, actually 12 bit Left Address, 12 bit Right Address, 8 bit diagnostic
             if(n<4):
                 init_val = int(initial[section][1+(n*2)][0])
                 init_val2 = int(initial[section][2+(n*2)][0])
             elif(n==4):
-                init_val =  (int(initial[section][1+(n*2)][0]) & 0x0000_0FFF) | ((int(initial[section][1+(n*2)][0]) & 0x0F00_0000) >> 12)
+                init_val = (int(initial[section][9][0]) & 0x0000_0FFF) | ((int(initial[section][9][0]) & 0x0F00_0000) >> 12)
                 init_val2 = 0
             elif(n==5):
-                init_val = ((int(initial[section][1+((n-1)*2)][0]) & 0x00FF_F000) >> 12) | ((int(initial[section][1+((n-1)*2)][0]) & 0xF000_0000) >> 16)
+                init_val = ((int(initial[section][9][0]) & 0x00FF_F000) >> 12) | ((int(initial[section][9][0]) & 0xF000_0000) >> 16)
                 init_val2 = 0
-            else:
-                raise Exception
 
             tunebox.append([int(initial[section][0][0]), init_val, init_val2, n])
 
+        # Check to make sure no position will starve out before this time jump is over
+        # Iterate thru so in a long jump we don't fill one FIFO before starting on the next
+        check_overrun = True
+        while(check_overrun):
+            check_overrun = False
+            for n in range(6):
+                if(tunebox[n][0] > MAX_RUN_ALLOWED_RLE):
+                    rle[tunebox[n][3]] = (n, MAX_RUN_ALLOWED_RLE-1, tunebox[n][1], tunebox[n][2])
+                    rle.append([])
+                    tunebox[n][0] = tunebox[n][0] - MAX_RUN_ALLOWED_RLE
+                    tunebox[n][3] = len(rle)-1
+                    check_overrun = True
+
         # Now we iterate thru using the 'time' in the first array position
         for time_div in range(1, len(initial[section][0])):
             time_jump = int(initial[section][0][time_div])
 
             # For each Tune and Address line (9 lines total)
             for n in range(6):
 
                 if(n<4):
                     pos_value = int(initial[section][1+(n*2)][time_div])
                     pos_value2 = int(initial[section][2+(n*2)][time_div])
                 elif(n==4):
-                    pos_value = (int(initial[section][1+(n*2)][time_div]) & 0x0000_0FFF) | ((int(initial[section][1+(n*2)][time_div]) & 0x0F00_0000) >> 12)
+                    pos_value = (int(initial[section][9][time_div]) & 0x0000_0FFF) | ((int(initial[section][9][time_div]) & 0x0F00_0000) >> 12)
                     pos_value2 = 0
                 elif(n==5):
-                    pos_value = ((int(initial[section][1+((n-1)*2)][time_div]) & 0x00FF_F000) >> 12) | ((int(initial[section][1+((n-1)*2)][time_div]) & 0xF000_0000) >> 16)
+                    pos_value = ((int(initial[section][9][time_div]) & 0x00FF_F000) >> 12) | ((int(initial[section][9][time_div]) & 0xF000_0000) >> 16)
                     pos_value2 = 0
-                else:
-                    raise Exception
 
                 # Check if the value has changed for this position
                 # This means we will write out its length and old value to the file
                 # Then restart the 'run' count on the new value
                 # If a count is greater than MAX_RUN_ALLOWED_RLE, may have to write multiple times
                 if(tunebox[n][1] == pos_value) and (tunebox[n][2] == pos_value2):
                     tunebox[n][0] = tunebox[n][0] + time_jump
+
+                    if(tunebox[n][0] > MAX_RUN_ALLOWED_RLE):
+                        rle[tunebox[n][3]] = (n, MAX_RUN_ALLOWED_RLE-1, tunebox[n][1], tunebox[n][2])
+                        rle.append([])
+                        tunebox[n][0] = tunebox[n][0] - MAX_RUN_ALLOWED_RLE
+                        tunebox[n][3] = len(rle)-1
                 else:
                     # Value changed, dump previous value to rle array
                     rle[tunebox[n][3]] = (n, tunebox[n][0] - 1 ,tunebox[n][1], tunebox[n][2])
                     rle.append([])
 
                     # Update to new values
                     tunebox[n][0] = time_jump
@@ -296,31 +311,31 @@
                     if(tunebox[n][0] > MAX_RUN_ALLOWED_RLE):
                         rle[tunebox[n][3]] = (n, MAX_RUN_ALLOWED_RLE-1, tunebox[n][1], tunebox[n][2])
                         rle.append([])
                         tunebox[n][0] = tunebox[n][0] - MAX_RUN_ALLOWED_RLE
                         tunebox[n][3] = len(rle)-1
                         check_overrun = True
 
-            # Write any outstanding final
-            for n in range(6):
-                if(time_div == len(initial[section][0]) - 1):
-                    rle[tunebox[n][3]] = (n, tunebox[n][0] - 1, tunebox[n][1], tunebox[n][2])
-
+        # Write any outstanding final
+        for n in range(6):
+            # if(time_div == len(initial[section][0]) - 1):
+            if(tunebox[n][0] > 0):
+                rle[tunebox[n][3]] = (n, tunebox[n][0] - 1, tunebox[n][1], tunebox[n][2])
 
+        # pprint.pprint(rle)
         # Generate bitstream for each section
         final[section].extend(struct.pack(">I", len(rle)))
         for pos in rle:
             pos_and_time = ((pos[0] & 0x7) << 13) | (pos[1] & 0x1FFF)
 
             if(pos[0] == 4) or (pos[0] == 5):
                 value = pos[2] & 0xFFFF
             else:
                 value = (pos[3] & 0xFF) << 8 | (pos[2] & 0xFF)
 
-            #f.write(struct.pack(">HH", pos_and_time, value))
             final[section].extend(struct.pack(">HH", pos_and_time, value))
 
         time_required = 0
         for time_div in range(len(initial[section][0])):
             time_required = time_required + int(initial[section][0][time_div])
 
         # print("Time required for section " + str(section) + ":" + str(time_required * 10) + "ns (" + str(time_required * 10 / 1000000) + "ms)")
@@ -328,15 +343,14 @@
         # byte_count = 0
         # num_entries = len(rle)
         # byte_count = len(rle) * 4
 
         # print("Total entries: " + str(num_entries))
         # print(str(byte_count) + " bytes required (" + str(byte_count*8) + " bits)")
         # print()
-        # final[section] = rle
 
     return final
 
 
 
 def convert_rle2raw(rle_file_name: str) -> list[list[int]]:
     """Convert RLE file to raw format. Typical use for allowing comparisons between different formats
@@ -345,24 +359,25 @@
         rle_file_name(str): File to convert to 'raw' format
 
     Returns:
         List containing each section, inside of which is an array of the 8 tuneboxes, and the address (Left + Right + Front Panel)
 
     """
 
-    final = [[],[]]
-    for n in range(10):
-        final[0].append([])
-        final[1].append([])
-
     byte_offset = 0
     section = 0
+    final = []
     with open(rle_file_name, "rb") as f:
+
         data = f.read()
         while(byte_offset < len(data)):
+            final.append([])
+            for n in range(10):
+                final[section].append([])
+
             entries = struct.unpack_from(">I", data, byte_offset)[0]
 
             for n in range(entries):
                 pos_time, value = struct.unpack_from(">HH", data, byte_offset + 4 + (n*4))
                 pos = pos_time >> 13
                 time = pos_time & 0x1FFF
                 for t in range(time+1):
@@ -377,48 +392,49 @@
                     except Exception as e:
                         print(e)
 
             byte_offset = byte_offset + 4 + (entries * 4)
 
             #for n in range(len(final[section])):
             #    print("Total entries in section " + str(section) + ": " + str(n) + ": " + str(len(final[section][n])))
-                # val = 0
-                # for i in range(len(final[section][n])):
-                #     val = val + final[section][n][i]
-                # print("Sum per line: " + str(val))
+            #    val = 0
+            #    for i in range(len(final[section][n])):
+            #        val = val + final[section][n][i]
+            #    print("Sum per line: " + str(val))
 
-            # print()
+            #print()
             section = section + 1
 
     return final
 
 def convert_derived2raw(derived_file_name: str) -> list[list[int]]:
     """Convert derived file to raw format. Typical use for allowing comparisons between different formats
 
     Args:
         derived_file_name(str): File to convert to 'raw' format
 
     Returns:
         List containing each section, inside of which is an array of the 8 tuneboxes, and the address (Left + Right + Front Panel)
 
     """
-    initial = [[],[]]
+    initial = []
     final = []
 
     with open(derived_file_name, 'r') as fp:
         for num_lines, line in enumerate(fp):
             pass
     num_sections = int((num_lines) / 10)
 
     with open(derived_file_name, "r") as f:
         # First line is discarded
         f.readline()
 
         # 8 Tune, 1 Address per MLD, two MLDs
         for section in range(num_sections):
+            initial.append([])
             final.append([])
             for n in range(10):
                 initial[section].append(f.readline().split())
 
             for n in range(10):
                 final[section].append([])
 
@@ -440,21 +456,21 @@
                 else:
                     value = pos_value & 0xFF
                     for j in range(time_jump):
                         final[section][n].append(value)
 
 
         #for n in range(len(final[section])):
-        #    print("Total entries in section " + str(section) ": " + str(n) + ": " + str(len(final[section][n])))
-            # val = 0
-            # for i in range(len(final[section][n])):
-            #     val = val + final[section][n][i]
-            # print("Sum per line: " + str(val))
+        #    print("Total entries in section " + str(section) + ": " + str(n) + ": " + str(len(final[section][n])))
+        #    val = 0
+        #    for i in range(len(final[section][n])):
+        #        val = val + final[section][n][i]
+        #    print("Sum per line: " + str(val))
 
-        # print()
+        #print()
 
     return final
 
 def load_rle_from_file(rle_file_name: str) -> list[list[int]]:
     """Load an RLE file from disk into memory. Each section is loaded as an array of 32-bit integer values
 
     Args:
```

### Comparing `haicu-0.9.2/haicu/ftdi.py` & `haicu-0.9.3/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.9.2/haicu.egg-info/PKG-INFO` & `haicu-0.9.3/haicu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.9.2
+Version: 0.9.3
 Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.9.2/pyproject.toml` & `haicu-0.9.3/pyproject.toml`

 * *Files identical despite different names*

