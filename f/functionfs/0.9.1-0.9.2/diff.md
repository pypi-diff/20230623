# Comparing `tmp/functionfs-0.9.1.tar.gz` & `tmp/functionfs-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionfs-0.9.1.tar", last modified: Wed Nov 23 23:58:32 2022, max compression
+gzip compressed data, was "functionfs-0.9.2.tar", last modified: Fri Jun 23 12:22:05 2023, max compression
```

## Comparing `functionfs-0.9.1.tar` & `functionfs-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-11-23 23:58:32.563208 functionfs-0.9.1/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    35147 2007-07-01 22:55:35.000000 functionfs-0.9.1/COPYING
--rw-r--r--   0 vincent   (1000) vincent   (1000)       53 2020-12-02 14:42:59.000000 functionfs-0.9.1/MANIFEST.in
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1368 2022-11-23 23:58:32.563208 functionfs-0.9.1/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)      521 2020-12-02 14:42:59.000000 functionfs-0.9.1/README.rst
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-11-23 23:58:32.563208 functionfs-0.9.1/functionfs/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    61901 2022-11-23 23:45:56.000000 functionfs-0.9.1/functionfs/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      497 2022-11-23 23:58:32.563208 functionfs-0.9.1/functionfs/_version.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    15498 2021-09-10 23:50:55.000000 functionfs-0.9.1/functionfs/ch9.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2156 2021-10-02 00:46:35.000000 functionfs-0.9.1/functionfs/common.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    11463 2021-09-10 23:50:55.000000 functionfs-0.9.1/functionfs/functionfs.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    33775 2022-11-23 23:50:57.000000 functionfs-0.9.1/functionfs/gadget.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2754 2021-09-10 23:50:55.000000 functionfs-0.9.1/functionfs/hid.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-11-23 23:58:32.563208 functionfs-0.9.1/functionfs/tests/
--rw-r--r--   0 vincent   (1000) vincent   (1000)        0 2017-01-05 22:22:54.000000 functionfs-0.9.1/functionfs/tests/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      837 2021-12-21 12:54:31.000000 functionfs-0.9.1/functionfs/tests/common.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     9649 2021-12-22 00:51:15.000000 functionfs-0.9.1/functionfs/tests/device.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     5082 2021-12-22 00:51:15.000000 functionfs-0.9.1/functionfs/tests/host.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-11-23 23:58:32.563208 functionfs-0.9.1/functionfs.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1368 2022-11-23 23:58:32.000000 functionfs-0.9.1/functionfs.egg-info/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)      489 2022-11-23 23:58:32.000000 functionfs-0.9.1/functionfs.egg-info/SOURCES.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2022-11-23 23:58:32.000000 functionfs-0.9.1/functionfs.egg-info/dependency_links.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       17 2022-11-23 23:58:32.000000 functionfs-0.9.1/functionfs.egg-info/requires.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       11 2022-11-23 23:58:32.000000 functionfs-0.9.1/functionfs.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)      209 2022-11-23 23:58:32.563208 functionfs-0.9.1/setup.cfg
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2140 2022-11-23 23:55:51.000000 functionfs-0.9.1/setup.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    80044 2021-12-01 12:14:20.000000 functionfs-0.9.1/versioneer.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-23 12:22:05.761033 functionfs-0.9.2/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    35147 2007-07-01 22:55:35.000000 functionfs-0.9.2/COPYING
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       53 2020-12-02 14:42:59.000000 functionfs-0.9.2/MANIFEST.in
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1368 2023-06-23 12:22:05.761033 functionfs-0.9.2/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      521 2020-12-02 14:42:59.000000 functionfs-0.9.2/README.rst
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-23 12:22:05.761033 functionfs-0.9.2/functionfs/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    62620 2023-06-21 00:02:59.000000 functionfs-0.9.2/functionfs/__init__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      497 2023-06-23 12:22:05.761033 functionfs-0.9.2/functionfs/_version.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    15498 2021-09-10 23:50:55.000000 functionfs-0.9.2/functionfs/ch9.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2156 2021-10-02 00:46:35.000000 functionfs-0.9.2/functionfs/common.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    11463 2021-09-10 23:50:55.000000 functionfs-0.9.2/functionfs/functionfs.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    33775 2022-11-23 23:50:57.000000 functionfs-0.9.2/functionfs/gadget.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2754 2021-09-10 23:50:55.000000 functionfs-0.9.2/functionfs/hid.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-23 12:22:05.761033 functionfs-0.9.2/functionfs/tests/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        0 2017-01-05 22:22:54.000000 functionfs-0.9.2/functionfs/tests/__init__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      837 2021-12-21 12:54:31.000000 functionfs-0.9.2/functionfs/tests/common.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     9649 2021-12-22 00:51:15.000000 functionfs-0.9.2/functionfs/tests/device.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     5082 2021-12-22 00:51:15.000000 functionfs-0.9.2/functionfs/tests/host.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-23 12:22:05.761033 functionfs-0.9.2/functionfs.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1368 2023-06-23 12:22:05.000000 functionfs-0.9.2/functionfs.egg-info/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      489 2023-06-23 12:22:05.000000 functionfs-0.9.2/functionfs.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2023-06-23 12:22:05.000000 functionfs-0.9.2/functionfs.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       17 2023-06-23 12:22:05.000000 functionfs-0.9.2/functionfs.egg-info/requires.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       11 2023-06-23 12:22:05.000000 functionfs-0.9.2/functionfs.egg-info/top_level.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      209 2023-06-23 12:22:05.761033 functionfs-0.9.2/setup.cfg
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2140 2022-11-23 23:55:51.000000 functionfs-0.9.2/setup.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    80044 2021-12-01 12:14:20.000000 functionfs-0.9.2/versioneer.py
```

### Comparing `functionfs-0.9.1/COPYING` & `functionfs-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/PKG-INFO` & `functionfs-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionfs
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pythonic API for linux's functionfs.
 Home-page: http://github.com/vpelletier/python-functionfs
 Author: Vincent Pelletier
 Author-email: plr.vincent@gmail.com
 License: GPLv3+
 Keywords: linux usb gadget functionfs
 Platform: linux
