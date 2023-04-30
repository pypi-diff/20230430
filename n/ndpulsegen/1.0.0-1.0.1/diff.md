# Comparing `tmp/ndpulsegen-1.0.0.tar.gz` & `tmp/ndpulsegen-1.0.1.tar.gz`

## Comparing `ndpulsegen-1.0.0.tar` & `ndpulsegen-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/.DS_Store
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/examples/example_simple.py
--rw-r--r--   0        0        0    28914 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/examples/examples.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/.DS_Store
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/__init__.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/comms.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/compiler.py
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/console_read.py
--rw-r--r--   0        0        0    52437 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/src/ndpulsegen/transcode.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/hardware_validation.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/quick_check_with_scope.py
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/rigol_ds1202z_e.py
--rw-r--r--   0        0        0    15445 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/run_plotter.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/stuff.py
--rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/tests/testing.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/README.md
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ndpulsegen-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/.DS_Store
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/docs/building_process.txt
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/examples/example_simple.py
+-rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/examples/examples.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/.DS_Store
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/__init__.py
+-rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/comms.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/compiler.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/console_read.py
+-rw-r--r--   0        0        0    52419 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/src/ndpulsegen/transcode.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/hardware_validation.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/quick_check_with_scope.py
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/rigol_ds1202z_e.py
+-rw-r--r--   0        0        0    15445 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/run_plotter.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/stuff.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/testing.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/trigger_latency_multiboard/dual_clock_and_trigger_or_enable.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/trigger_latency_multiboard/hardware_enabled_1.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/tests/trigger_latency_multiboard/hardware_enabled_2.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/LICENSE
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/README.md
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ndpulsegen-1.0.1/PKG-INFO
```

### Comparing `ndpulsegen-1.0.0/.DS_Store` & `ndpulsegen-1.0.1/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
-00000050: 0000 0001 0000 1000 0070 006c 0065 0073  .........p.l.e.s
-00000060: 6c67 3153 0000 0000 0000 0000 0000 0000  lg1S............
+00000040: 0000 0000 0000 0002 0000 0000 0000 000d  ................
+00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
+00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,41 +26,41 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0009 0000 0008  ................
-00000210: 0065 0078 0061 006d 0070 006c 0065 0073  .e.x.a.m.p.l.e.s
-00000220: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
-00000230: 0000 0008 0065 0078 0061 006d 0070 006c  .....e.x.a.m.p.l
-00000240: 0065 0073 6d6f 4444 626c 6f62 0000 0008  .e.smoDDblob....
-00000250: 1fe7 be94 d1bb c441 0000 0008 0065 0078  .......A.....e.x
-00000260: 0061 006d 0070 006c 0065 0073 6d6f 6444  .a.m.p.l.e.smodD
-00000270: 626c 6f62 0000 0008 1fe7 be94 d1bb c441  blob...........A
-00000280: 0000 0008 0065 0078 0061 006d 0070 006c  .....e.x.a.m.p.l
-00000290: 0065 0073 7068 3153 636f 6d70 0000 0000  .e.sph1Scomp....
-000002a0: 0000 0000 0000 0003 0073 0072 0063 6c67  .........s.r.clg
-000002b0: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
-000002c0: 0003 0073 0072 0063 6d6f 4444 626c 6f62  ...s.r.cmoDDblob
-000002d0: 0000 0008 8283 931d d1bb c441 0000 0003  ...........A....
-000002e0: 0073 0072 0063 6d6f 6444 626c 6f62 0000  .s.r.cmodDblob..
-000002f0: 0008 8283 931d d1bb c441 0000 0003 0073  .........A.....s
-00000300: 0072 0063 7068 3153 636f 6d70 0000 0000  .r.cph1Scomp....
-00000310: 0000 0000 0000 0005 0074 0065 0073 0074  .........t.e.s.t
-00000320: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 000d 0000 0004  ................
+00000210: 0064 006f 0063 0073 6c67 3153 636f 6d70  .d.o.c.slg1Scomp
+00000220: 0000 0000 0000 0000 0000 0004 0064 006f  .............d.o
+00000230: 0063 0073 6d6f 4444 626c 6f62 0000 0008  .c.smoDDblob....
+00000240: 60c9 240c e2bb c441 0000 0004 0064 006f  `.$....A.....d.o
+00000250: 0063 0073 6d6f 6444 626c 6f62 0000 0008  .c.smodDblob....
+00000260: 60c9 240c e2bb c441 0000 0004 0064 006f  `.$....A.....d.o
+00000270: 0063 0073 7068 3153 636f 6d70 0000 0000  .c.sph1Scomp....
+00000280: 0000 0000 0000 0008 0065 0078 0061 006d  .........e.x.a.m
+00000290: 0070 006c 0065 0073 6c67 3153 636f 6d70  .p.l.e.slg1Scomp
+000002a0: 0000 0000 0000 0000 0000 0008 0065 0078  .............e.x
+000002b0: 0061 006d 0070 006c 0065 0073 6d6f 4444  .a.m.p.l.e.smoDD
+000002c0: 626c 6f62 0000 0008 1fe7 be94 d1bb c441  blob...........A
+000002d0: 0000 0008 0065 0078 0061 006d 0070 006c  .....e.x.a.m.p.l
+000002e0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
+000002f0: 1fe7 be94 d1bb c441 0000 0008 0065 0078  .......A.....e.x
+00000300: 0061 006d 0070 006c 0065 0073 7068 3153  .a.m.p.l.e.sph1S
+00000310: 636f 6d70 0000 0000 0000 0000 0000 0003  comp............
+00000320: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
+00000330: 0000 0000 0000 0000 0003 0073 0072 0063  ...........s.r.c
+00000340: 6d6f 4444 626c 6f62 0000 0008 8283 931d  moDDblob........
+00000350: d1bb c441 0000 0003 0073 0072 0063 6d6f  ...A.....s.r.cmo
+00000360: 6444 626c 6f62 0000 0008 8283 931d d1bb  dDblob..........
+00000370: c441 0000 0003 0073 0072 0063 7068 3153  .A.....s.r.cph1S
+00000380: 636f 6d70 0000 0000 0000 0000 0000 0005  comp............
+00000390: 0074 0065 0073 0074 0073 7653 726e 6c6f  .t.e.s.t.svSrnlo
+000003a0: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `ndpulsegen-1.0.0/examples/example_simple.py` & `ndpulsegen-1.0.1/examples/example_simple.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/examples/examples.py` & `ndpulsegen-1.0.1/examples/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,19 +424,20 @@
     instr3 =  ndpulsegen.encode_instruction(3, 3, [0, 0, 0])
     instructions = [instr0, instr1, instr2, instr3]
     pg.write_instructions(instructions)
 
     pg.write_device_options(final_ram_address=3, run_mode='single', trigger_source='software', trigger_out_length=1, trigger_out_delay=0, notify_on_main_trig_out=False, notify_when_run_finished=False, software_run_enable=True)
     pg.write_action(trigger_now=True)
 
+    [print(key,':',value) for key, value in pg.get_state().items()]
 
 #Make program run now...
 if __name__ == "__main__":
     pg = ndpulsegen.PulseGenerator()
-    # print(pg.get_connected_devices())
+    print(pg.get_connected_devices())
     # pg.connect(serial_number=12582914)
     pg.connect()
     '''These give an introduction on how to program the device, and what capabilities it has'''
 
     # quick_test(pg)
 
     software_trig(pg)
```