```

### Comparing `functionfs-0.9.1/README.rst` & `functionfs-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/__init__.py` & `functionfs-0.9.2/functionfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1464,26 +1464,26 @@
         country_code=0,
         in_report_max_length=0,
         out_report_max_length=0,
         full_speed_interval=64,
         high_speed_interval=10,
     ):
         """
-        path, ss_list, os_list, lang_dict, all_ctrl_recip, config0_setup
+        path, os_list, lang_dict, all_ctrl_recip, config0_setup
             See Function.__init__ .
-        fs_list, hs_list:
+        fs_list, hs_list, ss_list:
             If provided, these values are used instead of automatically
             generating minimal valid descriptors, with IN endpoint at index 1
             and OUT endpoint (if out_report_max_length is non-zero) at
             index 2.
 
         report_descriptor (bytes)
             The report descriptor. Describes the structure of all reports
             the interface may generate.
-        hid_descriptor_list (dict)
+        descriptor_dict (dict)
             keys (int)
                 hid.HID_DT_* values
                 Note: hid.HID_DT_REPORT descriptor should rather be provided
                 using report_descriptor argument (see above).
             values (list of bytes)
                 List of descriptors of this type.
                 Note for hid.HID_DT_PHYSICAL: descriptor 0 (see HID 1.11,
@@ -1532,15 +1532,15 @@
             15: 2048000
             16: 4096000
         """
         descriptor_dict = dict(descriptor_dict)
         descriptor_count = 1 + sum(
             (len(x) for x in descriptor_dict.values()),
         )