### Comparing `ndpulsegen-1.0.0/src/.DS_Store` & `ndpulsegen-1.0.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/src/ndpulsegen/.DS_Store` & `ndpulsegen-1.0.1/src/ndpulsegen/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/src/ndpulsegen/comms.py` & `ndpulsegen-1.0.1/src/ndpulsegen/comms.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,25 +53,26 @@
                 raise Exception(ex)
 
     def get_connected_devices(self):
         # This attmpts to connect to all serial devices with valid parameters, and if it is a valid Narwhal Device, it adds them to a list and disconnects
         valid_ports = []
         comports = list(serial.tools.list_ports.comports())
         for comport in comports:
-            # print(com
+            print(comport)
             if 'vid' in vars(comport) and 'pid' in vars(comport):
                 if vars(comport)['vid'] == 1027 and vars(comport)['pid'] == 24592:
                     valid_ports.append(comport)
         # For every valid port, ask for an echo (which also sends serial number etc.) and store the info
         validated_devices = []
         unvalidated_devices = []
         for comport in valid_ports:
             self.ser.port = comport.device
             try:
                 self.ser.open()
+                # print(f'open comport {comport.device}')
             except Exception as ex: # Poor practice? Catch only the exception that happens when you can open a port...?
                 unvalidated_devices.append(comport.device)
                 # print(ex)
                 continue
             self.ser.reset_input_buffer()
             self.ser.reset_output_buffer()
             self.serial_read_thread = threading.Thread(target=self.monitor_serial, daemon=True)
@@ -100,33 +101,35 @@
             try:
                 byte_message_identifier = self.ser.read(1)
             except serial.serialutil.SerialException as ex:
                 self.close_readthread_event.set()
                 break
             # Normally the read will timeout and return empty, but if it returns someting try to read the reminder of the message
             if byte_message_identifier:
+                timestamp = time.time()
                 message_identifier, = struct.unpack('B', byte_message_identifier)
                 # Only read more bytes if the identifier is valid
                 if message_identifier not in transcode.msgin_decodeinfo.keys():
-                    self.msgin_queues['bytes_dropped'].put(message_identifier)
+                    self.msgin_queues['bytes_dropped'].put({'message_identifier':message_identifier, 'message':None, 'timestamp':timestamp})
                 else:
                     decodeinfo = transcode.msgin_decodeinfo[message_identifier]
                     message_length = decodeinfo['message_length'] - 1
                     try:
                         byte_message = self.ser.read(message_length)
                     except serial.serialutil.SerialException as ex:
                         self.close_readthread_event.set()
                         break   
                     # A random byte still a chance of being valid, so the read could timeout without reading a whole message worth of bytes
                     if len(byte_message) != message_length:
-                        self.msgin_queues['bytes_dropped'].put(message_identifier)
+                        self.msgin_queues['bytes_dropped'].put({'message_identifier':message_identifier, 'message':None, 'timestamp':timestamp})
                     else:
                         # At this point, just decode the message and put it in the queue corresponding to its type.
                         decode_function = decodeinfo['decode_function']
                         message = decode_function(byte_message)
+                        message['timestamp'] = timestamp
                         queue_name = decodeinfo['message_type']
                         self.msgin_queues[queue_name].put(message)
 
     def disconnect(self):
         self.close_readthread_event.set()
         self.serial_read_thread.join()
         self.close_readthread_event.clear()
```

### Comparing `ndpulsegen-1.0.0/src/ndpulsegen/console_read.py` & `ndpulsegen-1.0.1/src/ndpulsegen/console_read.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/src/ndpulsegen/transcode.py` & `ndpulsegen-1.0.1/src/ndpulsegen/transcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     trigger_source =            decode_lookup['trigger_source'][trigger_source_tag]
     notify_on_main_trig_out =   decode_lookup['notify_on_main_trig_out'][notify_on_main_trig_out_tag]
     clock_source =              decode_lookup['clock_source'][clock_source_tag]
     running =                   decode_lookup['running'][running_tag]
     software_run_enable =       decode_lookup['software_run_enable'][software_run_enable_tag]
     hardware_run_enable =       decode_lookup['hardware_run_enable'][hardware_run_enable_tag]
     notify_on_run_finished =    decode_lookup['notify_on_run_finished'][notify_on_run_finished_tag]