-        def buildDescriptor(max_packet, interval):
+        def buildDescriptor(max_packet, interval, need_companion=False):
             if (
                 in_report_max_length > max_packet or
                 out_report_max_length > max_packet
             ):
                 return ()
             tail = (hid.USBHIDDescriptorTail * descriptor_count)()
             tail[0].bDescriptorType = hid.HID_DT_REPORT
@@ -1574,37 +1574,55 @@
                     USBEndpointDescriptorNoAudio,
                     bEndpointAddress=1 | ch9.USB_DIR_IN,
                     bmAttributes=ch9.USB_ENDPOINT_XFER_INT,
                     wMaxPacketSize=in_report_max_length,
                     bInterval=interval,
                 ),
             ]
+            if need_companion:
+                result.append(getDescriptor(
+                    USBSSEPCompDescriptor,
+                    bMaxBurst=0,
+                    bmAttributes=0,
+                    wBytesPerInterval=0,
+                ))
             if out_report_max_length:
                 result.append(
                     getDescriptor(
                         USBEndpointDescriptorNoAudio,
                         bEndpointAddress=2 | ch9.USB_DIR_OUT,
                         bmAttributes=ch9.USB_ENDPOINT_XFER_INT,
                         wMaxPacketSize=out_report_max_length,
                         # XXX: what is the meaning of bInterval on INT OUT ?
                         bInterval=interval,
                     ),
                 )
+                if need_companion:
+                    result.append(getDescriptor(
+                        USBSSEPCompDescriptor,
+                        bMaxBurst=0,
+                        bmAttributes=0,
+                        wBytesPerInterval=0,
+                    ))
             return result
         super().__init__(
             path,
             fs_list=fs_list or buildDescriptor(
                 _MAX_PACKET_SIZE_DICT[ch9.USB_ENDPOINT_XFER_INT][0],
                 full_speed_interval,
             ),
             hs_list=hs_list or buildDescriptor(
                 _MAX_PACKET_SIZE_DICT[ch9.USB_ENDPOINT_XFER_INT][1],
                 high_speed_interval,
             ),
-            ss_list=ss_list,
+            ss_list=ss_list or buildDescriptor(
+                _MAX_PACKET_SIZE_DICT[ch9.USB_ENDPOINT_XFER_INT][2],
+                high_speed_interval,
+                need_companion=True,
+            ),
             os_list=os_list,
             lang_dict=lang_dict,
             all_ctrl_recip=all_ctrl_recip,
             config0_setup=config0_setup,
         )
         self.hid_descritptor_dict = hid_descritptor_dict = {
             hid.HID_DT_REPORT: [report_descriptor],
```

### Comparing `functionfs-0.9.1/functionfs/ch9.py` & `functionfs-0.9.2/functionfs/ch9.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/common.py` & `functionfs-0.9.2/functionfs/common.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/functionfs.py` & `functionfs-0.9.2/functionfs/functionfs.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/gadget.py` & `functionfs-0.9.2/functionfs/gadget.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/hid.py` & `functionfs-0.9.2/functionfs/hid.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/tests/common.py` & `functionfs-0.9.2/functionfs/tests/common.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/tests/device.py` & `functionfs-0.9.2/functionfs/tests/device.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs/tests/host.py` & `functionfs-0.9.2/functionfs/tests/host.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/functionfs.egg-info/PKG-INFO` & `functionfs-0.9.2/functionfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionfs
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pythonic API for linux's functionfs.
 Home-page: http://github.com/vpelletier/python-functionfs
 Author: Vincent Pelletier
 Author-email: plr.vincent@gmail.com
 License: GPLv3+
 Keywords: linux usb gadget functionfs
 Platform: linux
```

### Comparing `functionfs-0.9.1/setup.py` & `functionfs-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `functionfs-0.9.1/versioneer.py` & `functionfs-0.9.2/versioneer.py`

 * *Files identical despite different names*