-    return {'state':state, 'final_ram_address':final_ram_address, 'trigger_out_delay':trigger_out_delay, 'run_mode':run_mode, 'trigger_source':trigger_source, 'notify_on_main_trig_out':notify_on_main_trig_out, 'notify_on_run_finished':notify_on_run_finished, 'trigger_out_length':trigger_out_length, 'clock_source':clock_source, 'running':running, 'software_run_enable':software_run_enable, 'hardware_run_enable':hardware_run_enable, 'current_address_approx':current_ram_address}
+    return {'state':state, 'final_ram_address':final_ram_address, 'trigger_out_delay':trigger_out_delay, 'run_mode':run_mode, 'trigger_source':trigger_source, 'notify_on_main_trig_out':notify_on_main_trig_out, 'notify_on_run_finished':notify_on_run_finished, 'trigger_out_length':trigger_out_length, 'clock_source':clock_source, 'running':running, 'software_run_enable':software_run_enable, 'hardware_run_enable':hardware_run_enable, 'current_address':current_ram_address}
 
 def decode_powerlinestate(message):
     ''' 
     Decodes the powerlinestate type message which contains information about 
     global powerline triggering settings, and information about the current
     powerline period.
 
@@ -487,15 +487,15 @@
         'finished_notify':True, and the 'address' field will be equal to the
         address of the final instruction. If `run_mode`='continuous', only a
         single notification is sent after the completion of the last run (which
         is induced by sending a command generated with the `encode_action' 
         function with argument `disable_after_current_run`=True).
     software_run_enable: bool, optional
         If False, and a run is in progress the timer in the run is immediately
-        paused, and all channels maintain their current output the output. The
+        paused, and all channels maintain their current output. The
         timer immediately resumes when `software_run_enable`=True. If False, and
         a run is not in progress, the run will be prevented from starting until
         `software_run_enable`=True. Triggers are ignored while
         `software_run_enable`=False.
 
     Returns
     -------
```

### Comparing `ndpulsegen-1.0.0/tests/.DS_Store` & `ndpulsegen-1.0.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/tests/hardware_validation.py` & `ndpulsegen-1.0.1/tests/hardware_validation.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/tests/quick_check_with_scope.py` & `ndpulsegen-1.0.1/tests/quick_check_with_scope.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/tests/rigol_ds1202z_e.py` & `ndpulsegen-1.0.1/tests/rigol_ds1202z_e.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/tests/run_plotter.py` & `ndpulsegen-1.0.1/tests/run_plotter.py`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/tests/testing.py` & `ndpulsegen-1.0.1/tests/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import struct
 import time
 
 import sys
 import os
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+from pathlib import Path
+current_file_path = Path(__file__).resolve()
+sys.path.insert(0, str(current_file_path.parent.parent / 'src'))
 import ndpulsegen
 
 
 def echo_terminal_characters(pg):
     print('Echoing terminal. Press \'Esc\' to stop.')
     kb = ndpulsegen.console_read.KBHit()
     while True:
@@ -25,38 +27,38 @@
     kb.set_normal_term()
 
 def cause_invalid_receive(pg):
     '''This function deliberatly sends a message with an invalid message identifier
     to test that the FPGA is dealing with the error correctly'''
     message_identifier = struct.pack('B', 15)
     pg.write_command(message_identifier)
-    pg.read_all_messages(timeout=0.5)
+    print(pg.read_all_messages(timeout=0.5))
 
 def cause_timeout_on_receive(pg):
     '''This function deliberatly sends a message that is incomplete'''
     message_identifier = struct.pack('B', 153)
     pg.write_command(message_identifier)
     pg.write_command(struct.pack('B', 1))
     pg.write_command(struct.pack('B', 2))
-    pg.read_all_messages(timeout=0.5)
+    print(pg.read_all_messages(timeout=0.5))
 
 def cause_timeout_on_message_forward(pg):
     '''This demonstrates a limitation of the instruction loading process on the FPGA. If a run is actually running,
     and that run contains ONLY instructions that last a SINGLE cycle, then there is never a 'gap' in the updating of
     old instructions to load a new instruction in there. This is unlikely to happen in practise, but it came up once.'''
     #address, duration, state, goto_address=0, goto_counter=0, stop_and_wait=False, hardware_trig_out=False, notify_computer=False, powerline_sync=False
     instr0 = ndpulsegen.transcode.encode_instruction(0, 1, 0b11111111)
     instr1 = ndpulsegen.transcode.encode_instruction(1, 1, 0b10101010)
     instructions = [instr0, instr1]
     pg.write_instructions(instructions)
     pg.write_device_options(final_ram_address=1, run_mode='continuous', trigger_source='software', trigger_out_length=1, trigger_out_delay=0, notify_on_main_trig_out=False, notify_when_run_finished=False, software_run_enable=True)
     pg.write_action(trigger_now=True)
 
     pg.write_instructions(instructions)
-    pg.read_all_messages(timeout=0.5)
+    print(pg.read_all_messages(timeout=0.5))
     time.sleep(1)
     pg.write_action(disable_after_current_run=True)
 
 
 
 def fully_load_ram_test(pg):
     # address, duration, state, goto_address=0, goto_counter=0, stop_and_wait=False, hardware_trig_out=False, notify_computer=False, powerline_sync=False
@@ -70,15 +72,15 @@
     tend = time.time()
 
     time_total = tend-tstart
     print('Time required to load the RAM FULL of instructions = {:.2f} ms \nWhich is {:.2f} instructions/ms \nOr {:.2f} μs/instruction '.format(time_total*1E3, (ram_address+1)/(time_total*1E3), (time_total*1E6)/(ram_address+1)))
 
     pg.write_device_options(final_ram_address=ram_address+1, run_mode='single', trigger_source='software', trigger_out_length=1, trigger_out_delay=0, notify_on_main_trig_out=False, notify_when_run_finished=False, software_run_enable=True)
     pg.write_action(trigger_now=True)
-    pg.read_all_messages(timeout=1)
+    print(pg.read_all_messages(timeout=1))
 
 
 
 def test_notifications(pg):
     # address, duration, state, goto_address=0, goto_counter=0, stop_and_wait=False, hardware_trig_out=False, notify_computer=False, powerline_sync=False
     # address, state, countdown, loopto_address, loops, stop_and_wait_tag, hard_trig_out_tag, notify_computer_tag
     # pg.write_action(reset_output_coordinator=True)
@@ -89,15 +91,15 @@
     for ram_address in range(0, instruction_number):
         instructions.append(ndpulsegen.transcode.encode_instruction(ram_address, 1, [1, 1, 1], notify_computer=True))
     pg.write_instructions(instructions)
 
     pg.write_device_options(final_ram_address=instruction_number-1, run_mode='single', trigger_source='software', trigger_out_length=255, trigger_out_delay=0, notify_on_main_trig_out=False, notify_when_run_finished=True, software_run_enable=True)
 
     pg.write_action(trigger_now=True)
-    pg.read_all_messages(timeout=2)
+    print(pg.read_all_messages(timeout=2))
 
 
 def pcb_connection_check(pg):
      #address, duration, state, goto_address=0, goto_counter=0, stop_and_wait=False, hardware_trig_out=False, notify_computer=False, powerline_sync=False
     states = []
     state = np.ones(24)
     for idx in range(1, 25):
@@ -127,15 +129,15 @@
     print('Press \'Esc\' to stop.')
     while True:
         if kb.kbhit():
             input_character = kb.getch()
             if input_character.encode() == chr(27).encode():
                 break
     pg.write_action(disable_after_current_run=True)
-    pg.read_all_messages(timeout=0.5)
+    print(pg.read_all_messages(timeout=0.5))
 
 
 def print_bytes(bytemessage):
     print('Message:')
     for letter in bytemessage[::-1]:
         print('{:08b}'.format(letter), end =" ")
     print('')
@@ -175,28 +177,28 @@
 '''
 
 
 
 if __name__ == "__main__":
 
     usb_port ='COM6'
-    # # usb_port ='tty.usbserial-FT3KRFFN0'
     pg = ndpulsegen.PulseGenerator()
+    print(pg.get_connected_devices())
     pg.connect()
 
 
 
     # echo_terminal_characters(pg)
     # cause_invalid_receive(pg)
     # cause_timeout_on_receive(pg)
     # cause_timeout_on_message_forward(pg)
     # fully_load_ram_test(pg)                  
     # test_notifications(pg)
-    pcb_connection_check(pg)
-    # current_address_problem(pg)
+    # pcb_connection_check(pg)
+    current_address_problem(pg)
 
 
     # instruction = ndpulsegen.transcode.encode_instruction(address=1234, duration=5678, state=[0, 1, 0, 1], goto_address=69, goto_counter=13, stop_and_wait=False, hardware_trig_out=False, notify_computer=False, powerline_sync=False)
     # print_bytes(instruction)
 
 
 '''
```

### Comparing `ndpulsegen-1.0.0/LICENSE` & `ndpulsegen-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndpulsegen-1.0.0/pyproject.toml` & `ndpulsegen-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ndpulsegen"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Rory Speirs", email="rory@narwhaldevices.com" },
 ]
 description = "A package to interface with the Narwhal Devices Pulse Generator"
 readme = "README.md"
-requires-python = ">=3.1"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
```

### Comparing `ndpulsegen-1.0.0/PKG-INFO` & `ndpulsegen-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ndpulsegen
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to interface with the Narwhal Devices Pulse Generator
 Project-URL: Homepage, https://github.com/RorySpeirs/narwhaldevs-pulsegen
 Project-URL: Device manufacturer, https://www.narwhaldevices.com
 Author-email: Rory Speirs <rory@narwhaldevices.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.1
+Requires-Python: >=3.7
 Requires-Dist: numpy
 Requires-Dist: pyserial
 Description-Content-Type: text/markdown
 
 # ndpulsegen
 The computer based software to communicate with the Narwhal Devices Pulse Generator
```

