# Comparing `tmp/sts_libs-0.0.4.tar.gz` & `tmp/sts_libs-0.0.5.dev0.tar.gz`

## Comparing `sts_libs-0.0.4.tar` & `sts_libs-0.0.5.dev0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20604 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    40316 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17015 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    49132 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    46093 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    64839 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35438 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42191 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28682 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    15159 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22311 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/atomic_run.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/tc.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.4/LICENSE
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 sts_libs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 sts_libs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    42311 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17423 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    49941 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    47069 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    66802 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    36092 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42761 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    29049 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    23144 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/atomic_run.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/LICENSE
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/README.md
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/PKG-INFO
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/dm.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/dm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """dm.py: Module to manipulate Device mapper devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re  # regex
 
-from sts.utils import sts_print
 from sts.utils.cmdline import run, run_ret_out
 
 
-def dm_show_status(dm_device=None):
+def dm_show_status(dm_device=None):  # noqa: ANN001, ANN201
     """Show dmsetup status.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     True
     or
     False.
     """
     cmd = "dmsetup status"
     if dm_device:
         cmd += f" {dm_device}"
 
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not show dmsetup status")
+        print("FAIL: Could not show dmsetup status")
         return False
     return True
 
 
-def dm_query_status(dm_device=None):
+def dm_query_status(dm_device=None):  # noqa: ANN001, ANN201
     """Query dmsetup status and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with status info for each device.
     """
     cmd = "dmsetup status"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not list status")
+        print("FAIL: Could not list status")
         return None
     devices = output.split("\n")
 
     status_basic_format_regex = r"(.*):\s+(\d+)\s+(\d+)\s+(\S+)"
     # Thin formats are available on: https://www.kernel.org/doc/Documentation/device-mapper/thin-provisioning.txt
     status_thin_format_regex = status_basic_format_regex + r"\s+(\d+)\s+(\d+|-)"
     status_thin_pool_format_regex = status_basic_format_regex + r"\s+(\d+)\s+(\d+)\/(\d+)\s+(\d+)\/(\d+)(.*)"
@@ -52,40 +51,40 @@
         status_basic_format_regex + r"\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(.*)"
     )
 
     dev_status_dict = {}
     for device in devices:
         m = re.match(status_basic_format_regex, device)
         if not m:
-            sts_print(f"FAIL: dm_query_status() - ({device}) does not match dmsetup status output format")
+            print(f"FAIL: dm_query_status() - ({device}) does not match dmsetup status output format")
             continue
         dm_type = m.group(4)
         dm_status_format_dict = {}
         if dm_type == "linear":
             dm_status_format_dict = {
                 "logical_start_sector": m.group(2),
                 "num_sec": m.group(3),
                 "target_type": dm_type,
             }
         elif dm_type == "thin":
             t = re.match(status_thin_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_status_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "nr_mapped_sec": t.group(5),
                 "highest_mapped_sec": t.group(6),
             }
         elif dm_type == "thin-pool":
             t = re.match(status_thin_pool_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_status_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "trans_id": t.group(5),
                 "used_metadata": t.group(6),
@@ -93,15 +92,15 @@
                 "used_data_block": t.group(8),
                 "total_data_block": t.group(9),
                 "metadata": t.group(10),
             }
         elif dm_type == "multipath":
             t = re.match(status_multipath_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_status_format_dict = {
                 "logical_start_sector": m.group(2),
                 "num_sec": m.group(3),
                 "target_type": dm_type,
                 "nr_status_feature": t.group(5),
                 "all_io_queued": t.group(6),
@@ -116,43 +115,43 @@
             status_multipath_path_format_regex = r"\s+(\S+)\s+(\S+)\s+(\S+)"
             status_multipath_grp_header_format_regex = r"\s?(\S)\s+(\d+)\s+(\d+)\s+(\d+)"
 
             nr_groups = int(dm_status_format_dict["nr_path_grps"])
             for group_nr in range(1, int(nr_groups) + 1):
                 grp_match = re.match(status_multipath_grp_header_format_regex, remaining_data)
                 if not grp_match:
-                    sts_print("FAIL: dm_query_status() - Could not parse group multipath data")
+                    print("FAIL: dm_query_status() - Could not parse group multipath data")
                     return None
                 if "path_grp" not in list(dm_status_format_dict.keys()):
                     dm_status_format_dict["path_grp"] = {}
                 dm_status_format_dict["path_grp"][group_nr] = {}
                 path_grp = dm_status_format_dict["path_grp"][group_nr]
                 path_grp["state"] = grp_match.group(1)
                 path_grp["nr_grp_status_arg"] = grp_match.group(2)
                 path_grp["nr_paths"] = grp_match.group(3)
                 path_grp["nr_path_status_arg"] = grp_match.group(4)
                 nr_paths = int(path_grp["nr_paths"])  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
                 remaining_data = re.sub(status_multipath_grp_header_format_regex, "", remaining_data, 1)
                 for p_nr in range(1, int(nr_paths) + 1):
                     path_match = re.match(status_multipath_path_format_regex, remaining_data)
                     if not path_match:
-                        sts_print("FAIL: dm_query_status() - Could not parse path multipath data")
+                        print("FAIL: dm_query_status() - Could not parse path multipath data")
                         return None
                     if "path" not in list(path_grp.keys()):
                         path_grp["path"] = {}
                     path_grp["path"][p_nr] = {}  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
                     path = path_grp["path"][p_nr]  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
                     path["device"] = path_match.group(1)
                     path["state"] = path_match.group(2)
                     path["failure_cnt"] = path_match.group(3)
                     remaining_data = re.sub(status_multipath_path_format_regex, "", remaining_data, 1)
                     for _ in range(1, int(grp_match.group(4)) + 1):
                         path_arg_match = re.match(status_multipath_path_args_format_regex, remaining_data)
                         if not path_arg_match:
-                            sts_print("FAIL: dm_query_status() - Could not parse path args multipath data")
+                            print("FAIL: dm_query_status() - Could not parse path args multipath data")
                             return None
                         if "path_status_args" not in list(path.keys()):
                             path["path_status_args"] = ""
                         path["path_status_args"] += f"{path_arg_match.group(1)} "
                         remaining_data = re.sub(
                             status_multipath_path_args_format_regex,
                             "",
@@ -160,56 +159,56 @@
                             1,
                         )
                     # remove trailing space from the end of string
                     if "path_status_args" in list(path.keys()):
                         path["path_status_args"] = path["path_status_args"].strip()
 
         else:
-            sts_print(f"FAIL: dm_query_status() - ({device}) can't parse status for device type {dm_type}")
+            print(f"FAIL: dm_query_status() - ({device}) can't parse status for device type {dm_type}")
 
         dev_status_dict[m.group(1)] = dm_status_format_dict
     if dm_device:
         if dm_device in list(dev_status_dict.keys()):
             return dev_status_dict[dm_device]
         return None
     return dev_status_dict
 
 
-def dm_show_table(dm_device=None):
+def dm_show_table(dm_device=None):  # noqa: ANN001, ANN201
     """Show dmsetup table.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     True
     or
     False.
     """
     cmd = "dmsetup table"
     if dm_device:
         cmd += f" {dm_device}"
 
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not show dmsetup table")
+        print("FAIL: Could not show dmsetup table")
         return False
     return True
 
 
-def dm_query_table(dm_device=None):
+def dm_query_table(dm_device=None):  # noqa: ANN001, ANN201
     """Query dmsetup table and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with table info for each device.
     """
     cmd = "dmsetup table"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not list table")
+        print("FAIL: Could not list table")
         return None
     devices = output.split("\n")
 
     # Basic format information is found on man dmsetup under "TABLE FORMAT" section
     # format of dmsetup table: logical_start_sector num_sectors target_type target_args
     table_basic_format_regex = r"(.*):\s+(\S+)\s+(\S+)\s+(\S+)"
     # format for linear type
@@ -221,61 +220,61 @@
     # delayed: 0 20971520 delay 7:0 0 100
     table_delay_format_regex = table_basic_format_regex + r"\s+(\S+)\s+(\S+)\s+(\S+)$"
 
     dev_table_dict = {}
     for device in devices:
         m = re.match(table_basic_format_regex, device)
         if not m:
-            sts_print(f"FAIL: ({device}) does not match dmsetup table output format")
+            print(f"FAIL: ({device}) does not match dmsetup table output format")
             continue
         dm_type = m.group(4)
         dm_table_format_dict = {}
         if dm_type == "linear":
             t = re.match(table_linear_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid linear table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid linear table output format")
                 continue
             dm_table_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "dev": t.group(5),
                 "start_sec": t.group(6),
             }
         elif dm_type == "thin":
             t = re.match(table_thin_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_table_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "pool_dev": t.group(5),
                 "dev_num": t.group(6),
             }
         elif dm_type == "thin-pool":
             t = re.match(table_thin_pool_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_table_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "metadata_dev": t.group(5),
                 "data_dev": t.group(6),
                 "data_block_size": t.group(7),
                 "low_water_mark": t.group(8),
                 "target_args": t.group(9),
             }
         elif dm_type == "delay":
             t = re.match(table_delay_format_regex, device)
             if not t:
-                sts_print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
                 continue
             dm_table_format_dict = {
                 "logical_start_sector": t.group(2),
                 "num_sec": t.group(3),
                 "target_type": dm_type,
                 "dev": t.group(5),
                 "start_sec": t.group(6),
@@ -320,42 +319,42 @@
             table_multipath_grp_header_format_regex = r"\s?(\S+)\s+(\d+)\s+(\d+)\s+(\d+)"
             table_multipath_path_header_format_regex = r"\s?(\S+)"
             table_multipath_path_args_format_regex = r"\s?(\S+)"
             nr_groups = dm_table_format_dict["nr_path_grps"]
             for group_nr in range(1, int(nr_groups) + 1):
                 grp_match = re.match(table_multipath_grp_header_format_regex, remaining_data)
                 if not grp_match:
-                    sts_print("FAIL: dm_query_table() - Could not parse group multipath data")
+                    print("FAIL: dm_query_table() - Could not parse group multipath data")
                     return None
                 if "path_grp" not in list(dm_table_format_dict.keys()):
                     dm_table_format_dict["path_grp"] = {}
                 dm_table_format_dict["path_grp"][group_nr] = {}
                 path_grp = dm_table_format_dict["path_grp"][group_nr]
                 path_grp["path_selector"] = grp_match.group(1)
                 path_grp["nr_selector_args"] = grp_match.group(2)
                 path_grp["nr_paths_grp"] = grp_match.group(3)
                 path_grp["nr_path_args"] = grp_match.group(4)
                 # remove processed data
                 remaining_data = re.sub(table_multipath_grp_header_format_regex, "", remaining_data, 1)
                 for path_nr in range(1, int(path_grp["nr_paths_grp"]) + 1):
                     path_match = re.match(table_multipath_path_header_format_regex, remaining_data)
                     if not path_match:
-                        sts_print("FAIL: dm_query_table() - Could not parse path multipath data")
+                        print("FAIL: dm_query_table() - Could not parse path multipath data")
                         return None
                     if "path" not in list(dm_table_format_dict.keys()):
                         dm_table_format_dict["path"] = {}
                     dm_table_format_dict["path"][path_nr] = {}
                     path = dm_table_format_dict["path"][path_nr]
                     path["device"] = path_match.group(1)
 
                     remaining_data = re.sub(table_multipath_path_header_format_regex, "", remaining_data, 1)
                     for _ in range(1, int(path_grp["nr_path_args"]) + 1):
                         arg_match = re.match(table_multipath_path_args_format_regex, remaining_data)
                         if not arg_match:
-                            sts_print("FAIL: dm_query_table() - Could not parse path arg multipath data")
+                            print("FAIL: dm_query_table() - Could not parse path arg multipath data")
                             return None
                         if "path_status_args" not in list(path.keys()):
                             path["path_status_args"] = ""
                         path["path_status_args"] += f"{arg_match.group(1)} "
                         remaining_data = re.sub(
                             table_multipath_path_args_format_regex,
                             "",
@@ -363,40 +362,40 @@
                             1,
                         )
                     if "path_status_args" in list(path.keys()):
                         # remove trailing space
                         path["path_status_args"] = path["path_status_args"].strip()
 
         else:
-            sts_print(f"FAIL: dm_query_table() - ({device}) can't parse table for device type '{dm_type}'")
+            print(f"FAIL: dm_query_table() - ({device}) can't parse table for device type '{dm_type}'")
         dev_table_dict[m.group(1)] = dm_table_format_dict
 
     if dm_device:
         if dm_device in list(dev_table_dict.keys()):
             return dev_table_dict[dm_device]
         return None
     return dev_table_dict
 
 
-def dm_get_table_device(dm_name):
+def dm_get_table_device(dm_name):  # noqa: ANN001, ANN201
     """Get table information for specific device.
     The table info is not parsed.
     """
     if not dm_name:
         return None
     cmd = f"dmsetup table {dm_name}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: Could not query table for {dm_name}")
+        print(f"FAIL: Could not query table for {dm_name}")
         return None
 
     return output
 
 
-def dm_set_target_type(dm_name, target_type):
+def dm_set_target_type(dm_name, target_type):  # noqa: ANN001, ANN201
     """Change the target type of specific DM device
     it is necessary to suspend the device before loading new table
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
@@ -410,83 +409,83 @@
 
     # We need to suspend the device first
     if not dm_suspend_dev(dm_name):
         return False
 
     m = re.match(table_format_regex, table_info)
     if not m:
-        sts_print(f"FAIL: dm_set_target_type() - ({table_info}) does not match dmsetup table output format")
+        print(f"FAIL: dm_set_target_type() - ({table_info}) does not match dmsetup table output format")
         return False
     # load the table with new target type
     new_table = f'"{m.group(1)} {m.group(2)} {target_type} {m.group(4)}"'
 
     cmd = f"dmsetup load {dm_name} --table {new_table}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: dm_set_target_type() - could not load table on {dm_name}")
+        print(f"FAIL: dm_set_target_type() - could not load table on {dm_name}")
         dm_resume_dev(dm_name)
         return False
 
     if not dm_resume_dev(dm_name):
         return False
 
     return True
 
 
-def dm_suspend_dev(dm_name):
+def dm_suspend_dev(dm_name):  # noqa: ANN001, ANN201
     """Executes dmsetup suspend to suspend a specific DM device
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup suspend {dm_name}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: could not suspend {dm_name}")
+        print(f"FAIL: could not suspend {dm_name}")
         return False
 
     return True
 
 
-def dm_resume_dev(dm_name):
+def dm_resume_dev(dm_name):  # noqa: ANN001, ANN201
     """Executes dmsetup resume to suspend a specific DM device
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup resume {dm_name}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: could not resume {dm_name}")
+        print(f"FAIL: could not resume {dm_name}")
         return False
 
     return True
 
 
-def dm_message_dev(dm_name, message):
+def dm_message_dev(dm_name, message):  # noqa: ANN001, ANN201
     """Executes dmsetup message to send a message to a specific DM device
     The arguments are:
     Device name: e.g. mpatha
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup message {dm_name} {message}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: could not send message to {dm_name}")
+        print(f"FAIL: could not send message to {dm_name}")
         return False
 
     return True
 
 
-def dm_remove(dm_name):
+def dm_remove(dm_name):  # noqa: ANN001, ANN201
     """Remove the specified device
     The arguments are:
     Device name: e.g. Device mapped device name
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
@@ -494,10 +493,10 @@
     devs = dm_query_table()
     if dm_name not in list(devs.keys()):
         # device name does not exist
         return True
 
     cmd = f"dmsetup remove {dm_name}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: could not remove {dm_name}")
+        print(f"FAIL: could not remove {dm_name}")
         return False
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/dmpd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 """dmpd.py: Module to manipulate LVM thinp and cache metadata devices and snapshot eras."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import sys
 from pathlib import Path
+from typing import Dict, List, Union
 
 from sts import linux, lvm
-from sts.utils import sts_print
 from sts.utils.cli_tools import Wrapper
 from sts.utils.cmdline import run, run_ret_out
 
 
-def _get_devices():
+def _get_devices():  # noqa: ANN202
     return lvm.lv_query()
 
 
-def _get_active_devices():
+def _get_active_devices():  # noqa: ANN202
     cmd = "ls /dev/mapper/"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not find active dm devices")
+        print("FAIL: Could not find active dm devices")
         return False
     return output.split()
 
 
-def _get_device_path(vg_name, lv_name):
+def _get_device_path(vg_name, lv_name):  # noqa: ANN001, ANN202
     device_path = vg_name + "-" + lv_name
     if "/dev/mapper/" not in device_path:
         device_path = "/dev/mapper/" + device_path
     return device_path
 
 
-def _check_device(vg_name, lv_name):
+def _check_device(vg_name, lv_name):  # noqa: ANN001, ANN202
     devices = _get_devices()
     device_list = [f["name"] for f in devices]
     if lv_name not in device_list:
-        sts_print(f"FAIL: {lv_name} is not a device")
+        print(f"FAIL: {lv_name} is not a device")
         return False
     for x in devices:
         if x["name"] == lv_name and x["vg_name"] == vg_name:
-            sts_print(f"INFO: Found device {lv_name} in group {vg_name}")
+            print(f"INFO: Found device {lv_name} in group {vg_name}")
             return True
     return False
 
 
-def _activate_device(vg_name, lv_name):
+def _activate_device(vg_name, lv_name):  # noqa: ANN001, ANN202
     devices_active = _get_active_devices()
     if vg_name + "-" + lv_name not in devices_active:
         ret = lvm.lv_activate(lv_name, vg_name)
         if not ret:
-            sts_print(f"FAIL: Could not activate device {lv_name}")
+            print(f"FAIL: Could not activate device {lv_name}")
             return False
-        sts_print(f"INFO: device {lv_name} was activated")
-    sts_print(f"INFO: device {lv_name} is active")
+        print(f"INFO: device {lv_name} was activated")
+    print(f"INFO: device {lv_name} is active")
     return True
 
 
-def _fallocate(_file, size, command_message):
+def _fallocate(_file, size, command_message):  # noqa: ANN001, ANN202
     cmd = f"fallocate -l {size}M {_file}"
     try:
         retcode = run(cmd).returncode
         if retcode != 0:
-            sts_print(f"FAIL: Command failed with code {retcode}.")
-            sts_print(f"FAIL: Could not create file to {command_message} metadata to.")
+            print(f"FAIL: Command failed with code {retcode}.")
+            print(f"FAIL: Could not create file to {command_message} metadata to.")
             return False
     except OSError as e:
         print("command failed: ", e, file=sys.stderr)
         return False
     return True
 
 
-def get_help(cmd):
+def get_help(cmd):  # noqa: ANN001, ANN201
     commands = [
         "cache_check",
         "cache_dump",
         "cache_metadata_size",
         "cache_repair",
         "cache_restore",
         "era_check",
@@ -90,27 +90,27 @@
         "thin_repair",
         "thin_restore",
         "thin_rmap",
         "thin_show_duplicates",
         "thin_trim",
     ]
     if cmd not in commands:
-        sts_print(f"FAIL: Unknown command {cmd}")
+        print(f"FAIL: Unknown command {cmd}")
         return False
 
     command = f"{cmd} -h"
     retcode = run(command, verbose=True).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not get help for {cmd}.")
+        print(f"FAIL: Could not get help for {cmd}.")
         return False
 
     return True
 
 
-def get_version(cmd):
+def get_version(cmd):  # noqa: ANN001, ANN201
     commands = [
         "cache_check",
         "cache_dump",
         "cache_metadata_size",
         "cache_repair",
         "cache_restore",
         "era_check",
@@ -125,33 +125,33 @@
         "thin_repair",
         "thin_restore",
         "thin_rmap",
         "thin_show_duplicates",
         "thin_trim",
     ]
     if cmd not in commands:
-        sts_print(f"FAIL: Unknown command {cmd}")
+        print(f"FAIL: Unknown command {cmd}")
         return False
 
     command = f"{cmd} -V"
     retcode = run(command, verbose=True).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not get version of {cmd}.")
+        print(f"FAIL: Could not get version of {cmd}.")
         return False
 
     return True
 
 
-def _get_dev_id(dev_id, path=None, lv_name=None, vg_name=None):
+def _get_dev_id(dev_id, path=None, lv_name=None, vg_name=None):  # noqa: ANN001, ANN202
     dev_ids = []
 
     if path is None:
         retcode, data = thin_dump(source_vg=vg_name, source_lv=lv_name, formatting="xml", return_output=True)
         if not retcode:
-            sts_print(f"FAIL: Could not dump metadata from {vg_name}/{lv_name}")
+            print(f"FAIL: Could not dump metadata from {vg_name}/{lv_name}")
             return False
         data_lines = data.splitlines()
         for line in data_lines:
             blocks = line.split()
             for block in blocks:
                 if not block.startswith("dev_"):
                     continue
@@ -168,51 +168,51 @@
 
     if dev_id in dev_ids:
         return True
 
     return False
 
 
-def _metadata_size(source=None, lv_name=None, vg_name=None):
+def _metadata_size(source=None, lv_name=None, vg_name=None):  # noqa: ANN001, ANN202
     if source is None:
         cmd = "lvs -a --units m"
         ret, data = run_ret_out(cmd, return_output=True)
         if ret != 0:
-            sts_print("FAIL: Could not list LVs")
+            print("FAIL: Could not list LVs")
         data_line = data.splitlines()
         for line in data_line:
             cut = line.split()
             if not cut or lv_name != cut[0] and vg_name != cut[1]:
                 continue
             cut = cut[3]
             cut = cut.split("m")
             size = float(cut[0])
             run(cmd)
             return int(size)
-        sts_print(f"FAIL: Could not find {lv_name} {vg_name} in lvs, setting size to 100m")
+        print(f"FAIL: Could not find {lv_name} {vg_name} in lvs, setting size to 100m")
         return 100
     return int(Path(source).stat().st_size) / 1000000
 
 
 ###########################################
 # cache section
 ###########################################
 
 
-def cache_check(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    quiet=False,
-    super_block_only=False,
-    clear_needs_check_flag=False,
-    skip_mappings=False,
-    skip_hints=False,
-    skip_discards=False,
-    verbose=True,
+def cache_check(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    quiet=False,  # noqa: ANN001
+    super_block_only=False,  # noqa: ANN001
+    clear_needs_check_flag=False,  # noqa: ANN001
+    skip_mappings=False,  # noqa: ANN001
+    skip_hints=False,  # noqa: ANN001
+    skip_discards=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Check cache pool metadata from either file or device.
     The arguments are:
     source_file
     source_vg VG name
     source_lv LV name
     quiet Mute STDOUT
@@ -225,28 +225,28 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: cache_check requires either source_file OR source_vg and source_lv.")
+        print("FAIL: cache_check requires either source_file OR source_vg and source_lv.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         device = source_file
 
     if quiet:
         options += "--quiet "
 
     if super_block_only:
@@ -263,28 +263,28 @@
 
     if skip_discards:
         options += "--skip-discards "
 
     cmd = f"cache_check {device} {options}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not check {device} metadata")
+        print(f"FAIL: Could not check {device} metadata")
         return False
 
     return True
 
 
-def cache_dump(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    output=None,
-    repair=False,
-    verbose=True,
-    return_output=False,
+def cache_dump(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    output=None,  # noqa: ANN001
+    repair=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
+    return_output=False,  # noqa: ANN001
 ):
     """Dumps cache metadata from device of source file to standard output or file.
     The arguments are:
     source_file
     source_vg: VG name
     source_lv: LV name
     output: specify output xml file
@@ -296,34 +296,34 @@
     False in case of failure,
     Boolean and data if return_output True.
     """
     options = ""
     data = None
 
     if return_output and output:
-        sts_print("INFO: Cannot return to both STDOUT and file, returning only to file.")
+        print("INFO: Cannot return to both STDOUT and file, returning only to file.")
         return_output = False
 
     ret_fail = (False, None) if return_output else False
 
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: cache_dump requires either source_file OR source_vg and source_lv.")
+        print("FAIL: cache_dump requires either source_file OR source_vg and source_lv.")
         return ret_fail
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return ret_fail
         device = source_file
 
     if output:
         if not Path(output).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
             ret = _fallocate(output, size + 1, "dump")
@@ -336,59 +336,59 @@
 
     cmd = f"cache_dump {device} {options}"
     if return_output:
         retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
     else:
         retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not dump {device} metadata.")
+        print(f"FAIL: Could not dump {device} metadata.")
         return ret_fail
 
     if return_output:
         return True, data
     return True
 
 
-def cache_repair(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    target_file=None,
-    target_vg=None,
-    target_lv=None,
-    verbose=True,
+def cache_repair(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    target_file=None,  # noqa: ANN001
+    target_vg=None,  # noqa: ANN001
+    target_lv=None,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Repairs cache metadata from source file/device to target file/device
     The arguments are:
     source as either source_file OR source_vg and source_lv
     target as either target_file OR target_vg and target_lv
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: cache_repair requires either source_file OR source_vg and source_lv as source.")
+        print("FAIL: cache_repair requires either source_file OR source_vg and source_lv as source.")
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        sts_print("FAIL: cache_repair requires either target_file OR target_vg and target_lv as target.")
+        print("FAIL: cache_repair requires either target_file OR target_vg and target_lv as target.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         source = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         source = source_file
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
@@ -403,30 +403,30 @@
             if not ret:
                 return False
         target = target_file
 
     cmd = f"cache_repair -i {source} -o {target}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not repair metadata from {source} to {target}")
+        print(f"FAIL: Could not repair metadata from {source} to {target}")
         return False
 
     return True
 
 
-def cache_restore(
-    source_file,
-    target_vg=None,
-    target_lv=None,
-    target_file=None,
-    quiet=False,
-    metadata_version=None,
-    omit_clean_shutdown=False,
-    override_metadata_version=None,
-    verbose=True,
+def cache_restore(  # noqa: ANN201
+    source_file,  # noqa: ANN001
+    target_vg=None,  # noqa: ANN001
+    target_lv=None,  # noqa: ANN001
+    target_file=None,  # noqa: ANN001
+    quiet=False,  # noqa: ANN001
+    metadata_version=None,  # noqa: ANN001
+    omit_clean_shutdown=False,  # noqa: ANN001
+    override_metadata_version=None,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Restores cache metadata from source xml file to target device/file
     The arguments are:
     source_file Source xml file
     target as either target_file OR target_vg and target_lv
     quiet Mute STDOUT
     metadata_version Specify metadata version to restore
@@ -436,23 +436,23 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if source_file is None:
-        sts_print("FAIL: cache_restore requires source file.")
+        print("FAIL: cache_restore requires source file.")
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        sts_print("FAIL: cache_restore requires either target_file OR target_vg and target_lv as target.")
+        print("FAIL: cache_restore requires either target_file OR target_vg and target_lv as target.")
         return False
 
     if not Path(source_file).is_file():
-        sts_print("FAIL: Source file is not a file.")
+        print("FAIL: Source file is not a file.")
         return False
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
@@ -479,35 +479,35 @@
     if override_metadata_version:
         options += f"--debug-override-metadata-version {override_metadata_version}"
 
     cmd = f"cache_restore -i {source_file} -o {target} {options}"
 
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not restore metadata from {source_file} to {target}")
+        print(f"FAIL: Could not restore metadata from {source_file} to {target}")
         return False
 
     return True
 
 
 ###########################################
 # thinp section
 ###########################################
 
 
-def thin_check(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    quiet=False,
-    super_block_only=False,
-    clear_needs_check_flag=False,
-    skip_mappings=False,
-    ignore_non_fatal_errors=False,
-    verbose=True,
+def thin_check(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    quiet=False,  # noqa: ANN001
+    super_block_only=False,  # noqa: ANN001
+    clear_needs_check_flag=False,  # noqa: ANN001
+    skip_mappings=False,  # noqa: ANN001
+    ignore_non_fatal_errors=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Check thin pool metadata from either file or device.
     The arguments are:
     source_file
     source_vg VG name
     source_lv LV name
     quiet Mute STDOUT
@@ -519,28 +519,28 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: thin_check requires either source_file OR source_vg and source_lv.")
+        print("FAIL: thin_check requires either source_file OR source_vg and source_lv.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         device = source_file
 
     if quiet:
         options += "--quiet "
 
     if super_block_only:
@@ -554,36 +554,36 @@
 
     if ignore_non_fatal_errors:
         options += "--ignore-non-fatal-errors "
 
     cmd = f"thin_check {device} {options}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not check {device} metadata")
+        print(f"FAIL: Could not check {device} metadata")
         return False
 
     return True
 
 
-def thin_ls(source_vg, source_lv, no_headers=False, fields=None, snapshot=False, verbose=True):
+def thin_ls(source_vg, source_lv, no_headers=False, fields=None, snapshot=False, verbose=True):  # noqa: ANN001, ANN201
     """List information about thin LVs on thin pool.
     The arguments are:
     source_vg VG name
     source_lv LV name
     fields list of fields to output, default is all
     snapshot Use metadata snapshot, able to run on live snapshotted pool
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if not source_vg or not source_lv:
-        sts_print("FAIL: thin_ls requires source_vg and source_lv.")
+        print("FAIL: thin_ls requires source_vg and source_lv.")
         return False
 
     ret = _check_device(source_vg, source_lv)
     if not ret:
         return False
     ret = _activate_device(source_vg, source_lv)
     if not ret:
@@ -612,43 +612,43 @@
         "SNAP_TIME",
     ]
     if fields is None:
         options += f" --format \"{','.join([str(i) for i in fields_possible])}\" "
     else:
         for field in fields:
             if field not in fields_possible:
-                sts_print(f"FAIL: Unknown field {field} specified.")
-                sts_print(f"INFO: Possible fields are: {', '.join([str(i) for i in fields_possible])}")
+                print(f"FAIL: Unknown field {field} specified.")
+                print(f"INFO: Possible fields are: {', '.join([str(i) for i in fields_possible])}")
                 return False
         options += f" --format \"{','.join([str(i) for i in fields])}\" "
 
     if snapshot:
         options += "--metadata-snap"
 
     cmd = f"thin_ls {device} {options}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not list {device} metadata")
+        print(f"FAIL: Could not list {device} metadata")
         return False
 
     return True
 
 
-def thin_dump(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    output=None,
-    repair=False,
-    formatting=None,
-    snapshot=None,
-    dev_id=None,
-    skip_mappings=False,
-    verbose=True,
-    return_output=False,
+def thin_dump(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    output=None,  # noqa: ANN001
+    repair=False,  # noqa: ANN001
+    formatting=None,  # noqa: ANN001
+    snapshot=None,  # noqa: ANN001
+    dev_id=None,  # noqa: ANN001
+    skip_mappings=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
+    return_output=False,  # noqa: ANN001
 ):
     """Dumps thin metadata from device of source file to standard output or file.
     The arguments are:
     source_file
     source_vg: VG name
     source_lv: LV name
     output: specify output xml file
@@ -663,34 +663,34 @@
     False in case of failure
     Boolean and data if return_output True.
     """
     options = ""
     data = None
 
     if return_output and output:
-        sts_print("INFO: Cannot return to both STDOUT and file, returning only to file.")
+        print("INFO: Cannot return to both STDOUT and file, returning only to file.")
         return_output = False
 
     ret_fail = (False, None) if return_output else False
 
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: thin_dump requires either source_file OR source_vg and source_lv.")
+        print("FAIL: thin_dump requires either source_file OR source_vg and source_lv.")
         return ret_fail
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return ret_fail
         device = source_file
 
     if output:
         if not Path(output).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
             ret = _fallocate(output, size + 1, "dump")
@@ -703,64 +703,64 @@
 
     if snapshot:
         if isinstance(snapshot, bool):
             options += "--metadata-snap "
         elif isinstance(snapshot, int):
             options += f"--metadata-snap {snapshot} "
         else:
-            sts_print("FAIL: Unknown snapshot value, use either Boolean or Int.")
+            print("FAIL: Unknown snapshot value, use either Boolean or Int.")
             return ret_fail
 
     if formatting:
         if formatting in ["xml", "human_readable"]:
             options += f"--format {formatting} "
         elif formatting.startswith("custom="):
             if not Path(formatting[8:-1]).is_file():
-                sts_print("FAIL: Specified custom formatting file is not a file.")
+                print("FAIL: Specified custom formatting file is not a file.")
                 return ret_fail
             options += f"--format {formatting} "
         else:
-            sts_print("FAIL: Unknown formatting specified, please use one of [xml, human_readable, custom='file'].")
+            print("FAIL: Unknown formatting specified, please use one of [xml, human_readable, custom='file'].")
             return ret_fail
 
     if dev_id:
         if isinstance(dev_id, int):
             if _get_dev_id(dev_id, source_file, source_lv, source_vg):
                 options += f"--dev-id {dev_id} "
             else:
-                sts_print(f"FAIL: Unknown dev_id value, device with id {dev_id} does not exist.")
+                print(f"FAIL: Unknown dev_id value, device with id {dev_id} does not exist.")
                 return ret_fail
         else:
-            sts_print("FAIL: Unknown dev_id value, must be Int.")
+            print("FAIL: Unknown dev_id value, must be Int.")
             return ret_fail
 
     if skip_mappings:
         options += "--skip-mappings "
 
     cmd = f"thin_dump {device} {options}"
     if return_output:
         retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
     else:
         retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not dump {device} metadata.")
+        print(f"FAIL: Could not dump {device} metadata.")
         return ret_fail
 
     if return_output:
         return True, data
     return True
 
 
-def thin_restore(
-    source_file,
-    target_vg=None,
-    target_lv=None,
-    target_file=None,
-    quiet=False,
-    verbose=True,
+def thin_restore(  # noqa: ANN201
+    source_file,  # noqa: ANN001
+    target_vg=None,  # noqa: ANN001
+    target_lv=None,  # noqa: ANN001
+    target_file=None,  # noqa: ANN001
+    quiet=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Restores thin metadata from source xml file to target device/file
     The arguments are:
     source_file Source xml file
     target as either target_file OR target_vg and target_lv
     quiet Mute STDOUT
     metadata_version Specify metadata version to restore
@@ -770,23 +770,23 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if source_file is None:
-        sts_print("FAIL: thin_restore requires source file.")
+        print("FAIL: thin_restore requires source file.")
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        sts_print("FAIL: thin_restore requires either target_file OR target_vg and target_lv as target.")
+        print("FAIL: thin_restore requires either target_file OR target_vg and target_lv as target.")
         return False
 
     if not Path(source_file).is_file():
-        sts_print("FAIL: Source file is not a file.")
+        print("FAIL: Source file is not a file.")
         return False
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
@@ -804,57 +804,57 @@
     if quiet:
         options += "--quiet"
 
     cmd = f"thin_restore -i {source_file} -o {target} {options}"
 
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not restore metadata from {source_file} to {target}")
+        print(f"FAIL: Could not restore metadata from {source_file} to {target}")
         return False
 
     return True
 
 
-def thin_repair(
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    target_file=None,
-    target_vg=None,
-    target_lv=None,
-    verbose=True,
+def thin_repair(  # noqa: ANN201
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    target_file=None,  # noqa: ANN001
+    target_vg=None,  # noqa: ANN001
+    target_lv=None,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Repairs thin metadata from source file/device to target file/device
     The arguments are:
     source as either source_file OR source_vg and source_lv
     target as either target_file OR target_vg and target_lv
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: thin_repair requires either source_file OR source_vg and source_lv as source.")
+        print("FAIL: thin_repair requires either source_file OR source_vg and source_lv as source.")
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        sts_print("FAIL: thin_repair requires either target_file OR target_vg and target_lv as target.")
+        print("FAIL: thin_repair requires either target_file OR target_vg and target_lv as target.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         source = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         source = source_file
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
@@ -869,45 +869,45 @@
             if not ret:
                 return False
         target = target_file
 
     cmd = f"thin_repair -i {source} -o {target}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not repair metadata from {source} to {target}")
+        print(f"FAIL: Could not repair metadata from {source} to {target}")
         return False
 
     return True
 
 
-def thin_rmap(region, source_file=None, source_vg=None, source_lv=None, verbose=True):
+def thin_rmap(region, source_file=None, source_vg=None, source_lv=None, verbose=True):  # noqa: ANN001, ANN201
     """Output reverse map of a thin provisioned region of blocks from metadata device.
     The arguments are:
     source_vg VG name
     source_lv LV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: thin_rmap requires either source_file OR source_vg and source_lv as source.")
+        print("FAIL: thin_rmap requires either source_file OR source_vg and source_lv as source.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         device = source_file
 
     regions = region.split(".")
     try:
         int(regions[0])
         if regions[1] != "":
@@ -925,27 +925,27 @@
         print("FAIL: Beginning of the region must be before its end.")
         return False
     options = f"--region {region}"
 
     cmd = f"thin_rmap {device} {options}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not output reverse map from {device} metadata device")
+        print(f"FAIL: Could not output reverse map from {device} metadata device")
         return False
 
     return True
 
 
-def thin_trim(
-    data_vg,
-    data_lv,
-    metadata_vg=None,
-    metadata_lv=None,
-    metadata_file=None,
-    verbose=True,
+def thin_trim(  # noqa: ANN201
+    data_vg,  # noqa: ANN001
+    data_lv,  # noqa: ANN001
+    metadata_vg=None,  # noqa: ANN001
+    metadata_lv=None,  # noqa: ANN001
+    metadata_file=None,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Issue discard requests for free pool space.
     The arguments are:
     data_vg VG name of data device
     data_lv LV name of data device
     metadata_vg VG name of metadata device
     metadata_lv LV name of metadata device
@@ -954,19 +954,19 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if not data_vg or not data_lv:
-        sts_print("FAIL: thin_trim requires data_vg and data_lv.")
+        print("FAIL: thin_trim requires data_vg and data_lv.")
         return False
 
     if not metadata_file and (not metadata_vg or not metadata_lv):
-        sts_print("FAIL: thin_trim requires either metadata_file OR metadata_vg and metadata_lv as target.")
+        print("FAIL: thin_trim requires either metadata_file OR metadata_vg and metadata_lv as target.")
         return False
 
     ret = _check_device(data_vg, data_lv)
     if not ret:
         return False
 
     ret = _activate_device(data_vg, data_lv)
@@ -979,37 +979,37 @@
             return False
         ret = _activate_device(metadata_vg, metadata_lv)
         if not ret:
             return False
         metadata_dev = _get_device_path(metadata_vg, metadata_lv)
     else:
         if not Path(metadata_file).is_file():
-            sts_print(f"FAIL: metadata_file {metadata_file} is not a file.")
+            print(f"FAIL: metadata_file {metadata_file} is not a file.")
             return False
         metadata_dev = metadata_file
 
     data_dev = _get_device_path(data_vg, data_lv)
     cmd = f"thin_trim --data-dev {data_dev} --metadata-dev {metadata_dev} {options}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not discard free pool space on device {data_dev} with metadata device {metadata_dev}.")
+        print(f"FAIL: Could not discard free pool space on device {data_dev} with metadata device {metadata_dev}.")
         return False
 
     return True
 
 
-def thin_delta(
-    thin1,
-    thin2,
-    source_file=None,
-    source_vg=None,
-    source_lv=None,
-    snapshot=False,
-    verbosity=False,
-    verbose=True,
+def thin_delta(  # noqa: ANN201
+    thin1,  # noqa: ANN001
+    thin2,  # noqa: ANN001
+    source_file=None,  # noqa: ANN001
+    source_vg=None,  # noqa: ANN001
+    source_lv=None,  # noqa: ANN001
+    snapshot=False,  # noqa: ANN001
+    verbosity=False,  # noqa: ANN001
+    verbose=True,  # noqa: ANN001
 ):
     """Print the differences in the mappings between two thin devices.
     The arguments are:
     source_vg VG name
     source_lv LV name
     thin1 numeric identificator of first thin volume
     thin2 numeric identificator of second thin volume
@@ -1019,64 +1019,64 @@
     Boolean:
     True if success
     False in case of failure.
     """
     options = ""
 
     if not source_file and (not source_vg or not source_lv):
-        sts_print("FAIL: thin_delta requires either source_file OR source_vg and source_lv.")
+        print("FAIL: thin_delta requires either source_file OR source_vg and source_lv.")
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            sts_print("FAIL: Source file is not a file.")
+            print("FAIL: Source file is not a file.")
             return False
         device = source_file
 
     if snapshot:
         if isinstance(snapshot, bool):
             options += "--metadata-snap "
         elif isinstance(snapshot, int):
             options += f"--metadata-snap {snapshot} "
         else:
-            sts_print("FAIL: Unknown snapshot value, use either Boolean or Int.")
+            print("FAIL: Unknown snapshot value, use either Boolean or Int.")
             return False
 
     if verbosity:
         options += "--verbose"
 
     if _get_dev_id(thin1, source_file, source_lv, source_vg) and _get_dev_id(thin2, source_file, source_lv, source_vg):
         cmd = f"thin_delta {options} --thin1 {thin1} --thin2 {thin2} {device}"
         retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
-            sts_print("FAIL: Could not get differences in mappings between two thin LVs.")
+            print("FAIL: Could not get differences in mappings between two thin LVs.")
             return False
     else:
-        sts_print("FAIL: Specified id does not exist.")
+        print("FAIL: Specified id does not exist.")
         return False
     return True
 
 
 class DMPD(Wrapper):
-    def __init__(self, disable_check=True):
+    def __init__(self, disable_check=True) -> None:  # noqa: ANN001
         self.disable_check = disable_check
 
         pkg = "device-mapper-persistent-data"
         if not linux.is_installed(pkg) and not linux.install_package(pkg, check=False):
-            sts_print(f"FATAL: Could not install {pkg} package")
+            print(f"FATAL: Could not install {pkg} package")
 
-        self.commands = {
+        self.commands: Dict[str, Union[str, List[str]]] = {
             "cache_check": "cache_check",
             "cache_dump": "cache_dump",
             "cache_metadata_size": "cache_metadata_size",
             "cache_repair": "cache_repair",
             "cache_restore": "cache_restore",
             "cache_writeback": "cache_writeback",
             "thin_check": "thin_check",
@@ -1161,109 +1161,109 @@
             "thin2": [["thin_delta"], " --thin2&"],
             "unit": [["thin_metadata_size"], " --unit&"],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
-    def _remove_nones(kwargs):
+    def _remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
-    def _get_possible_arguments(self, command=None):
+    def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
         return super()._get_possible_arguments(command.split()[0])
 
-    def _run(self, cmd, verbosity=True, **kwargs):
+    def _run(self, cmd, verbosity=True, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
         cmd = self._add_arguments(cmd, **kwargs)
 
         ret = run(cmd, verbose=verbosity).returncode
         if isinstance(ret, tuple) and ret[0] != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+            print(f"WARN: Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
-    def cache_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def cache_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "cache_check "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def cache_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def cache_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "cache_dump "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def cache_metadata_size(self, **kwargs):
+    def cache_metadata_size(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "cache_metadata_size "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def cache_repair(self, **kwargs):
+    def cache_repair(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "cache_repair "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def cache_restore(self, **kwargs):
+    def cache_restore(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "cache_restore "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def cache_writeback(self, **kwargs):
+    def cache_writeback(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "cache_writeback "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def thin_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "thin_check "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_delta(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def thin_delta(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "thin_delta "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def thin_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "thin_dump "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_ls(self, source_vg=None, source_lv=None, **kwargs):
+    def thin_ls(self, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "thin_ls "
         if source_vg and source_lv:
             cmd += _get_device_path(source_vg, source_lv)
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_metadata_size(self, **kwargs):
+    def thin_metadata_size(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "thin_metadata_size "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_repair(self, **kwargs):
+    def thin_repair(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "thin_repair "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_restore(self, **kwargs):
+    def thin_restore(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "thin_restore "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_rmap(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
+    def thin_rmap(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "thin_rmap "
         if source_file:
             cmd += f"{source_file} "
         if source_vg and source_lv:
             cmd += f"{_get_device_path(source_vg, source_lv)} "
         return self._run(cmd, **self._remove_nones(kwargs))
 
-    def thin_trim(self, **kwargs):
+    def thin_trim(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "thin_trim "
         return self._run(cmd, **self._remove_nones(kwargs))
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/fc.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/fc.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,42 +5,41 @@
 
 import os
 import os.path
 import re  # regex
 from pathlib import Path
 
 from sts import linux, scsi
-from sts.utils import sts_print
 from sts.utils.cmdline import run_ret_out
 
 host_path = "/sys/class/fc_host/"
 
 remote_port_path = "/sys/class/fc_remote_ports/"
 
 regex_target_id = re.compile(r"target(\d+):(\d+):(\d+)")
 regex_target = re.compile(r"(\d+):(\d+):(\d+)")
 wwn_regex = re.compile(r"(?:[0-9a-f]{2}:){7}[0-9a-f]{2}")
 
 
-def is_wwn(wwn):
+def is_wwn(wwn):  # noqa: ANN001, ANN201
     """Checks if the entry is on valid WWN format.
     example: 10:00:5c:b9:01:c1:ec:71
     The arguments are:
     a WWN
     Returns:
     True if it is a valid WWN
     False if the entry is not valid.
     """
     m = wwn_regex.match(wwn)
     if m:
         return True
     return False
 
 
-def standardize_wwpn(wwpn):
+def standardize_wwpn(wwpn):  # noqa: ANN001, ANN201
     """Usage
         standardize_wwpn(wwpn)
     Purpose
         Convert all possible format wwpn into stand type:
             (?:[0-9a-f]{2}:){7}[0-9a-f]{2} #like: 10:00:00:00:c9:95:2f:de
         Return STRING or ARRAY base on context.
     Parameter
@@ -59,15 +58,15 @@
     # append ":" every 2nd character
     wwpn = ":".join(wwpn[i : i + 2] for i in range(0, len(wwpn), 2))
     if is_wwn(wwpn):
         return wwpn
     return None
 
 
-def query_all_fc_disks(host_id=None):
+def query_all_fc_disks(host_id=None):  # noqa: ANN001, ANN201
     """Return SCSI disk info all all FC/FCoE devices."""
     hosts = get_fc_hosts()
     if not hosts:
         # there is no FC/FCoE session
         return None
 
     if host_id:
@@ -78,85 +77,85 @@
     for scsi_id in list(scsi_disks.keys()):
         scsi_disk = scsi_disks[scsi_id]
         if scsi_disk["host_id"] in hosts:
             fc_disks[scsi_id] = scsi_disk
     return fc_disks
 
 
-def scsi_wwid_of_fc_disks():
+def scsi_wwid_of_fc_disks():  # noqa: ANN201
     """Return a list of all WWIDs of FC/FCoE disks."""
     disks_info = query_all_fc_disks()
     if not disks_info:
         return None
     wwids = []
     for info in list(disks_info.values()):
         if "wwid" not in list(info.keys()):
             continue
         if info["wwid"] and info["wwid"] not in wwids:
             wwids.append(info["wwid"])
     return wwids
 
 
-def is_fc_boot():
+def is_fc_boot():  # noqa: ANN201
     """Check if it boots from FC/FCoE device."""
     fc_wwids = scsi_wwid_of_fc_disks()
     if not fc_wwids:
         return False
 
     boot_dev = linux.get_boot_device()
     if not boot_dev:
-        sts_print("FAIL: is_fc_boot() - Could not determine boot device")
+        print("FAIL: is_fc_boot() - Could not determine boot device")
         return False
 
     boot_wwid = linux.get_device_wwid(boot_dev)
     if not boot_dev:
-        sts_print(f"WARN: is_fc_boot() - Could not determine boot WWID for {boot_dev}")
+        print(f"WARN: is_fc_boot() - Could not determine boot WWID for {boot_dev}")
         return False
 
     if boot_wwid in fc_wwids:
         return True
 
     return False
 
 
 # Return an array with all fc_hosts numbers
-def get_fc_hosts():
+def get_fc_hosts():  # noqa: ANN201
     cmd = "ls " + host_path
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     # remove 'host' prefix
     output = re.sub("host", "", output)
     return output.split()
 
 
-def get_fc_host_wwpn(host):
+def get_fc_host_wwpn(host):  # noqa: ANN001, ANN201
     """Return the WWPN of specific sts."""
     host_port_path = f"/sys/class/fc_host/host{host}/port_name"
     cmd = "cat " + host_port_path
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
-def fc_host_id_of_wwpn(wwpn):
+def fc_host_id_of_wwpn(wwpn):  # noqa: ANN001, ANN201
     """Given a WWPN, return its host id."""
     if not wwpn:
-        sts_print("FAIL: fc_host_id_of_wwpn() - requires wwpn parameter")
+        print("FAIL: fc_host_id_of_wwpn() - requires wwpn parameter")
         return None
     fc_hosts = get_fc_hosts()
     for fc_host in fc_hosts:
         if get_fc_host_wwpn(fc_host) == wwpn:
             return fc_host
 
     return None
 
 
-def h_wwpn_of_host(host=None):
+def h_wwpn_of_host(host=None):  # noqa: ANN001, ANN201
     """h_wwpn_of_host
     Usage:
         h_wwpn_of_host(host)
         h_wwpn_of_host()
     Purpose:
         Return a list with the WWPN of specific host
         If no host is given return all WwPNs
@@ -177,38 +176,38 @@
         if wwpn:
             if not wwpns:
                 wwpns = []
             wwpns.append(wwpn)
     return wwpns
 
 
-def get_rports():
+def get_rports():  # noqa: ANN201
     rports = os.listdir(remote_port_path)
     if not rports:
         return None
     return rports
 
 
-def get_fc_host_remote_ports(host):
+def get_fc_host_remote_ports(host):  # noqa: ANN001, ANN201
     cmd = f"ls {remote_port_path} | grep rport-{host}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output.split()
 
 
-def wwpn_of_rport(r_port):
+def wwpn_of_rport(r_port):  # noqa: ANN001, ANN201
     cmd = f"cat {remote_port_path}/{r_port}/port_name"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
-def rport_of_h_wwpn_t_wwpn(h_wwpn, t_wwpn):
+def rport_of_h_wwpn_t_wwpn(h_wwpn, t_wwpn):  # noqa: ANN001, ANN201
     """Return the remote port of given wwpn
     Return:
         r_port       #like rport-7:0-0
             or
         None.
     """
     h_wwpn = standardize_wwpn(h_wwpn)
@@ -226,24 +225,24 @@
     host_rports = get_fc_host_remote_ports(host_id)
     if not host_rports:
         return None
 
     for rport in host_rports:
         r_wwpn = wwpn_of_rport(rport)
         if not r_wwpn:
-            # sts_print("FAIL: rport_of_h_wwpn_t_wwpn() - Could not get wwpn of rport %s" % rport)
+            # print("FAIL: rport_of_h_wwpn_t_wwpn() - Could not get wwpn of rport %s" % rport)
             continue
         if t_wwpn == r_wwpn:
             return rport
     return None
 
 
-def fc_target_id_of_wwpn(wwpn):
+def fc_target_id_of_wwpn(wwpn):  # noqa: ANN001, ANN201
     if not wwpn:
-        sts_print("FAIL: fc_target_id_of_wwpn() - requires wwpn parameter")
+        print("FAIL: fc_target_id_of_wwpn() - requires wwpn parameter")
         return None
     t_ids = None
 
     # Get target id of all ports
     rport_id_2_target_id_dict = rport_id_2_target_id()
     if not rport_id_2_target_id_dict:
         return None
@@ -262,15 +261,15 @@
                     t_ids = []
                 if r_port in list(rport_id_2_target_id_dict.keys()):
                     t_ids.append(rport_id_2_target_id_dict[r_port])
 
     return t_ids
 
 
-def t_wwpn_of_host(host=None):
+def t_wwpn_of_host(host=None):  # noqa: ANN001, ANN201
     """t_wwpn_of
     Usage:
         t_wwpn_of(host)
         t_wwpn_of()
     Purpose:
         Return a list with the WWPN of targets of specific host
         If no host is given return all WwPNs
@@ -292,58 +291,58 @@
 
     for host in hosts:
         r_ports = get_fc_host_remote_ports(host)
         if r_ports:
             for r_port in r_ports:
                 wwpn = wwpn_of_rport(r_port)
                 if not wwpn:
-                    # sts_print("FAIL: Could not find wwpn for r_port %s" % r_port)
+                    # print("FAIL: Could not find wwpn for r_port %s" % r_port)
                     continue
                 if wwpn in h_wwpns:
                     # We actually found our own WWPN, skip it
                     continue
                 if not wwpns:
                     wwpns = []
                 if wwpn not in wwpns:
                     wwpns.append(wwpn)
     return wwpns
 
 
-def fc_target_id_of_htwwpn(t_wwpn=None, h_wwpn=None):
+def fc_target_id_of_htwwpn(t_wwpn=None, h_wwpn=None):  # noqa: ANN001, ANN201
     """Usage
         fc_target_id_of_htwwpn(h_wwpn=>h_wwpn, t_wwpn=>t_wwpn)
     Purpose
         Query out the target_id came from h_wwpn and t_wwpn. If FC has FSPF,
         protocol, we will only have ONE target_id for 1 combination.
     Parameter
         h_wwpn         # Host HBA WWPN
         t_wwpn         # Storage Array front point WWPN
     Returns
         target_id      # like "0:1:0"
             or
         None           # error.
     """
     if not t_wwpn or not h_wwpn:
-        sts_print("FAIL: fc_target_id_of_htwwpn() - requires t_wwpn and h_wwpn parameters")
+        print("FAIL: fc_target_id_of_htwwpn() - requires t_wwpn and h_wwpn parameters")
         return None
 
     scsi_host_id = fc_host_id_of_wwpn(h_wwpn)
     target_ids = fc_target_id_of_wwpn(t_wwpn)
     if not target_ids:
-        sts_print("FAIL: fc_target_id_of_htwwpn(): No FC target assigned to target WWPN {t_wwpn}")
+        print("FAIL: fc_target_id_of_htwwpn(): No FC target assigned to target WWPN {t_wwpn}")
         return None
 
     for t_id in target_ids:
         m = regex_target.match(t_id)
         if m and scsi_host_id == m.group(1):
             return t_id
     return None
 
 
-def scsi_disk_of_htwwpn_wwid(h_wwpn, t_wwpn, wwid):
+def scsi_disk_of_htwwpn_wwid(h_wwpn, t_wwpn, wwid):  # noqa: ANN001, ANN201
     """Get the scsi disk name connected to specific host and target port and has
     given wwid.
     """
     if not h_wwpn or not t_wwpn or not wwid:
         print("FAIL: scsi_disk_of_htwwpn_wwid() - requires h_wwpn, t_wwpn and wwid as parameters")
         return None
 
@@ -355,43 +354,43 @@
     if not scsi_disk_ids:
         return False
 
     for scsi_disk_id in scsi_disk_ids:
         if re.match(r"%s:\d+$" % target_id, scsi_disk_id):
             disk_name = scsi.get_scsi_disk_name(scsi_disk_id)
             if not disk_name:
-                sts_print(f"FAIL: Could not get SCSI disk name of: {scsi_disk_id}")
+                print(f"FAIL: Could not get SCSI disk name of: {scsi_disk_id}")
                 return False
             return disk_name
     return None
 
 
-def get_fc_host_rport_targets(host, r_port):
+def get_fc_host_rport_targets(host, r_port):  # noqa: ANN001, ANN201
     cmd = f"ls /sys/bus/scsi/devices/host{host}/{r_port} | grep target"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     output = re.sub("target", "", output)
     return output.split()
 
 
-def get_fc_host_rport_target_devices(host, r_port, target):
+def get_fc_host_rport_target_devices(host, r_port, target):  # noqa: ANN001, ANN201
     if not host or not r_port or not target:
-        sts_print("FAIL: get_fc_host_rport_target_devices. Usage: host, r_port, target")
+        print("FAIL: get_fc_host_rport_target_devices. Usage: host, r_port, target")
         return None
 
     cmd = f'ls /sys/bus/scsi/devices/host{host}/{r_port}/target{target} | grep "{target}"'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     output = re.sub("target", "", output)
     return output.split()
 
 
-def rport_id_2_target_id():
+def rport_id_2_target_id():  # noqa: ANN201
     """Usage
         rport_id_2_target_id()
     Purpose
         For lpfc card, their rport_id is different from target_id.
         This function will return this reference:
             rport_id_2_target_id = {
                 rport_id : target_id
@@ -422,17 +421,17 @@
                 if not rport_id_2_target_id_dict:
                     rport_id_2_target_id_dict = {}
                 rport_id_2_target_id_dict[rport] = f"{m.group(1)}:{m.group(2)}:{m.group(3)}"
 
     return rport_id_2_target_id_dict
 
 
-def fc_host_transport_type(scsi_host_id):
+def fc_host_transport_type(scsi_host_id):  # noqa: ANN001, ANN201
     if not scsi_host_id:
-        sts_print("FAIL: fc_host_transport_type - requires scsi_host_id")
+        print("FAIL: fc_host_transport_type - requires scsi_host_id")
         return None
 
     host_model2transport = {
         "QLE2462": "FC",
         "QLE2772": "FC",
         "QLE8262": "FCoE",
         "QLE8362": "FCoE",
@@ -492,53 +491,53 @@
             return "FC"
         if fcoe_regex.search(host_info["symbolic_name"]):
             return "FCoE"
 
     if "driver" in list(host_info.keys()) and host_info["driver"] in ["bnx2fc", "qedf"]:
         return "FCoE"
 
-    sts_print(f"DEBUG: Could not figure out if controller {scsi_host_id} is FC or FCoE")
+    print(f"DEBUG: Could not figure out if controller {scsi_host_id} is FC or FCoE")
     print(host_info)
     return "(TODO)FC/FCoE"
 
 
-def get_value_rport_parameter(r_port, r_port_param):
+def get_value_rport_parameter(r_port, r_port_param):  # noqa: ANN001, ANN201
     """Usage
         get_value_rport_parameter(r_port, r_port_param)
     Purpose
         Query out the r_port_param via sys:
         /sys/class/fc_remote_ports/rport-3:0-0/dev_loss_tmo
     Parameters
         r_port:         # like "rport0:0-1"
         r_port_param    # like "dev_loss_tmo"
     Returns
         parameter value
             or
         None.
     """
     if not r_port or not r_port_param:
-        sts_print("FAIL: get_value_rport_parameter() - requires r_port and r_port_param as parameter")
+        print("FAIL: get_value_rport_parameter() - requires r_port and r_port_param as parameter")
         return None
 
     sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
     if not Path(sys_r_port_param).is_file():
-        sts_print(f"FAIL: get_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
+        print(f"FAIL: get_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return None
 
     ret, value = run_ret_out(f"cat {sys_r_port_param}", return_output=True, verbose=False)
     if ret != 0:
-        sts_print(f"FAIL: get_value_rport_parameter() - Could not read {sys_r_port_param}")
+        print(f"FAIL: get_value_rport_parameter() - Could not read {sys_r_port_param}")
         # print command output
         print(value)
         return None
 
     return value
 
 
-def set_value_rport_parameter(r_port, r_port_param, value):
+def set_value_rport_parameter(r_port, r_port_param, value):  # noqa: ANN001, ANN201
     """Usage
         set_value_rport_parameter(r_port, r_port_param, value)
     Purpose
         Write value to r_port_param via sys:
         /sys/class/fc_remote_ports/rport-3:0-0/dev_loss_tmo
     Parameters
         r_port:         # like "rport-0:0-1"
@@ -546,22 +545,22 @@
         value           # like "60"
     Returns
         True
             or
         False.
     """
     if not r_port or not r_port_param or value is None:
-        sts_print("FAIL: set_value_rport_parameter() - requires r_port, r_port_param and value as parameter")
+        print("FAIL: set_value_rport_parameter() - requires r_port, r_port_param and value as parameter")
         return False
 
     sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
     if not Path(sys_r_port_param).is_file():
-        sts_print(f"FAIL: set_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
+        print(f"FAIL: set_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return False
 
     ret, output = run_ret_out(f"echo {value} > {sys_r_port_param}", return_output=True, verbose=False)
     if ret != 0:
-        sts_print(f"FAIL: set_value_rport_parameter() - Could not set {sys_r_port_param} to {value}")
+        print(f"FAIL: set_value_rport_parameter() - Could not set {sys_r_port_param} to {value}")
         # print command output
         print(output)
         return False
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/fio.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/fio.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import os
 import subprocess
 import sys
 
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.cmdline import exists, run, run_ret_out
 
 fio_default_options = {
     "rw": "randrw",  # Type of I/O pattern. Supported(read, write, trim, randread, randwrite, rw, randrw, trimwrite)
     "name": "fio_test",  # signalling the start of a new job.
     "filename": None,  # device or filename
     "direct": 1,  # If true, use non-buffered I/O (usually O_DIRECT)
@@ -32,52 +31,52 @@
     # Set to None to verify after all IO is written
     "verify_fatal": 1,  # If true, exit the job on the first observed verification failure
     "do_verify": 1,
     "verify": "crc32c",
 }
 
 
-def install_fio():
+def install_fio():  # noqa: ANN201
     pkg = "fio"
     if linux.install_package(pkg):
         return True
     if run("fio >/dev/null 2>&1").returncode == 1:
         return True
     # Try to install FIO from source
     return install_fio_from_src()
 
 
-def install_fio_from_src():
+def install_fio_from_src():  # noqa: ANN201
     git_url = "git://git.kernel.org/pub/scm/linux/kernel/git/axboe/fio.git"
 
     if not linux.install_package("libaio-devel"):
-        sts_print("FAIL: Could not install libaio-devel")
+        print("FAIL: Could not install libaio-devel")
         return False
 
     if not linux.install_package("zlib-devel"):
-        sts_print("FAIL: Could not install zlib-devel")
+        print("FAIL: Could not install zlib-devel")
         return False
 
     if run(f"git clone {git_url}").returncode != 0:
-        sts_print("FAIL: Could not clone fio repo")
+        print("FAIL: Could not clone fio repo")
         return False
 
-    sts_print("INFO: Installing FIO")
+    print("INFO: Installing FIO")
     if run("cd fio && ./configure && make && make install").returncode != 0:
-        sts_print("FAIL: Could not build fio")
+        print("FAIL: Could not build fio")
         return False
 
     if not exists("fio"):
-        sts_print("FAIL: FIO did not install properly")
+        print("FAIL: FIO did not install properly")
         return False
     return True
 
 
 # TODO: rewrite to cmdline.run()
-def fio_stress(of, verbose=False, return_output=False, **fio_opts):
+def fio_stress(of, verbose=False, return_output=False, **fio_opts):  # noqa: ANN001, ANN003, ANN201
     # For compatibility with tests using other named parameters
     convert_param = {
         "io_type": "rw",
         "time": "runtime",
         "thread": "numjobs",
         "log_file": "output",
     }
@@ -95,15 +94,15 @@
     if int(fio_opts["numjobs"]) > 1:
         fio_opts["group_reporting"] = 1
 
     if fio_opts["verify"] is not None:
         fio_opts.update(fio_default_verify_options)
 
     if not exists("fio"):
-        sts_print("FATAL: fio is not installed")
+        print("FATAL: fio is not installed")
         return False
 
     fio_param = ""
     for key in list(fio_opts.keys()):
         if fio_opts[key]:
             fio_param += f"--{key}='{fio_opts[key]}' "
 
@@ -114,40 +113,40 @@
     # Append time information to command
     date = 'date "+%Y-%m-%d %H:%M:%S"'
     p = subprocess.Popen(date, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     stdout, _ = p.communicate()
     stdout = stdout.decode("ascii", "ignore")
     stdout = stdout.rstrip("\n")
     if not verbose:  # If verbose option is selected, the run() will print the fio command.
-        sts_print(f"INFO: [{stdout}] FIO Running: '{cmd}'...")
+        print(f"INFO: [{stdout}] FIO Running: '{cmd}'...")
 
-    # sts_print("INFO: Running %s" % cmd)
+    # print("INFO: Running %s" % cmd)
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print("FAIL: running FIO")
+        print("FAIL: running FIO")
         print(output)
         if return_output:
             return False, None
         return False
 
-    sts_print("INFO: FIO executed successfully")
+    print("INFO: FIO executed successfully")
     if return_output:
         return True, output
 
     return True
 
 
-def fio_stress_background(of, verbose=False, **fio_opts):
+def fio_stress_background(of, verbose=False, **fio_opts):  # noqa: ANN001, ANN003, ANN201
     """Run FIO on background."""
     newpid = os.fork()
     if newpid == 0:
         # Trying to flush stdout to avoid duplicated lines when running hba_test
         sys.stdout.flush()
         rt = fio_stress(of, verbose=verbose, **fio_opts)
         if not rt:
             os._exit(1)  # noqa: SLF001
         os._exit(0)  # noqa: SLF001
         return None
 
     sys.stdout.flush()
-    sts_print("INFO: fio_stress_background(): Child thread %d is running FIO Stress" % newpid)
+    print("INFO: fio_stress_background(): Child thread %d is running FIO Stress" % newpid)
     return newpid
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/iscsi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """iscsi.py: Module with methods for iSCSI initiator."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
-import subprocess
 from ast import literal_eval
 from os import getenv
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Union
+from typing import ClassVar, Dict, List, Literal, Optional, Union
 
 from sts import linux, mp, net, scsi
-from sts.utils import sts_print
-from sts.utils.cmdline import run, run_ret_out
+from sts.utils.cmdline import StsCompletedProcess, run, run_ret_out
 
 PACKAGE_NAME = "iscsi-initiator-utils"
 CLI_NAME = "iscsiadm"
 ISCSID_SERVICE_NAME = "iscsid"
 ISCSIUIO_SERVICE_NAME = "iscsiuio"
 
 
@@ -24,38 +22,38 @@
     """Class for `iscsiadm` cli tool (iscsi-initiator-utils)."""
 
     def __init__(
         self,
         debug_level: Literal[0, 1, 2, 3, 4, 5, 6, 7, 8] = 0,
         disable_check: bool = False,
         verbose: bool = True,
-    ):
+    ) -> None:
         """Args:
         debug_level: print iscsiadm debug info (0-8)
         disable_check: disable argument validation.
         """
         self.disable_check = disable_check
         self.debug_level = debug_level
         self.verbose = verbose
 
         if not linux.install_package(PACKAGE_NAME, check=True, verbose=self.verbose):
-            sts_print(f"FATAL: Could not install {PACKAGE_NAME}")
+            print(f"FATAL: Could not install {PACKAGE_NAME}")
 
     # available modes and respective short options available as per iscsiadm.c
-    MODES: Dict[str, str] = {
+    MODES: ClassVar[Dict[str, str]] = {
         "discovery": "DSIPdntplov",
         "discoverydb": "DSIPdntplov",
         "node": "RsPIdlSonvupTULW",
         "session": "PiRdrusonuSv",
         "host": "CHdPotnvxA",
         "iface": "HIdnvPoCabci",
         "fw": "dlWnv",
     }
 
-    OPTIONS: Dict[str, str] = {
+    OPTIONS: ClassVar[Dict[str, str]] = {
         "p": "portal",
         "T": "targetname",
         "I": "interface",
         "o": "op",
         "t": "type",
         "n": "name",
         "v": "value",
@@ -90,92 +88,95 @@
         Args:
           mode: Example: "discovery"
         """
         if mode not in self.MODES:
             err_msg = f"Invalid {CLI_NAME} mode: {mode}"
             raise ValueError(err_msg)
 
-    def validate_arguments(self, mode: str, arguments) -> None:
-        available_options: list = self.get_short_options_list(mode) + self.get_long_options_list(mode)
+    def validate_arguments(self, mode: str, arguments: Union[Dict[str, str], Dict[str, Optional[str]]]) -> None:
+        available_options: List[str] = self.get_short_options_list(mode) + self.get_long_options_list(mode)
         for key, _value in arguments.items():
             key_to_check = key.strip("-")
             if key_to_check not in available_options:
                 err_msg = f"Invalid {CLI_NAME} argument: {key}"
                 raise ValueError(err_msg)
 
-    def get_short_options_list(self, mode) -> list:
+    def get_short_options_list(self, mode: str) -> List[str]:
         if mode not in self.MODES.keys():
             raise ValueError
         return [*self.MODES[mode]]
 
-    def get_long_options_list(self, mode: str) -> list:
+    def get_long_options_list(self, mode: str) -> List[str]:
         if mode not in self.MODES.keys():
             raise ValueError
         return [self.OPTIONS[short_option] for short_option in [*self.MODES[mode]]]
 
     def available_options(self, mode: str) -> List[str]:
         return self.get_short_options_list(mode) + self.get_long_options_list(mode)
 
     def _run(
         self,
         mode: str = "",
-        capture_output: bool = False,
         arguments: Optional[Union[Dict[str, str], Dict[str, Optional[str]]]] = None,
         timeout: Union[int, None] = None,
-    ) -> subprocess.CompletedProcess:
+    ) -> StsCompletedProcess:
         if mode is not None:
             self.validate_mode(mode)
         if arguments is not None and self.disable_check is not True:
             self.validate_arguments(mode, arguments)
 
-        command_list: list = [CLI_NAME, "--mode", mode]
+        command_list: List[str] = [CLI_NAME, "--mode", mode]
         if arguments is not None:
             command_list = command_list + [f"{k}" if v is None else f"{k} {v}" for k, v in arguments.items()]
         if self.debug_level:
             command_list = [*command_list, "--debug", str(self.debug_level)]
         command: str = " ".join(command_list)
+        return run(command, capture_output=True, timeout=timeout, verbose=self.verbose)
 
-        return run(command, capture_output=capture_output, timeout=timeout, verbose=self.verbose)
-
-    def iface(self, op: str, iface: str, name: Optional[str] = None, value: Optional[str] = None, capture_output=True):
+    def iface(
+        self,
+        op: str,
+        iface: str,
+        name: Optional[str] = None,
+        value: Optional[str] = None,
+    ) -> StsCompletedProcess:
         return self._run(
             mode="iface",
-            capture_output=capture_output,
             arguments={"-o": op, "-n": name, "-v": value, "-I": iface},
         )
 
-    def iface_update(self, iface: str, name: str, value: str):
+    def iface_update(self, iface: str, name: str, value: str) -> StsCompletedProcess:
         return self.iface(op="update", iface=iface, name=f"iface.{name}", value=value)
 
-    def iface_update_iqn(self, iface: str, iqn: str):
+    def iface_update_iqn(self, iface: str, iqn: str) -> StsCompletedProcess:
         return self.iface_update(iface=iface, name="initiatorname", value=iqn)
 
-    def iface_update_ip(self, iface: str, ip: str):
+    def iface_update_ip(self, iface: str, ip: str) -> StsCompletedProcess:
         return self.iface_update(iface=iface, name="iface.ipaddress", value=ip)
 
     def discovery(
         self,
         portal: str,
         discovery_type: str = "st",
         iface: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: str,
+    ) -> StsCompletedProcess:
         arguments = {"-t": discovery_type, "-p": portal, **kwargs}
         if iface:
             arguments.update({"-I": iface})
         return self._run(mode="discovery", arguments=arguments)
 
-    def node(self, **kwargs):
+    def node(self, **kwargs: Union[str, Optional[str]]) -> StsCompletedProcess:
         return self._run(mode="node", arguments={**kwargs})
 
-    def node_login(self, **kwargs):
+    def node_login(self, **kwargs: str) -> StsCompletedProcess:
         arguments = {"--login": None, **kwargs}
         return self.node(**arguments)
 
-    def node_logout(self, **kwargs):
+    def node_logout(self, **kwargs: str) -> StsCompletedProcess:
         arguments = {"--logout": None, **kwargs}
         return self.node(**arguments)
 
 
 def get_env_vars() -> dict:
     """Parse general environmental variables needed for iscsi initiator
     Accepts following env vars:
@@ -197,23 +198,23 @@
         print(f"INFO: Detected target portal: {target_portal}")
 
     iface_data: Optional[str] = getenv("ISCSI_IFACES")
     if iface_data:
         iqn_in_iface_vars = True  # Setting back to False below, in case at least one iface does not have iqn
         ifaces: List[dict] = literal_eval(iface_data)
         vars_to_return.update({"ifaces": ifaces})
-        sts_print("INFO: Detected ifaces:")
+        print("INFO: Detected ifaces:")
         for iface_dict in ifaces:
             print(iface_dict)
             if "iqn" not in iface_dict:
                 iqn_in_iface_vars = False
 
     # Check if we have necessary initiator iqns
     if not initiatorname and not iqn_in_iface_vars:
-        sts_print("WARN: No iSCSI initiator iqn specified")
+        print("WARN: No iSCSI initiator iqn specified")
 
     return vars_to_return
 
 
 def setup(env_vars: Optional[dict] = None, discover_targets: bool = False) -> bool:
     """Configure iSCSI initiator based on env variables."""
     iscsiadm = IscsiAdm(verbose=True)
@@ -234,50 +235,50 @@
             if "hwaddress" in values_to_set:
                 create_iscsi_iface(iface_name=ifacename)
             for n, v in values_to_set.items():
                 completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=v)
                 ret = completed_process.returncode
                 out = completed_process.output
                 if ret != 0:
-                    sts_print(f"FAIL: iscsi update command returned {ret}. Output: {out}")
+                    print(f"FAIL: iscsi update command returned {ret}. Output: {out}")
                     return False
             if discover_targets:
                 iface_targets = iface["targets"]
                 for t in iface_targets:
                     if not t["portal"]:
-                        sts_print(f"FAIL: No portal specified for iSCSI discovery: {iface}")
+                        print(f"FAIL: No portal specified for iSCSI discovery: {iface}")
                         return False
                     if iscsiadm.discovery(iface=ifacename, portal=t["portal"]) != 0:
                         return False
     if not linux.is_service_enabled(ISCSID_SERVICE_NAME):
         linux.service_enable(ISCSID_SERVICE_NAME)
     return True
 
 
-def discovery_login(iface_name, portal, iqn, iface_ip=None, subnet_mask=None, gateway=None):
+def discovery_login(iface_name, portal, iqn, iface_ip=None, subnet_mask=None, gateway=None) -> bool:  # noqa: ANN001
     if not iface_name or not portal or not iqn:
         print("FAIL: auto_conf() - Missing iface_name, portal or iqn")
         return False
 
     if iface_ip and not iface_set_ip(iface_name, iface_ip, subnet_mask, gateway):
-        sts_print(f"FAIL: auto_conf() - Could not set IP for {iface_name}")
+        print(f"FAIL: auto_conf() - Could not set IP for {iface_name}")
         return False
 
     print("INFO: IQN will be set to " + iqn)
 
     if not iface_set_iqn(iqn, iface_name):
-        sts_print(f"FAIL: auto_conf() - Could not set {iqn} to iface {iface_name}")
+        print(f"FAIL: auto_conf() - Could not set {iqn} to iface {iface_name}")
         return False
 
     if not discovery_st(portal, ifaces=iface_name, disc_db=True):
         print(f"FAIL: auto_conf() - Could not discover any target on {portal} using iface {iface_name}")
         return False
 
     if not node_login():
-        sts_print("FAIL: auto_conf() - Could not login to new discovered portal")
+        print("FAIL: auto_conf() - Could not login to new discovered portal")
         return False
     print(f"INFO: Iface {iface_name} logged in successfully to {portal}")
 
     return True
 
 
 # used to match regex for each session information that we support
@@ -313,48 +314,48 @@
     "initial_r2t": r".*InitialR2T: (\S+)",
     "max_outst_r2t": r".*MaxOutstandingR2T: (\S+)",
 }
 
 host_path = "/sys/class/iscsi_host/"
 
 
-def is_iqn(iqn):
+def is_iqn(iqn):  # noqa: ANN001, ANN201
     if re.match(r"^iqn\.", iqn):
         return True
     return False
 
 
-def install():
+def install():  # noqa: ANN201
     """Install iscsiadm tool
     The arguments are:
     None
     Returns:
     True: If iscsiadm is installed correctly
     False: If some problem happened.
     """
     if not linux.install_package(PACKAGE_NAME):
-        sts_print(f"FAIL: Could not install {PACKAGE_NAME}")
+        print(f"FAIL: Could not install {PACKAGE_NAME}")
         return False
 
     return True
 
 
 # Return an array with all iscsi_hosts numbers
-def get_iscsi_hosts():
+def get_iscsi_hosts():  # noqa: ANN201
     cmd = "ls " + host_path
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     # remove 'host' prefix
     output = re.sub("host", "", output)
     return output.split()
 
 
 # iSCSI discovery ###
-def query_discovery():
+def query_discovery():  # noqa: ANN201
     """Query all iSCSI targets
     The arguments are:
     None
     Returns:
     Dict:    Dict with all discovered targets
     None:    If some problem happened.
     """
@@ -428,15 +429,15 @@
             discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["iface"].append(iface)
             continue
             # print "Found %s: %s" % (key, m.group(1))
 
     return discovery_info_dict
 
 
-def discovery_st(target, ifaces=None, disc_db=False):
+def discovery_st(target, ifaces=None, disc_db=False):  # noqa: ANN001, ANN201
     """Discover iSCSI target
     The arguments are:
     target:   Address of target to be discovered
     ifaces:   iSCSI interfaces to be used, separated by space (optional)
     disc_db:  To use discoverydb instead of discovery (optional).
 
     Returns:
@@ -469,29 +470,29 @@
     cmd += " -t st"
     retries = 0
     retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
     while retcode == 0 and "(err 29)" in data and retries < max_retries:
         retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
         retries += 1
     if retcode != 0 or retries == max_retries:
-        sts_print(f"FAIL: Could not discover iSCSI target. Return code: {retcode}")
+        print(f"FAIL: Could not discover iSCSI target. Return code: {retcode}")
         return False
     return True
 
 
-def is_target_discovered(t_iqn):
+def is_target_discovered(t_iqn):  # noqa: ANN001, ANN201
     """Check if an iSCSI target is already discovered
     The arguments are:
     iSCSI Target:   iQN of iSCSI target
     Returns:
     True:     If target is discovered
     False:    If was not found.
     """
     if not t_iqn:
-        sts_print("FAIL: is_target_discovered() - requires target iqn as parameter")
+        print("FAIL: is_target_discovered() - requires target iqn as parameter")
 
     disc_dict = query_discovery()
     if not disc_dict:
         return False
 
     for disc_type in list(disc_dict.keys()):
         for disc_addr in list(disc_dict[disc_type].keys()):
@@ -499,118 +500,118 @@
                 continue
             if t_iqn in list(disc_dict[disc_type][disc_addr]["targets"].keys()):
                 # Target is already discovered we do not need to do anything
                 return True
     return False
 
 
-def get_disc_ifaces_of_t_iqn(t_iqn):
+def get_disc_ifaces_of_t_iqn(t_iqn):  # noqa: ANN001, ANN201
     """From given target IQN, return the interfaces that discovered it
     The arguments are:
     iSCSI Target:   iQN of iSCSI target
     Returns:
     List ifaces:     Discovered interfaces
     None:             If iface was not found.
     """
     if not t_iqn:
-        sts_print("FAIL: get_t_iqn_disc_ifaces() - requires target iqn")
+        print("FAIL: get_t_iqn_disc_ifaces() - requires target iqn")
         return None
 
     if not is_target_discovered(t_iqn):
-        sts_print(f"FAIL: get_t_iqn_disc_ifaces() - target iqn: {t_iqn} is not discovered")
+        print(f"FAIL: get_t_iqn_disc_ifaces() - target iqn: {t_iqn} is not discovered")
         return None
 
     disc_dict = query_discovery()
     for disc_type in list(disc_dict.keys()):
         for disc_addr in list(disc_dict[disc_type].keys()):
             if "targets" not in list(disc_dict[disc_type][disc_addr].keys()):
                 continue
             if t_iqn in list(disc_dict[disc_type][disc_addr]["targets"].keys()) and "iface" in list(
                 disc_dict[disc_type][disc_addr]["targets"][t_iqn].keys(),
             ):
                 return disc_dict[disc_type][disc_addr]["targets"][t_iqn]["iface"]
     return None
 
 
-def delete_discovery_target_portal(portal, port="3260", tp="st"):
+def delete_discovery_target_portal(portal, port="3260", tp="st"):  # noqa: ANN001, ANN201
     """Delete discovered iSCSI target
     The arguments are:
     portal:   Address of target to be discovered
     port:     Port of iSCSI target to be deleted
     tp:       Discovery type, sendtargets, isns...
 
     Returns:
     True:     If deleted discovered iSCSI target
     False:    If some problem happened.
     """
-    sts_print(f"INFO: Deleting target portal: {portal}")
+    print(f"INFO: Deleting target portal: {portal}")
     if net.get_ip_version(portal) == 6:
         # IF IPv6 we need to append squared brackets to the address
         portal = "[" + portal + "]"
 
     cmd = f'iscsiadm -m discoverydb --type {tp} --portal "{portal}:{port}" -o delete'
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not delete discover iSCSI target")
+        print("FAIL: Could not delete discover iSCSI target")
         return False
     return True
 
 
-def clean_up(portal="all"):
+def clean_up(portal="all"):  # noqa: ANN001, ANN201
     """Remove iSCSI session and discover information for specific target
     The arguments are:
     target:   Address of target to be removed
     Returns:
     True:     If iSCSI target is removed
     False:    If some problem happened.
     """
     error = 0
     # TODO: iSCSI boot clean up
     if is_iscsi_boot():
         boot_dev = linux.get_boot_device()
         if not boot_dev:
-            sts_print("FAIL: clean_up() - Could not determine boot device")
+            print("FAIL: clean_up() - Could not determine boot device")
             return False
 
         boot_wwid = linux.get_device_wwid(boot_dev)
         if not boot_wwid:
-            sts_print(f"FAIL: clean_up() - Could not determine boot WWID for {boot_dev}")
+            print(f"FAIL: clean_up() - Could not determine boot WWID for {boot_dev}")
             return False
 
         ses_ids = get_all_session_ids()
         if not ses_ids:
-            sts_print("FAIL: is_iscsi_boot() - It is iSCSI boot, but did not find any session id")
+            print("FAIL: is_iscsi_boot() - It is iSCSI boot, but did not find any session id")
             return False
 
         if portal == "all":
             # Logout from all iSCSI session, that do not have boot device
             for ses_id in ses_ids:
                 iscsi_wwids = scsi_wwid_of_iscsi_session(sid=ses_id)
                 if boot_wwid in iscsi_wwids:
-                    sts_print(f"INFO: Can't log out of session {ses_id}, because it is used for iSCSI boot")
+                    print(f"INFO: Can't log out of session {ses_id}, because it is used for iSCSI boot")
                 else:
-                    sts_print(f"INFO: Logging out of session {ses_id}")
+                    print(f"INFO: Logging out of session {ses_id}")
                     session_logout(ses_id)
                     # TODO Clean up discovery info
         else:
             # TODO Logout single portal from iSCSI boot
-            sts_print(f"FAIL: clean_up() - Does not know how to clean up portal {portal} for iSCSI boot")
+            print(f"FAIL: clean_up() - Does not know how to clean up portal {portal} for iSCSI boot")
             return False
 
         return True
 
     # Not iSCSI boot
     if portal == "all":
         # log out of all iSCSI sessions
         if get_all_session_ids():  # noqa: SIM102
             # There is at least one session
             if not node_logout():
-                sts_print(f"FAIL: Could not logout from {portal} iSCSI target")
+                print(f"FAIL: Could not logout from {portal} iSCSI target")
                 error += 1
     elif not node_logout(portal=portal):
-        sts_print(f"FAIL: Could not logout from {portal} iSCSI target")
+        print(f"FAIL: Could not logout from {portal} iSCSI target")
         error += 1
 
     disc_dict = query_discovery()
     # If there is discovery information
     if disc_dict:
         # We will search for this portal on sendtargets and iSNS
         for mode in list(disc_dict.keys()):
@@ -622,15 +623,15 @@
             for addr in list(m_dict.keys()):
                 d_dict = m_dict[addr]
 
                 disc_addr = d_dict["disc_addr"]
                 port = d_dict["disc_port"]
                 if disc_addr == portal or portal == "all":  # noqa: SIM102
                     if not delete_discovery_target_portal(disc_addr, port=port, tp=d_dict["mode"]):
-                        sts_print(f"FAIL: Deleting iSCSI target {d_dict['disc_addr']}")
+                        print(f"FAIL: Deleting iSCSI target {d_dict['disc_addr']}")
                         error += 1
 
     if error:
         return False
     return True
 
 
@@ -653,43 +654,43 @@
 #            ses_dict["portal"] = m.group(3)
 #            ses_dict["portal_port"] = m.group(4)
 #            ses_dict["target_iqn"] = m.group(6)
 #            sessions[sid] = ses_dict
 #    return sessions_dict
 
 
-def get_all_session_ids():
+def get_all_session_ids():  # noqa: ANN201
     cmd = "iscsiadm -m session -P1"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        # sts_print ("INFO: there is no iSCSI session")
+        # print ("INFO: there is no iSCSI session")
         return None
     lines = output.split("\n")
 
     session_ids = []
 
     for line in lines:
         m = re.match(supported_session_info["sid"], line)
         if not m:
             continue
         # print "Found session id: %s" %m.group(1)
         session_ids.append(m.group(1))
     return session_ids
 
 
-def query_iscsi_session(sid):
+def query_iscsi_session(sid):  # noqa: ANN001, ANN201
     """Query information from a specific iSCSI session
     The arguments are:
     sid:      Session id
     Returns:
     Dict:     A dictionary with session info
     None:     If some problem happened.
     """
     if not sid:
-        sts_print("FAIL: query_iscsi_session() - requires sid as argument")
+        print("FAIL: query_iscsi_session() - requires sid as argument")
         return None
 
     regex_session_scsi_id = "^[ \t]+scsi([0-9]+) Channel ([0-9]+) Id ([0-9])+ Lun: ([0-9]+)$"
     cmd = f"iscsiadm -m session -P3 -S -r {sid}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
@@ -763,41 +764,41 @@
         session_info_dict = query_iscsi_session(sid)
         iscsi_sessions[sid] = session_info_dict
 
     # print iscsi_sessions
     return iscsi_sessions
 
 
-def session_logout(sid=None):
+def session_logout(sid=None):  # noqa: ANN001, ANN201
     cmd = "iscsiadm -m session -u"
     if sid:
         cmd += f" -r {sid}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(output)
-        sts_print("FAIL: session_logout() - Could not logout from session")
+        print("FAIL: session_logout() - Could not logout from session")
         return None
     return True
 
 
-def get_iscsi_session_by_scsi_id(scsi_id):
+def get_iscsi_session_by_scsi_id(scsi_id):  # noqa: ANN001, ANN201
     """Return the Session Dict that has the scsi_id."""
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     for ses in sessions:
         if "scsi_id_info" not in list(sessions[ses].keys()):
             continue
         if scsi_id in list(sessions[ses]["scsi_id_info"].keys()):
             return sessions[ses]
     return None
 
 
-def h_iqn_of_sessions():
+def h_iqn_of_sessions():  # noqa: ANN201
     """Usage
         h_iqn_of_sessions()
     Purpose
         Get the Host IQNs of all active iSCSI sessions
     Parameter
         None
     Returns
@@ -816,15 +817,15 @@
             if not h_iqns:
                 h_iqns = []
             if info["h_iqn"] not in h_iqns:
                 h_iqns.append(info["h_iqn"])
     return h_iqns
 
 
-def t_iqn_of_sessions():
+def t_iqn_of_sessions():  # noqa: ANN201
     """Usage
         t_iqn_of_sessions()
     Purpose
         Get the Target IQNs of all active iSCSI sessions
     Parameter
         None
     Returns
@@ -843,15 +844,15 @@
             if not t_iqns:
                 t_iqns = []
             if info["t_iqn"] not in t_iqns:
                 t_iqns.append(info["t_iqn"])
     return t_iqns
 
 
-def mac_of_iscsi_session():
+def mac_of_iscsi_session():  # noqa: ANN201
     """Usage
         mac_of_iscsi_session()
     Purpose
         We only check host IQN in active iSCSI session.
     Parameter
         None
     Returns
@@ -870,15 +871,15 @@
             if not macs:
                 macs = []
             if info["mac"] != "<empty>" and info["mac"] and info["mac"] not in macs:
                 macs.append(info["mac"])
     return macs
 
 
-def scsi_names_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):
+def scsi_names_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):  # noqa: ANN001, ANN201
     """Usage
         scsi_names_of_iscsi_session();
         scsi_names_of_iscsi_session(sid=1);
         scsi_names_of_iscsi_session(h_iqn=h_iqn, t_iqn=t_iqn);
     # we should not support this method since the h_iqn for qla4xxx
     #    scsi_names_of_iscsi_session(t_iqn=t_iqn, h_iqn=h_iqn);
         scsi_names_of_iscsi_session(iface=iface,target_ip=target_ip,;
@@ -919,19 +920,19 @@
                 sessions[sid].keys(),
             ):
                 if not scsi_names:
                     scsi_names = []
                 scsi_names.extend(list(sessions[sid]["disks"].keys()))
         return scsi_names
 
-    sts_print("FAIL: scsi_names_of_iscsi_session() - Unsupported parameters given")
+    print("FAIL: scsi_names_of_iscsi_session() - Unsupported parameters given")
     return None
 
 
-def scsi_wwid_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):
+def scsi_wwid_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):  # noqa: ANN001, ANN201
     """Usage
         scsi_wwid_of_iscsi_session();
         scsi_wwid_of_iscsi_session(sid=1);
         scsi_wwid_of_iscsi_session(h_iqn=h_iqn, t_iqn=t_iqn);
     # we should not support this method since the h_iqn for qla4xxx
     #    scsi_wwid_of_iscsi_session(t_iqn=t_iqn, h_iqn=h_iqn);
         scsi_wwid_of_iscsi_session(iface=iface,target_ip=target_ip,;
@@ -988,120 +989,120 @@
                     wwids = []
                 for scsi_name in list(sessions[sid]["disks"].keys()):
                     wwid = scsi.wwid_of_disk(scsi_name)
                     if wwid and wwid not in wwids:
                         wwids.append(wwid)
         return wwids
 
-    sts_print("FAIL: scsi_wwid_of_iscsi_session() - Unsupported parameters given")
+    print("FAIL: scsi_wwid_of_iscsi_session() - Unsupported parameters given")
     return None
 
 
-def is_iscsi_boot():
+def is_iscsi_boot():  # noqa: ANN201
     iscsi_wwids = scsi_wwid_of_iscsi_session()
     if not iscsi_wwids:
         return False
     boot_dev = linux.get_boot_device()
     if not boot_dev:
-        sts_print("FAIL: is_iscsi_boot() - Could not determine boot device")
+        print("FAIL: is_iscsi_boot() - Could not determine boot device")
         return False
 
     boot_wwid = linux.get_device_wwid(boot_dev)
     if not boot_wwid:
-        sts_print(f"WARN: is_iscsi_boot() - Could not determine boot WWID for {boot_dev}")
+        print(f"WARN: is_iscsi_boot() - Could not determine boot WWID for {boot_dev}")
         return False
 
     if boot_wwid in iscsi_wwids:
         return True
 
     return False
 
 
 # iSCSI node ###
-def node_login(options=None, target=None, portal=None, udev_wait_time=15):
+def node_login(options=None, target=None, portal=None, udev_wait_time=15):  # noqa: ANN001, ANN201
     """Login to an iSCSI portal, or all discovered portals
     The arguments are:
     arget:    iSCSI targets to be used, separated by space (optional)
     options:   extra parameters. eg: "-T <target> -p <portal>"
     Returns:
     True:     If iSCSI node is logged in
     False:    If some problem happened.
     """
     # Going to delete discovered target information
-    sts_print("INFO: Performing iSCSI login")
+    print("INFO: Performing iSCSI login")
     cmd = "iscsiadm -m node -l"
     if options:
         cmd += f" {options}"
 
     if target:
         for target_iqn in target.split():
             cmd += f" -T {target_iqn}"
 
     if portal:
         cmd += f" -p {portal}"
 
     retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
-        sts_print("FAIL: Could not login to iSCSI target")
+        print("FAIL: Could not login to iSCSI target")
         print(output)
         return False
 
     linux.wait_udev(udev_wait_time)
     return True
 
 
-def node_logout(options=None, target=None, portal=None):
+def node_logout(options=None, target=None, portal=None):  # noqa: ANN001, ANN201
     """Logout from an iSCSI node
     The arguments are:
     options:   extra parameters. eg: "-T <target> -p <portal>"
     Returns:
     True:     If iSCSI node is removed
     False:    If some problem happened.
     """
     ses_dict = query_all_iscsi_sessions()
     if not ses_dict:
         # There is no session to logout just skip
         return True
-    sts_print("INFO: Performing iSCSI logout")
+    print("INFO: Performing iSCSI logout")
     cmd = "iscsiadm -m node -u"
     if options:
         cmd += f" {options}"
 
     if target:
         cmd += f" -T {target}"
 
     if portal:
         cmd += f" -p {portal}"
 
     retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
-        sts_print("FAIL: Could not logout from iSCSI target")
+        print("FAIL: Could not logout from iSCSI target")
         print(output)
         return False
     return True
 
 
-def node_delete(options=None):
+def node_delete(options=None):  # noqa: ANN001, ANN201
     """Delete node information."""
     if not options:
-        sts_print("FAIL: node_delete() - requires portal and/or target parameters")
+        print("FAIL: node_delete() - requires portal and/or target parameters")
         return False
 
     cmd = "iscsiadm -m node -o delete"
     if options:
         cmd += f" {options}"
 
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not delete node iSCSI target")
+        print("FAIL: Could not delete node iSCSI target")
         return False
     return True
 
 
 # iSCSI iface ###
-def iface_query_all_info(iface_name=None):
+def iface_query_all_info(iface_name=None):  # noqa: ANN001, ANN201
     """Return a dict with interface names as key with detailed information of
     interface.
     """
     ifaces = [iface_name] if iface_name else get_iscsi_iface_names()
 
     if not ifaces:
         return None
@@ -1109,15 +1110,15 @@
     all_iface_dict = {}
     iface_info_regex = re.compile(r"iface\.(\S+) = (\S+)")
 
     for iface in ifaces:
         cmd = f"iscsiadm -m iface -I {iface}"
         retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print("FAIL: Could not delete node iSCSI target")
+            print("FAIL: Could not delete node iSCSI target")
             continue
         details = output.split("\n")
         for info in details:
             m = iface_info_regex.match(info)
             if not m:
                 continue
             if iface not in list(all_iface_dict.keys()):
@@ -1131,33 +1132,33 @@
         if iface_name not in list(all_iface_dict.keys()):
             return None
         return all_iface_dict[iface_name]
 
     return all_iface_dict
 
 
-def iface_update(iface, name, value):
+def iface_update(iface, name, value):  # noqa: ANN001, ANN201
     """Updates iSCSI interface parameter
     The arguments are:
     iface # Interface name (-I $)
     name  # Name of parameter (-n iface.$)
     value  # Value to set (-v $).
 
     Returns:
     True:     If value is set successfully
     False:    If some problem happened.
     """
     if not iface or not name or not value:
-        sts_print("FAIL: iface_update() - required parameters: iface, name, value")
+        print("FAIL: iface_update() - required parameters: iface, name, value")
         return False
 
     cmd = f"iscsiadm -m iface -I {iface} -o update -n iface.{name} -v {value}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: Could not set {name} to {value} on iface {iface}")
+        print(f"FAIL: Could not set {name} to {value} on iface {iface}")
         print(output)
         return False
 
     return True
 
 
 def set_initiatorname(iqn: str) -> bool:
@@ -1166,98 +1167,98 @@
     try:
         path = Path(initiatorname_file)
         if not path.is_file():
             linux.service_start(ISCSID_SERVICE_NAME)
         existing_name = path.read_text()
         if str_to_write != existing_name:
             with path.open(mode="w") as i:
-                sts_print(f"INFO: Writing {iqn} to {initiatorname_file}")
+                print(f"INFO: Writing {iqn} to {initiatorname_file}")
                 i.write(str_to_write)
                 linux.service_restart(ISCSID_SERVICE_NAME, verbose=True)
     except Exception as e:
-        sts_print(f"FAIL: Could not set iqn in {initiatorname_file}. Exception: {e}")
+        print(f"FAIL: Could not set iqn in {initiatorname_file}. Exception: {e}")
         return False
     return True
 
 
-def iface_set_iqn(iqn, iface="default"):
+def iface_set_iqn(iqn, iface="default"):  # noqa: ANN001, ANN201
     """Set IQN in /etc/iscsi/initiatorname or for specific iface
     Return:
         True
         of
         False.
     """
     if not iqn:
-        sts_print("FAIL: iface_set_iqn() - requires iqn to be set")
+        print("FAIL: iface_set_iqn() - requires iqn to be set")
         return False
 
     if iface == "default":
         set_initiatorname(iqn=iqn)
         return True
 
     iscsiadm = IscsiAdm()
     if not iscsiadm.iface_update(iface, name="initiatorname", value=iqn):
         return False
 
     return True
 
 
-def iface_set_ip(iface, ip, mask=None, gw=None):
+def iface_set_ip(iface, ip, mask=None, gw=None):  # noqa: ANN001, ANN201
     """Set IP information for specific iface
     Return:
         True
         of
         False.
     """
     if not iface or not ip:
-        sts_print("FAIL: iface_set_ip() - requires iface and ip parameters")
+        print("FAIL: iface_set_ip() - requires iface and ip parameters")
         return False
 
     if not iface_update(iface, "ipaddress", ip):
         return False
 
     if mask and not iface_update(iface, "subnet_mask", mask):
         return False
 
     if gw and not iface_update(iface, "gateway", gw):
         return False
 
     return True
 
 
-def get_iscsi_iface_names():
+def get_iscsi_iface_names():  # noqa: ANN201
     """Return a list with the name of all iSCSI interfaces on the host."""
     cmd = 'iscsiadm -m iface | cut -d " " -f 1'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not read iSCSI interfaces")
+        print("FAIL: Could not read iSCSI interfaces")
         print(output)
         return None
     ifaces = output.split("\n")
     ifaces[:] = (value for value in ifaces if "iSCSI ERROR" not in value)  # bz1997710
     return ifaces
 
 
 def set_iscsid_parameter(parameters: dict) -> bool:
     """Change parameter in iscsid.conf file and restarts iscsid service
     Use dictionary with parameter:value as argument.
     """
     filename = "/etc/iscsi/iscsid.conf"
     if not linux.edit_config(filename, parameters, list_values=False):
-        sts_print(f"FAIL: Unable to set iscsi parameters: {parameters}")
+        print(f"FAIL: Unable to set iscsi parameters: {parameters}")
         return False
 
     if not linux.service_restart(ISCSID_SERVICE_NAME):
-        sts_print("FAIL: Unable to restart iscsid service")
+        print("FAIL: Unable to restart iscsid service")
         return False
 
     return True
 
 
-def set_chap(target_user, target_pass, initiator_user=None, initiator_pass=None):
+def set_chap(target_user, target_pass, initiator_user=None, initiator_pass=None):  # noqa: ANN001, ANN201
     """Set CHAP authentication."""
     if not target_user or not target_pass:
         print("FAIL: set_chap() - requires username and password")
         return False
 
     parameters = {
         "node.session.auth.authmethod": "CHAP",
@@ -1283,15 +1284,15 @@
         print("FAIL: Unable to restart iscsid service")
         return False
 
     print("INFO: CHAP authentication enabled")
     return True
 
 
-def disable_chap():
+def disable_chap():  # noqa: ANN201
     """Disable CHAP authentication in iscsid.conf and restarts the service."""
     # Removing all previously set auth parameters.
     parameters = [
         "node.session.auth.authmethod",
         "node.session.auth.username",
         "node.session.auth.password",
         "discovery.sendtargets.auth.authmethod",
@@ -1308,15 +1309,15 @@
     if not linux.service_restart("iscsid"):
         print("FAIL: Unable to restart iscsid service")
         return False
 
     return True
 
 
-def multipath_timeo(seconds=None):
+def multipath_timeo(seconds=None):  # noqa: ANN001, ANN201
     """If multipath is used for iSCSI session, session replacement
     timeout time should be decreased from default 120 seconds
     https://access.redhat.com/solutions/1171203
     multipathd service should be running when calling this
     The arguments are:
     Seconds - default 10 or number of seconds
     Returns:
@@ -1337,37 +1338,37 @@
 
     if not set_iscsid_parameter({param: seconds}):
         return False
 
     return True
 
 
-def create_iscsi_iface(iface_name, mac=None):
+def create_iscsi_iface(iface_name: str, mac: Optional[str] = None) -> bool:
     """Create a new iSCSI interface, assign mac if specified."""
     if not iface_name:
-        sts_print("FAIL: create_iscsi_iface() - requires iface name as parameter")
+        print("FAIL: create_iscsi_iface() - requires iface name as parameter")
         return False
 
     if iface_name in get_iscsi_iface_names():
-        sts_print(f"INFO: iSCSI interface {iface_name} already exists")
+        print(f"INFO: iSCSI interface {iface_name} already exists")
         return True
     iscsiadm = IscsiAdm(verbose=True)
     retcode, output = iscsiadm.iface(op="new", iface=iface_name)
     if retcode != 0:
-        sts_print("FAIL: Could not create iSCSI interface")
+        print("FAIL: Could not create iSCSI interface")
         print(output)
         return False
 
     if mac is not None and not iscsiadm.iface_update(iface=iface_name, name="iface.hwaddress", value=mac):
         return False
 
     return True
 
 
-def clone_iscsi_iface(new_iface_name, base_iface):
+def clone_iscsi_iface(new_iface_name, base_iface):  # noqa: ANN001, ANN201
     print(f"Cloning iface: {base_iface} to {new_iface_name}")
     if not create_iscsi_iface(new_iface_name):
         return False
 
     iface_info = iface_query_all_info(base_iface)
     if iface_info is None:
         print(f"FAIL: Could not query all info about iface: {base_iface}")
@@ -1387,42 +1388,42 @@
     if iface_info["ipaddress"] is not None and not iface_update(new_iface_name, "ipaddress", iface_info["ipaddress"]):
         return False
 
     print(f"successfully cloned {base_iface}. new iface: {new_iface_name}")
     return True
 
 
-def remove_iscsi_iface(iface_name):
+def remove_iscsi_iface(iface_name):  # noqa: ANN001, ANN201
     if iface_name not in get_iscsi_iface_names():
-        sts_print(f"INFO: iSCSI interface '{iface_name}' does not exist")
+        print(f"INFO: iSCSI interface '{iface_name}' does not exist")
         return False
 
     cmd = f"iscsiadm -m iface -o delete -I {iface_name}"
     if run(cmd, verbose=False).returncode != 0:
-        sts_print("FAIL: Could not remove iSCSI interface")
+        print("FAIL: Could not remove iSCSI interface")
         return False
 
     return True
 
 
-def node_iface_info(iface_name):
+def node_iface_info(iface_name):  # noqa: ANN001, ANN201
     cmd = f"iscsiadm -m node -I {iface_name}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not get iface info!")
+        print("FAIL: Could not get iface info!")
         print(output)
         return False
 
     return True
 
 
 # iSCSI disks ###
 
 
-def get_all_iscsi_disks():
+def get_all_iscsi_disks():  # noqa: ANN201
     sessions = query_all_iscsi_sessions()
     disks = []
     if not sessions:
         # there is no iSCSI session
         return None
 
     # search for disks in each session
@@ -1431,22 +1432,22 @@
         if ses["disks"]:
             # disk names are key values
             disks.extend(list(ses["disks"].keys()))
 
     return disks
 
 
-def get_session_id_from_disk(disk_name: str):
+def get_session_id_from_disk(disk_name: str):  # noqa: ANN201
     sids = query_all_iscsi_sessions()
     fail_msg = f"FAIL: Could not find disk '{disk_name}' in iscsi sessions."
     if not sids:
-        sts_print(fail_msg)
+        print(fail_msg)
         return None
     for sid in sids:
         session = query_iscsi_session(sid)
         if not session:
-            sts_print(f"FAIL: Could not query iscsi session sid: '{sid}'.")
+            print(f"FAIL: Could not query iscsi session sid: '{sid}'.")
             continue
         if disk_name in session["disks"]:
             return session["sid"]
-    sts_print(fail_msg)
+    print(fail_msg)
     return None
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/linux.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 from pathlib import Path
 from typing import Any, List, Literal, Optional, Tuple, Union
 
 from configobj import ConfigObj
 from pkg_resources import parse_version
 
 from sts import mp, scsi
-from sts.utils import sts_print
 from sts.utils.cmdline import exists, run, run_ret_out
 
 
-def hostname():
+def hostname():  # noqa: ANN201
     ret, host = run_ret_out("hostname", verbose=False, return_output=True)
     if ret != 0:
-        sts_print("FAIL: hostname() - could not run command")
+        print("FAIL: hostname() - could not run command")
         print(host)
         return None
     return host
 
 
-def linux_distribution():
+def linux_distribution():  # noqa: ANN201
     # Not using platform module, as it doesn't provide needed information
     # on recent python3 versions
     # see: https://bugzilla.redhat.com/show_bug.cgi?id=1920385
     # see: https://bugs.python.org/issue28167
     data = {}
     with Path("/etc/os-release").open(encoding="UTF-8") as f:
         for line in f:
@@ -43,78 +42,78 @@
             if line == "":
                 continue
             k, v = line.split("=")
             data[k] = v.strip('"')
     return [data["ID"], data["VERSION_ID"]]
 
 
-def dist_release():
+def dist_release():  # noqa: ANN201
     """Find out the release number of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
     # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
-        sts_print("FAIL: Could not determine dist release!")
+        print("FAIL: Could not determine dist release!")
         return None
     return dist[1]
 
 
-def dist_ver():
+def dist_ver():  # noqa: ANN201
     """Check the distribution version."""
     release = dist_release()
     if not release:
         return None
     m = re.match(r"(\d+).\d+", release)
     if m:
         return int(m.group(1))
 
     # See if it is only digits, in that case return it
     m = re.match(r"(\d+)", release)
     if m:
         return int(m.group(1))
 
-    sts_print(f"FAIL: dist_ver() - Invalid release output {release}")
+    print(f"FAIL: dist_ver() - Invalid release output {release}")
     return None
 
 
-def dist_ver_minor():
+def dist_ver_minor():  # noqa: ANN201
     """Check the distribution minor version.
     For example: RHEL-7.4 returns 4.
     """
     release = dist_release()
     if not release:
         return None
     m = re.match(r"\d+.(\d+)", release)
     if m:
         return int(m.group(1))
 
-    sts_print(f"FAIL: dist_ver_minor() - Release does not seem to have minor version: {release}")
+    print(f"FAIL: dist_ver_minor() - Release does not seem to have minor version: {release}")
     return None
 
 
-def dist_name():
+def dist_name():  # noqa: ANN201
     """Find out the name of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
     # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
-        sts_print("FAIL: dist_name() - Could not determine dist name")
+        print("FAIL: dist_name() - Could not determine dist name")
         return None
 
     if dist[0] == "rhel":
         return "RHEL"
 
     return dist[0]
 
 
-def service_start(service_name):
+def service_start(service_name):  # noqa: ANN001, ANN201
     """Start service
     The arguments are:
     None
     Returns:
     True: Service started
     False: There was some problem.
     """
@@ -123,23 +122,23 @@
 
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} start"
 
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: Could not start {service_name}")
+        print(f"FAIL: Could not start {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
 
-def service_stop(service_name):
+def service_stop(service_name):  # noqa: ANN001, ANN201
     """Stop service
     The arguments are:
     Name of the service
     Returns:
     True: Service stopped
     False: There was some problem.
     """
@@ -148,23 +147,23 @@
 
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} stop"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not stop {service_name}")
+        print(f"FAIL: Could not stop {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
 
-def service_restart(service_name, verbose=True):
+def service_restart(service_name, verbose=True):  # noqa: ANN001, ANN201
     """Restart service
     The arguments are:
     Name of the service
     Returns:
     True: Service restarted
     False: There was some problem.
     """
@@ -179,15 +178,15 @@
     if service_timestamp is not None:
         timestamp_struct = time.strptime(service_timestamp, "%a %Y-%m-%d %H:%M:%S %Z")
         actual_time = time.localtime()
         if time.mktime(actual_time) - time.mktime(timestamp_struct) < 5:
             print("Waiting 5 seconds before restart.")
             time.sleep(5)
     if run(cmd, capture_output=False, verbose=verbose).returncode != 0:
-        sts_print(f"FAIL: Could not restart {service_name}")
+        print(f"FAIL: Could not restart {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
 
@@ -197,35 +196,35 @@
     return True
 
 
 def is_service_enabled(service_name: str) -> bool:
     return systemctl_is_enabled(f"{service_name}.service")
 
 
-def service_enable(service_name, now=False):
+def service_enable(service_name, now=False):  # noqa: ANN001, ANN201
     """Enable service
     The arguments are:
     Name of the service
     Returns:
     True: Service got enabled
     False: There was some problem.
     """
     cmd = f"systemctl enable {service_name}"
     if now:
         cmd = cmd + " --now"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not enable {service_name}")
+        print(f"FAIL: Could not enable {service_name}")
         run(f"systemctl status {service_name}")
         run("journalctl -xn")
         return False
     return True
 
 
-def service_status(service_name, verbose=True):
+def service_status(service_name, verbose=True):  # noqa: ANN001, ANN201
     """Check service status
     The arguments are:
     Name of service
     Returns:
     0 - service is running and OK
     1 - service is dead and /run pid file exists
     2 - service is dead and /lock lock file exists
@@ -239,104 +238,104 @@
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} status"
 
     retcode = run(cmd, capture_output=False, verbose=verbose).returncode
     if retcode == 0:
-        sts_print(f"INFO: Service {service_name} is running.")
+        print(f"INFO: Service {service_name} is running.")
     elif retcode == 1:
-        sts_print(f"INFO: Service {service_name} is dead and /run pid file exists.")
+        print(f"INFO: Service {service_name} is dead and /run pid file exists.")
     elif retcode == 2:
-        sts_print(f"INFO: Service {service_name} is dead and /lock lock file exists.")
+        print(f"INFO: Service {service_name} is dead and /lock lock file exists.")
     elif retcode == 3:
-        sts_print(f"INFO: Service {service_name} is not running.")
+        print(f"INFO: Service {service_name} is not running.")
     elif retcode == 4:
-        sts_print(f"INFO: Service {service_name} could not be found.")
+        print(f"INFO: Service {service_name} could not be found.")
     else:
-        sts_print(f"INFO: Service {service_name} returned unknown code {retcode}.")
+        print(f"INFO: Service {service_name} returned unknown code {retcode}.")
     return retcode
 
 
-def is_service_running(service_name):
+def is_service_running(service_name):  # noqa: ANN001, ANN201
     """Check if service is running
     The arguments are:
     Name of service
     Returns:
      True: service is running
      False: service is not running.
     """
     return service_status(service_name, verbose=False) == 0
 
 
-def os_arch():
+def os_arch():  # noqa: ANN201
     ret, arch = run_ret_out("uname -m", verbose=False, return_output=True)
     if ret != 0:
-        sts_print("FAIL: could not get OS arch")
+        print("FAIL: could not get OS arch")
         return None
 
     return arch
 
 
-def is_installed(pack, verbose=False):
+def is_installed(pack, verbose=False):  # noqa: ANN001, ANN201
     """Checks if package is installed."""
     ret, ver = run_ret_out(f"rpm -q {pack}", verbose=False, return_output=True)
     if ret == 0:
         if verbose:
             print(f"INFO: {pack} is installed ({ver})")
         return True
 
     if verbose:
         print(f"INFO: {pack} is not installed ")
     return False
 
 
-def install_package(pack, check=True, verbose=True):
+def install_package(pack, check=True, verbose=True):  # noqa: ANN001, ANN201
     """Install a package "pack" via `yum|dnf install -y`."""
     # Check if package is already installed
     if check and is_installed(pack, verbose):
         return True
 
     packmngr = "yum"
     if is_installed("dnf"):
         packmngr = "dnf"
 
     if run(f"{packmngr} install -y {pack}").returncode != 0:
         msg = f"FAIL: Could not install {pack}"
-        sts_print(msg)
+        print(msg)
         return False
 
     if verbose:
         print(f"INFO: {pack} was successfully installed")
     return True
 
 
-def package_version(pkg):
+def package_version(pkg):  # noqa: ANN001, ANN201
     """Get the version of specific package."""
     if not pkg:
-        sts_print("FAIL: package_version requires package name as parameter")
+        print("FAIL: package_version requires package name as parameter")
         return None
 
     release = dist_name().lower()
     if not release:
-        sts_print("FAIL: package_version() - Couldn't get release")
+        print("FAIL: package_version() - Couldn't get release")
         return None
     if exists("rpm"):
         ret, output = run_ret_out(
             "rpm -qa --qf='%%{version}.%%{release}' %s" % pkg,
             return_output=True,
             verbose=False,
         )
         if ret != 0:
-            sts_print(f"FAIL: Could not get version for package: {pkg}")
+            print(f"FAIL: Could not get version for package: {pkg}")
             print(output)
             return None
         return output
 
-    sts_print(f"FAIL: package_version() - Unsupported release: {release}")
+    print(f"FAIL: package_version() - Unsupported release: {release}")
     return None
 
 
 def compare_version(package: str, version: str, release: str, equal: bool = True) -> Union[bool, None]:
     """Returns 'True' if installed version is newer or equal than asked,
     'False' if older Return 'None' if the package is not installed (not found).
 
@@ -360,213 +359,213 @@
             pack.append(p)
         pkg = ".".join(pack)
     if equal:
         return parse_version(version + "." + release) <= parse_version(pkg)
     return parse_version(version + "." + release) < parse_version(pkg)
 
 
-def wait_udev(sleeptime=15):
+def wait_udev(sleeptime=15):  # noqa: ANN001, ANN201
     """Wait udev to finish. Often used after scsi rescan."""
-    sts_print("INFO: Waiting udev to finish storage scan")
+    print("INFO: Waiting udev to finish storage scan")
     # For example, on RHEL 7 scsi_wait_scan module is deprecated
     if run("modinfo scsi_wait_scan", verbose=False).returncode == 0:
         run("modprobe -q scsi_wait_scan")
         run("modprobe -r -q scsi_wait_scan")
 
     run("udevadm settle")
     sleep(sleeptime)
 
     return True
 
 
-def get_all_loaded_modules():
+def get_all_loaded_modules():  # noqa: ANN201
     """Check /proc/modules and return a list of all modules that are loaded."""
     cmd = 'cat /proc/modules | cut -d " " -f 1'
     ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
-        sts_print(f"FAIL: load_module() - Could not execute: {cmd}")
+        print(f"FAIL: load_module() - Could not execute: {cmd}")
         print(output)
         return None
 
     return output.split("\n")
 
 
-def load_module(module):
+def load_module(module):  # noqa: ANN001, ANN201
     """Run modprobe using module with parameters given as input
     Parameters:
     module:       module name and it's parameters.
     """
     if not module:
-        sts_print("FAIL: load_module() - requires module parameter")
+        print("FAIL: load_module() - requires module parameter")
         return False
     cmd = f"modprobe {module}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: load_module() - Could not execute: {module}")
+        print(f"FAIL: load_module() - Could not execute: {module}")
         return False
     return True
 
 
-def unload_module(module_name, remove_dependent=False):
+def unload_module(module_name, remove_dependent=False):  # noqa: ANN001, ANN201
     """Run rmmod to unload module
     Parameters:
     module_name:       module name.
     """
     if not module_name:
-        sts_print("FAIL: unload_module() - requires module_name parameter")
+        print("FAIL: unload_module() - requires module_name parameter")
         return False
     cmd = f"modprobe -r {module_name}"
 
     if remove_dependent:
         dep_modules = get_dependent_modules(module_name)
         if dep_modules:  # print info only if there are any modules to remove
-            sts_print(f"INFO: Removing modules dependent on {module_name}")
+            print(f"INFO: Removing modules dependent on {module_name}")
             for module in dep_modules:
                 if not unload_module(module, remove_dependent=remove_dependent):
-                    sts_print("FAIL: unload_module() - Could not unload dependent modules")
+                    print("FAIL: unload_module() - Could not unload dependent modules")
                     return False
 
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: unload_module() - Could not unload: {module_name}")
+        print(f"FAIL: unload_module() - Could not unload: {module_name}")
         return False
 
     return True
 
 
-def get_dependent_modules(module_name):
+def get_dependent_modules(module_name):  # noqa: ANN001, ANN201
     """Returns list of modules that loaded this module as a dependency
     Useful when removing parent modules (error "Module is in use by: ")
     Parameters:
     module_name:      module_name.
     """
     if not module_name:
-        sts_print("FAIL: get_dependent_modules() - requires module_name parameter")
+        print("FAIL: get_dependent_modules() - requires module_name parameter")
         return None
     cmd = f'cat /proc/modules | grep -Ew "^{module_name}" | cut -d \' \' -f 4 | tr "," " "'
     ret, dependent_modules = run_ret_out(cmd, return_output=True, verbose=False)
     if dependent_modules == "-":
         return []  # No dependent modules found
     if ret != 0:
-        sts_print("FAIL: get_dependent_modules() - failed to get a list of modules")
+        print("FAIL: get_dependent_modules() - failed to get a list of modules")
         return None
     return dependent_modules.split()
 
 
-def is_module_loaded(module_name):
+def is_module_loaded(module_name):  # noqa: ANN001, ANN201
     """Check if given module is loaded
     Parameters:
     module_name:      module_name.
     """
     if module_name in get_all_loaded_modules():
         return True
     return False
 
 
-def sleep(duration):
+def sleep(duration):  # noqa: ANN001, ANN201
     """It basically calls sys.sleep, but as stdout and stderr can be buffered
     We flush them before sleep.
     """
     sys.stdout.flush()
     sys.stderr.flush()
     time.sleep(duration)
 
 
-def is_mounted(device=None, mountpoint=None):
+def is_mounted(device=None, mountpoint=None):  # noqa: ANN001, ANN201
     """Check if mountpoint is already mounted."""
     if device and run(f"mount | grep {device}", verbose=False) != 0:
         return False
     if mountpoint and run(f"mount | grep {mountpoint}", verbose=False) != 0:
         return False
     return True
 
 
-def mount(device=None, mountpoint=None, fs=None, options=None):
+def mount(device=None, mountpoint=None, fs=None, options=None):  # noqa: ANN001, ANN201
     cmd = "mount"
     if fs:
         cmd += f" -t {fs}"
     if options:
         cmd += f" -o {options}"
     if device:
         cmd += f" {device}"
     if mountpoint:
         cmd += f" {mountpoint}"
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not mount partition")
+        print("FAIL: Could not mount partition")
         return False
 
     return True
 
 
-def umount(device=None, mountpoint=None):
+def umount(device=None, mountpoint=None):  # noqa: ANN001, ANN201
     cmd = "umount"
     if device:
         cmd += f" {device}"
         if not is_mounted(device):
             # Device is not mounted
             return True
 
     if mountpoint:
         cmd += f" {mountpoint}"
         if not is_mounted(mountpoint=mountpoint):
             # Device is not mounted
             return True
 
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not umount partition")
+        print("FAIL: Could not umount partition")
         return False
 
     return True
 
 
-def get_default_fs():
+def get_default_fs():  # noqa: ANN201
     """Return the default FileSystem for this release."""
     if dist_name() == "RHEL" and dist_ver() > 6:
         return "xfs"
 
     return "ext4"
 
 
-def run_cmd_background(cmd):
+def run_cmd_background(cmd):  # noqa: ANN001, ANN201
     """Run Command on background
     Returns:
     subprocess.
     PID is on process.pid
     Exit code is on process.returncode (after run process.communicate())
     Wait for process to finish
     while process.poll() is None:
     sleep(1)
     Get stdout and stderr
     (stdout, stderr) = process.communicate().
     """
     process = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     if not process:
-        sts_print(f"FAIL: Could not run '{cmd}' on background")
+        print(f"FAIL: Could not run '{cmd}' on background")
         return None
-    sts_print("INFO: running %s on background. PID is %d" % (cmd, process.pid))
+    print("INFO: running %s on background. PID is %d" % (cmd, process.pid))
     return process
 
 
-def kill_pid(pid):
+def kill_pid(pid):  # noqa: ANN001, ANN201
     os.kill(pid, signal.SIGTERM)
     sleep(1)
     if check_pid(pid):
         os.kill(pid, signal.SIGKILL)
         sleep(1)
         if check_pid(pid):
             return False
     return True
 
 
-def kill_all(process_name):
+def kill_all(process_name):  # noqa: ANN001, ANN201
     ret = run(f"killall {process_name}", verbose=False).returncode
     # Wait few seconds for process to finish
     sleep(3)
     return ret
 
 
-def check_pid(pid):
+def check_pid(pid):  # noqa: ANN001, ANN201
     """Check there is a process running with this PID."""
     # try:
     # #0 is the signal, it does not kill the process
     # os.kill(int(pid), 0)
     # except OSError:
     # return False
     # else:
@@ -574,133 +573,133 @@
     try:
         return os.waitpid(pid, os.WNOHANG) == (0, 0)
     except OSError as e:
         if e.errno != errno.ECHILD:
             raise
 
 
-def time_stamp(utc: bool = False, in_seconds: bool = False):
+def time_stamp(utc: bool = False, in_seconds: bool = False):  # noqa: ANN201
     now = datetime.now(tz=timezone.utc if utc else None)
 
     # ts = "%s%s%s%s%s%s" % (now.year, now.month, now.day, now.hour, now.minute, now.second)
     ts = now.strftime("%Y%m%d%H%M%S")
     if in_seconds:
         ts = now.strftime("%s")
     return ts
 
 
-def kernel_command_line():
+def kernel_command_line():  # noqa: ANN201
     """Return the kernel command line used to boot."""
     retcode, output = run_ret_out("cat /proc/cmdline", return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: could not get kernel command line")
+        print("FAIL: could not get kernel command line")
         print(output)
         return None
     return output
 
 
-def kernel_version():
+def kernel_version():  # noqa: ANN201
     """Usage
         kernel_version()
     Purpose
         Check out running kernel version. The same as output of `uname -r`
     Parameter
         N/A
     Returns
         kernel_version.
     """
     retcode, output = run_ret_out("uname -r", return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: could not get kernel version")
+        print("FAIL: could not get kernel version")
         print(output)
         return None
     # remove arch detail and kernel type
     return re.sub(r"\.%s.*" % os_arch(), "", output)
 
 
-def kernel_type():
+def kernel_type():  # noqa: ANN201
     """Usage
         kernel_type()
     Purpose
         Check the kernel type. Current we support detection of these types:
             1. default kernel.
             2. debug kernel.
             3. rt kernel.
     Parameter
         N/A
     Returns
         kernel_type        # 'debug|rt|default'.
     """
     retcode, version = run_ret_out("uname -r", return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: kernel_type() - could not get kernel version")
+        print("FAIL: kernel_type() - could not get kernel version")
         print(version)
         return None
 
     if re.match(r".*\.debug$", version):
         return "debug"
 
     if re.match(r".*\.rt$", version):
         return "rt"
 
     return "default"
 
 
-def kmem_leak_start():
+def kmem_leak_start():  # noqa: ANN201
     """Usage
         kmem_leak_start()
     Purpose
         Start and clear kernel memory leak detection.
     Parameter
         N/A
     Returns
         True
           or
         False       # not debug kernel or failure found.
     """
     k_type = kernel_type()
 
     if not k_type or k_type != "debug":
-        sts_print("WARN: Not debug kernel, will not enable kernel memory leak check")
+        print("WARN: Not debug kernel, will not enable kernel memory leak check")
         return False
 
     arch = os_arch()
     if arch == "i386" or arch == "i686":
         print("INFO: Not enabling kmemleak on 32 bits server.")
         return False
 
     k_commandline = kernel_command_line()
     if not re.search("kmemleak=on", k_commandline):
-        sts_print("WARN: kmem_leak_start(): need 'kmemleak=on' kernel_option to enable kernel memory leak detection")
+        print("WARN: kmem_leak_start(): need 'kmemleak=on' kernel_option to enable kernel memory leak detection")
 
     check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
     retcode = run(check_debugfs_mount_cmd, verbose=False).returncode
     if retcode != 0:
         # debugfs is not mounted
         mount_debugfs_cli_cmd = "mount -t debugfs nodev /sys/kernel/debug"
         run(mount_debugfs_cli_cmd, verbose=True)
         check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
         retcode, output = run_ret_out(check_debugfs_mount_cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print("WARN: Failed to mount debugfs to /sys/kernel/debug")
+            print("WARN: Failed to mount debugfs to /sys/kernel/debug")
             print(output)
             return False
 
     # enable kmemleak and clear
-    sts_print("INFO: Begin kernel memory leak check")
+    print("INFO: Begin kernel memory leak check")
     if run("echo scan=on > /sys/kernel/debug/kmemleak") != 0:
         return False
     if run("echo stack=on > /sys/kernel/debug/kmemleak") != 0:
         return False
     if run("echo clear > /sys/kernel/debug/kmemleak") != 0:
         return False
     return True
 
 
-def kmem_leak_check():
+def kmem_leak_check():  # noqa: ANN201
     """Usage
         kmem_leak_check()
     Purpose
         Read out kernel memory leak check log and then clear it up.
     Parameter
         N/A
     Returns
@@ -711,29 +710,29 @@
     """
     sysfs_kmemleak = "/sys/kernel/debug/kmemleak"
     if not Path(sysfs_kmemleak).is_file():
         return None
 
     with Path(sysfs_kmemleak).open() as f:
         if not f:
-            sts_print(f"FAIL: Could not read {sysfs_kmemleak}")
+            print(f"FAIL: Could not read {sysfs_kmemleak}")
             return None
         kmemleak_log = f.read()
 
     if kmemleak_log:
-        sts_print(f"WARN: Found kernel memory leak:\n{kmemleak_log}")
-        sts_print("INFO: Clearing memory leak for next check")
+        print(f"WARN: Found kernel memory leak:\n{kmemleak_log}")
+        print("INFO: Clearing memory leak for next check")
         run(f"echo 'clear' > {sysfs_kmemleak}")
         return kmemleak_log
 
-    sts_print("INFO: No kernel memory leak found")
+    print("INFO: No kernel memory leak found")
     return None
 
 
-def kmem_leak_disable():
+def kmem_leak_disable():  # noqa: ANN201
     """Usage
         kmem_leak_disable()
     Purpose
         Disable kmemleak by 'scan=off' and 'stack=off' to
         '/sys/kernel/debug/kmemleak'.
     Parameter
         N/A
@@ -742,28 +741,28 @@
           or
         False       # failed to run 'echo' command.
     """
     sysfs_kmemleak = "/sys/kernel/debug/kmemleak"
     if not Path(sysfs_kmemleak).is_file():
         return True
 
-    sts_print("INFO: kmem_leak_disable(): Disabling kernel memory leak detection")
+    print("INFO: kmem_leak_disable(): Disabling kernel memory leak detection")
     ok1, ok1_output = run_ret_out(f"echo scan=off > {sysfs_kmemleak}", return_output=True)
     ok2, ok2_output = run_ret_out(f"echo stack=off > {sysfs_kmemleak}", return_output=True)
     if ok1 != 0 or ok2 != 0:
         print("FAIL: kmem_leak_disable(): Failed to disable kernel memory leak detection")
         print(ok1_output)
         print(ok2_output)
         return False
 
-    sts_print("INFO: kmem_leak_disable(): Kernel memory leak detection disabled")
+    print("INFO: kmem_leak_disable(): Kernel memory leak detection disabled")
     return True
 
 
-def query_os_info():
+def query_os_info():  # noqa: ANN201
     """Query OS information and set a reference below:
         os_info = {
             dist_name       = dist_name,
             dist_release    = dist_release,
             kernel_version  = kernel_version,
             os_arch         = os_arch,
             arch            = os_arch,
@@ -785,28 +784,28 @@
         "arch": os_arch(),
         "pkg_arch": os_arch(),
         "kernel_version": kernel_version(),
         "kernel_type": kernel_type(),
     }
 
 
-def get_driver_info(driver: str):
+def get_driver_info(driver: str):  # noqa: ANN201
     if not driver:
-        sts_print("FAIL: get_driver_info() - requires driver parameter")
+        print("FAIL: get_driver_info() - requires driver parameter")
         return None
 
     sys_fs_dir = "/sys/module"
     sys_fs_path = Path(sys_fs_dir)
     if not sys_fs_path.is_dir():
-        sts_print(f"FAIL: get_driver_info() - {sys_fs_path} is not a valid directory")
+        print(f"FAIL: get_driver_info() - {sys_fs_path} is not a valid directory")
         return None
 
     sysfs_driver_folder = sys_fs_path / driver
     if not sysfs_driver_folder.is_dir():
-        sts_print(f"FAIL: get_driver_info() - module {driver} is not loaded")
+        print(f"FAIL: get_driver_info() - module {driver} is not loaded")
         return None
 
     driver_info = {}
     infos = ["srcversion", "version", "taint"]
     for info in infos:
         info_path = sysfs_driver_folder / info
         if not Path(info_path).is_file():
@@ -822,89 +821,89 @@
             output = run(f"cat {sys_driver_parameter}/{param}", capture_output=True, verbose=False).output
             if "parameters" not in driver_info:
                 driver_info["parameters"] = {}
             driver_info["parameters"][param] = output
     return driver_info
 
 
-def mkdir(new_dir):
+def mkdir(new_dir):  # noqa: ANN001, ANN201
     if Path(new_dir).is_dir():
-        sts_print(f"INFO: {new_dir} already exist")
+        print(f"INFO: {new_dir} already exist")
         return True
     cmd = f"mkdir -p {new_dir}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: could create directory {new_dir}")
+        print(f"FAIL: could create directory {new_dir}")
         print(output)
         return False
     return True
 
 
-def rmdir(dir_name):
+def rmdir(dir_name):  # noqa: ANN001, ANN201
     """Remove directory and all content from it."""
     if not Path(dir_name).is_dir():
-        sts_print(f"INFO: {dir_name} does not exist")
+        print(f"INFO: {dir_name} does not exist")
         return True
     cmd = f"rm -rf {dir_name}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: could remove directory {dir_name}")
+        print(f"FAIL: could remove directory {dir_name}")
         print(output)
         return False
     return True
 
 
-def mkfs(device_name, fs_type, force=False):
+def mkfs(device_name, fs_type, force=False):  # noqa: ANN001, ANN201
     """Create a Filesystem on device."""
     if not device_name or not fs_type:
-        sts_print("INFO: mkfs() requires device_name and fs_type")
+        print("INFO: mkfs() requires device_name and fs_type")
         return False
 
     force_option = "-F"
     if fs_type == "xfs":
         force_option = "-f"
 
     cmd = f"mkfs.{fs_type} "
     if force:
         cmd += f"{force_option} "
     cmd += device_name
     retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
-        sts_print(f"FAIL: could create filesystem {fs_type} on {device_name}")
+        print(f"FAIL: could create filesystem {fs_type} on {device_name}")
         print(output)
         return False
     return True
 
 
-def sync(directory=None):
+def sync(directory=None):  # noqa: ANN001, ANN201
     cmd = "sync"
     if directory:
         cmd += f" {directory}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: could not sync")
+        print("FAIL: could not sync")
         print(output)
         return False
     return True
 
 
-def get_free_space(path):
+def get_free_space(path):  # noqa: ANN001, ANN201
     """Get free space of a path.
     Path could be:
     /dev/sda
     /root
     ./.
     """
     if not path:
         return None
 
     cmd = f"df -B 1 {path}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: get_free_space() - could not run {cmd}")
+        print(f"FAIL: get_free_space() - could not run {cmd}")
         print(output)
         return None
     fs_list = output.split("\n")
     # delete the header info
     del fs_list[0]
 
     if len(fs_list) > 1:
@@ -917,140 +916,140 @@
     free_space_regex = re.compile(r"\S+\s+\d+\s+\d+\s+(\d+)")
     m = free_space_regex.search(fs_list[0])
     if m:
         return int(m.group(1))
     return None
 
 
-def get_block_device_name(device):
+def get_block_device_name(device):  # noqa: ANN001, ANN201
     """Returns kernel name from block device
     eg. lvm1 from /dev/mapper/lvm1.
     """
     if not device.startswith("/dev/"):
         device = get_full_path(device)
     if not device:
-        sts_print("FAIL: get_block_device_name - unknown device")
+        print("FAIL: get_block_device_name - unknown device")
     cmd = f"lsblk -ndlo NAME {device}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: run {cmd}")
+        print(f"FAIL: run {cmd}")
         print(output)
         return None
     return output
 
 
-def get_full_path(device_name):
+def get_full_path(device_name):  # noqa: ANN001, ANN201
     """Returns full block device path, eg. from device: /dev/mapper/device."""
     cmds = [
         f"lsblk -pnalo NAME  | grep {device_name} -m1",  # should be more robust
         f"find /dev/ -name {device_name}",
     ]  # older OS(rhel-6), will fail with partitions
 
     for cmd in cmds:
         retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode == 0 and output != "":
             return output
 
-    sts_print(f"FAIL: get_full_path() - {device_name}")
+    print(f"FAIL: get_full_path() - {device_name}")
     return None
 
 
-def get_parent_device(child_device, only_direct=False):
+def get_parent_device(child_device, only_direct=False):  # noqa: ANN001, ANN201
     """Returns block device's parent device: eg. sda, nvme0n1
     child_device: eg. /dev/sda2, nvme0n1p1, /dev/mapper/device
     only_direct: returns only the direct parent. eg. lvm -> sda3, not sda.
     """
     if not child_device.startswith("/dev/"):
         child_device = get_full_path(child_device)
     if not child_device:  # get_full_path would return None if device does not exist
-        sts_print(f"FAIL: get_parent_device - unknown child_device '{child_device}'")
+        print(f"FAIL: get_parent_device - unknown child_device '{child_device}'")
     cmd = f"lsblk -nsl {child_device} -o KNAME | tail -n 1"
     if only_direct:
         cmd = f"lsblk -nsl {child_device} -o KNAME | sed -n 2p"  # if no parent, returns nothing
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: run {cmd}")
+        print(f"FAIL: run {cmd}")
         print(output)
         return None
     if output == "" or output == child_device:
-        sts_print("WARN: get_parent_device - device has no parent")
+        print("WARN: get_parent_device - device has no parent")
         return None
     return output
 
 
 def get_udev_property(device_name: str, property_key: str) -> Union[str, None]:
     """Given an /dev device name, returns specified property using udevadm.
 
     Args:
       device_name: e.g. 'sda', 'mpatha', 'dm-0', 'nvme0n1', 'sr0', ...
       property_key: eg. 'ID_SERIAL', 'DM_WWN', 'ID_PATH', ...
     :return property_value: eg. for ID_SERIAL: '360fff19abdd9f5fb943525d45126ca27'
     """
     if not device_name:
-        sts_print("WARN: get_udev_property() - requires device_name parameter")
+        print("WARN: get_udev_property() - requires device_name parameter")
         return None
 
     # Converts for example mpatha to /dev/mapper/mpatha or sda to /dev/sda
     device = get_full_path(device_name)
     if not device:
-        sts_print(f"FAIL: get_udev_property - unknown device_name '{device_name}'")
+        print(f"FAIL: get_udev_property - unknown device_name '{device_name}'")
 
     # Trying to catch wrong key name when dm-multipath is used.
     if mp.is_mpath_device(device_name, print_fail=False):  # noqa: SIM102
         if property_key.startswith("ID_") and not property_key.startswith("ID_FS_"):
             property_key = property_key.replace("ID_", "DM_")
 
     ret, property_value = run_ret_out(
         f"udevadm info -q property --name={device} | grep {property_key}= | cut -d = -f 2",
         return_output=True,
         verbose=False,
     )
     if ret:
-        sts_print(f"WARN: Could not get udevadm info of device '{device}'")
+        print(f"WARN: Could not get udevadm info of device '{device}'")
         return None
     if not property_value:
-        sts_print(f"WARN: Could not find property '{property_key}' in udevadm info of device '{device}'")
+        print(f"WARN: Could not find property '{property_key}' in udevadm info of device '{device}'")
         return None
 
     return property_value
 
 
-def get_boot_device(parent_device=False, full_path=False):
+def get_boot_device(parent_device=False, full_path=False):  # noqa: ANN001, ANN201
     """Returns boot device, eg. 'sda1'
     parent_device, eg. 'sda'
     full_path, eg. '/dev/sda1'.
     """
     boot_mount = "/boot"
     root_mount = "/"
     # get boot device
     cmd = f"mount | grep ' {boot_mount} ' | cut -d ' ' -f 1"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: run {cmd}")
+        print(f"FAIL: run {cmd}")
         print(output)
         return None
     boot_device = output
     # get root device
     cmd = f"mount | grep ' {root_mount} ' | cut -d ' ' -f 1"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: run {cmd}")
+        print(f"FAIL: run {cmd}")
         print(output)
         return None
     root_device = output
 
     if not boot_device and not root_device:
-        sts_print("FAIL: Could not find '/boot' and '/' mounted!")
+        print("FAIL: Could not find '/boot' and '/' mounted!")
         return None
     if not boot_device:
         # /boot is not mounted on openstack virtual machines
-        sts_print("INFO: Could not find /boot mounted... Assuming this is a virtual machine")
+        print("INFO: Could not find /boot mounted... Assuming this is a virtual machine")
         boot_device = root_device
     if boot_device == "overlay":
-        sts_print("INFO: / mounted on overlay device. Assuming running in a container")
+        print("INFO: / mounted on overlay device. Assuming running in a container")
         return None
 
     if parent_device:
         boot_device = get_parent_device(boot_device)
     if full_path:
         return get_full_path(boot_device)
     return get_block_device_name(boot_device)
@@ -1061,105 +1060,105 @@
 
     Args:
       device_name: e.g. 'sda', 'mpatha', ...
     """
     # Converts for example mpatha to /dev/mapper/mpatha or sda to /dev/sda
     device = get_full_path(device_name)
     if not device:
-        sts_print(f"FAIL: is_dm_device - unknown device_name '{device_name}'")
+        print(f"FAIL: is_dm_device - unknown device_name '{device_name}'")
         return False
     ret, name = run_ret_out(f"udevadm info -q name --name={device}", return_output=True, verbose=False)
     if ret:
-        sts_print(f"FAIL: Could not get udevadm info for device '{device}'")
+        print(f"FAIL: Could not get udevadm info for device '{device}'")
         return False
     if not name:
-        sts_print(f"FAIL: Could not find udev name for '{device}'")
+        print(f"FAIL: Could not find udev name for '{device}'")
         return False
 
     if name.startswith("dm"):
         return True
 
     return False
 
 
-def is_nvme_device(device):
+def is_nvme_device(device):  # noqa: ANN001, ANN201
     """Checks if device is nvme device."""
     return bool(re.match("^nvme[0-9]n[0-9]$", device))
 
 
-def get_wwid_of_nvme(device):
+def get_wwid_of_nvme(device):  # noqa: ANN001, ANN201
     """Reads WWID from udev ID_WWN."""
     return get_udev_property(device, property_key="ID_WWN")
 
 
-def get_device_wwid(device):
+def get_device_wwid(device):  # noqa: ANN001, ANN201
     """Given an SCSI, NVMe or multipath device, returns its WWID."""
     if device.startswith("vd"):
         print(f"INFO: {device}: Presuming virtual disk does not have wwid.")
         return None
 
     serial = get_udev_property(device_name=device, property_key="ID_SERIAL")
     if not serial and is_dm_device(device):  # RHEL-6 workaround
         dm_uuid = get_udev_property(device_name=device, property_key="DM_UUID")
         serial = dm_uuid.replace("mpath-", "")
     if not serial:
-        sts_print(f"INFO: get_device_wwid() - Could not find WWID for {device}")
+        print(f"INFO: get_device_wwid() - Could not find WWID for {device}")
         return None
 
     return serial
 
 
-def remove_device_wwid(wwid):
+def remove_device_wwid(wwid):  # noqa: ANN001, ANN201
     if not wwid:
-        sts_print("FAIL: remove_device_wwid() - requires wwid as parameter")
+        print("FAIL: remove_device_wwid() - requires wwid as parameter")
         return False
 
     mpath_wwid = mp.mpath_name_of_wwid(wwid)
     if mpath_wwid:
         mp.remove_mpath(mpath_wwid)
 
     scsi_ids_wwid = scsi.scsi_ids_of_wwid(wwid)
     if scsi_ids_wwid:
         for scsi_id in scsi_ids_wwid:
             scsi_name = scsi.get_scsi_disk_name(scsi_id)
             if not scsi_name:
                 continue
-            sts_print(f"INFO: detaching SCSI disk {scsi_name}")
+            print(f"INFO: detaching SCSI disk {scsi_name}")
             scsi.delete_disk(scsi_name)
     return True
 
 
-def clear_dmesg():
+def clear_dmesg():  # noqa: ANN201
     cmd = "dmesg --clear"
     if dist_ver() < 7:
         cmd = "dmesg -c"
     run(cmd, verbose=False)
     return True
 
 
-def get_regex_pci_id():
+def get_regex_pci_id():  # noqa: ANN201
     regex_pci_id = r"(?:([0-0a-f]{4}):){0,1}"  # domain id (optional)
     regex_pci_id += r"([0-9a-f]{2})"  # bus id
     regex_pci_id += r":"
     regex_pci_id += r"([0-9a-f]{2})"  # slot id
     regex_pci_id += r"\."
     regex_pci_id += r"(\d+)"  # function id
     return regex_pci_id
 
 
-def get_partitions(device):
+def get_partitions(device):  # noqa: ANN001, ANN201
     """Return a list of all parition numbers from the device."""
     if not device:
-        sts_print("WARN: get_partitions() - requires device as parameter")
+        print("WARN: get_partitions() - requires device as parameter")
         return None
 
     cmd = f"parted -s {device} print"
     ret, output = run_ret_out(cmd, verbose=False, return_output=True)
     if ret != 0:
-        # sts_print("FAIL: get_partitions() - Could not read partition information from %s" % device)
+        # print("FAIL: get_partitions() - Could not read partition information from %s" % device)
         # print output
         return None
 
     lines = output.split("\n")
     if not lines:
         return None
 
@@ -1175,35 +1174,35 @@
             m = partition_regex.match(line)
             if m:
                 partitions.append(m.group(1))
 
     return partitions
 
 
-def delete_partition(device, partition):
+def delete_partition(device, partition):  # noqa: ANN001, ANN201
     """Delete specific partition from the device."""
     if not device or not partition:
-        sts_print("FAIL: delete_partition() - requires device and partition as argument")
+        print("FAIL: delete_partition() - requires device and partition as argument")
         return False
 
     cmd = f"parted -s {device} rm {partition}"
     ret, output = run_ret_out(cmd, verbose=False, return_output=True)
     if ret != 0:
-        sts_print("FAIL: delete_partition() - Could not delete partition %d from %s" % (partition, device))
+        print("FAIL: delete_partition() - Could not delete partition %d from %s" % (partition, device))
         print(output)
         return False
 
     return True
 
 
-def add_repo(name, address, metalink=False):
+def add_repo(name, address, metalink=False):  # noqa: ANN001, ANN201
     """Adds yum repository to /etc/yum.repos.d/NAME.repo."""
     repo = Path(f"/etc/yum.repos.d/{name.lower()}.repo")
     if repo.is_file():
-        sts_print(f"INFO: Repo {repo} already exists.")
+        print(f"INFO: Repo {repo} already exists.")
         return True
 
     url = "metalink" if metalink else "baseurl"
 
     repo_conf_table = {
         "name": name,
         url: address,
@@ -1218,15 +1217,15 @@
 
     with repo.open(mode="w") as f:
         f.write(repo_conf)
 
     return True
 
 
-def download_repo_file(url, name=None, overwrite=True):
+def download_repo_file(url, name=None, overwrite=True):  # noqa: ANN001, ANN201
     """Downloads .repo file to /etc.repos.d/."""
     if not url:
         print("FAIL: repo file url argument required")
         return False
     if not name:
         name = url.split("/")[-1]
     if name[-5:] != ".repo":
@@ -1241,25 +1240,25 @@
     install_package("curl", check=True, verbose=False)
     if not run(f"curl {url} --output {path}", verbose=True):
         return False
 
     return True
 
 
-def del_repo(name):
+def del_repo(name):  # noqa: ANN001, ANN201
     """Removes .repo file."""
     try:
         Path(f"/etc/yum.repos.d/{name}.repo").unlink()
     except FileNotFoundError:
-        sts_print(f"WARN: Removing repository {name} failed.")
+        print(f"WARN: Removing repository {name} failed.")
         return False
     return True
 
 
-def check_repo(name, check_if_enabled=True):
+def check_repo(name, check_if_enabled=True):  # noqa: ANN001, ANN201
     """Checks if repository works and is enabled."""
     if not name:
         print("FAIL: repo name argument required")
         return False
 
     cmd = f"yum repoinfo {name} | grep Repo-status"  # yum=dnf alias works here
     ret, out = run_ret_out(cmd, return_output=True)
@@ -1269,41 +1268,41 @@
     if check_if_enabled and "enabled" not in out:
         print(f"{name} repo is not enabled")
         return False
 
     return True
 
 
-def is_docker():
+def is_docker():  # noqa: ANN201
     """Check if we are running inside docker container."""
     cmd = "cat /proc/self/cgroup | grep docker"
     if run(cmd, verbose=False).returncode == 0:
         # It is docker
         return True
     return False
 
 
-def get_memory(units="m", total=False):
+def get_memory(units="m", total=False):  # noqa: ANN001, ANN201
     """Returns data from 'free' as a dict."""
     possible_units = "b bytes k kilo m mega  g giga tera peta".split()
     if units not in possible_units:
-        sts_print("FAIL: 'units' must be one of %s" % [str(x) for x in possible_units])
+        print("FAIL: 'units' must be one of %s" % [str(x) for x in possible_units])
         return None
 
     memory = {}
     columns = []
 
     if len(units) > 1:
         units = "-" + units
     cmd = f"free -{units}"
     if total:
         cmd += " -t"
     ret, mem = run_ret_out(cmd=cmd, return_output=True)
     if ret != 0:
-        sts_print(f"FAIL: Running '{cmd}' failed.")
+        print(f"FAIL: Running '{cmd}' failed.")
         return None
 
     for row, m in enumerate(mem.splitlines()):
         if row == 0:
             columns = [c.strip() for c in m.split()]
             continue
         m = [x.strip() for x in m.split()]  # noqa: PLW2901
@@ -1329,15 +1328,15 @@
         cmd = f"systemctl show {service_name} --property=ActiveEnterTimestamp"
         ret, data = run_ret_out(cmd, return_output=True)
         if ret == 0:
             timestamp = data.split("=")
             if timestamp[1] != "":
                 return timestamp[1]
             return None
-        sts_print(f"WARN: Could not get active enter timestamp of service: {service_name}")
+        print(f"WARN: Could not get active enter timestamp of service: {service_name}")
     return None
 
 
 def get_system_logs(
     length: Optional[int] = None,
     reverse: bool = False,
     kernel_only: bool = False,
@@ -1376,15 +1375,15 @@
         cmd += " " + " ".join(options)
 
     if grep:
         cmd += f" | grep '{grep}'"
 
     ret, journal = run_ret_out(cmd, return_output=return_output, verbose=verbose)
     if ret:
-        sts_print(f"FAIL: cmd '{cmd}' failed with retcode {ret}.")
+        print(f"FAIL: cmd '{cmd}' failed with retcode {ret}.")
         return None
     if not return_output:
         return ret
 
     # shorten the hostname to match /var/log/messages format
     data = ""
     for line in journal.splitlines():
@@ -1417,61 +1416,61 @@
         config = ConfigObj(file, file_error=file_error, list_values=list_values)
     except OSError as e:
         print(e)
         return False
 
     config.filename = file
 
-    sts_print(f"INFO: Updating {file}")
+    print(f"INFO: Updating {file}")
     if update:
         config.update(parameters)
     else:
         config.merge(parameters)
 
     config.write()
     return True
 
 
-def remove_from_config(file, parameters_to_remove, section=None, warn=True) -> bool:
+def remove_from_config(file, parameters_to_remove, section=None, warn=True) -> bool:  # noqa: ANN001
     """Removes objects from a configuration file.
 
     Args:
       file: (str) Path to the configuration file.
       parameters_to_remove: (list) Parameters to remove.
       section: (str) Specify section of config file parameters are nested in.
       warn: (bool) Set False to supress warning when deleting nonexistent parameter.
     """
     try:
         config = ConfigObj(file, file_error=True)
     except OSError as e:
-        sts_print("FAIL: Unable to open {}. It might not exist")
+        print("FAIL: Unable to open {}. It might not exist")
         print(e)
         return False
 
     config.filename = file
     fail = False
     for param in parameters_to_remove:
-        sts_print(f'INFO: Removing "{param}" from {file}')
+        print(f'INFO: Removing "{param}" from {file}')
         try:
             if section:
                 config[section].pop(param)
             else:
                 config.pop(param)
         except KeyError:
             if warn:
-                sts_print("WARN: Parameter to remove is not in config")
+                print("WARN: Parameter to remove is not in config")
             fail = True
 
     config.write()
     if fail:
         return False
     return True
 
 
-def generate_sosreport(skip_plugins=None, plugin_timeout=300, timeout=900):
+def generate_sosreport(skip_plugins=None, plugin_timeout=300, timeout=900):  # noqa: ANN001, ANN201
     """Generates a sos report.
 
     Args:
       skip_plugins: (string) comma separated list of plugins to skip (no space after comma)
       plugin_timeout: (int) timeout in seconds to allow each plugin to run for (only applicable to rhel-8+)
       timeout: (int) timeout for the sosreport proces in seconds. Use `None` for no timeout.
     """
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/lio.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/lio.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re  # regex
 
 from sts import fc, linux
-from sts.utils import sts_print
 from sts.utils.cmdline import run, run_ret_out
 
 regex_tgtcli_wwpn = "naa.\\S+"
 
 
-def _tgt_wwn_2_wwn(wwn):
+def _tgt_wwn_2_wwn(wwn):  # noqa: ANN001, ANN202
     """On RHEL-6 targetcli stores WWN on WWN format,
     but on RHEL-7 it is something like: naa.200090e2baa397ca
     The arguments are:
     None
     Returns:
     String: WWN as: 20:00:90:e2:ba:a3:97:ca.
     """
@@ -25,48 +24,46 @@
         return wwn
 
     wwn_regex = r"naa\."
     wwn = re.sub(wwn_regex, "", wwn)
     # append ":" after every 2nd character
     wwn = re.sub(r"(\S{2})", r"\1:", wwn)
     # remove trail :
-    wwn = re.sub(":$", "", wwn)
-    return wwn
+    return re.sub(":$", "", wwn)
 
 
-def _wwn_2_tgt_wwn(wwn) -> str:
+def _wwn_2_tgt_wwn(wwn) -> str:  # noqa: ANN001
     """On RHEL-6 targetcli stores WWN on WWN format,
     but on RHEL-7 it is something like: naa.200090e2baa397ca
     The arguments are:
     WWN:      20:00:90:e2:ba:a3:97:ca
     Returns:
     String: target WWN format as: naa.200090e2baa397ca.
     """
     # Converting Targetcli wwpn format to common format
     if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
         return wwn
 
     # remove all ':'
     wwn = re.sub(":", "", wwn)
     # append "naa." after every 2nd character
-    wwn = "naa." + wwn
-    return wwn
+    return "naa." + wwn
 
 
-def lio_query(show_output=False):
+def lio_query(show_output=False):  # noqa: ANN001, ANN201
     """Query all information from targetcli using targetcli ls
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with targetcli information.
     """
     cmd = "targetcli ls"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not run targetcli")
+        print("FAIL: Could not run targetcli")
         return None
     lio_data = output.split("\n")
 
     lio_field_regex = re.compile(r"o-\s(.*?)\s.*\[(.*)\]")
     # supported types for LIO
     lio_supported_types = ("backstores", "iscsi", "loopback", "tcm_fc")
     lio_supported_backstores = (
@@ -103,15 +100,15 @@
     tcm_fc_processing_acls = False
     tcm_fc_processing_luns = False
 
     for data in lio_data:
         m = lio_field_regex.search(data)
         if not m:
             # Just ignore entry we can't parse
-            # sts_print("FAIL: (%s) does not match LIO field format" % data)
+            # print("FAIL: (%s) does not match LIO field format" % data)
             continue
         entry = m.group(1)
         entry_details = m.group(2)
 
         if entry == "/":
             # Skip root
             continue
@@ -119,15 +116,15 @@
         # print "INFO: LIO field %s" % entry
         if entry in lio_supported_types:
             data_type = entry
             # bs_type_dict = {}
             lio_dict[data_type] = {}
             continue
         if not data_type:
-            sts_print(f"FATAL: {entry} is does not belong to any supported data type")
+            print(f"FATAL: {entry} is does not belong to any supported data type")
             continue
         # print "INFO: %s is subitem of %s" % (entry, data_type)
         # ################# PROCESSING BACKSTORES data type ####################
         if data_type == "backstores":
             if entry in lio_supported_backstores:
                 # print "INFO: Processing backstores %s subtiems" % entry
                 bs_type = entry
@@ -311,15 +308,15 @@
         print(lio_dict)
     return lio_dict
 
 
 ##################################################
 # ############### BACKSTORES ######################
 ##################################################
-def lio_create_backstore(bs_type=None, lun_name=None, lun_size=None, device_name=None):
+def lio_create_backstore(bs_type=None, lun_name=None, lun_size=None, device_name=None):  # noqa: ANN001, ANN201
     """Create new backstore device
     The arguments are:
     None
     Returns:
     True: Device was created
     False: There was some problem.
     """
@@ -330,25 +327,25 @@
     if bs_type == "fileio":
         created = _lio_create_backstore_fileio(lun_name, lun_size=lun_size)
 
     if bs_type == "pscsi":
         created = _lio_create_backstore_pscsi(lun_name, device_name)
 
     if not created:
-        sts_print(f"FAIL: Could not create lun using ({bs_type}) on lio_create_backstore")
+        print(f"FAIL: Could not create lun using ({bs_type}) on lio_create_backstore")
         return False
 
     if lun_name not in list(lio_get_backstores(bs_type).keys()):
-        sts_print(f"FAIL: It seems {lun_name} was created, but it was not")
+        print(f"FAIL: It seems {lun_name} was created, but it was not")
         return False
 
     return True
 
 
-def lio_get_backstores(bs_type=None, lio_dict=None):
+def lio_get_backstores(bs_type=None, lio_dict=None):  # noqa: ANN001, ANN201
     """Return a dict with all backstores. If a backstore type
     is provided return a list of backstore of this type
     The arguments are:
     bs_type (Optional): Backstore type
     lio_dict (Optional): For optmization, if we already have the lio query no need to do it again
     Returns:
     List
@@ -356,56 +353,56 @@
     Dict
     Dict: All backstore devices.
     """
     if not lio_dict:
         lio_dict = lio_query()
 
     if "backstores" not in list(lio_dict.keys()):
-        sts_print("FAIL: there is not backstore defined on targetcli")
+        print("FAIL: there is not backstore defined on targetcli")
         print(lio_dict)
         return None
 
     if not bs_type:
         return lio_dict["backstores"]
 
     if bs_type not in list(lio_dict["backstores"].keys()):
         return None
 
     return lio_dict["backstores"][bs_type]
 
 
-def lio_get_backstore_details(bs_type, lun_name, lio_dict=None):
+def lio_get_backstore_details(bs_type, lun_name, lio_dict=None):  # noqa: ANN001, ANN201
     """Get the size of specific Backstore device
     Returns:
     Dic:      Detailed information about this device
     None:     If something went wrong.
     """
     bs_dict = lio_get_backstores(bs_type, lio_dict=lio_dict)
     if not bs_dict:
         return None
 
     if lun_name not in list(bs_dict.keys()):
-        sts_print(f"FAIL: {lun_name} is not defined on {bs_type}")
+        print(f"FAIL: {lun_name} is not defined on {bs_type}")
         lio_dict = lio_query()
         print(lio_dict)
         return None
 
     return bs_dict[lun_name]
 
 
-def lio_get_backstore_lun_details(bs_type, lun_name):
+def lio_get_backstore_lun_details(bs_type, lun_name):  # noqa: ANN001, ANN201
     """Get the detailed information about the lun."""
     if not bs_type or not lun_name:
-        sts_print("FAIL: lio_get_backstore_lun_details() - requires bs_type and lun_name")
+        print("FAIL: lio_get_backstore_lun_details() - requires bs_type and lun_name")
         return None
 
     cmd = f"targetcli /backstores/{bs_type}/{lun_name} info"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: Could not get {bs_type} details for {lun_name}")
+        print(f"FAIL: Could not get {bs_type} details for {lun_name}")
         return None
 
     details = output.split("\n")
     supported_details = {
         "dev": r"^dev: (\S+)",
         "name": r"^name: (\S+)",
         "size_bytes": r"^size: (\S+)",
@@ -419,25 +416,24 @@
             m = re.match(supported_details[sup_detail], info)
             if m:
                 lun_details[sup_detail] = m.group(1)
 
     return lun_details
 
 
-def _lun_wwn2wwid(wwn):
+def _lun_wwn2wwid(wwn):  # noqa: ANN001, ANN202
     """From the LUN WWN is possible to get WWID."""
     wwid = wwn
     wwid = wwid.replace("-", "")
     # Just the first 26 bytes are the wwid
     wwid = wwid[:25]
-    wwid = "36001405" + wwid
-    return wwid
+    return "36001405" + wwid
 
 
-def lio_delete_backstore(bs_type=None, lun_name=None):
+def lio_delete_backstore(bs_type=None, lun_name=None):  # noqa: ANN001, ANN201
     """Delete backstore device
     The arguments are:
     Backstore type
     LUN name
     Returns:
     True: Device was deleted
     False: There was some problem.
@@ -449,125 +445,125 @@
     if bs_type == "fileio":
         deleted = _lio_delete_backstore_fileio(lun_name)
 
     if bs_type == "pscsi":
         deleted = _lio_delete_backstore_pscsi(lun_name)
 
     if not deleted:
-        sts_print(f"FAIL: Could not delete lun using ({bs_type}) on lio_create_backstore")
+        print(f"FAIL: Could not delete lun using ({bs_type}) on lio_create_backstore")
         return False
 
     if lun_name in list(lio_get_backstores(bs_type).keys()):
-        sts_print(f"FAIL: It seems {lun_name} was deleted, but it was not")
+        print(f"FAIL: It seems {lun_name} was deleted, but it was not")
         return False
 
     return True
 
 
 # ## BLOCK ###
-def _lio_create_backstore_block(lun_name, device):
+def _lio_create_backstore_block(lun_name, device):  # noqa: ANN001, ANN202
     if not lun_name:
         print("FAIL: _lio_create_backstore_block needs lun_name parameter")
         return False
     if not device:
         print("FAIL: _lio_create_backstore_block needs device parameter")
         return False
 
     cmd = f"targetcli /backstores/block create {lun_name} {device}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: Could not create block {lun_name}")
+        print(f"FAIL: Could not create block {lun_name}")
         return False
     return True
 
 
-def _lio_delete_backstore_block(lun_name):
+def _lio_delete_backstore_block(lun_name):  # noqa: ANN001, ANN202
     cmd = f"targetcli /backstores/block delete {lun_name}"
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: Could not delete block {lun_name}")
+        print(f"FAIL: Could not delete block {lun_name}")
         return False
 
     return True
 
 
 # ## FILEIO ###
-def _lio_create_backstore_fileio(lun_name, file_name=None, lun_size=None):
+def _lio_create_backstore_fileio(lun_name, file_name=None, lun_size=None):  # noqa: ANN001, ANN202
     if not lun_name:
-        sts_print("_lio_create_backstore_fileio() - requires lun_name parameter")
+        print("_lio_create_backstore_fileio() - requires lun_name parameter")
         return False
 
     if not file_name:
         # Set default backend file name
         file_name = f"{lun_name}.img"
 
     # disable spare, to force targetcli to allocate the whole file to avoid problem
     # of running out of disk space and not have enough space to store data
     cmd = f"targetcli /backstores/fileio create {lun_name} {file_name} sparse=false"
     if lun_size:
         cmd = cmd + f" {lun_size}"
 
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: Could not create fileio {lun_name}")
+        print(f"FAIL: Could not create fileio {lun_name}")
         return False
     return True
 
 
-def _lio_delete_backstore_fileio(lun_name):
+def _lio_delete_backstore_fileio(lun_name):  # noqa: ANN001, ANN202
     file_name = _lio_get_backstore_fileio_file(lun_name)
 
     if run(f"targetcli /backstores/fileio delete {lun_name}").returncode != 0:
-        sts_print(f"FAIL: Could not delete fileio {lun_name}")
+        print(f"FAIL: Could not delete fileio {lun_name}")
         return False
 
     if file_name and run(f"rm -f {file_name}").returncode != 0:
-        sts_print(f"WARN: could not delete file {file_name}")
+        print(f"WARN: could not delete file {file_name}")
 
     return True
 
 
-def _lio_get_backstore_fileio_file(lun_name):
+def _lio_get_backstore_fileio_file(lun_name):  # noqa: ANN001, ANN202
     """Get the file used by a specific LUN."""
     cmd = f"targetcli /backstores/fileio/{lun_name} ls"
     completed_process = run(cmd, capture_output=True, verbose=False)
     if completed_process.returncode != 0:
-        sts_print(f"FAIL: Could not get fileio file {lun_name}")
+        print(f"FAIL: Could not get fileio file {lun_name}")
         return None
 
     path_regex = re.compile(r"\[(.*)\s\(")
     m = path_regex.search(completed_process.output)
     if m:
         return m.group(1)
     return None
 
 
 # ## PSCSI ###
-def _lio_create_backstore_pscsi(lun_name, device, lun_size=None):
+def _lio_create_backstore_pscsi(lun_name, device, lun_size=None):  # noqa: ANN001, ANN202
     cmd = f"targetcli /backstores/pscsi create {lun_name} {device}"
     if lun_size:
         cmd = cmd + f" {lun_size}M"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not create pscsi {lun_name}")
+        print(f"FAIL: Could not create pscsi {lun_name}")
         return False
     return True
 
 
-def _lio_delete_backstore_pscsi(lun_name):
+def _lio_delete_backstore_pscsi(lun_name):  # noqa: ANN001, ANN202
     cmd = f"targetcli /backstores/pscsi delete {lun_name}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete pscsi {lun_name}")
+        print(f"FAIL: Could not delete pscsi {lun_name}")
         return False
 
     return True
 
 
 ##################################################
 # ################# iSCSI ########################
 ##################################################
-def lio_support_iscsi_target():
+def lio_support_iscsi_target():  # noqa: ANN201
     """Check if host supports iSCSI target
     The arguments are:
     None
     Returns:
     True: Host supports iscsi
     False: Host does not support iscsi.
     """
@@ -576,52 +572,52 @@
     if "iscsi" not in list(lio_dict.keys()):
         # Host does not support iSCSI target
         return False
     return True
 
 
 # ## iSCSI target ###
-def lio_iscsi_create_target(iqn):
+def lio_iscsi_create_target(iqn):  # noqa: ANN001, ANN201
     """Add the iqn to iSCSI target
     The arguments are:
     iqn:     Target IQN
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not lio_support_iscsi_target():
-        sts_print("FAIL: server does not support iSCSI target")
+        print("FAIL: server does not support iSCSI target")
         return False
 
     cmd = f"targetcli /iscsi/ create {iqn}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not create iSCSI target {iqn}")
+        print(f"FAIL: Could not create iSCSI target {iqn}")
         return False
 
     if iqn not in lio_iscsi_get_target():
-        sts_print("FAIL: It seems to have added iSCSI target, but it did not")
+        print("FAIL: It seems to have added iSCSI target, but it did not")
         lio_dict = lio_query()
         print(lio_dict["iscsi"])
         return False
     # targetcli by default enable only IPv$ connection
     # we want also IPv6
     if not lio_iscsi_delete_target_portal(iqn, "tpg1", "0.0.0.0"):
-        sts_print("FAIL: could not remove default iSCSI target portal")
+        print("FAIL: could not remove default iSCSI target portal")
         lio_dict = lio_query()
         print(lio_dict["iscsi"])
 
     if not lio_iscsi_create_target_portal(iqn, "tpg1", "::0"):
-        sts_print("FAIL: could not create IPv6 iSCSI target portal")
+        print("FAIL: could not create IPv6 iSCSI target portal")
         lio_dict = lio_query()
         print(lio_dict["iscsi"])
     return True
 
 
-def lio_iscsi_get_target():
+def lio_iscsi_get_target():  # noqa: ANN201
     """Return a list of all iSCSI targets configured
     The arguments are:
     None
     Returns:
     list: Return a list of IQNs that are configured.
     """
     lio_dict = lio_query()
@@ -629,15 +625,15 @@
     if not lio_support_iscsi_target():
         # Host does not support iSCSI target
         return None
 
     return list(lio_dict["iscsi"].keys())
 
 
-def lio_iscsi_target_set_parameter(tgt_iqn, tpg, group, attr_name, attr_value):
+def lio_iscsi_target_set_parameter(tgt_iqn, tpg, group, attr_name, attr_value):  # noqa: ANN001, ANN201
     """Set a parameter to an iSCSI target
     if tgt_iqn is not set, set it globally
     The arguments are:
     tgt_iqn       HOST IQN
     tpg           Target Portal Group
     group         eg: attribute, parameter, discovery_auth...
     attr_name     Attribute name
@@ -647,59 +643,59 @@
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi set {group} {attr_name}={attr_value}"
     if tgt_iqn:
         cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/ set {group} {attr_name}={attr_value}"
 
     if run(cmd).returncode != 0:
-        sts_print(f"FAIL: Could not set iSCSI target attribute {attr_name}")
+        print(f"FAIL: Could not set iSCSI target attribute {attr_name}")
         return False
     return True
 
 
 # ## iSCSI ACLS ###
-def lio_iscsi_create_acl(tgt_iqn, tpg, init_iqn):
+def lio_iscsi_create_acl(tgt_iqn, tpg, init_iqn):  # noqa: ANN001, ANN201
     """Add an initiator IQN to target IQN
     The arguments are:
     tgt_iqn:     Host IQN
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init IQN is created
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls create {init_iqn} add_mapped_luns=false"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not add iSCSI initiator {init_iqn}")
+        print(f"FAIL: Could not add iSCSI initiator {init_iqn}")
         return False
     return True
 
 
-def lio_iscsi_delete_acl(tgt_iqn, tpg, init_iqn):
+def lio_iscsi_delete_acl(tgt_iqn, tpg, init_iqn):  # noqa: ANN001, ANN201
     """Remove an initiator IQN from target IQN
     The arguments are:
     tgt_iqn:     Host IQN
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init iqn is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls delete {init_iqn}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete iSCSI initiator {init_iqn}")
+        print(f"FAIL: Could not delete iSCSI initiator {init_iqn}")
         return False
 
     return True
 
 
 # ## iSCSI LUNs ###
-def lio_iscsi_add_lun(tgt_iqn, tpg, bs_type, lun_name):
+def lio_iscsi_add_lun(tgt_iqn, tpg, bs_type, lun_name):  # noqa: ANN001, ANN201
     """Add a LUN to target IQN
     The arguments are:
     tgt_iqn:      Host IQN
     tpg:          Target Portal Group
     bs_type:      Backstore type
     lun_name:     Lun Name
     Returns:
@@ -710,40 +706,40 @@
         tgt_iqn,
         tpg,
         bs_type,
         lun_name,
     )
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not add lun to iSCSI target {tgt_iqn}")
+        print(f"FAIL: Could not add lun to iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
-def lio_iscsi_remove_lun(tgt_iqn, tpg, lun_id):
+def lio_iscsi_remove_lun(tgt_iqn, tpg, lun_id):  # noqa: ANN001, ANN201
     """Remove a LUN target IQN
     The arguments are:
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/luns delete {lun_id}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete LUN from iSCSI target {tgt_iqn}")
+        print(f"FAIL: Could not delete LUN from iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
-def lio_iscsi_get_luns(tgt_iqn, tpg):
+def lio_iscsi_get_luns(tgt_iqn, tpg):  # noqa: ANN001, ANN201
     """Return a list with all LUNs added to an iSCSI target.
     The arguments are:
     None
     Returns:
     List: list of luns
     None if something went wrong.
     """
@@ -756,15 +752,15 @@
         print("INFO: target %s does not have any LUN\n")
         return None
 
     return lio_dict["tcm_fc"][tgt_iqn][tpg]["luns"]
 
 
 # ## iSCSI Portals ###
-def lio_iscsi_create_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):
+def lio_iscsi_create_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):  # noqa: ANN001, ANN201
     """Remove a Portal target IQN
     The arguments are:
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     portal_ip:   IP of host allowed to connect. (0.0.0.0) any IPv4 address
     portal_port  Port to listen for connection, default 3260
     Returns:
@@ -780,21 +776,21 @@
     if portal in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
         print(f"INFO: portal {portal} does already exist on target {tgt_iqn}")
         return True
 
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals create {portal_ip} {portal_port}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
+        print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
-def lio_iscsi_delete_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):
+def lio_iscsi_delete_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):  # noqa: ANN001, ANN201
     """Remove a Portal target IQN
     The arguments are:
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     portal_ip:   IP of host allowed to connect. (0.0.0.0) any IPv4 address
     portal_port  Port to listen for connection, default 3260
     Returns:
@@ -810,98 +806,98 @@
     if portal not in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
         print(f"INFO: portal {portal} does not exist on target {tgt_iqn}")
         return True
 
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals delete {portal_ip} {portal_port}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
+        print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
         return False
     return True
 
 
 # ## iSCSI LUNs mapping ###
-def lio_iscsi_map_lun(tgt_iqn, tpg, init_iqn, init_lun_id, bs_type, lun_name):
+def lio_iscsi_map_lun(tgt_iqn, tpg, init_iqn, init_lun_id, bs_type, lun_name):  # noqa: ANN001, ANN201
     """Map a LUN to target IQN / Initiator IQN
     The arguments are:
     tgt_iqn:      Target IQN
     tpg:          Target Portal group
     init_iqn:     Host IQN
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
     lun_path = f"/backstores/{bs_type}/{lun_name}"
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls/{init_iqn} create {init_lun_id} {lun_path}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not map lun to iSCSI target {tgt_iqn}/{init_iqn}")
+        print(f"FAIL: Could not map lun to iSCSI target {tgt_iqn}/{init_iqn}")
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
-        sts_print(f"FAIL: It seems to have mapped lun {init_lun_id}, but it did not")
+        print(f"FAIL: It seems to have mapped lun {init_lun_id}, but it did not")
         return False
 
     return True
 
 
-def lio_iscsi_unmap_lun(tgt_iqn, init_iqn, tpg, init_lun_id):
+def lio_iscsi_unmap_lun(tgt_iqn, init_iqn, tpg, init_lun_id):  # noqa: ANN001, ANN201
     """Un map LUN from tgt_wwn/init_wwn
     The arguments are:
     tgt_iqn:      Target IQN
     init_iqn:     Host IQN
     tpg:          Target Portal group
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{init_iqn}/acls/{tpg} delete {init_lun_id}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not unmap LUN from target {tgt_iqn}/{init_iqn}")
+        print(f"FAIL: Could not unmap LUN from target {tgt_iqn}/{init_iqn}")
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
-        sts_print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
+        print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
         return False
     return True
 
 
-def lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, tgt_lun_id):
+def lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, tgt_lun_id):  # noqa: ANN001, ANN201
     """Check if a LUN is mapped to target WWN / Initiator port
     The arguments are:
     tgt_iqn:      Target IQN
     init_iqn:     Host IQN
     tpg:          Target Portal group no.
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/tpg{tpg}/acls/{init_iqn} ls | grep {tgt_lun_id}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}")
+        print(f"FAIL: Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}")
         return False
 
     if output == "":
         return False
     return True
 
 
-def lio_add_iscsi_target(
-    tgt_iqn=None,
-    init_iqn=None,
-    bs_type="fileio",
-    lun_name=None,
-    lun_size="1G",
-    device_name=None,
-    tgt_cnt=1,
-    lun_cnt=1,
+def lio_add_iscsi_target(  # noqa: ANN201
+    tgt_iqn=None,  # noqa: ANN001
+    init_iqn=None,  # noqa: ANN001
+    bs_type="fileio",  # noqa: ANN001
+    lun_name=None,  # noqa: ANN001
+    lun_size="1G",  # noqa: ANN001
+    device_name=None,  # noqa: ANN001
+    tgt_cnt=1,  # noqa: ANN001
+    lun_cnt=1,  # noqa: ANN001
 ):
     """Create new iSCSI target, create LUNs and do LUN mapping
     The arguments are:
     tgt_iqn:          Target IQN, if not specified LIO will create a target IQN
     init_iqn:         Initiator IQN, set LUN map to specific IQN, otherwise any IQN will access the LUN
     bs_type:          Backstores storage type, default: 'fileio'
     lun_name:         LUN name when creating the target, if not set default lun name will be used
@@ -926,15 +922,15 @@
                 new_tgt_iqns.append(tmp_iqn)
             iqn_suffix += 1
     else:
         new_tgt_iqns = [tgt_iqn]
 
     for target_iqn in new_tgt_iqns:
         if not lio_iscsi_create_target(target_iqn):
-            sts_print(f"FAIL: Could not create iSCSI target '{target_iqn}'")
+            print(f"FAIL: Could not create iSCSI target '{target_iqn}'")
             return False
 
         m = re.match(r"%s(\d+)" % iqn_preffix, target_iqn)
         tgt_name = "tgt%d" % int(m.group(1)) if m else target_iqn.split(":")[1]
 
         for lun_num in range(1, lun_cnt + 1):
             tgt_lun_name = "%s_lun%d" % (tgt_name, lun_num)
@@ -944,61 +940,61 @@
 
             if not lio_create_backstore(
                 bs_type=bs_type,
                 lun_name=tgt_lun_name,
                 lun_size=lun_size,
                 device_name=device_name,
             ):
-                sts_print("FAIL: Could not create backstore for iSCSI target")
+                print("FAIL: Could not create backstore for iSCSI target")
                 return False
 
             tpg = "tpg1"
 
             if not lio_iscsi_add_lun(target_iqn, tpg, bs_type, tgt_lun_name):
-                sts_print("FAIL: Could not add LUN to iSCSI target")
+                print("FAIL: Could not add LUN to iSCSI target")
                 return False
 
             # This is a global setting
             if not lio_iscsi_target_set_parameter(None, None, "discovery_auth", "enable", "0"):
-                sts_print("FAIL: Could not set Attr to iSCSI target")
+                print("FAIL: Could not set Attr to iSCSI target")
                 return False
 
             if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "authentication", "0"):
-                sts_print("FAIL: Could not set Attr to iSCSI target")
+                print("FAIL: Could not set Attr to iSCSI target")
                 return False
 
             if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "generate_node_acls", "1"):
-                sts_print("FAIL: Could not set Attr to iSCSI target")
+                print("FAIL: Could not set Attr to iSCSI target")
                 return False
 
             if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "demo_mode_write_protect", "0"):
-                sts_print("FAIL: Could not set Attr to iSCSI target")
+                print("FAIL: Could not set Attr to iSCSI target")
                 return False
 
             lun_id = "0"
             if init_iqn:
                 if not lio_iscsi_create_acl(target_iqn, tpg, init_iqn):
-                    sts_print("FAIL: Could not create iSCSI initiator ACL")
+                    print("FAIL: Could not create iSCSI initiator ACL")
                     return False
                 if not lio_iscsi_map_lun(target_iqn, tpg, init_iqn, lun_id, bs_type, tgt_lun_name):
-                    sts_print("FAIL: Could not map LUN to iSCSI initiator")
+                    print("FAIL: Could not map LUN to iSCSI initiator")
                     return False
 
     return True
 
 
-def lio_setup_iscsi_target(
-    tgt_iqn=None,
-    init_iqn=None,
-    bs_type="fileio",
-    lun_name=None,
-    lun_size="1G",
-    device_name=None,
-    tgt_cnt=1,
-    lun_cnt=1,
+def lio_setup_iscsi_target(  # noqa: ANN201
+    tgt_iqn=None,  # noqa: ANN001
+    init_iqn=None,  # noqa: ANN001
+    bs_type="fileio",  # noqa: ANN001
+    lun_name=None,  # noqa: ANN001
+    lun_size="1G",  # noqa: ANN001
+    device_name=None,  # noqa: ANN001
+    tgt_cnt=1,  # noqa: ANN001
+    lun_cnt=1,  # noqa: ANN001
 ):
     """Create a basic iSCSI target
     The arguments are:
     tgt_iqn:          Target IQN, if not specified LIO will create a target IQN
     init_iqn:         Initiator IQN, set LUN map to specific IQN, otherwise any IQN will access the LUN
     bs_type:          Backstores storage type, default: 'fileio'
     lun_name:         LUN name when creating the target, if not set default lun name will be used
@@ -1015,26 +1011,26 @@
     lio_restart()
     lio_clearconfig()
 
     ver = lio_version()
     print(f"INFO: Running targetcli version {ver}")
 
     if not lio_support_iscsi_target():
-        sts_print("FAIL: Server does not support iSCSI target")
+        print("FAIL: Server does not support iSCSI target")
         return False
 
     lio_add_iscsi_target(tgt_iqn, init_iqn, bs_type, lun_name, lun_size, device_name, tgt_cnt, lun_cnt)
 
     return True
 
 
 ##################################################
 # ################# TCM_FC ########################
 ##################################################
-def lio_support_fc_target():
+def lio_support_fc_target():  # noqa: ANN201
     """Check if host supports FC target
     The arguments are:
     None
     Returns:
     True: Host supports tcm_fc
     False: Host does not support tcm_fc.
     """
@@ -1044,75 +1040,75 @@
         # Host does not support FC target
         return False
 
     return True
 
 
 # ## FC target ###
-def lio_create_fc_target(wwn):
+def lio_create_fc_target(wwn):  # noqa: ANN001, ANN201
     """Add the wwn to tcm_fc target
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not wwn:
-        sts_print("FAIL: lio_create_fc_target() - requires wwn parameter")
+        print("FAIL: lio_create_fc_target() - requires wwn parameter")
         return False
 
     cmd = f"targetcli /tcm_fc/ create {wwn}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: lio_create_fc_target() - Could not create FC target {wwn}")
+        print(f"FAIL: lio_create_fc_target() - Could not create FC target {wwn}")
         return False
 
     if wwn not in lio_get_fc_target():
         lio_dict = lio_query()
         run("targetcli ls", verbose=True)
-        sts_print("FAIL: lio_create_fc_target() - It seems to have added FC target, but it did not")
+        print("FAIL: lio_create_fc_target() - It seems to have added FC target, but it did not")
         print(lio_dict["tcm_fc"])
         print(lio_dict)
 
         return False
 
     return True
 
 
-def lio_delete_fc_target(wwn):
+def lio_delete_fc_target(wwn):  # noqa: ANN001, ANN201
     """Delete the wwn to tcm_fc target
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not wwn:
-        sts_print("FAIL: lio_delete_fc_target() - requires wwn parameter")
+        print("FAIL: lio_delete_fc_target() - requires wwn parameter")
         return False
 
     cmd = f"targetcli /tcm_fc/ delete {wwn}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: lio_delete_fc_target() - Could not delete FC target {wwn}")
+        print(f"FAIL: lio_delete_fc_target() - Could not delete FC target {wwn}")
         return False
 
     if wwn in lio_get_fc_target():
         lio_dict = lio_query()
         run("targetcli ls", return_output=False, verbose=True)
-        sts_print("FAIL: lio_delete_fc_target() - It seems to have deleted FC target, but it did not")
+        print("FAIL: lio_delete_fc_target() - It seems to have deleted FC target, but it did not")
         print(lio_dict["tcm_fc"])
         print(lio_dict)
 
         return False
 
     return True
 
 
-def lio_get_fc_target(lio_dict=None):
+def lio_get_fc_target(lio_dict=None):  # noqa: ANN001, ANN201
     """Return a list of all FC targets configured
     The arguments are:
     None
     Returns:
     list: Return a list of wwns that are configured.
     """
     if not lio_dict:
@@ -1122,15 +1118,15 @@
         # Host does not support FC target
         return None
 
     return list(lio_dict["tcm_fc"].keys())
 
 
 # ## FC ACLS ###
-def lio_create_fc_target_acl(tgt_wwn, init_wwn, lio_dict=None):
+def lio_create_fc_target_acl(tgt_wwn, init_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Add an initiator WWN to target WWN port
     The arguments are:
     tgt_wwn:     Host WWN
     init_wwn:    Initiator WWN
     Returns:
     True: If init wwn is created
     False: If some problem happened.
@@ -1139,66 +1135,66 @@
     if tgt_acls and (init_wwn in tgt_acls):
         print(f"INFO: {init_wwn} is already added to target {tgt_wwn}")
         return True
 
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls create {init_wwn} add_mapped_luns=false"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not add FC initiator {init_wwn}")
+        print(f"FAIL: Could not add FC initiator {init_wwn}")
         return False
 
     return True
 
 
-def lio_delete_fc_target_acl(tgt_wwn, init_wwn):
+def lio_delete_fc_target_acl(tgt_wwn, init_wwn):  # noqa: ANN001, ANN201
     """Remove an initiator WWN from target WWN port
     The arguments are:
     tgt_wwn:     Host WWN
     init_wwn:    Initiator WWN
     Returns:
     True: If init wwn is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls delete {init_wwn}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete FC initiator {init_wwn}")
+        print(f"FAIL: Could not delete FC initiator {init_wwn}")
         return False
 
     return True
 
 
-def lio_get_fc_target_acl(tgt_wwn, lio_dict=None):
+def lio_get_fc_target_acl(tgt_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Get all acls from a specifc target
     The arguments are:
     tgt_wwn:     Host WWN
     Returns:
     List: List of initiators
     None: If some problem happened.
     """
     if not tgt_wwn:
-        sts_print("FAIL: lio_get_fc_target_acl() - requires tgt_wwpn as argument")
+        print("FAIL: lio_get_fc_target_acl() - requires tgt_wwpn as argument")
         return None
     if not lio_dict:
         lio_dict = lio_query()
     if not lio_dict["tcm_fc"][tgt_wwn]:
-        sts_print(f"FAIL: {tgt_wwn} does not exist")
+        print(f"FAIL: {tgt_wwn} does not exist")
         print(lio_dict)
         return None
 
     if "acls" not in list(lio_dict["tcm_fc"][tgt_wwn].keys()):
-        # sts_print("FAIL: %s does not have acls" % tgt_wwn)
+        # print("FAIL: %s does not have acls" % tgt_wwn)
         # print lio_dict
         return None
 
     return list(lio_dict["tcm_fc"][tgt_wwn]["acls"].keys())
 
 
 # ## FC LUNs ###
-def lio_create_fc_target_lun(tgt_wwn, bs_type, lun_name):
+def lio_create_fc_target_lun(tgt_wwn, bs_type, lun_name):  # noqa: ANN001, ANN201
     """Add a LUN to target WWN port
     The arguments are:
     tgt_wwn:      Host WWN
     bs_type:      Backstore type
     lun_name:     Lun Name
     Returns:
     True: If LUN is created
@@ -1207,39 +1203,39 @@
     cmd = "targetcli /tcm_fc/{}/luns create /backstores/{}/{} add_mapped_luns=false".format(
         _wwn_2_tgt_wwn(tgt_wwn),
         bs_type,
         lun_name,
     )
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not add lun to FC target {tgt_wwn}")
+        print(f"FAIL: Could not add lun to FC target {tgt_wwn}")
         return False
 
     return True
 
 
-def lio_delete_fc_target_lun(tgt_wwn, lun_id):
+def lio_delete_fc_target_lun(tgt_wwn, lun_id):  # noqa: ANN001, ANN201
     """Remove an initiator WWN from target WWN port
     The arguments are:
     tgt_wwn:     Target WWN
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/luns delete {lun_id}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not delete LUN from target {tgt_wwn}")
+        print(f"FAIL: Could not delete LUN from target {tgt_wwn}")
         return False
 
     return True
 
 
-def lio_get_fc_target_luns(tgt_wwn, lio_dict=None):
+def lio_get_fc_target_luns(tgt_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Return a dict with all backstores. If a backstore type
     is provided return a list of backstore of this type
     The arguments are:
     None
     Returns:
     List: list of luns
     None if something went wrong.
@@ -1254,15 +1250,15 @@
     if "luns" not in list(lio_dict["tcm_fc"][tgt_wwn].keys()):
         print(f"INFO: target {tgt_wwn} does not have any LUN\n")
         return None
 
     return lio_dict["tcm_fc"][tgt_wwn]["luns"]
 
 
-def lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=None):
+def lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=None):  # noqa: ANN001, ANN201
     """Return the target LUN id.
     The arguments are:
     tgt_wwn:      Target WWN
     bs_type:      Backstore Type
     lun_name:     LUN name
     Returns:
     String: LUN id. eg: lun0
@@ -1280,98 +1276,98 @@
             return lun_id
     return None
 
 
 #    cmd = "targetcli /tcm_fc/%s/luns ls | grep %s/%s | awk '{print$2}'" % (_wwn_2_tgt_wwn(tgt_wwn), bs_type, lun_name)
 #    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
 #    if (retcode != 0):
-#        sts_print ("FAIL: Could not get lun %s for FC target %s" % (lun_name, tgt_wwn))
+#        print ("FAIL: Could not get lun %s for FC target %s" % (lun_name, tgt_wwn))
 #        return None
 #
 #    if output == "":
 #        return None
 #    return output
 
 
 # ## FC LUNs mapping ###
-def lio_fc_lun_map(lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id):
+def lio_fc_lun_map(lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id):  # noqa: ANN001, ANN201
     """Map a LUN to a t_wwpn and h_wwpn."""
     if not lun_name or not bs_type or not tgt_wwn or not init_wwn or not init_lun_id:
-        sts_print("FAIL: lio_fc_lun_map() - requires lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id parameters")
+        print("FAIL: lio_fc_lun_map() - requires lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id parameters")
         return False
 
-    sts_print(f"INFO: Mapping LUN {bs_type}/{lun_name} to {tgt_wwn}/{init_wwn}...")
+    print(f"INFO: Mapping LUN {bs_type}/{lun_name} to {tgt_wwn}/{init_wwn}...")
     lio_dict = lio_query()
     if tgt_wwn not in lio_get_fc_target(lio_dict=lio_dict):
         lio_create_fc_target(tgt_wwn)
         # update lio_dict with new fc target
         lio_dict = lio_query()
 
     if not lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=lio_dict):
         lio_create_fc_target_lun(tgt_wwn, bs_type, lun_name)
         # update lio_dict with new fc target
         lio_dict = lio_query()
 
     # Do not pass lio_dict as parameter as we need to query it again to get updated info
     lun_id = lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=lio_dict)
     if not lun_id:
-        sts_print(f"FAIL: lio_fc_lun_map() - Could not find lun {bs_type}/{lun_name} on target {tgt_wwn}")
+        print(f"FAIL: lio_fc_lun_map() - Could not find lun {bs_type}/{lun_name} on target {tgt_wwn}")
         lio_show()
         return False
 
     if not lio_create_fc_target_acl(tgt_wwn, init_wwn, lio_dict=lio_dict):
-        sts_print(f"FAIL: Could not create ACL to host {init_wwn}")
+        print(f"FAIL: Could not create ACL to host {init_wwn}")
         lio_show()
         return False
 
     if not lio_create_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id, lun_id, lio_dict=lio_dict):
-        sts_print(f"FAIL: Could not map LUN {lun_name} to host {init_wwn}")
+        print(f"FAIL: Could not map LUN {lun_name} to host {init_wwn}")
         return False
 
-    sts_print(f"INFO: LUN {lun_name} mapped successfully")
+    print(f"INFO: LUN {lun_name} mapped successfully")
     return True
 
 
-def lio_create_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id, tgt_lun_id, lio_dict=None):
+def lio_create_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id, tgt_lun_id, lio_dict=None):  # noqa: ANN001, ANN201
     """Map a LUN to target WWN / Initiator port
     The arguments are:
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     init_lun_id   LUN id for the initiator
     tgt_lun_id:   LUN id on target
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
     print("BRUNO lio_create_fc_target_map_lun")
     # print lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id)
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=lio_dict):
-        sts_print(f"INFO: lun {tgt_lun_id} is already mapped to FC target {tgt_wwn}/{init_wwn}")
+        print(f"INFO: lun {tgt_lun_id} is already mapped to FC target {tgt_wwn}/{init_wwn}")
         return True
 
     cmd = "targetcli /tcm_fc/{}/acls/{} create {} {}".format(
         _wwn_2_tgt_wwn(tgt_wwn),
         _wwn_2_tgt_wwn(init_wwn),
         init_lun_id,
         tgt_lun_id,
     )
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not map lun to FC target {tgt_wwn}/{init_wwn}")
+        print(f"FAIL: Could not map lun to FC target {tgt_wwn}/{init_wwn}")
         return False
 
     if not lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id):
-        sts_print(f"FAIL: It seems to have mapped lun {tgt_lun_id}, but it did not")
+        print(f"FAIL: It seems to have mapped lun {tgt_lun_id}, but it did not")
         return False
 
     return True
 
 
-def lio_fc_target_get_mapped_luns(tgt_wwn, init_wwn, lio_dict=None):
+def lio_fc_target_get_mapped_luns(tgt_wwn, init_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Get LUN mapping from tgt_wwn/init_wwn
     The arguments are:
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     Returns:
     Dict:         Dictionary with tgt_lunid : init_lun_id
     None:         No mapping was found.
@@ -1384,37 +1380,37 @@
 
     mapped_luns_dict = lio_dict["tcm_fc"][tgt_wwn]["acls"][init_wwn]
     if not mapped_luns_dict:
         return None
     return mapped_luns_dict
 
 
-def lio_fc_target_unmap_lun(tgt_wwn, init_wwn, init_lun_id):
+def lio_fc_target_unmap_lun(tgt_wwn, init_wwn, init_lun_id):  # noqa: ANN001, ANN201
     """Un map LUN from tgt_wwn/init_wwn
     The arguments are:
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls/{_wwn_2_tgt_wwn(init_wwn)} delete {init_lun_id}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not unmap LUN from target {tgt_wwn}/{init_wwn}")
+        print(f"FAIL: Could not unmap LUN from target {tgt_wwn}/{init_wwn}")
         return False
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id):
-        sts_print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
+        print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
         return False
     return True
 
 
-def lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=None):
+def lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=None):  # noqa: ANN001, ANN201
     """Get initator LUN ID if a LUN is mapped to target WWN / Initiator port
     The arguments are:
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     tgt_lun_id:   LUN id on target
     Returns:
     init_lun_id: If LUN is mapped
@@ -1428,21 +1424,21 @@
         return None
 
     # print "DEBUG lio_get_fc_target_map_lunt t: %s" % tgt_wwn
     # print "DEBUG lio_get_fc_target_map_lunt i: %s" % init_wwn
     # print "DEBUG lio_get_fc_target_map_lunt tgt_id: %s" % tgt_lun_id
     init_acls_dict = lio_dict["tcm_fc"][tgt_wwn]["acls"][init_wwn]
     if tgt_lun_id not in list(init_acls_dict.keys()):
-        # sts_print ("FAIL: Could not get mapping for lun %s on FC target %s/%s" % (tgt_lun_id, tgt_wwn, init_wwn))
+        # print ("FAIL: Could not get mapping for lun %s on FC target %s/%s" % (tgt_lun_id, tgt_wwn, init_wwn))
         return None
 
     return init_acls_dict[tgt_lun_id]
 
 
-def lio_get_fc_target_lun_mapping(bs_type, lun_name, lio_dict=None):
+def lio_get_fc_target_lun_mapping(bs_type, lun_name, lio_dict=None):  # noqa: ANN001, ANN201
     """Get the mapping information for a specifc LUN
     The arguments are:
     bs_type:      Backstore Type
     lun_name:     LUN name
     Returns:
     List:         A list with a dictionary for each mapping found
     None:         If no mapping was found.
@@ -1458,52 +1454,52 @@
     if "mapping" not in list(bs_details_dict.keys()):
         return None
 
     return bs_details_dict["mapping"]
 
 
 # ## FC tag ###
-def lio_tag_fc_initiator(tgt_wwn, init_wwn, tag):
+def lio_tag_fc_initiator(tgt_wwn, init_wwn, tag):  # noqa: ANN001, ANN201
     """Create a tag for initiator wwn
     The arguments are:
     tgt_wwn:     Host wwn
     init_wwn:    Initiator wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls tag {_wwn_2_tgt_wwn(init_wwn)} {tag}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not tag FC initiator {init_wwn}")
+        print(f"FAIL: Could not tag FC initiator {init_wwn}")
         return False
 
     return True
 
 
-def lio_untag_fc_initiator(tgt_wwn, tag):
+def lio_untag_fc_initiator(tgt_wwn, tag):  # noqa: ANN001, ANN201
     """Remove tag from initiator wwn
     The arguments are:
     tgt_wwn:     Host wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls untag {tag}"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print(f"FAIL: Could not untag FC tag {tag}")
+        print(f"FAIL: Could not untag FC tag {tag}")
         return False
 
     return True
 
 
-def lio_is_fc_tag(tgt_wwn, tag):
+def lio_is_fc_tag(tgt_wwn, tag):  # noqa: ANN001, ANN201
     """Check if a tag is an FC initiator tag
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
@@ -1512,15 +1508,15 @@
         return False
     return True
 
 
 ##################################################
 # ################ LIO General ####################
 ##################################################
-def lio_install():
+def lio_install():  # noqa: ANN201
     """Install targetcli tool
     The arguments are:
     None
     Returns:
     True: If targetcli is installed correctly
     False: If some problem happened.
     """
@@ -1529,21 +1525,21 @@
         return False
 
     targetcli_pack = "targetcli"
     if linux.dist_name() == "RHEL" and ver < 7:
         targetcli_pack = "fcoe-target-utils"
 
     if not linux.install_package(targetcli_pack):
-        sts_print(f"FAIL: Could not install {targetcli_pack}")
+        print(f"FAIL: Could not install {targetcli_pack}")
         return False
 
     return True
 
 
-def lio_get_service_name():
+def lio_get_service_name():  # noqa: ANN201
     """Get service name that targetcli uses
     The arguments are:
     None
     Returns:
     String: Name of the service
     None: If some problem happened.
     """
@@ -1554,119 +1550,119 @@
 
     if linux.dist_name() == "RHEL" and ver < 7:
         targetcli_service = "fcoe-target"
 
     return targetcli_service
 
 
-def lio_restart():
+def lio_restart():  # noqa: ANN201
     """Restart LIO service
     The arguments are:
     None
     Returns:
     True: Service started
     False: If some problem happened.
     """
     targetcli_service = lio_get_service_name()
     if not targetcli_service:
-        sts_print("FAIL: lio_restart() - Could not get LIO service name")
+        print("FAIL: lio_restart() - Could not get LIO service name")
         return False
 
     if not linux.service_restart(targetcli_service):
-        sts_print("FAIL: Could not restart LIO service")
+        print("FAIL: Could not restart LIO service")
         return False
     # sleep 5s to avoid service to not be restarted
     # target.service start request repeated too quickly, refusing to start.
     linux.sleep(5)
     return True
 
 
-def lio_show():
+def lio_show():  # noqa: ANN201
     """List LIO configuration
     The arguments are:
     None
     Returns:
     True: If listed config
     False: If some problem happened.
     """
     cmd = "targetcli ls"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print("FAIL: Could not show LIO config")
+        print("FAIL: Could not show LIO config")
         return False
     return True
 
 
-def lio_saveconfig():
+def lio_saveconfig():  # noqa: ANN201
     """Save LIO configuration
     The arguments are:
     None
     Returns:
     True: If config is saved
     False: If some problem happened.
     """
     cmd = "targetcli saveconfig"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print("FAIL: Could not save LIO config")
+        print("FAIL: Could not save LIO config")
         return False
     return True
 
 
-def lio_clearconfig():
+def lio_clearconfig():  # noqa: ANN201
     """Clear LIO configuration
     The arguments are:
     None
     Returns:
     True: If config is deleted
     False: If some problem happened.
     """
-    sts_print("INFO: Cleaning up LIO configuration")
+    print("INFO: Cleaning up LIO configuration")
 
     if not linux.is_installed("targetcli"):
         return True
 
     fileio_dict = lio_get_backstores("fileio")
     if fileio_dict:
         # Delete all files before cleaning configuration
         for lun in list(fileio_dict.keys()):
             lio_delete_backstore(bs_type="fileio", lun_name=lun)
 
     cmd = "targetcli clearconfig true"
 
     if run(cmd, verbose=True).returncode != 0:
-        sts_print("FAIL: Could not delete LIO config")
+        print("FAIL: Could not delete LIO config")
         return False
 
     return True
 
 
-def lio_version():
+def lio_version():  # noqa: ANN201
     """Get targetcli version
     The arguments are:
     None
     Returns:
     String: TargetCli version
     None: If some problem happened.
     """
     cmd = "targetcli version"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: Could not get targetcli version")
+        print("FAIL: Could not get targetcli version")
         return None
 
     version_regex = re.compile(".* version (.*)$")
     m = version_regex.search(output)
     if m:
         return m.group(1)
-    sts_print(f"FAIL: Could not parse targetcli version output ({output})")
+    print(f"FAIL: Could not parse targetcli version output ({output})")
     return None
 
 
-def lio_clean_up_targets(lio_dict=None):
+def lio_clean_up_targets(lio_dict=None):  # noqa: ANN001, ANN201
     """Removing backstore might leave targets with empty mapping
     They should be removed.
     """
     lio_dict = lio_query(lio_dict)
     fc_targets = lio_get_fc_target(lio_dict=lio_dict)
     if not fc_targets:
         # nothing to clean up
@@ -1675,86 +1671,86 @@
     need_to_query_lio = False
     success = True
     for tgt in fc_targets:
         initiators = lio_get_fc_target_acl(tgt, lio_dict=lio_dict)
         if initiators:
             for init in initiators:
                 if not lio_fc_target_get_mapped_luns(tgt, init, lio_dict=lio_dict):
-                    sts_print(f"DEBUG: Should remove initiator {init} from tgt {tgt}")
+                    print(f"DEBUG: Should remove initiator {init} from tgt {tgt}")
                     if not lio_delete_fc_target_acl(tgt, init):
                         success = False
                     need_to_query_lio = True
 
     # Check again for targets without any initiator
     if need_to_query_lio:
         lio_dict = lio_query()
     fc_targets = lio_get_fc_target(lio_dict=lio_dict)
     for tgt in fc_targets:
         initiators = lio_get_fc_target_acl(tgt, lio_dict=lio_dict)
         if not initiators:
-            sts_print(f"DEBUG: Should remove target {tgt}")
+            print(f"DEBUG: Should remove target {tgt}")
             if not lio_delete_fc_target(tgt):
                 success = False
 
     return success
 
 
 class TargetCLI:
-    def __init__(self, path="", disable_check=False):
+    def __init__(self, path="", disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
         self.path = path
         if linux.dist_ver() < 7:
-            sts_print("FATAL: TargetCLI is not supported on RHEL < 7.")
+            print("FATAL: TargetCLI is not supported on RHEL < 7.")
 
         if not linux.install_package("targetcli", check=False):
-            sts_print("FATAL: Could not install targetcli package")
+            print("FATAL: Could not install targetcli package")
 
     @staticmethod
-    def remove_nones(kwargs):
+    def remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @staticmethod
-    def _extract_args(kwargs, keys=None):
+    def _extract_args(kwargs, keys=None):  # noqa: ANN001, ANN205
         keys = keys or ["return_output", "verbosity", "path"]
         arguments = {}
         for key in keys:
             if key not in kwargs:
                 continue
             arguments[key] = kwargs.pop(key)
         return arguments, kwargs
 
-    def _run(self, cmd, verbosity=True, return_output=False, path=None):
+    def _run(self, cmd, verbosity=True, return_output=False, path=None):  # noqa: ANN001, ANN202
         # Constructs the command to run and runs it
 
         if path is not None:
             self.path = path
 
         cmd = "targetcli cd" if cmd == "cd" and self.path is None else "targetcli " + self.path + " " + cmd
 
         if return_output:
             ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
-                sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
         ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
-    def ls(self, depth="", **kwargs):
+    def ls(self, depth="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"ls {depth}", **kwargs)
 
-    def cd(self, **kwargs):
+    def cd(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("cd", **kwargs)
 
-    def pwd(self, **kwargs):
+    def pwd(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("pwd", **kwargs)
 
-    def create(self, **kwargs):
+    def create(self, **kwargs):  # noqa: ANN003, ANN201
         keys = None
         cmd = "create "
         arguments, kwargs = self._extract_args(kwargs)
         # the following ensures the ordering is correct in correct paths
         # True means it is required, False it is optional
         if "backstores/block" in self.path:
             keys = {"name": True, "dev": True, "readonly": False, "wwn": False}
@@ -1827,19 +1823,19 @@
         else:
             keys = {"wwn": False}
         for key in keys:
             try:
                 cmd += f"{key}={kwargs[key]} "
             except KeyError:
                 if not self.disable_check and keys[key]:
-                    sts_print(f"FAIL: Create on path '{self.path}' requires argument {key}.")
+                    print(f"FAIL: Create on path '{self.path}' requires argument {key}.")
                     return 1
         return self._run(cmd, **arguments)
 
-    def delete(self, **kwargs):
+    def delete(self, **kwargs):  # noqa: ANN003, ANN201
         keys = None
         cmd = "delete "
         arguments, kwargs = self._extract_args(kwargs)
         # the following ensures the ordering is correct in correct paths
         # True means it is required, False it is optional
         if "backstores/block" in self.path:  # noqa: SIM114
             keys = {"name": True}
@@ -1877,79 +1873,84 @@
             keys = {"wwn": True}
 
         for key in keys:
             try:
                 cmd += f"{key}={kwargs[key]} "
             except KeyError:
                 if not self.disable_check and keys[key]:
-                    sts_print(f"FAIL: Delete on path '{self.path}' requires argument {key}.")
+                    print(f"FAIL: Delete on path '{self.path}' requires argument {key}.")
                     return 1
 
         return self._run(cmd, **arguments)
 
-    def help(self, topic="", **kwargs):  # noqa: A003
+    def help(self, topic="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
         return self._run(f"help {topic}", **kwargs)
 
-    def saveconfig(self, savefile=None, **kwargs):
+    def saveconfig(self, savefile=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         cmd = "saveconfig"
         if savefile:
             cmd += f" {savefile}"
         return self._run(cmd, **kwargs)
 
-    def restoreconfig(self, savefile="/etc/target/saveconfig.json", clearexisting=False, **kwargs):
+    def restoreconfig(  # noqa: ANN201
+        self,
+        savefile="/etc/target/saveconfig.json",  # noqa: ANN001
+        clearexisting=False,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
+    ):
         return self._run(f"restoreconfig {savefile} {clearexisting}", **kwargs)
 
-    def clearconfig(self, confirm=True, **kwargs):
+    def clearconfig(self, confirm=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"clearconfig {confirm}", **kwargs)
 
-    def sessions(self, action="", sid="", **kwargs):
+    def sessions(self, action="", sid="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"sessions {action} {sid}", **kwargs)
 
-    def exit(self, **kwargs):  # noqa: A003
+    def exit(self, **kwargs):  # noqa: A003, ANN003, ANN201
         return self._run("exit", **kwargs)
 
-    def get(self, group="", **kwargs):
+    def get(self, group="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
         cmd = f"get {group} {' '.join(kwargs.keys())}"
         return self._run(cmd, **arguments)
 
-    def set(self, group="", **kwargs):  # noqa: A003
+    def set(self, group="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
         params = [
             f"{kwarg}='{kwargs[kwarg]}'" if kwargs[kwarg] != "" else f"{kwarg}='{kwargs[kwarg]}'" for kwarg in kwargs
         ]
         cmd = f"set {group} {' '.join(params)}"
         return self._run(cmd, **arguments)
 
-    def info(self, **kwargs):
+    def info(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("info", **kwargs)
 
-    def version(self, **kwargs):
+    def version(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("version", **kwargs)
 
-    def status(self, **kwargs):
+    def status(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("status", **kwargs)
 
-    def refresh(self, **kwargs):
+    def refresh(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("refresh", **kwargs)
 
-    def disable(self, **kwargs):
+    def disable(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("disable", **kwargs)
 
-    def enable(self, **kwargs):
+    def enable(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("enable", **kwargs)
 
-    def bookmarks(self, **kwargs):
+    def bookmarks(self, **kwargs):  # noqa: ANN003, ANN201
         # How to use this?
         return self._run("bookmarks", **kwargs)
 
-    def enable_iser(self, boolean="", **kwargs):
+    def enable_iser(self, boolean="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"enable_iser {boolean}", **kwargs)
 
-    def enable_offload(self, boolean="", **kwargs):
+    def enable_offload(self, boolean="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"enable_offload {boolean}", **kwargs)
 
-    def tag(self, wwn_or_tag="", new_tag="", **kwargs):
+    def tag(self, wwn_or_tag="", new_tag="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"tag {wwn_or_tag} {new_tag}", **kwargs)
 
-    def untag(self, wwn_or_tag="", **kwargs):
+    def untag(self, wwn_or_tag="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run(f"untag {wwn_or_tag}", **kwargs)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/loopdev.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import sys
 from pathlib import Path
 
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.size import size_bytes_2_size_human, size_human_2_size_bytes
 
 
-def _get_loop_path(name):
+def _get_loop_path(name):  # noqa: ANN001, ANN202
     loop_path = name
     if "/dev/" not in name:
         loop_path = "/dev/" + name
 
     return loop_path
 
 
-def _get_image_file(name, image_path):
+def _get_image_file(name, image_path):  # noqa: ANN001, ANN202
     return f"{image_path}/{name}.img"
 
 
-def _standardize_name(name):
+def _standardize_name(name):  # noqa: ANN001, ANN202
     """Make sure use same standard for name, for example remove /dev/ from it if exists."""
     if not name:
-        sts_print("FAIL: _standardize_name() - requires name as parameter")
+        print("FAIL: _standardize_name() - requires name as parameter")
         return None
     return name.replace("/dev/", "")
 
 
-def create_loopdev(name=None, size=1024, image_path="/var/tmp", reuse_file=False):
+def create_loopdev(name=None, size=1024, image_path="/var/tmp", reuse_file=False):  # noqa: ANN001, ANN201
     """Create a loop device
     Parameters:
     name:         eg. loop0 (optional)
     size:         Size in MB (default: 1024MB)
     image_path:   Path to store the image (default: /var/tmp)
     reuse_file:   Reuse a previous image file (default: False).
     """
@@ -48,15 +47,15 @@
     #    if size is None:
     #        size = 1024
 
     if not name:
         cmd = "losetup -f"
         retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print("FAIL: Could not find free loop device")
+            print("FAIL: Could not find free loop device")
             print(output)
             return None
         name = output
     name = _standardize_name(name)
 
     fname = _get_image_file(name, image_path)
     print("INFO: Creating loop device %s with size %d" % (fname, size))
@@ -67,136 +66,136 @@
         run(f"rm -f {fname}")
 
     # make sure we have enough space to create the file
     free_space_bytes = linux.get_free_space(image_path)
     # Convert the size given in megabytes to bytes
     size_bytes = int(size_human_2_size_bytes(f"{size}MiB"))
     if free_space_bytes <= size_bytes:
-        sts_print(
+        print(
             f"FAIL: Not enough space to create loop device with size {size_bytes_2_size_human(size_bytes)}",
         )
-        sts_print(f"available space: {size_bytes_2_size_human(free_space_bytes)}")
+        print(f"available space: {size_bytes_2_size_human(free_space_bytes)}")
         return None
     print(f"INFO: Creating file {fname}")
     # cmd = "dd if=/dev/zero of=%s seek=%d bs=1M count=0" % (fname, size)
     cmd = f"fallocate -l {size}M {fname}"
     try:
         # We are just creating the file, not writting zeros to it
         if run(cmd).returncode != 0:
-            sts_print(f"command failed with code {retcode}")
-            sts_print("FAIL: Could not create loop device image file")
+            print(f"command failed with code {retcode}")
+            print("FAIL: Could not create loop device image file")
             return None
     except OSError as e:
         print("command failed: ", e, file=sys.stderr)
         return None
 
     loop_path = _get_loop_path(name)
     # detach loop device if it exists
     detach_loopdev(loop_path)
 
     # Going to associate the file to the loopdevice
     cmd = f"losetup {loop_path} {fname}"
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not create loop device")
+        print("FAIL: Could not create loop device")
         return None
 
     return loop_path
 
 
-def delete_loopdev(name):
+def delete_loopdev(name):  # noqa: ANN001, ANN201
     """Delete a loop device
     Parameters:
     name:     eg. loop0 or /dev/loop0.
     """
     if not name:
-        sts_print("FAIL: delete_loopdev() - requires name parameter")
+        print("FAIL: delete_loopdev() - requires name parameter")
         return False
 
     print(f"INFO: Deleting loop device {name}")
     name = _standardize_name(name)
 
     loop_path = _get_loop_path(name)
 
     # find image file
     fname = get_loopdev_file(loop_path)
     if fname is None:
-        sts_print(f"WARN: could not find loopdev named {name}")
+        print(f"WARN: could not find loopdev named {name}")
         # loopdev does not exist, nothing to do
         return True
 
     # detach loop device if it exists
     if not detach_loopdev(name):
-        sts_print(f"FAIL: could not detach {loop_path}")
+        print(f"FAIL: could not detach {loop_path}")
         return False
 
     if Path(fname).is_file():
         cmd = f"rm -f {fname}"
         if run(cmd).returncode != 0:
-            sts_print(f"FAIL: Could not delete loop device file {fname}")
+            print(f"FAIL: Could not delete loop device file {fname}")
             return False
 
     # check if loopdev file is deleted as it sometimes remains
     if Path(fname).is_file():
-        sts_print(f"FAIL: Deleted loop device file {fname} but it is still there")
+        print(f"FAIL: Deleted loop device file {fname} but it is still there")
         return False
 
     return True
 
 
 # show loop devices
-def list_loopdev():
+def list_loopdev():  # noqa: ANN201
     retcode, output = run_ret_out("losetup -a", return_output=True)
     return retcode, output
 
 
 # Return all loop devices
-def get_loopdev():
+def get_loopdev():  # noqa: ANN201
     # example of output on rhel-6.7
     # /dev/loop0: [fd00]:396428 (/var/tmp/loop0.img)
     retcode, output = run_ret_out("losetup -a | awk '{print$1}'", return_output=True, verbose=False)
     # retcode, output = run_ret_out("losetup -l | tail -n +2", return_output=True, verbose=False)
     if retcode != 0:
-        sts_print("FAIL: get_loopdev failed to execute")
+        print("FAIL: get_loopdev failed to execute")
         print(output)
         return None
 
     devs = None
     if output:
         devs = output.split("\n")
         # remove the ":" character from all devices
         devs = [d.replace(":", "") for d in devs]
 
     return devs
 
 
 # Return loop device file for given path
-def get_loopdev_file(loop_path):
+def get_loopdev_file(loop_path):  # noqa: ANN001, ANN201
     # example of output on rhel-6.7
     # /dev/loop0: [fd00]:396428 (/var/tmp/loop0.img)
     retcode, output = run_ret_out(
         "losetup -a | grep '%s:' | awk '{print$3}'" % loop_path,
         return_output=True,
         verbose=False,
     )
     if retcode != 0:
-        sts_print("FAIL: get_loopdev_file failed to execute")
+        print("FAIL: get_loopdev_file failed to execute")
         print(output)
         return None
 
     if output:
         # remove the "(" and ")" character from device
         dev = output[1:-1]
     else:
-        sts_print("WARN: get_loopdev_file failed to requested loopdev")
+        print("WARN: get_loopdev_file failed to requested loopdev")
         return None
 
     return dev
 
 
-def detach_loopdev(name=None):
+def detach_loopdev(name=None):  # noqa: ANN001, ANN201
     cmd = "losetup -D"
     if name:
         devs = get_loopdev()
         if not devs:
             # No device was found
             return False
 
@@ -209,11 +208,11 @@
             cmd = f"losetup -d {dev_path}"
         else:
             # if loop device does not exist just ignore it
             return True
 
     # run losetup -D or -d <device>
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not detach loop device")
+        print("FAIL: Could not detach loop device")
         return False
 
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/lsm.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import os
 import re
 import sys
 from contextlib import suppress
 from time import sleep
+from typing import Dict, List, Union
 
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.cli_tools import (
     FailedCheckExceptionError,
     Wrapper,
     WrongArgumentExceptionError,
     WrongCommandExceptionError,
 )
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.persistent_vars import read_env, read_var
 
 
-def check_ssl(protocol) -> bool:
+def check_ssl(protocol) -> bool:  # noqa: ANN001
     """Checks if fmf_protocol is ssl/no_ssl and limits the protocol by this."""
     try:
         ssl = read_env("fmf_protocol")
     except KeyError:
         # Protocol not limited
         return True
     if ssl == "ssl" and "ssl" in protocol or ssl == "no_ssl" and "ssl" not in protocol:
         return True
     return False
 
 
-def yield_lsm_config():
+def yield_lsm_config():  # noqa: ANN201
     config = {"protocols": [], "username": None, "password": None, "target": None}
 
     for conf in config:
         with suppress(OSError):
             config[conf] = read_var("LSM_" + conf.upper())
 
     try:
@@ -53,15 +53,15 @@
     for protocol in protocols:
         if not check_ssl(protocol):
             continue
         config["protocol"] = protocol
         yield config
 
 
-def get_data_from_script_output(data, id="id"):
+def get_data_from_script_output(data, id="id"):  # noqa: ANN001, ANN201
     split_string = re.match("(-*)", data).group()
     try:
         items = [x for x in data.split(split_string) if id in x]
     except ValueError as e:
         print(repr(e))
         return None
     data = {}
@@ -75,147 +75,147 @@
                 data[item_id] = {}
             else:
                 line_data = line.split("|")
                 data[item_id][line_data[0].strip()] = line_data[1].strip()
     return data
 
 
-def get_local_disk_data(data):
+def get_local_disk_data(data):  # noqa: ANN001, ANN201
     return get_data_from_script_output(data, id="Path")
 
 
-def get_id_from_name(data, name, field="Name", item_id="id"):
+def get_id_from_name(data, name, field="Name", item_id="id"):  # noqa: ANN001, ANN201
     data = get_data_from_script_output(data, id=item_id)
     for line in data:
         if data[line][field] == name:
             return line
     print(f"FAIL: Could not find item named '{name}'.")
     return None
 
 
-def get_data_from_id(data, name, field="Name", item_id="id"):
+def get_data_from_id(data, name, field="Name", item_id="id"):  # noqa: ANN001, ANN201
     data = get_data_from_script_output(data, id=item_id)
     for line in data:
         if line != name:
             continue
         return data[line][field]
     print(f"FAIL: Could not find item named '{name}'.")
     return None
 
 
-def get_ag_id_from_name(data, name):
+def get_ag_id_from_name(data, name):  # noqa: ANN001, ANN201
     return get_id_from_name(data, name)
 
 
-def get_fs_id_from_name(data, name):
+def get_fs_id_from_name(data, name):  # noqa: ANN001, ANN201
     return get_id_from_name(data, name)
 
 
-def get_vol_id_from_name(data, name):
+def get_vol_id_from_name(data, name):  # noqa: ANN001, ANN201
     return get_id_from_name(data, name)
 
 
-def get_export_id_from_export_path(data, export_path):
+def get_export_id_from_export_path(data, export_path):  # noqa: ANN001, ANN201
     # policy is 'disabled' but cli takes 'disable'
     return get_id_from_name(data, export_path, field="Export Path")
 
 
-def get_system_read_pct_of_sys(data, sys):
+def get_system_read_pct_of_sys(data, sys):  # noqa: ANN001, ANN201
     return get_data_from_script_output(data)[sys]["Read Cache Percentage"]
 
 
-def get_cache_policy_from_id(data, vol_id, field):
+def get_cache_policy_from_id(data, vol_id, field):  # noqa: ANN001, ANN201
     return translate_cache_policy(get_data_from_id(data, vol_id, field=field, item_id="Volume id"))
 
 
-def translate_cache_policy(policy):
+def translate_cache_policy(policy):  # noqa: ANN001, ANN201
     dictionary = {
         "Write Back": "WB",
         "Write Through": "WT",
         "Auto": "AUTO",
         "Enabled": "enable",
         "Disabled": "disable",
     }
     try:
         return dictionary[policy]
     except KeyError:
         return policy
 
 
-def get_replace_dict():
+def get_replace_dict():  # noqa: ANN201
     """Returns dict of keys to replace from fmf to sts.lsm.LibStorageMgmt.
 
     Returns:
       dict.
     """
     return {
         "ag_name": "name",
         "vol_name": "name",
         "fs_name": "name",
         "snap_name": "name",
         "rep_name": "name",
     }
 
 
-def _cli(func):
+def _cli(func):  # noqa: ANN001, ANN202
     # This is a decorator to mark functions callable by 'lsmcli'
     func.cli = True
     return func
 
 
 class LibStorageMgmt(Wrapper):
     def __init__(
         self,
-        username=None,
-        password=None,
-        target=None,
-        protocol=None,
-        disable_check=False,
-    ):
+        username=None,  # noqa: ANN001
+        password=None,  # noqa: ANN001
+        target=None,  # noqa: ANN001
+        protocol=None,  # noqa: ANN001
+        disable_check=False,  # noqa: ANN001
+    ) -> None:
         self.disable_check = disable_check
         if linux.dist_ver() < 7:
-            sts_print("FATAL: libstoragemgmt is not supported on RHEL < 7.")
+            print("FATAL: libstoragemgmt is not supported on RHEL < 7.")
 
         self.username = None
         self.password = None
         self.target = None
         self.protocol = None
         self.port = None
         self.query_params = None
         self.timeout = None
 
         # persistent previous values
-        self.previous_sys_read_pct = {}
-        self.previous_phy_disk_cache_policy = {}
-        self.previous_read_cache_policy = {}
-        self.previous_write_cache_policy = {}
-        self.previous_local_disk_ident_led = {}
-        self.previous_local_disk_fault_led = {}
+        self.previous_sys_read_pct: dict = {}
+        self.previous_phy_disk_cache_policy: dict = {}
+        self.previous_read_cache_policy: dict = {}
+        self.previous_write_cache_policy: dict = {}
+        self.previous_local_disk_ident_led: dict = {}
+        self.previous_local_disk_fault_led: dict = {}
 
         # local target does not require anything of this and megaraid/sim needs only protocol
         if username and password and target and protocol:
             self.username = username
             self.password = password
             self.target = target
             self.protocol = protocol
         elif protocol and "megaraid" in protocol or "sim" in protocol:
             self.protocol = protocol
 
         if self.password:
             os.environ["LSMCLI_PASSWORD"] = self.password
-            sts_print("INFO: Password set")
+            print("INFO: Password set")
         elif os.environ.get("LSMCLI_PASSWORD"):
             del os.environ["LSMCLI_PASSWORD"]
-            sts_print("INFO: Password cleaned")
+            print("INFO: Password cleaned")
 
         requires_restart = False
         # stop if lsm package cannot be installed
         if not linux.is_installed("libstoragemgmt"):
             if not linux.install_package("libstoragemgmt", check=False):
-                sts_print("FATAL: Could not install libstoragemgmt package")
+                print("FATAL: Could not install libstoragemgmt package")
             else:
                 requires_restart = True
 
         if self.protocol == "smispy":
             self.port = "5988"
             self.query_params = "?namespace=root/emc"
         if self.protocol == "smispy+ssl":
@@ -225,51 +225,51 @@
             self.query_params = "?namespace=root/emc&no_ssl_verify=yes"
 
         # install protocol specific packages
         if self.protocol:
             if "ontap" in self.protocol:
                 if not linux.is_installed("libstoragemgmt-netapp-plugin"):
                     if not linux.install_package("libstoragemgmt-netapp-plugin", check=False):
-                        sts_print("FATAL: Could not install LSM NetApp plugin")
+                        print("FATAL: Could not install LSM NetApp plugin")
                     else:
                         requires_restart = True
             elif "smispy" in self.protocol:
                 if not linux.is_installed("libstoragemgmt-smis-plugin"):
                     if not linux.install_package("libstoragemgmt-smis-plugin", check=False):
-                        sts_print("FATAL: Could not install LSM SMIS plugin")
+                        print("FATAL: Could not install LSM SMIS plugin")
                     else:
                         requires_restart = True
             elif "targetd" in self.protocol:
                 if not linux.is_installed("libstoragemgmt-targetd-plugin"):
                     if not linux.install_package("libstoragemgmt-targetd-plugin", check=False):
-                        sts_print("FATAL: Could not install LSM targetd plugin")
+                        print("FATAL: Could not install LSM targetd plugin")
                     else:
                         requires_restart = True
             elif "megaraid" in self.protocol:
                 if not linux.is_installed("libstoragemgmt-megaraid-plugin"):
                     if not linux.install_package("libstoragemgmt-megaraid-plugin", check=False):
-                        sts_print("FATAL: Could not install LSM megaraid plugin")
+                        print("FATAL: Could not install LSM megaraid plugin")
                     else:
                         requires_restart = True
                 # needs to install 3rd party tool
                 if not linux.install_package("storcli"):
-                    sts_print("FATAL: Could not install storcli")
+                    print("FATAL: Could not install storcli")
 
         if requires_restart:
             if run("service libstoragemgmt restart", verbose=True).returncode != 0:
-                sts_print("FATAL: Could not restart libstoragemgmt service")
+                print("FATAL: Could not restart libstoragemgmt service")
             else:
-                sts_print("INFO: Waiting for service to restart.")
+                print("INFO: Waiting for service to restart.")
                 sleep(5)
         elif linux.service_status("libstoragemgmt") != 0:  # noqa: SIM102
             if linux.service_start("libstoragemgmt"):
-                sts_print("INFO: Waiting for service to start.")
+                print("INFO: Waiting for service to start.")
                 sleep(5)
 
-        self.commands = {
+        self.commands: Dict[str, Union[str, List[str]]] = {
             "list": "list",
             "job_status": "job-status",
             "capabilities": "capabilities",
             "plugin_info": "plugin-info",
             "volume_create": "volume-create",
             "volume_raid_create": "volume-raid-create",
             "volume_raid_create_cap": "volume-raid-create-cap",
@@ -482,44 +482,44 @@
                 ],
                 " --path=",
             ],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
-        sts_print("INFO: LSM configured")
+        print("INFO: LSM configured")
 
-    def _check(self, cmd):
+    def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check or cmd:
             # Do not check if checking is disabled
             return True
 
         return True
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):
+    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
 
         ret_fail = False
         if return_output:
             ret_fail = (False, None)
 
         try:
             command = self._add_command(cmd)
             command = self._add_arguments(command, **kwargs)
 
         except WrongCommandExceptionError as e:
-            sts_print(f"WARN: Given command '{e.command}' is not allowed in this version.")
+            print(f"WARN: Given command '{e.command}' is not allowed in this version.")
             return ret_fail
         except WrongArgumentExceptionError as e:
             message = f"WARN: Given argument '{e.argument}' is not allowed for given command."
             if e.command:
                 message = message[:-1] + " '" + e.command + "'."
             if e.arguments:
                 message += f"\nPlease use only these: {', '.join(e.arguments)}."
-            sts_print(message)
+            print(message)
             return ret_fail
 
         cmd = "lsmcli "
         if self.timeout:
             cmd += f"-w {self.timeout} "
         if self.protocol:
             cmd += f'-u "{self.protocol}://'
@@ -533,45 +533,45 @@
         cmd += command
 
         try:
             self._check(cmd)
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
-            sts_print(f"WARN: Failed checking on argument {e.argument}")
+            print(f"WARN: Failed checking on argument {e.argument}")
             return ret_fail
 
         if return_output:
             ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
-                sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
         ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
-    def _remove_nones(kwargs):
+    def _remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @_cli
-    def list(  # noqa: A003
+    def list(  # noqa: A003, ANN201
         self,
-        lsm_type=None,
-        fs=None,
-        sys=None,
-        pool=None,
-        vol=None,
-        disk=None,
-        ag=None,
-        nfs_export=None,
-        tgt=None,
-        **kwargs,
+        lsm_type=None,  # noqa: ANN001
+        fs=None,  # noqa: ANN001
+        sys=None,  # noqa: ANN001
+        pool=None,  # noqa: ANN001
+        vol=None,  # noqa: ANN001
+        disk=None,  # noqa: ANN001
+        ag=None,  # noqa: ANN001
+        nfs_export=None,  # noqa: ANN001
+        tgt=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
                 "lsm_type": lsm_type,
                 "fs": fs,
                 "sys": sys,
                 "pool": pool,
@@ -581,220 +581,234 @@
                 "nfs_export": nfs_export,
                 "tgt": tgt,
             },
         )
         return self._run("list", **self._remove_nones(kwargs))
 
     @_cli
-    def job_status(self, job=None, **kwargs):
+    def job_status(self, job=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"job": job})
         return self._run("job_status", **self._remove_nones(kwargs))
 
     @_cli
-    def capabilities(self, sys=None, **kwargs):
+    def capabilities(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"sys": sys})
         return self._run("capabilities", **self._remove_nones(kwargs))
 
     @_cli
-    def plugin_info(self, **kwargs):
+    def plugin_info(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("plugin_info", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_create(self, name=None, size=None, pool=None, provisioning=None, **kwargs):
+    def volume_create(  # noqa: ANN201
+        self,
+        name=None,  # noqa: ANN001
+        size=None,  # noqa: ANN001
+        pool=None,  # noqa: ANN001
+        provisioning=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
+    ):
         kwargs.update({"name": name, "size": size, "pool": pool, "provisioning": provisioning})
         return self._run("volume_create", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_raid_create(self, name=None, raid_type=None, disk=None, strip_size=None, **kwargs):
+    def volume_raid_create(  # noqa: ANN201
+        self,
+        name=None,  # noqa: ANN001
+        raid_type=None,  # noqa: ANN001
+        disk=None,  # noqa: ANN001
+        strip_size=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
+    ):
         kwargs.update(
             {
                 "name": name,
                 "raid_type": raid_type,
                 "disk": disk,
                 "strip_size": strip_size,
             },
         )
         return self._run("volume_raid_create", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_raid_create_cap(self, sys=None, **kwargs):
+    def volume_raid_create_cap(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"sys": sys})
         return self._run("volume_raid_create_cap", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_ident_led_on(self, vol=None, **kwargs):
+    def volume_ident_led_on(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_ident_led_on", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_ident_led_off(self, vol=None, **kwargs):
+    def volume_ident_led_off(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_ident_led_off", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_delete(self, vol=None, **kwargs):
+    def volume_delete(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_delete", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_resize(self, vol=None, size=None, **kwargs):
+    def volume_resize(self, vol=None, size=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "size": size})
         return self._run("volume_resize", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_replicate(self, vol=None, name=None, rep_type=None, pool=None, **kwargs):
+    def volume_replicate(self, vol=None, name=None, rep_type=None, pool=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "name": name, "rep_type": rep_type, "pool": pool})
         return self._run("volume_replicate", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_replicate_range(
+    def volume_replicate_range(  # noqa: ANN201
         self,
-        src_vol=None,
-        dst_vol=None,
-        rep_type=None,
-        src_start=None,
-        dst_start=None,
-        count=None,
-        **kwargs,
+        src_vol=None,  # noqa: ANN001
+        dst_vol=None,  # noqa: ANN001
+        rep_type=None,  # noqa: ANN001
+        src_start=None,  # noqa: ANN001
+        dst_start=None,  # noqa: ANN001
+        count=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
                 "src_vol": src_vol,
                 "dst_vol": dst_vol,
                 "rep_type": rep_type,
                 "src_start": src_start,
                 "dst_start": dst_start,
                 "count": count,
             },
         )
         return self._run("volume_replicate_range", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_replicate_range_block_size(self, sys=None, **kwargs):
+    def volume_replicate_range_block_size(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"sys": sys})
         return self._run("volume_replicate_range_block_size", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_dependants(self, vol=None, **kwargs):
+    def volume_dependants(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_dependants", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_dependants_rm(self, vol=None, **kwargs):
+    def volume_dependants_rm(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_dependants_rm", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_access_group(self, vol=None, **kwargs):
+    def volume_access_group(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_access_group", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_mask(self, vol=None, ag=None, **kwargs):
+    def volume_mask(self, vol=None, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "ag": ag})
         return self._run("volume_mask", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_unmask(self, vol=None, ag=None, **kwargs):
+    def volume_unmask(self, vol=None, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "ag": ag})
         return self._run("volume_unmask", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_enable(self, vol=None, **kwargs):
+    def volume_enable(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_enable", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_disable(self, vol=None, **kwargs):
+    def volume_disable(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_disable", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_raid_info(self, vol=None, **kwargs):
+    def volume_raid_info(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_raid_info", **self._remove_nones(kwargs))
 
     @_cli
-    def pool_member_info(self, pool=None, **kwargs):
+    def pool_member_info(self, pool=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"pool": pool})
         return self._run("pool_member_info", **self._remove_nones(kwargs))
 
     @_cli
-    def access_group_create(self, name=None, init=None, sys=None, **kwargs):
+    def access_group_create(self, name=None, init=None, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"name": name, "init": init, "sys": sys})
         return self._run("access_group_create", **self._remove_nones(kwargs))
 
     @_cli
-    def access_group_add(self, ag=None, init=None, **kwargs):
+    def access_group_add(self, ag=None, init=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"ag": ag, "init": init})
         return self._run("access_group_add", **self._remove_nones(kwargs))
 
     @_cli
-    def access_group_remove(self, ag=None, init=None, **kwargs):
+    def access_group_remove(self, ag=None, init=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"ag": ag, "init": init})
         return self._run("access_group_remove", **self._remove_nones(kwargs))
 
     @_cli
-    def access_group_delete(self, ag=None, **kwargs):
+    def access_group_delete(self, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"ag": ag})
         return self._run("access_group_delete", **self._remove_nones(kwargs))
 
     @_cli
-    def access_group_volumes(self, ag=None, **kwargs):
+    def access_group_volumes(self, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"ag": ag})
         return self._run("access_group_volumes", **self._remove_nones(kwargs))
 
     @_cli
-    def iscsi_chap(
+    def iscsi_chap(  # noqa: ANN201
         self,
-        init=None,
-        in_user=None,
-        in_pass=None,
-        out_user=None,
-        out_pass=None,
-        **kwargs,
+        init=None,  # noqa: ANN001
+        in_user=None,  # noqa: ANN001
+        in_pass=None,  # noqa: ANN001
+        out_user=None,  # noqa: ANN001
+        out_pass=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
                 "init": init,
                 "in_user": in_user,
                 "in_pass": in_pass,
                 "out_user": out_user,
                 "out_pass": out_pass,
             },
         )
         return self._run("iscsi_chap", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_create(self, fs=None, **kwargs):
+    def fs_create(self, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs})
         return self._run("fs_create", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_delete(self, fs=None, **kwargs):
+    def fs_delete(self, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs})
         return self._run("fs_delete", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_resize(self, fs=None, size=None, **kwargs):
+    def fs_resize(self, fs=None, size=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs, "size": size})
         return self._run("fs_resize", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_export(
+    def fs_export(  # noqa: ANN201
         self,
-        fs=None,
-        exportpath=None,
-        anonguid=None,
-        anongid=None,
-        auth_type=None,
-        root_host=None,
-        ro_host=None,
-        rw_host=None,
-        **kwargs,
+        fs=None,  # noqa: ANN001
+        exportpath=None,  # noqa: ANN001
+        anonguid=None,  # noqa: ANN001
+        anongid=None,  # noqa: ANN001
+        auth_type=None,  # noqa: ANN001
+        root_host=None,  # noqa: ANN001
+        ro_host=None,  # noqa: ANN001
+        rw_host=None,  # noqa: ANN001
+        **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
                 "fs": fs,
                 "exportpath": exportpath,
                 "anonguid": anonguid,
                 "anongid": anongid,
@@ -803,132 +817,132 @@
                 "ro_host": ro_host,
                 "rw_host": rw_host,
             },
         )
         return self._run("fs_export", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_unexport(self, export=None, **kwargs):
+    def fs_unexport(self, export=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"export": export})
         return self._run("fs_unexport", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_clone(self, src_fs=None, dst_name=None, backing_snapshot=None, **kwargs):
+    def fs_clone(self, src_fs=None, dst_name=None, backing_snapshot=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update(
             {
                 "src_fs": src_fs,
                 "dst_name": dst_name,
                 "backing_snapshot": backing_snapshot,
             },
         )
         return self._run("fs_clone", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_snap_create(self, name=None, fs=None, **kwargs):
+    def fs_snap_create(self, name=None, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"name": name, "fs": fs})
         return self._run("fs_snap_create", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_snap_delete(self, snap=None, fs=None, **kwargs):
+    def fs_snap_delete(self, snap=None, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"snap": snap, "fs": fs})
         return self._run("fs_snap_delete", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_snap_restore(self, fs=None, snap=None, lsm_file=None, fileas=None, **kwargs):
+    def fs_snap_restore(self, fs=None, snap=None, lsm_file=None, fileas=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs, "snap": snap, "lsm_file": lsm_file, "fileas": fileas})
         return self._run("fs_snap_restore", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_dependants(self, fs=None, lsm_file=None, **kwargs):
+    def fs_dependants(self, fs=None, lsm_file=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs, "lsm_file": lsm_file})
         return self._run("fs_dependants", **self._remove_nones(kwargs))
 
     @_cli
-    def fs_dependants_rm(self, fs=None, lsm_file=None, **kwargs):
+    def fs_dependants_rm(self, fs=None, lsm_file=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs, "lsm_file": lsm_file})
         return self._run("fs_dependants_rm", **self._remove_nones(kwargs))
 
     @_cli
-    def file_clone(self, fs=None, src=None, dst=None, backing_snapshot=None, **kwargs):
+    def file_clone(self, fs=None, src=None, dst=None, backing_snapshot=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"fs": fs, "src": src, "dst": dst, "backing_snapshot": backing_snapshot})
         return self._run("file_clone", **self._remove_nones(kwargs))
 
     @_cli
-    def system_read_cache_pct_update(self, sys=None, read_pct=None, **kwargs):
+    def system_read_cache_pct_update(self, sys=None, read_pct=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"sys": sys, "read_pct": read_pct})
         return self._run("system_read_cache_pct_update", **self._remove_nones(kwargs))
 
     @_cli
-    def local_disk_list(self, **kwargs):
+    def local_disk_list(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("local_disk_list", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_cache_info(self, vol=None, **kwargs):
+    def volume_cache_info(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol})
         return self._run("volume_cache_info", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_phy_disk_cache_update(self, vol=None, policy=None, **kwargs):
+    def volume_phy_disk_cache_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "policy": policy})
         return self._run("volume_phy_disk_cache_update", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_read_cache_policy_update(self, vol=None, policy=None, **kwargs):
+    def volume_read_cache_policy_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "policy": policy})
         return self._run("volume_read_cache_policy_update", **self._remove_nones(kwargs))
 
     @_cli
-    def volume_write_cache_policy_update(self, vol=None, policy=None, **kwargs):
+    def volume_write_cache_policy_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"vol": vol, "policy": policy})
         return self._run("volume_write_cache_policy_update", **self._remove_nones(kwargs))
 
     @_cli
-    def local_disk_ident_led_on(self, path=None, **kwargs):
+    def local_disk_ident_led_on(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"path": path})
         return self._run("local_disk_ident_led_on", **self._remove_nones(kwargs))
 
     @_cli
-    def local_disk_ident_led_off(self, path=None, **kwargs):
+    def local_disk_ident_led_off(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"path": path})
         return self._run("local_disk_ident_led_off", **self._remove_nones(kwargs))
 
     @_cli
-    def local_disk_fault_led_on(self, path=None, **kwargs):
+    def local_disk_fault_led_on(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"path": path})
         return self._run("local_disk_fault_led_on", **self._remove_nones(kwargs))
 
     @_cli
-    def local_disk_fault_led_off(self, path=None, **kwargs):
+    def local_disk_fault_led_off(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update({"path": path})
         return self._run("local_disk_fault_led_off", **self._remove_nones(kwargs))
 
-    def help(self, cmd=""):  # noqa: A003
+    def help(self, cmd=""):  # noqa: A003, ANN001, ANN201
         """Retrieve help.
         The arguments are:
         cmd - optional | get help on this command
         Returns:
         Boolean:
         True if success
         False in case of failure.
         """
         if cmd and cmd not in list(self.commands.keys()):
-            sts_print(f"FAIL: Unknown command {cmd}.")
+            print(f"FAIL: Unknown command {cmd}.")
             return False
 
         command = f"{cmd.replace('_', '-')} -h"
         return run(command, verbose=True)
 
-    def version(self, cmd=""):
+    def version(self, cmd=""):  # noqa: ANN001, ANN201
         """Retrieve plugin version.
         The arguments are:
         cmd - optional | get version of this command
         Returns:
         Boolean:
         True if success
         False in case of failure.
         """
         if cmd and cmd not in list(self.commands.keys()):
-            sts_print(f"FAIL: Unknown command {cmd}.")
+            print(f"FAIL: Unknown command {cmd}.")
             return False
 
         command = f"{cmd.replace('_', '-')} -v"
         return run(command, verbose=True)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/lvm.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import fileinput
 import re
 from functools import wraps
 from pathlib import Path
+from typing import Dict, List, Union
 
 from sts import vdo
-from sts.utils import sts_print
 from sts.utils.cli_tools import Wrapper
 from sts.utils.cmdline import run, run_ret_out
 
 
-def check_lv_expected_value(test_obj, lv_name, vg_name, opt_val_dict):
+def check_lv_expected_value(test_obj, lv_name, vg_name, opt_val_dict):  # noqa: ANN001, ANN201
     if not test_obj or not opt_val_dict or not lv_name or not vg_name:
         return
 
     opt_str = ",".join(opt_val_dict)
     lv = lv_info(lv_name, vg_name, options=opt_str)
     if not lv:
         test_obj.tfail(f"{vg_name}/{lv_name} does not exist")
@@ -34,237 +34,237 @@
             run(f"lvs -a -o +{opt_str}")
             continue
 
 
 ###########################################
 # PV section
 ###########################################
-def pv_query(verbose=False):
+def pv_query(verbose=False):  # noqa: ANN001, ANN201
     """Query Physical Volumes and return a dictionary with PV information for each PV.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with PV info for each PV.
     """
     cmd = 'pvs --noheadings --separator ","'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print("INFO: there is no VGs")
+        print("INFO: there is no VGs")
         return None
     pvs = output.split("\n")
 
     # format of PV info: PV,VG,Fmt,Attr,PSize,PFree
     pv_info_regex = r"\s+(\S+),(\S+)?,(\S+),(.*),(.*),(.*)$"
 
     pv_dict = {}
     for pv in pvs:
         m = re.match(pv_info_regex, pv)
         if not m:
-            # sts_print("WARN: (%s) does not match vgdisplay output format" % vg)
+            # print("WARN: (%s) does not match vgdisplay output format" % vg)
             continue
         pv_info_dict = {
             "vg": m.group(2),
             "fmt": m.group(3),  # not sure what it is
             "attr": m.group(4),
             "psize": m.group(5),
             "pfree": m.group(6),
         }
         pv_dict[m.group(1)] = pv_info_dict
 
     return pv_dict
 
 
-def pv_create(pv_name: str, options="", verbose=True):
+def pv_create(pv_name: str, options="", verbose=True):  # noqa: ANN001, ANN201
     """Create a Volume Group.
     The arguments are:
     PV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not pv_name:
-        sts_print("FAIL: pv_create requires pv_name")
+        print("FAIL: pv_create requires pv_name")
         return False
     cmd = f"pvcreate {options} {pv_name}"
     if run(cmd, verbose=verbose).returncode != 0:
-        # sts_print ("FAIL: Could not create %s" % pv_name)
+        # print ("FAIL: Could not create %s" % pv_name)
         return False
     return True
 
 
-def pv_remove(pv_name: str, force=None, verbose=True):
+def pv_remove(pv_name: str, force=None, verbose=True):  # noqa: ANN001, ANN201
     """Delete a Volume Group.
     The arguments are:
     VG name
     force (boolean)
     verbose (boolean).
 
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not pv_name:
-        sts_print("FAIL: pv_remove requires pv_name")
+        print("FAIL: pv_remove requires pv_name")
         return False
 
     pv_dict = pv_query()
 
     pv_names = pv_name.split()
     for pv_name in pv_names:
         if pv_name not in list(pv_dict.keys()):
-            sts_print(f"INFO: pv_remove - {pv_name} does not exist. Skipping...")
+            print(f"INFO: pv_remove - {pv_name} does not exist. Skipping...")
             return True
 
         options = ""
         if force:
             options += "--force --force"
         cmd = f"pvremove {options} {pv_name}"
         retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
-            sts_print(f"FAIL: Could not delete {pv_name}")
+            print(f"FAIL: Could not delete {pv_name}")
             return False
     return True
 
 
 ###########################################
 # VG section
 ###########################################
 
 
-def vg_show():
+def vg_show():  # noqa: ANN201
     """Show information for Volume Groups
     The arguments are:
     None
     Returns:
     True
     or
     False.
     """
     cmd = "vgs -a"
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not show VGs")
+        print("FAIL: Could not show VGs")
         return False
     return True
 
 
-def vg_query(verbose=False):
+def vg_query(verbose=False):  # noqa: ANN001, ANN201
     """Query Volume Groups and return a dictonary with VG information for each VG.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with VG info for each VG.
     """
     cmd = 'vgs --noheadings --separator ","'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print("INFO: there is no VGs")
+        print("INFO: there is no VGs")
         return None
     vgs = output.split("\n")
 
     # format of VG info: name #PV #LV #SN Attr VSize VFree
     vg_info_regex = r"\s+(\S+),(\S+),(\S+),(.*),(.*),(.*),(.*)$"
 
     vg_dict = {}
     for vg in vgs:
         m = re.match(vg_info_regex, vg)
         if not m:
-            # sts_print("WARN: (%s) does not match vgdisplay output format" % vg)
+            # print("WARN: (%s) does not match vgdisplay output format" % vg)
             continue
         vg_info_dict = {
             "num_pvs": m.group(2),
             "num_lvs": m.group(3),
             "num_sn": m.group(4),  # not sure what it is
             "attr": m.group(5),
             "vsize": m.group(6),
             "vfree": m.group(7),
         }
         vg_dict[m.group(1)] = vg_info_dict
 
     return vg_dict
 
 
-def vg_create(vg_name: str, pv_name: str, force=False, verbose=True):
+def vg_create(vg_name: str, pv_name: str, force=False, verbose=True):  # noqa: ANN001, ANN201
     """Create a Volume Group.
     The arguments are:
     PV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name or not pv_name:
-        sts_print("FAIL: vg_create requires vg_name and pv_name")
+        print("FAIL: vg_create requires vg_name and pv_name")
         return False
 
     options = ""
     if force:
         options += "--force"
     cmd = f"vgcreate {options} {vg_name} {pv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        # sts_print ("FAIL: Could not create %s" % vg_name)
+        # print ("FAIL: Could not create %s" % vg_name)
         return False
     return True
 
 
-def vg_remove(vg_name: str, force=False, verbose=True):
+def vg_remove(vg_name: str, force=False, verbose=True):  # noqa: ANN001, ANN201
     """Delete a Volume Group.
     The arguments are:
     VG name
     force (boolean).
 
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name:
-        sts_print("FAIL: vg_remove requires vg_name")
+        print("FAIL: vg_remove requires vg_name")
         return False
 
     vg_dict = vg_query()
     if vg_name not in list(vg_dict.keys()):
-        sts_print(f"INFO: vg_remove - {vg_name} does not exist. Skipping...")
+        print(f"INFO: vg_remove - {vg_name} does not exist. Skipping...")
         return True
 
     options = ""
     if force:
         options += "--force"
     cmd = f"vgremove {options} {vg_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        # sts_print ("FAIL: Could not delete %s" % vg_name)
+        # print ("FAIL: Could not delete %s" % vg_name)
         return False
     return True
 
 
 ###########################################
 # LV section
 ###########################################
 
 
-def lv_show():
+def lv_show():  # noqa: ANN201
     """Show information for Logical Volumes
     The arguments are:
     None
     Returns:
     True
     or
     False.
     """
     cmd = "lvs -a"
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not show LVs")
+        print("FAIL: Could not show LVs")
         return False
     return True
 
 
-def lv_query(options="", verbose=False):
+def lv_query(options="", verbose=False):  # noqa: ANN001, ANN201
     """Query Logical Volumes and return a dictonary with LV information for each LV.
     The arguments are:
     options:  If not want to use default lvs output. Use -o for no default fields
     Returns:
     dict: Return a list with LV info for each LV.
     """
     # Use \",\" as separator, as some output might contain ','
@@ -302,248 +302,248 @@
             lv_info_regex += '","(.*)'
             param_names.append(param)
         lv_info_regex += "$"
         cmd += f" -o lv_name,vg_name,{options}"
 
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print("INFO: there is no LVs")
+        print("INFO: there is no LVs")
         return None
     lvs = output.split("\n")
 
     lv_list = []
     for lv in lvs:
         m = re.match(lv_info_regex, lv)
         if not m:
-            sts_print(f"FAIL: ({lv}) does not match lvs output format")
+            print(f"FAIL: ({lv}) does not match lvs output format")
             continue
         lv_info_dict = {}
         for index in range(len(param_names)):
             lv_info_dict[param_names[index]] = m.group(index + 1)
         lv_list.append(lv_info_dict)
 
     return lv_list
 
 
-def lv_create(vg_name: str, lv_name: str, options: list, verbose=True):
+def lv_create(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
     """Create a Logical Volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name or not lv_name:
-        sts_print("FAIL: lv_create requires vg_name and lv_name")
+        print("FAIL: lv_create requires vg_name and lv_name")
         return False
 
     cmd = f"lvcreate {' '.join(str(i) for i in options)} {vg_name} -n {lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        # sts_print ("FAIL: Could not create %s" % lv_name)
+        # print ("FAIL: Could not create %s" % lv_name)
         return False
     return True
 
 
-def lv_info(lv_name: str, vg_name: str, options="", verbose=False):
+def lv_info(lv_name: str, vg_name: str, options="", verbose=False):  # noqa: ANN001, ANN201
     """Show information of specific LV."""
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_info() - requires lv_name and vg_name as parameters")
+        print("FAIL: lv_info() - requires lv_name and vg_name as parameters")
         return None
 
     lvs = lv_query(options=options, verbose=verbose)
 
     if not lvs:
         return None
 
     for lv in lvs:
         if lv["name"] == lv_name and lv["vg_name"] == vg_name:
             return lv
     return None
 
 
-def lv_activate(lv_name: str, vg_name: str, verbose=True):
+def lv_activate(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
     """Activate a Logical Volume
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_activate requires lv_name and vg_name")
+        print("FAIL: lv_activate requires lv_name and vg_name")
         return False
 
     cmd = f"lvchange -ay {vg_name}/{lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not activate LV {lv_name}")
+        print(f"FAIL: Could not activate LV {lv_name}")
         return False
 
     # Maybe we should query the LVs and make sure it is really activated
     return True
 
 
-def lv_deactivate(lv_name: str, vg_name: str, verbose=True):
+def lv_deactivate(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
     """Deactivate a Logical Volume
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_deactivate requires lv_name and vg_name")
+        print("FAIL: lv_deactivate requires lv_name and vg_name")
         return False
 
     cmd = f"lvchange -an {vg_name}/{lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not deactivate LV {lv_name}")
+        print(f"FAIL: Could not deactivate LV {lv_name}")
         return False
 
     # Maybe we should query the LVs and make sure it is really deactivated
     return True
 
 
-def lv_remove(lv_name: str, vg_name: str, verbose=True):
+def lv_remove(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
     """Remove an LV from a VG
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_remove requires lv_name and vg_name")
+        print("FAIL: lv_remove requires lv_name and vg_name")
         return False
 
     lv_names = lv_name.split()
 
     for lv_name in lv_names:
         if not lv_info(lv_name, vg_name):
-            sts_print(f"INFO: lv_remove - LV {lv_name} does not exist. Skipping")
+            print(f"INFO: lv_remove - LV {lv_name} does not exist. Skipping")
             continue
 
         cmd = f"lvremove --force {vg_name}/{lv_name}"
         retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
-            sts_print(f"FAIL: Could not remove LV {lv_name}")
+            print(f"FAIL: Could not remove LV {lv_name}")
             return False
 
         if lv_info(lv_name, vg_name):
-            sts_print(f"INFO: lv_remove - LV {lv_name} still exists.")
+            print(f"INFO: lv_remove - LV {lv_name} still exists.")
             return False
 
     return True
 
 
-def lv_convert(vg_name: str, lv_name: str, options: list, verbose=True):
+def lv_convert(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
     """Change Logical Volume layout.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        sts_print("FAIL: lv_convert requires at least some options specified.")
+        print("FAIL: lv_convert requires at least some options specified.")
         return False
 
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_convert requires vg_name and lv_name")
+        print("FAIL: lv_convert requires vg_name and lv_name")
         return False
 
     cmd = f"lvconvert {' '.join(options)} {vg_name}/{lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not convert {lv_name}")
+        print(f"FAIL: Could not convert {lv_name}")
         return False
 
     return True
 
 
-def lv_extend(vg_name: str, lv_name: str, options: list, verbose=True):
+def lv_extend(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
     """Increase size of logical volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        sts_print("FAIL: lv_extend requires at least some options specified.")
+        print("FAIL: lv_extend requires at least some options specified.")
         return False
 
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_extend requires vg_name and lv_name")
+        print("FAIL: lv_extend requires vg_name and lv_name")
         return False
 
     cmd = f"lvextend {' '.join(options)} {vg_name}/{lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not extend {lv_name}")
+        print(f"FAIL: Could not extend {lv_name}")
         return False
 
     return True
 
 
-def lv_reduce(vg_name: str, lv_name: str, options: list, verbose=True):
+def lv_reduce(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
     """Decrease size of logical volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        sts_print("FAIL: lv_reduce requires at least some options specified.")
+        print("FAIL: lv_reduce requires at least some options specified.")
         return False
 
     if not lv_name or not vg_name:
-        sts_print("FAIL: lv_reduce requires vg_name and lv_name")
+        print("FAIL: lv_reduce requires vg_name and lv_name")
         return False
 
     cmd = f"lvreduce {' '.join(options)} {vg_name}/{lv_name}"
     retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
-        sts_print(f"FAIL: Could not reduce {lv_name}")
+        print(f"FAIL: Could not reduce {lv_name}")
         return False
 
     return True
 
 
 ###########################################
 # Config file
 ###########################################
 
 
-def get_config_file_path():
+def get_config_file_path():  # noqa: ANN201
     return "/etc/lvm/lvm.conf"
 
 
-def update_config(key: str, value: str):
+def update_config(key: str, value: str):  # noqa: ANN201
     config_file = get_config_file_path()
     search_regex = re.compile(r"(\s*)%s(\s*)=(\s*)\S*" % key)
     search_regex_with_comment = re.compile(r"(\s*#\s*)%s(\s*)=(\s*)\S*" % key)
     for line in fileinput.input(config_file, inplace=True):
         m = search_regex.match(line)
         m_with_comment = search_regex_with_comment.match(line)
         if m:
@@ -552,15 +552,15 @@
             line = f"{m_with_comment.group(1).replace('#', '')}{key} = {value}"  # noqa: PLW2901
         # print saves the line to the file
         # need to remove new line character as print will add it
         line = line.rstrip("\n")  # noqa: PLW2901
         print(line)
 
 
-def get_lvm_config_options(all_params=False):
+def get_lvm_config_options(all_params=False):  # noqa: ANN001, ANN201
     """Get all the configuration types from lvm.conf file."""
     out = run("lvmconfig --type full", capture_output=True, verbose=False).output
 
     options = {}
     category = ""
     for line in out.split("\n"):
         line = line.strip()  # noqa: PLW2901
@@ -580,75 +580,75 @@
 
     options_all = []
     for value in options.values():
         options_all.extend(value)
     return options_all
 
 
-def check_lvm_config(option):
+def check_lvm_config(option):  # noqa: ANN001, ANN201
     return run(f"lvs -o {option}", capture_output=True).output
 
 
-def get_all_lvm_config_options():
+def get_all_lvm_config_options():  # noqa: ANN201
     all_opts = check_lvm_config("asdf")  # needs just something that it doesn't know
     # we need to test_filter on lines that look like this
     # lvm_blahblah - explanation
     # and remove separators
 
     # at the end is '?' which should not be there therefore [:-1]
     return [i.split()[0] for i in all_opts if re.match(r".+-.+", i) and "--" not in i][:-1]
 
 
-def run_cmd(func):
+def run_cmd(func):  # noqa: ANN001, ANN201
     # TODO: Duplicate of run_command
     """Decorator for running commands
     kwargs need to be edited every time, so decorator is probably the best solution.
     """
 
     @wraps(func)
-    def wrapped(*args, **kwargs):
+    def wrapped(*args, **kwargs):  # noqa: ANN002, ANN003, ANN202
         return run_ret_out(func(), *args, **kwargs, return_output=True)  # cmd == func()
 
     return wrapped
 
 
 @run_cmd
-def get_all_lvmvdoconfig_options():
+def get_all_lvmvdoconfig_options():  # noqa: ANN201
     return "lvmconfig --type list"
 
 
 @run_cmd
-def lvdisplay():
+def lvdisplay():  # noqa: ANN201
     return "lvdisplay"
 
 
-def print_profile_file(profile_name, path=None):
+def print_profile_file(profile_name, path=None):  # noqa: ANN001, ANN201
     if not path:
         path = "/etc/lvm/profile"  # default profile location
     run(f"cat {path}/{profile_name}.profile")
 
 
-def get_lvdisplay_data():
+def get_lvdisplay_data():  # noqa: ANN201
     _, out = lvdisplay()
     try:
         lines = [line for line in out if "LV Name" in line and "pool" not in line][0].split()
     except Exception as exc:
         lines = [""]
         print("Exception", exc)
     print(lines)
     return lines[-1]
 
 
-def run_command(func):
+def run_command(func):  # noqa: ANN001, ANN201
     """Decorator for running commands
     kwargs need to be edited every time, so decorator is probably the best solution.
     """
 
     @wraps(func)
-    def wrapped(inst, **kwargs):
+    def wrapped(inst, **kwargs):  # noqa: ANN001, ANN003, ANN202
         inst.tmp_kwargs = kwargs
         # The first thing is to replace values that are
         # conf=fmf_conf_value -> conf=conf_value
         kwargs = inst.replace_multiple_option_values(**kwargs)
         # check configuration arguments from old conf to new
         # slab_size=minimum -> slab_size=compute(value)
         kwargs = inst.check_config_arguments(**kwargs)
@@ -669,19 +669,19 @@
 
     return wrapped
 
 
 class LVM(Wrapper):
     """Class for creating LVMVDO commands."""
 
-    def __init__(self, disable_check=True, vdo_arguments_flag=True):
+    def __init__(self, disable_check=True, vdo_arguments_flag=True) -> None:  # noqa: ANN001
         self.disable_check = disable_check
-        self.tmp_kwargs = {}
+        self.tmp_kwargs: dict = {}
 
-        self.commands = {
+        self.commands: Dict[str, Union[str, List[str]]] = {
             "lvcreate": "lvcreate",
             "lvremove": "lvremove",
             "lvconvert": "lvconvert",
             "lvchange": "lvchange",
             "lvextend": "lvextend",
             "lvreduce": "lvreduce",
             "lvresize": "lvresize",
@@ -785,19 +785,19 @@
         # backward compatibility between vdo and lvmvdo packages,
         # so that commands correspond to each other
         self.create = self.lvcreate
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
-    def remove_nones(kwargs):
+    def remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @staticmethod
-    def _add_value(value, command, argument):
+    def _add_value(value, command, argument):  # noqa: ANN001, ANN205
         """Copied from Wrapper."""
         if argument[-1:] in ["=", "&"]:
             if argument[-1:] == "&":
                 argument = argument[:-1] + " "
             if isinstance(value, list):
                 # allows to use repeatable arguments as a list of values
                 for val in value:
@@ -806,21 +806,21 @@
                 command += argument + "'" + str(value) + "'"
         elif argument[-1:] in "*":
             command += str(value)
         else:
             command += argument
         return command + " "  # added space at the end to fix formatting
 
-    def _add_argument(self, arg, value, command):
+    def _add_argument(self, arg, value, command):  # noqa: ANN001, ANN202
         """Copied from Wrapper."""
         # Checks if given argument is allowed for given command and adds it to cmd string
         self._check_allowed_argument(arg, command)
         return self._add_value(value, command, self._get_arg(arg))
 
-    def _add_arguments(self, cmd, **kwargs):
+    def _add_arguments(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         """Copied from Wrapper."""
         command = cmd
         for kwarg in kwargs:
             # skip adding this argument if the value is False
             if kwargs[kwarg] is False:
                 continue
             # skip:
@@ -831,55 +831,55 @@
             command = self._add_argument(kwarg, kwargs[kwarg], command)
 
         # vg_name must be the last in command
         if "vg_name" in kwargs:
             command += kwargs["vg_name"]
         return command
 
-    def _get_possible_arguments(self, command=None):
+    def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
         return super()._get_possible_arguments(command.split()[0])
 
-    def run(self, cmd, verbosity=True, **kwargs):
+    def run(self, cmd, verbosity=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         """Constructs the command to run and runs it."""
         cmd = self._add_arguments(cmd, **kwargs)
 
         print(cmd)
         ret = run(cmd, verbose=verbosity).returncode
 
         if isinstance(ret, tuple) and ret[0] != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+            print(f"WARN: Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
-    def number_of_conf_args(self, **kwargs):
+    def number_of_conf_args(self, **kwargs):  # noqa: ANN003, ANN201
         """Counts the number of configuration arguments in kwargs and returns it."""
         return sum(conf_arg in kwargs for conf_arg in self.config_arguments)
 
-    def _set_kwargs_value(self, arg, **kwargs):
+    def _set_kwargs_value(self, arg, **kwargs):  # noqa: ANN001, ANN003, ANN202
         """If the value in test declaration is 'enabled'
         it switches it to the one in the man page, e.g. 'y'
         self.argument_options['activate'].
         """
         fmf_options = self.argument_options[arg][0]
         opt_values = self.argument_options[arg][1]
 
         print(fmf_options)
         for idx, value in enumerate(fmf_options):
             kwargs[arg] = opt_values[idx] if kwargs[arg] == value else kwargs[arg]
 
         return kwargs
 
-    def get_option(self, argument):
+    def get_option(self, argument):  # noqa: ANN001, ANN201
         """Get an option to set up in a configuration file."""
         if argument in self.option_translator_dictionary:
             return self.option_translator_dictionary[argument]
         return argument  # maybe this should be None, so it is obvious that there is an error
 
-    def minimum_slab_size(self, device_name, default_to_2g=True):  # reused from vdo.py
+    def minimum_slab_size(self, device_name, default_to_2g=True):  # reused from vdo.py  # noqa: ANN001, ANN201
         """Computing minimum slab size, used from vdo.py."""
 
         class VDODeviceNotFoundError(Exception):
             pass
 
         print(device_name)
         ret, device_size = run_ret_out(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
@@ -894,15 +894,15 @@
         device_size = (float(size[:-1]) * (1024 ** multipliers.index(size[-1:]))).__int__()
         max_number_of_slabs = 8192
         minimum_size = max(2 ** int(device_size / max_number_of_slabs).bit_length(), 128)  # reused from vdo.py
         if default_to_2g and minimum_size < 2048:
             return "2G"
         return f"{minimum_size!s}M"
 
-    def check_conf_value(self, val):
+    def check_conf_value(self, val):  # noqa: ANN001, ANN201
         """Remove units K, G, T and convert accordingly."""
         if "fail" in self.tmp_kwargs["name"]:
             return val  # don't check
 
         units = {
             "K": 0.001,  # 1/1024 = 0.00097656,
             "k": 0.001,
@@ -928,24 +928,24 @@
                 multiplier = units[match.group(2)]
             except KeyError:  # because of "512B"
                 print("Argument value: ", match.group(2), ".")
                 print(f"Original {val}; will return {val[:-1]}")
                 return val[:-1]
         return str(int(match.group(1)) * multiplier)
 
-    def check_config_arguments(self, **kwargs):
+    def check_config_arguments(self, **kwargs):  # noqa: ANN003, ANN201
         """Check arguments in config."""
         if "slab_size" in kwargs:
             device_name = kwargs["device"].split("/")[-1]
             # Slab_size value should be in MB
             kwargs["slab_size"] = self.check_conf_value(self.minimum_slab_size(device_name))
 
         return kwargs
 
-    def create_profile_file(self, profile_name, args_to_remove, **kwargs):
+    def create_profile_file(self, profile_name, args_to_remove, **kwargs):  # noqa: ANN001, ANN003, ANN201
         """Example: category {
             arg1 = value,
             arg2 = value
         }.
         """
         run(f"rm /etc/lvm/profile/{profile_name}.profile")
 
@@ -970,64 +970,64 @@
                     for opt in value:
                         str_to_write += f"\t{opt}\n"
                 str_to_write += "}\n"
             fp.write(str_to_write)  # in 'with' section there is no need for fp.close()
 
         return args_to_remove
 
-    def replace_multiple_option_values(self, **kwargs):
+    def replace_multiple_option_values(self, **kwargs):  # noqa: ANN003, ANN201
         """Check and replace what is defined in .fmf test file with corresponding value from man page
         e.g. 'enabled' -> 'y'.
         """
         for arg in self.multiple_option_arguments:
             if arg in kwargs:
                 kwargs = self._set_kwargs_value(arg, **kwargs)
         # kwargs = {self._set_kwargs_value(i, **kwargs) for i in self.multiple_option_arguments if i in kwargs}
         return kwargs
 
-    def remove_vdo_arguments(self, **kwargs):
+    def remove_vdo_arguments(self, **kwargs):  # noqa: ANN003, ANN201
         """The rest of VDO arguments need to be removed otherwise unsupported arguments
         will propagate into the command.
         """
         arg_to_remove = [arg for arg in kwargs if arg in self.vdo_arguments]
         for arg in arg_to_remove:
             kwargs.pop(arg)
         return kwargs
 
-    def get_category(self, argument):
+    def get_category(self, argument):  # noqa: ANN001, ANN201
         """Get the list that contains the argument I am looking for.
 
         # not working for "check" (there are multiple) :( not fixed :/
         """
         for one_list in list(self.config_options.values()):
             if argument in one_list or self.option_translator_dictionary[argument] in one_list:
                 arguments_of_category = one_list
                 break  # find the first one
 
         # using the list containing the argument as item of the list
         index = list(self.config_options.values()).index(arguments_of_category)
         return list(self.config_options.keys())[index]
 
-    def check(self, **kwargs):
+    def check(self, **kwargs):  # noqa: ANN003, ANN201
         """Check arguments compatibility with command."""
         if "name" in kwargs:
             kwargs.pop("name")  # remove name, because it is not used in lvmvdo
 
         if "size" in kwargs:
             # value format for size parameter
             return bool(re.match(r"^([\+|\-]|)[0-9]+[T|G|M|K]$", kwargs["size"]))
         return True
 
     @staticmethod
-    def remove_args(to_remove, **kwargs):
+    def remove_args(to_remove, **kwargs):  # noqa: ANN001, ANN003, ANN205
         """Return only what is intended."""
         return {k: v for k, v in kwargs.items() if k not in to_remove}
 
     @run_command
-    def lvcreate(self, **kwargs):
+    def lvcreate(self, **kwargs):  # noqa: ANN003, ANN201
         print("LVCREATE", kwargs)
         cmd = "lvcreate --vdo "
 
         # config part START
         args_to_remove = []
         use_conf_file = False
 
@@ -1061,36 +1061,36 @@
         # config part END
 
         kwargs["yes"] = "-y"  # see lvremove
 
         return cmd, kwargs
 
     @run_command
-    def lvremove(self, **kwargs):
+    def lvremove(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "lvremove "
 
         # lvmvdo uses human interface for some activities like removing vdo pools
         # in automation we don't want this, so we add '-y' to force it
         kwargs["yes"] = "-y"
         return cmd, kwargs
 
     @run_command
-    def lvconvert(self, **kwargs):
+    def lvconvert(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "lvconvert --vdo "
         return cmd, kwargs
 
     @run_command
-    def lvchange(self, **kwargs):
+    def lvchange(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "lvchange "
         if "vdo_name" in kwargs:
             kwargs.pop("vdo_name")
         return cmd, kwargs
 
     @run_command
-    def lvextend(self, **kwargs):
+    def lvextend(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "lvextend "
         return cmd, kwargs
 
     @run_command
-    def lvmconfig(self, **kwargs):
+    def lvmconfig(self, **kwargs):  # noqa: ANN003, ANN201
         cmd = "lvmconfig "
         return cmd, kwargs
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/md.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/md.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,80 +2,79 @@
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 from pathlib import Path
 
-from sts.utils import sts_print
 from sts.utils.cmdline import exists, run_ret_out
 
 
-def _mdadm_query(md_device, verbose=False):
+def _mdadm_query(md_device, verbose=False):  # noqa: ANN001, ANN202
     if not exists("mdadm"):
         if verbose:
-            sts_print("INFO: mdadm is not installed")
+            print("INFO: mdadm is not installed")
         return None
 
     cmd = f"mdadm -D /dev/{md_device}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print(f"FAIL: couldn't query {md_device}")
+        print(f"FAIL: couldn't query {md_device}")
         if verbose:
             print(output)
         return None
     return output
 
 
-def md_query(verbose=False):
+def md_query(verbose=False):  # noqa: ANN001, ANN201
     """Query Soft RAID devices.
     The arguments are:
     verbose: Print additional information. Default: False
     Returns:
     dict: Return a list of md devices.
     """
     mdstat_file = "/proc/mdstat"
 
     if not Path(mdstat_file).exists():
         if verbose:
-            sts_print("INFO: there is no MD device")
+            print("INFO: there is no MD device")
         return False
 
     cmd = f"cat {mdstat_file}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         if verbose:
-            sts_print("INFO: there is no MD device")
+            print("INFO: there is no MD device")
         return None
 
     md_name_regex = r"^(md\d+) :"
     md_devices = []
     for line in output.split("\n"):
         m = re.match(md_name_regex, line)
         if not m:
             continue
         md_devices.append(m.group(1))
 
     return md_devices
 
 
-def md_get_info(md_device, verbose=False):
+def md_get_info(md_device, verbose=False):  # noqa: ANN001, ANN201
     """Query information of an MD device.
     The arguments are:
     md_device: md device name to get information about
     verbose: Print additional information. Default: False
     Returns:
     dict: Return a dictionary with details about the md device.
     """
     if not md_device:
         return None
 
     if md_device not in md_query():
         if verbose:
-            sts_print(f"INFO: {md_device} is not a MD device")
+            print(f"INFO: {md_device} is not a MD device")
         return None
 
     output = _mdadm_query(md_device, verbose)
     if not output:
         return None
 
     md_info = {}
@@ -109,15 +108,15 @@
             "state": storage_match.group(5).strip(),
         }
         md_info["storage_devices"][storage_match.group(6)] = storage_info
 
     return md_info
 
 
-def md_get_storage_dev(md_device, verbose=False):
+def md_get_storage_dev(md_device, verbose=False):  # noqa: ANN001, ANN201
     """Get the storage devices of an MD device.
     The arguments are:
     md_device: md device name to get information about
     verbose: Print additional information. Default: False
     Returns:
     list: Return a list of storage devices.
     """
@@ -129,55 +128,55 @@
         return None
 
     if "storage_devices" not in md_info:
         return None
     return md_info["storage_devices"].keys()
 
 
-def md_stop(md_device, verbose=False):
+def md_stop(md_device, verbose=False):  # noqa: ANN001, ANN201
     """Stop a specific md device.
     The arguments are:
     md_device: md device name to get information about
     verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     cmd = f"mdadm --stop /dev/{md_device}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print(f"FAIL: couldn't stop {md_device}")
+        print(f"FAIL: couldn't stop {md_device}")
         if verbose:
             print(output)
         return False
     return True
 
 
-def md_clean(device, verbose=False):
+def md_clean(device, verbose=False):  # noqa: ANN001, ANN201
     """Clean a specific storage device.
     The arguments are:
     device: storage device like /dev/sda
     verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     cmd = f"mdadm --zero-superblock {device}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
-        sts_print(f"FAIL: couldn't clean {device}")
+        print(f"FAIL: couldn't clean {device}")
         if verbose:
             print(output)
         return False
     return True
 
 
-def md_remove(md_device, clean=False, verbose=False):
+def md_remove(md_device, clean=False, verbose=False):  # noqa: ANN001, ANN201
     """Remove a specific md device.
     The arguments are:
     md_device: md device name to get information about
     verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
@@ -192,15 +191,15 @@
     retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if (
         retcode != 0
         and
         # error opening the device can be ignored
         f"mdadm: error opening /dev/{md_device}: No such file or directory" not in output
     ):
-        sts_print(f"FAIL: couldn't remove {md_device}")
+        print(f"FAIL: couldn't remove {md_device}")
         if verbose:
             print(output)
         return False
     if clean and sto_devices:
         for device in sto_devices:
             if not md_clean(device, verbose):
                 return False
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/mp.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/mp.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 from pathlib import Path
 from typing import Literal
 
 from sts import fc, iscsi, linux, lvm, net, scsi
-from sts.utils import sts_print
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.size import size_human_2_size_bytes
 
 MULTIPATH_CONF_PATH = "/etc/multipath.conf"
 aug_conf_path = "/files/etc/multipath.conf"
 package_name = "device-mapper-multipath"
 
 
-def mp_service_name():
+def mp_service_name():  # noqa: ANN201
     """Return the name of multipath service."""
     return "multipathd"
 
 
-def mp_start_service():
+def mp_start_service():  # noqa: ANN201
     """Start multipath service."""
     if linux.is_installed(package_name) and not Path(MULTIPATH_CONF_PATH).is_file():
         mpathconf_enable()
     return linux.service_start(mp_service_name())
 
 
-def mp_stop_service():
+def mp_stop_service():  # noqa: ANN201
     """Stop multipath service."""
     return linux.service_stop(mp_service_name())
 
 
-def is_multipathd_running():
+def is_multipathd_running():  # noqa: ANN201
     """Check if multipathd is running."""
     return linux.is_service_running(mp_service_name())
 
 
 def mpathconf_enable(find_mpaths: Literal["yes", "no", "strict", "greedy", "smart", None] = None) -> bool:
     """Runs 'mpathconf --enable' command."""
     cmd = "mpathconf --enable"
@@ -57,100 +56,100 @@
         mpathconf_enable()
         if not linux.service_start(mp_service_name()):
             return False
 
     return True
 
 
-def is_mpath_device(mpath_name, print_fail=True):
+def is_mpath_device(mpath_name, print_fail=True):  # noqa: ANN001, ANN201
     """Checks if given device is multipath.
 
     Args:
       mpath_name: name of device to check
       print_fail: Should we print "FAIL: ..." in case of fail?
 
     Returns:
       True / False.
     """
     cmd = f"multipath -l {mpath_name}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         if print_fail:
-            sts_print(f'FAIL: Could not execute "{cmd}"')
+            print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     # There could be error in the output, so we need to check if we really found the mpath device.
     # 'multipath -l device_name' always should return device_name at the beginning if found
     if output and len(output) > 0 and output.startswith(f"{mpath_name} "):
         return True
     return False
 
 
-def get_mpath_of_disk(disk):
+def get_mpath_of_disk(disk):  # noqa: ANN001, ANN201
     """Get the multipath device of a disk
     The arguments are:
     Disk:   Disk
     Returns:
     String: Return the name of multipath device.
     """
     if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
         device = f"/dev/{disk}"
         mmnum_cmd = 'ls -l %s | awk \'{print "("$5,$6")"}\'' % device
         retcode, output = run_ret_out(mmnum_cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print(f"FAIL: Could not get device information for {device}")
+            print(f"FAIL: Could not get device information for {device}")
             print(output)
             return None
         deps_cmd = rf"dmsetup deps | grep \"{output}\" | awk -v device={device} '{{print $1}}' | tr -d \"\:\""
         retcode, output = run_ret_out(deps_cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print(f"FAIL: Could not get dmsetup information for {device}")
+            print(f"FAIL: Could not get dmsetup information for {device}")
             print(output)
             return None
         mpath = output
     else:
         # BZ891921 - Multipath provides the mpath device of given scsi block device
         cmd = "pidof multipathd"
         retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print("FAIL: For some reason multipathd is not running")
+            print("FAIL: For some reason multipathd is not running")
             print(output)
             return None
         fmt = '"%d %m"'
         cmd = f"multipathd show paths format {fmt} | egrep \"^{disk}\" | awk '{{print$2}}'"
         retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
-            sts_print(f"FAIL: to find multipath of disk {disk}")
+            print(f"FAIL: to find multipath of disk {disk}")
             print(output)
             return None
         mpath = output
 
     if not mpath:
-        sts_print(f"WARN: Could not find multipath for {disk}")
+        print(f"WARN: Could not find multipath for {disk}")
         return None
     return mpath
 
 
-def get_disks_of_mpath(mpath_name):
+def get_disks_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return all SCSI devices that belong to this mpath."""
     if not mpath_name:
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
         return None
 
     if "disk" not in list(mpath_dict.keys()):
-        sts_print(f"WARN: mpath {mpath_name} has no disk")
+        print(f"WARN: mpath {mpath_name} has no disk")
         return None
 
     return list(mpath_dict["disk"].keys())
 
 
-def get_disks_of_mpath_by_wwpn(mpath_name, wwpn):
+def get_disks_of_mpath_by_wwpn(mpath_name, wwpn):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this WWPN.
     """
     if not mpath_name or not wwpn:
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
@@ -165,15 +164,15 @@
             for port_entry in port_entries:
                 if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
                     if mpath_dict["disk"][disk][port_entry] and wwpn in mpath_dict["disk"][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
-def get_disks_of_mpath_by_iqn(mpath_name, iqn):
+def get_disks_of_mpath_by_iqn(mpath_name, iqn):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this IQN.
     """
     if not mpath_name or not iqn:
         return None
 
     if not iscsi.is_iqn(iqn):
@@ -190,15 +189,15 @@
             for port_entry in port_entries:
                 if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
                     if mpath_dict["disk"][disk][port_entry] and iqn in mpath_dict["disk"][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
-def get_disks_of_mpath_by_mac(mpath_name, mac):
+def get_disks_of_mpath_by_mac(mpath_name, mac):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this MAC.
     """
     if not mpath_name or not mac:
         return None
 
     if not net.is_mac(mac):
@@ -215,15 +214,15 @@
             for port_entry in port_entries:
                 if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
                     if mpath_dict["disk"][disk][port_entry] and mac in mpath_dict["disk"][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
-def multipath_query_all(mpath_name=None):
+def multipath_query_all(mpath_name=None):  # noqa: ANN001, ANN201
     # Not sure with of these 2 commands I should use
     # multipath -ll
     # will force multipath to issue its own (synchronous) path checker call,
     # and report that result.
     # multipathd show top
     # multipath will not run a checker on the paths. It will simply report the
     # current state. This means that you get the results from the last time
@@ -233,19 +232,19 @@
     # port down.
     cmd = "multipath -ll"
     if mpath_name:
         cmd += f" {mpath_name}"
     # cmd = "multipathd -k\"show top\""
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f'FAIL: Could not execute "{cmd}"')
+        print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     if not output:
-        # sts_print("FAIL: Got no output from \"%s\"" % cmd)
+        # print("FAIL: Got no output from \"%s\"" % cmd)
         return None
 
     regex_mpath = r"^(?:create\:\ ){0,1}"  # might have when creating mpath
     regex_mpath += r"(?:reload\:\ ){0,1}"  # might have when creating mpath
     regex_mpath += r"([^ ]+?)\ +"  # 1. mpath_name
     regex_mpath += r"(?:\((\S+)\)\ +){0,1}"  # 2. wwid if different from #1
     regex_mpath += r"(?:(dm\-[0-9]+)\ +){0,1}"  # 3. dm_name if known
@@ -327,15 +326,15 @@
             mpath_dict["iface_macs"] = []
             mpath_dict["iface_names"] = []
             mpath_dict["target_ips"] = []
             mpath_dict["persist_ips"] = []
             mpath_dict["transport_types"] = []
             mpath_dict["scsi_drivers"] = []
             mpath_dict["host_ids"] = []
-            # sts_print("\n\nDEBUG - Feature - query all mpath [%s]" % line)
+            # print("\n\nDEBUG - Feature - query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         m = re.match(regex_pg, line)
         if m:
             if not wwid or not mpath_dict:
@@ -346,15 +345,15 @@
             mpath_dict["path_group"][pg_id]["mpath_name"] = _mpath_name
             mpath_dict["path_group"][pg_id]["wwid"] = wwid
             mpath_dict["path_group"][pg_id]["pg_id"] = pg_id
             mpath_dict["path_group"][pg_id]["policy"] = m.group(1)
             mpath_dict["path_group"][pg_id]["prio"] = m.group(2)
             mpath_dict["path_group"][pg_id]["status"] = m.group(3)
             mpath_dict["path_group"][pg_id]["disk"] = {}
-            # sts_print("\n\nDEBUG - PG : query all mpath [%s]" % line)
+            # print("\n\nDEBUG - PG : query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         m = re.match(regex_disk, line)
         if m:
             if not wwid or not mpath_dict or not pg_id:
@@ -480,15 +479,15 @@
 
             if persist_ip and persist_ip not in mpath_dict["persist_ips"]:
                 mpath_dict["persist_ips"].append(persist_ip)
 
             mpath_dict["disk"][disk_info_dict["scsi_disk"]] = disk_info_dict
             mpath_dict["path_group"][pg_id]["disk"][scsi_id] = disk_info_dict
             all_mpath_dict["by_scsi_id"][scsi_id] = disk_info_dict
-            # sts_print("\n\nDEBUG - Disk: query all mpath [%s]" % line)
+            # print("\n\nDEBUG - Disk: query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         # as regex_mpath is an aggressive regex, we leave it at the last
         # one to check.
         m = re.match(regex_mpath, line)
@@ -531,156 +530,156 @@
                 "disk": {},
                 "path_group": {},
                 "transport_types": [],
             }
 
             all_mpath_dict["by_wwid"][wwid] = mpath_dict
             all_mpath_dict["by_mpath_name"][_mpath_name] = mpath_dict
-            # sts_print("\n\nDEBUG: query all mpath [%s]" % line)
+            # print("\n\nDEBUG: query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
             continue
     if mpath_name:
         if mpath_name in list(all_mpath_dict["by_mpath_name"].keys()):
             return all_mpath_dict["by_mpath_name"][mpath_name]
         return None
 
     return all_mpath_dict
 
 
-def mpath_name_of_wwid(wwid):
+def mpath_name_of_wwid(wwid):  # noqa: ANN001, ANN201
     if not wwid:
-        sts_print("FAIL: mpath_name_of_wwid() - requires wwid parameter")
+        print("FAIL: mpath_name_of_wwid() - requires wwid parameter")
         return None
 
     mp_devs = multipath_query_all()
     if not mp_devs:
         return None
 
     if wwid in list(mp_devs["by_wwid"].keys()):
         return mp_devs["by_wwid"][wwid]["mpath_name"]
 
     return None
 
 
-def mpath_names_of_vendor(vendor):
+def mpath_names_of_vendor(vendor):  # noqa: ANN001, ANN201
     """Given a Vendor return a list with all multipath device names with this vendor."""
     if not vendor:
-        sts_print("FAIL: mpath_names_of_vendor() - requires vendor parameter")
+        print("FAIL: mpath_names_of_vendor() - requires vendor parameter")
         return None
 
     mp_devs = multipath_query_all()
     if not mp_devs:
         return None
 
     mpaths = []
     for mpath_info in list(mp_devs["by_mpath_name"].values()):
         if "vendor" in list(mpath_info.keys()) and mpath_info["vendor"] == vendor:
             mpaths.append(mpath_info["mpath_name"])
 
     return mpaths
 
 
-def mpath_check_disk_status(mpath_name, scsi_disk):
+def mpath_check_disk_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the online status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        sts_print("FAIL: mpath_check_disk_status() - requires mpath_name and scsi_disk parameters")
+        print("FAIL: mpath_check_disk_status() - requires mpath_name and scsi_disk parameters")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: mpath_check_disk_status() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_status() - Could not get mpath info for {mpath_name}")
         return None
 
     if "disk" not in list(mpath_dict.keys()):
-        sts_print(f"FAIL: mpath_check_disk_status() - Could not find any SCSI disk for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_status() - Could not find any SCSI disk for {mpath_name}")
         return None
 
     for disk in list(mpath_dict["disk"].keys()):
         if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
             return mpath_dict["disk"][disk]["online_status"]
 
     return None
 
 
-def mpath_check_disk_dm_status(mpath_name, scsi_disk):
+def mpath_check_disk_dm_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the dm status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        sts_print("FAIL: mpath_check_disk_dm_status() - requires mpath_name and scsi_disk parameters")
+        print("FAIL: mpath_check_disk_dm_status() - requires mpath_name and scsi_disk parameters")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: mpath_check_disk_dm_status() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_dm_status() - Could not get mpath info for {mpath_name}")
         return None
 
     if "disk" not in list(mpath_dict.keys()):
-        sts_print(f"FAIL: mpath_check_disk_dm_status() - Could not find any SCSI disk for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_dm_status() - Could not find any SCSI disk for {mpath_name}")
         return None
 
     for disk in list(mpath_dict["disk"].keys()):
         if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
             return mpath_dict["disk"][disk]["dm_status"]
 
     return None
 
 
-def mpath_check_disk_path_status(mpath_name, scsi_disk):
+def mpath_check_disk_path_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the path status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        sts_print("FAIL: mpath_check_disk_path_status() - requires mpath_name and scsi_disk parameters")
+        print("FAIL: mpath_check_disk_path_status() - requires mpath_name and scsi_disk parameters")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: mpath_check_disk_path_status() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_path_status() - Could not get mpath info for {mpath_name}")
         return None
 
     if "disk" not in list(mpath_dict.keys()):
-        sts_print(f"FAIL: mpath_check_disk_path_status() - Could not find any SCSI disk for {mpath_name}")
+        print(f"FAIL: mpath_check_disk_path_status() - Could not find any SCSI disk for {mpath_name}")
         return None
 
     for disk in list(mpath_dict["disk"].keys()):
         if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
             return mpath_dict["disk"][disk]["path_status"]
 
     return None
 
 
-def mpath_get_active_disk(mpath_name):
+def mpath_get_active_disk(mpath_name):  # noqa: ANN001, ANN201
     """From specific mpath device get which disk is the active one
     Return
     List of active SCSI disks.
     """
     if not mpath_name:
-        sts_print("FAIL: mpath_get_active_disk() - requires mpath_name parameter")
+        print("FAIL: mpath_get_active_disk() - requires mpath_name parameter")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: mpath_get_active_disk() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: mpath_get_active_disk() - Could not get mpath info for {mpath_name}")
         return None
 
     if "disk" not in list(mpath_dict.keys()):
-        sts_print(f"FAIL: mpath_get_active_disk() - Could not find any SCSI disk for {mpath_name}")
+        print(f"FAIL: mpath_get_active_disk() - Could not find any SCSI disk for {mpath_name}")
         return None
 
     active_disks = []
     for disk in list(mpath_dict["disk"].keys()):
         pg = mpath_dict["disk"][disk]["pg_id"]
         if mpath_dict["path_group"][pg]["status"] == "active":
             active_disks.append(disk)
 
     if active_disks:
         return active_disks
 
-    sts_print(f"FAIL: mpath_get_active_disk() - Could not find any active disk for {mpath_name}")
+    print(f"FAIL: mpath_get_active_disk() - Could not find any active disk for {mpath_name}")
     return None
 
 
-def get_free_mpaths(exclude_boot_device=True, exclude_lvm_device=True):
+def get_free_mpaths(exclude_boot_device=True, exclude_lvm_device=True):  # noqa: ANN001, ANN201
     """Return a dict of free mpath devices."""
     all_mp_info = multipath_query_all()
     if not all_mp_info:
         # could not query multipath devices
         return None
 
     if "by_wwid" not in list(all_mp_info.keys()):
@@ -698,105 +697,105 @@
 
     chosen_mpaths = {}
 
     for mp_wwid in list(all_mp_info["by_wwid"].keys()):
         mp_info = all_mp_info["by_wwid"][mp_wwid]
         # Skip if mpath device is used for boot
         if boot_wwid == mp_info["wwid"] and exclude_boot_device:
-            sts_print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for boot")
+            print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for boot")
             continue
 
         # Skip if it is used by LVM
         if pvs and exclude_lvm_device:
             mp_used_by_lvm = False
             for pv in list(pvs.keys()):
                 if mpath_device_2_mpath_name(pv) == mp_info["mpath_name"]:
                     mp_used_by_lvm = True
-                    sts_print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for LVM")
+                    print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for LVM")
                     continue
             if mp_used_by_lvm:
                 continue
 
         chosen_mpaths[mp_info["mpath_name"]] = mp_info
 
     return chosen_mpaths
 
 
-def h_wwpns_of_mpath(mpath_name):
+def h_wwpns_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the h_wwpns of specific mpath device."""
     if not mpath_name:
-        sts_print("FAIL: h_wwpns_of_mpath() - requires mpath_name parameter")
+        print("FAIL: h_wwpns_of_mpath() - requires mpath_name parameter")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: h_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: h_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
         return None
 
     if "h_wwpns" in mpath_dict:
         return mpath_dict["h_wwpns"]
     return None
 
 
-def t_wwpns_of_mpath(mpath_name):
+def t_wwpns_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the h_wwpns of specific mpath device."""
     if not mpath_name:
-        sts_print("FAIL: t_wwpns_of_mpath() - requires mpath_name parameter")
+        print("FAIL: t_wwpns_of_mpath() - requires mpath_name parameter")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: t_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: t_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
         return None
 
     if "t_wwpns" in mpath_dict:
         return mpath_dict["t_wwpns"]
     return None
 
 
-def iface_macs_of_mpath(mpath_name):
+def iface_macs_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the iface_macs_of_mpath of specific mpath device."""
     if not mpath_name:
-        sts_print("FAIL: iface_macs_of_mpath() - requires mpath_name parameter")
+        print("FAIL: iface_macs_of_mpath() - requires mpath_name parameter")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: iface_macs_of_mpath() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: iface_macs_of_mpath() - Could not get mpath info for {mpath_name}")
         return None
 
     if "iface_macs" in mpath_dict:
         return mpath_dict["iface_macs"]
     return None
 
 
-def transport_types_of_mpath(mpath_name):
+def transport_types_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the transport_types of specific mpath device."""
     if not mpath_name:
-        sts_print("FAIL: transport_types_of_mpath() - requires mpath_name parameter")
+        print("FAIL: transport_types_of_mpath() - requires mpath_name parameter")
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        sts_print(f"FAIL: transport_types_of_mpath() - Could not get mpath info for {mpath_name}")
+        print(f"FAIL: transport_types_of_mpath() - Could not get mpath info for {mpath_name}")
         return None
 
     if "transport_types" in mpath_dict:
         return mpath_dict["transport_types"]
     return None
 
 
-def multipath_show(mpath_name=None):
+def multipath_show(mpath_name=None):  # noqa: ANN001, ANN201
     cmd = "multipath -ll"
     if mpath_name:
         cmd += f" {mpath_name}"
     run(cmd)
 
 
-def multipath_reload(mpath_name=None):
+def multipath_reload(mpath_name=None):  # noqa: ANN001, ANN201
     """Usage
     multipath_reload()
     Purpose
         Execute 'multipath -r'
     Parameter
         N/A
     Returns
@@ -811,35 +810,35 @@
         cmd += f" {mpath_name}"
     if run(cmd).returncode != 0:
         return False
 
     return True
 
 
-def remove_mpath(mpath_name):
+def remove_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Remove specific mpath."""
     if not mpath_name:
-        sts_print("FAIL: remove_mpath() - requires mpath_name parameter")
+        print("FAIL: remove_mpath() - requires mpath_name parameter")
         return False
     if run(f"multipath -f {mpath_name}").returncode != 0:
-        sts_print(f"FAIL: Could not remove mpath {mpath_name}")
+        print(f"FAIL: Could not remove mpath {mpath_name}")
         return False
     return True
 
 
-def flush_all():
+def flush_all():  # noqa: ANN201
     """Flush all unused multipath device maps."""
     cmd = "multipath -F"
     if run(cmd).returncode != 0:
         return False
 
     return True
 
 
-def multipath_backup_conf(bak_file):
+def multipath_backup_conf(bak_file):  # noqa: ANN001, ANN201
     """backup_mp_conf ()
     Usage
     backup_mp_conf(bak_file)
     Purpose
     Check if bak_file exists, if not, copy current to it.
     Parameter
     bak_file       # like "/etc/multipath.conf.bak"
@@ -847,33 +846,33 @@
     true
         or
     False           # file exists or source file not exists;
     Exceptions
     N/A.
     """
     if not Path(MULTIPATH_CONF_PATH).is_file():
-        sts_print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
+        print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
         return False
 
     if Path(bak_file).is_file():
-        sts_print(f"FAIL: mpath backup file {bak_file} already exists")
+        print(f"FAIL: mpath backup file {bak_file} already exists")
         return False
 
-    sts_print(f"INFO: Backing up {MULTIPATH_CONF_PATH} to {bak_file}")
+    print(f"INFO: Backing up {MULTIPATH_CONF_PATH} to {bak_file}")
     cmd = f"cp -f {MULTIPATH_CONF_PATH} {bak_file}"
     ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        sts_print(f"FAIL: Could not backup {MULTIPATH_CONF_PATH}")
+        print(f"FAIL: Could not backup {MULTIPATH_CONF_PATH}")
         print(output)
         return False
 
     return True
 
 
-def multipath_restore_conf(bak_file):
+def multipath_restore_conf(bak_file):  # noqa: ANN001, ANN201
     """multipath_restore_conf ()
     Usage
     multipath_restore_conf(bak_file)
     Purpose
     Check if bak_file exists, if so, copy it to '/etc/multipath.conf'
     and reload mpath conf.
     Parameter
@@ -882,30 +881,30 @@
     True
         or
     False           # file exists or source file not exists;
     Exceptions
     N/A.
     """
     if not Path(bak_file).is_file():
-        sts_print(f"FAIL: {bak_file} does not exist")
+        print(f"FAIL: {bak_file} does not exist")
         return False
 
-    sts_print(f"INFO: Restoring multipath configuration from {bak_file}")
+    print(f"INFO: Restoring multipath configuration from {bak_file}")
     cmd = f"cp -f {bak_file} {MULTIPATH_CONF_PATH}"
     ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        sts_print(f"FAIL: Could not restore backup from {bak_file}")
+        print(f"FAIL: Could not restore backup from {bak_file}")
         print(output)
         return False
 
     multipath_reload_conf()
     return True
 
 
-def multipath_reload_conf():
+def multipath_reload_conf():  # noqa: ANN201
     """Usage
     multipath_reload_conf()
     Purpose
         Execute "multipathd -k'reconfig'" to load configuration.
         After that execute 'multipath -r'
     Parameter
         N/A
@@ -922,15 +921,15 @@
     multipath_reload()
     if ret != 0:
         return False
 
     return True
 
 
-def multipath_setup_blacklist():
+def multipath_setup_blacklist():  # noqa: ANN201
     """multipath_setup_blacklist ()
     Usage
     multipath_setup_blacklist()
     Purpose
     Add 'wwid .*' into blacklist and all exists mpath wwid to
     'blacklist_exceptions'. This will prevent mpath take over newly
     created LUN. This function DO NOT back up configuration, use
@@ -954,20 +953,20 @@
     if not mpath_conf_set("/blacklist/wwid", ".*"):
         return False
 
     for wwid in current_wwids:
         if not mpath_conf_set("/blacklist_exceptions/wwid[last()+1]", wwid):
             return False
 
-    sts_print("INFO: Reloading updated multipath configuration")
+    print("INFO: Reloading updated multipath configuration")
     multipath_reload_conf()
     return True
 
 
-def mpath_conf_remove(path, value):
+def mpath_conf_remove(path, value):  # noqa: ANN001, ANN201
     """Remove parameter from multipath config using augeas.
     For non-unique paths, use return of mpath_conf_match as path
     For valid options use 'man multipath.conf'.
 
     Args:
       path: eg. "/blacklist/wwid"
       value: eg. "<device wwid>"
@@ -979,50 +978,50 @@
       IOError: Augeas save fails. Check if multipath.conf changes are valid.
     """
     matched_path = mpath_conf_match(path, value)
 
     if matched_path:
         out = run(f'augtool -s rm "{matched_path}"', capture_output=True, verbose=False).output
         if "Saved 1 file(s)" not in out:
-            sts_print(f"FAIL: unable to set {path} to {value}")
+            print(f"FAIL: unable to set {path} to {value}")
             return False
 
     return True
 
 
-def mpath_conf_match(path, value):
+def mpath_conf_match(path, value):  # noqa: ANN001, ANN201
     """Checks if parameter is set in multipath.conf using augeas
     Use path expressions to get non-unique paths: https://github.com/hercules-team/augeas/wiki/Path-expressions
     e.g. path="/devices/device[*]/vendor" value="LIO-ORG"
     Successfully matches even if "end of the path" is not unique. e.g. path="/blacklist_exceptions/wwid" value="$wwid".
 
     Args:
       path: eg. "/blacklist/wwid"
       value: eg. "<device wwid>"
 
     Returns:
       matched path or None
     """
     if not linux.install_package("augeas", verbose=False):
-        sts_print("FAIL: Could not install augeas")
+        print("FAIL: Could not install augeas")
         return None
 
     full_path = path if path.startswith(aug_conf_path) else aug_conf_path + path
 
     # successfully matches also when end of path is not unique - path[*] value, but not path[*]/path value
     out = run(f'augtool match "{full_path}" "{value}"', capture_output=True, verbose=False).output
 
     # augtool prints path when matched, return codes seems useless
     if aug_conf_path in out:
         # returning path, as it can be useful when modifying non-unique paths
         return out
     return None
 
 
-def mpath_conf_set(path, value):
+def mpath_conf_set(path, value):  # noqa: ANN001, ANN201
     """Change multipath.conf parameters using augeas.
     To append to non-unique paths, use [last()+1].
     eg. path="/devices/device[last()+1]/vendor" value="LIO-ORG"
     For valid options use 'man multipath.conf'.
 
     Args:
       path: eg. "/defaults/path_selector" or "/files/etc/multipath.conf/defaults/path_selector"
@@ -1038,25 +1037,25 @@
 
     # Need to check if not already exists to avoid duplicates
     path_to_match = re.sub(r"\[[^]]*]", "[.]", path)  # in case path expressions are being used
     matched_path = mpath_conf_match(path_to_match, value)
 
     if not matched_path:
         if not linux.is_installed("augeas"):
-            sts_print("FAIL: Could not install augeas")
+            print("FAIL: Could not install augeas")
             return False
         out = run(f'augtool -s set "{full_path}" "{value}"', capture_output=True, verbose=False).output
         if "Saved 1 file(s)" not in out:
-            sts_print(f"FAIL: unable to set {path} to {value}. Try")
+            print(f"FAIL: unable to set {path} to {value}. Try")
             return False
 
     return True
 
 
-def mp_query_conf(config_str):
+def mp_query_conf(config_str):  # noqa: ANN001, ANN201
     """Parse string containing multipath config to a dict."""
     regex_option = r"^[ \t]*"
     regex_option += r"([^\ #=\t]+)"
     regex_option += r"[\ \t]+"
     regex_option += r"(?:'|\"){0,1}"
     regex_option += r"([^'\"]+)"
     regex_option += r"(?:'|\"){0,1}"
@@ -1124,42 +1123,42 @@
 
             current_section[key] = value
             continue
 
     return config_dict
 
 
-def mp_query_saved_conf():
+def mp_query_saved_conf():  # noqa: ANN201
     """Usage
         mp_query_saved_conf()
     Purpose
         Load multipath config file and return it as a dict
     Parameter
         N/A
     Returns
         mp_conf_dict.
     """
     if not Path(MULTIPATH_CONF_PATH).is_file():
-        sts_print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
+        print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
         return None
 
     cfg_text = _load_config(MULTIPATH_CONF_PATH)
     if not cfg_text:
         return None
 
     return mp_query_conf(cfg_text)
 
 
-def _load_config(config_file):
+def _load_config(config_file):  # noqa: ANN001, ANN202
     """Parse multipath config file to dict."""
     with Path(config_file).open() as f:
         return f.read()
 
 
-def _save_config(config_dict, config_file=MULTIPATH_CONF_PATH):
+def _save_config(config_dict, config_file=MULTIPATH_CONF_PATH):  # noqa: ANN001, ANN202
     """Convert multipath config dict to string and save to file."""
     config_str = ""
     if "defaults" in list(config_dict.keys()):
         config_str += "defaults {\n"
         for key in list(config_dict["defaults"].keys()):
             config_str += f"\t{key} {config_dict['defaults'][key]}\n"
         config_str += "}\n"
@@ -1207,15 +1206,15 @@
 
     with Path(config_file).open("w") as f:
         f.write(config_str)
 
     return True
 
 
-def mpath_device_2_mpath_name(mpath_device):
+def mpath_device_2_mpath_name(mpath_device):  # noqa: ANN001, ANN201
     """Convert a specific multipath device to mpath_name
     E.g. /dev/mapper/mpathap1 => mpatha.
     """
     multipath_dev_regex = r"/dev/mapper\/(.*)"
     m = re.match(multipath_dev_regex, mpath_device)
     if m:
         # need to remove partition information
@@ -1228,10 +1227,9 @@
         device_name = m.group(1)
         m = re.match(r"(.*)p?\d", device_name)
         if not m:
             # does not seem to be a valid mpath device
             return None
         device_name = m.group(1)
         # remove trailing p if it exists
-        device_name = re.sub(r"(\S+)p$", r"\1", device_name)
-        return device_name
+        return re.sub(r"(\S+)p$", r"\1", device_name)
     return None
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/net.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/net.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,115 +9,114 @@
 from os import listdir, readlink
 from os.path import lexists
 from pathlib import Path
 
 import netifaces
 
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.cmdline import exists, run, run_ret_out
 
 __author__ = "Bruno Goncalves"
 __copyright__ = "Copyright (c) 2016 Red Hat, Inc. All rights reserved."
 
 sysfs_class_net_path = "/sys/class/net"
 
 
-def is_mac(mac):
+def is_mac(mac):  # noqa: ANN001, ANN201
     """Check if given MAC is  on valid format."""
     if standardize_mac(mac):
         return True
     return False
 
 
-def get_nics():
+def get_nics():  # noqa: ANN201
     """Return list of all NICs on the server."""
     ifaces = netifaces.interfaces()
     if ifaces is None:  # No NIC on this server
         return None
 
     return ifaces
 
 
-def get_mac_of_nic(nic):
+def get_mac_of_nic(nic):  # noqa: ANN001, ANN201
     """Given a NIC name return its MAC address."""
     try:
         mac = netifaces.ifaddresses(nic)[netifaces.AF_PACKET][0]["addr"]
     except Exception as e:
         print(repr(e))
         return None
     else:
         return mac
 
 
-def get_nic_of_mac(mac_address):
+def get_nic_of_mac(mac_address):  # noqa: ANN001, ANN201
     """Give an MAC address return the server interface name."""
     if not mac_address:
-        sts_print("FAIL: get_nic_of_mac() - requires mac as argument")
+        print("FAIL: get_nic_of_mac() - requires mac as argument")
         return None
 
     mac = mac_address.lower()
 
     if not is_mac(mac):
-        sts_print(f"FAIL: get_nic_of_mac() - {mac} does not seem to be a valid MAC")
+        print(f"FAIL: get_nic_of_mac() - {mac} does not seem to be a valid MAC")
         return None
 
     nics = get_nics()
     if not nics:
         return None
 
     for nic in nics:
         if mac == get_mac_of_nic(nic):
             return nic
 
     return None
 
 
-def get_ip_address_of_nic(nic):
+def get_ip_address_of_nic(nic):  # noqa: ANN001, ANN201
     """Get IPv4 of specific network interface."""
     try:
         ip = netifaces.ifaddresses(nic)[netifaces.AF_INET][0]["addr"]
     except KeyError as e:
         print(f"KeyError - Iface probably does not have a IP address - {e!s}")
     except Exception as e:
         print(repr(e))
     else:
         return ip
     return None
 
 
-def get_ipv6_address_of_nic(nic):
+def get_ipv6_address_of_nic(nic):  # noqa: ANN001, ANN201
     """Get IPv6 of specific network interface."""
     try:
         ip = netifaces.ifaddresses(nic)[netifaces.AF_INET6][0]["addr"]
     except KeyError as e:
         print(f"KeyError - Iface probably does not have a IPv6 address - {e!s}")
     except Exception as e:
         print(repr(e))
     else:
         return ip
     return None
 
 
-def get_nic_of_ip(ip):
+def get_nic_of_ip(ip):  # noqa: ANN001, ANN201
     """Given an IP address return the NIC name using it."""
     if not ip:
         return None
 
     nics = get_nics()
     if not nics:
         return None
 
     for nic in nics:
         if ip == get_ip_address_of_nic(nic):
             return nic
     return None
 
 
-def nic_2_driver():
+def nic_2_driver():  # noqa: ANN201
     """Return a dictionary where nic name is the key and driver name is the value.
     Will skip sub interfaces, loop device, tun, vboxnet0.
     The arguments are:
     None
     return_output (Dict): Return a dictionary
     Returns:
     dict: Return dict containing all NICs.
@@ -137,15 +136,15 @@
     # print nic_dict
     return nic_dict
 
 
 # End of nic_2_driver()
 
 
-def driver_of_nic(nic):
+def driver_of_nic(nic):  # noqa: ANN001, ANN201
     """Given a specific NIC name it returns its driver name
     Find out the driver of certain NIC via sysfs file:
         /sys/class/net/eth0/device/driver   # it's a link.
     The arguments are:
     nic: NIC name, e.g. eth0
     Returns:
     str: Driver name.
@@ -168,39 +167,39 @@
         return None
     return m.group(1)
 
 
 # End of driver_of_nic()
 
 
-def phy_nic_of(nic):
+def phy_nic_of(nic):  # noqa: ANN001, ANN201
     """Translate sub-interface of NIC 'eth0.802-fcoe' to physical NIC 'eth0'.
     The arguments are:
     nic: NIC name, e.g. eth0.802-fcoe
     Returns:
     str: phy NIC, e.g. eth0.
     """
     if not nic:
         return None
     return re.sub(r"\..+$", "", nic)
 
 
-def get_pci_id_of_nic(nic):
+def get_pci_id_of_nic(nic):  # noqa: ANN001, ANN201
     """From a specific network interface return its PCI id."""
     regex_pci_id = linux.get_regex_pci_id()
     sys_path = f"{sysfs_class_net_path}/{nic}"
     link_path = readlink(sys_path)
-    # sts_print("DEBUG: get_pci_id_of_nic - %s" % link_path)
+    # print("DEBUG: get_pci_id_of_nic - %s" % link_path)
     m = re.search(f"({regex_pci_id})/net/{nic}", link_path)
     if m:
         return m.group(1)
     return None
 
 
-def get_ip_version(addr):
+def get_ip_version(addr):  # noqa: ANN001, ANN201
     """Given an address, tries to check if it is IPv6 or not
     The arguments are:
     addr:     Network address
     Returns:
     4:        If it is a valid IPv4 address
     6:        If it is a valid IPv6 address
     None:     addr is not an IPv4 or IPv6 address.
@@ -210,15 +209,15 @@
     except Exception as e:
         print(repr(e))
         return None
     else:
         return ipver
 
 
-def standardize_mac(mac):
+def standardize_mac(mac):  # noqa: ANN001, ANN201
     """Usage
         standardize_mac(mac)
     Purpose
         Convert all possible format mac into stand type:
             (?:[0-9A-F]{2}:){5}[0-9A-F]{2} #like: F0:DE:F1:0D:D3:C9
         Return STRING or ARRAY base on context.
     Parameter
@@ -243,34 +242,34 @@
 
     if re.match(regex_standard_mac, mac, re.IGNORECASE):
         return mac
 
     return None
 
 
-def convert_netmask(netmask="255.255.255.0"):
+def convert_netmask(netmask="255.255.255.0"):  # noqa: ANN001, ANN201
     """Converts subnet mask to CIDR prefix.
     netmask: common subnet mask.
     """
     try:
         cidr = ipaddress.IPv4Network((0, netmask)).prefixlen
     except ValueError as e:
         print(e)
         return None
     else:
         return cidr
 
 
-def if_down(nic_or_mac):
+def if_down(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface down using ifdown tool
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        sts_print("FAIL: if_down() - requires nic or mac as argument")
+        print("FAIL: if_down() - requires nic or mac as argument")
         return None
 
     # ifup/ifdown scripts are not shipped by default on RHEL-8+
     if (
         not exists("ifdown")
         and linux.is_installed("NetworkManager")
         and not linux.install_package("NetworkManager-initscripts-updown")
@@ -281,21 +280,21 @@
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
     if run(f"ifdown {nic}"):
         return True
     return False
 
 
-def if_up(nic_or_mac):
+def if_up(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface up using ifup tool
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        sts_print("FAIL: if_up() - requires nic or mac as argument")
+        print("FAIL: if_up() - requires nic or mac as argument")
         return None
 
     # ifup/ifdown scripts are not shipped by default on RHEL-8+
     if (
         not exists("ifup")
         and linux.is_installed("NetworkManager")
         and not linux.install_package("NetworkManager-initscripts-updown")
@@ -306,51 +305,51 @@
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
     if run(f"ifup {nic}"):
         return True
     return False
 
 
-def iface_up(nic_or_mac):
+def iface_up(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface up
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        sts_print("FAIL: iface_up() - requires nic or mac as argument")
+        print("FAIL: iface_up() - requires nic or mac as argument")
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
     retcode, output = run_ret_out(f"ip link set {nic} up", return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
-def iface_down(nic_or_mac):
+def iface_down(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface down
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        sts_print("FAIL: iface_down() - requires nic or mac as argument")
+        print("FAIL: iface_down() - requires nic or mac as argument")
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
     retcode, output = run_ret_out(f"ip link set {nic} down", return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
-def set_ifcfg(nic_or_mac, parameters):
+def set_ifcfg(nic_or_mac, parameters):  # noqa: ANN001, ANN201
     """Edit or create ifcfg files: IP, prefix, gateway, defroute...
     Parameters:
      nic_or_mac: interface name or mac address
      parameters: dict of params e.g. {'IPADDR': '10.37.151.7'}.
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
@@ -365,26 +364,26 @@
         return False
 
     if_down(nic)
     if_up(nic)
     return True
 
 
-def get_default_iface():
+def get_default_iface():  # noqa: ANN201
     """Returns tuple with ip and interface.
     example: ('10.1.1.1', 'eno1').
     """
     try:
         return netifaces.default_gateway()[netifaces.AF_INET]
     except Exception as e:
         print(repr(e))
         return None
 
 
-def nm_get_conn(nic_or_mac):
+def nm_get_conn(nic_or_mac):  # noqa: ANN001, ANN201
     """Returns NetworkManager connection UUID
     nic_or_mac: interface name or mac address.
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
         if not nic:
             print("FAIL: Couldn't find NIC from MAC.")
@@ -399,108 +398,108 @@
         if nm_get_conn_iface(nic) == nic:
             return nm_get_conn_uuid(nic)
         return None
     conn = str(conn)
     return nm_get_conn_uuid(conn)
 
 
-def nm_get_conn_iface(conn):
+def nm_get_conn_iface(conn):  # noqa: ANN001, ANN201
     """Returns interface name used by NM connection
     conn: connection id or uuid.
     """
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get connection.interface-name for connection " + conn)
         print(output)
         return None
     return output
 
 
-def nm_get_conn_uuid(conn):
+def nm_get_conn_uuid(conn):  # noqa: ANN001, ANN201
     """Returns NetworkManager connection UUID
     conn: connection id.
     """
     cmd = f"nmcli -g connection.uuid conn show '{conn}'"
     print(cmd)
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get NM connection uuid using " + conn)
         print(output)
         return None
     return output
 
 
-def nm_get_conn_from_dev(nic):
+def nm_get_conn_from_dev(nic):  # noqa: ANN001, ANN201
     """Returns connection id(name) using specified device.
     nic: network interface - device.
     """
     nic = str(nic)
     cmd = "nmcli -g GENERAL.CONNECTION device show " + nic
 
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get NM connection using device " + nic)
         print(output)
         return None
     return output
 
 
-def nm_get_dev_from_conn(conn):
+def nm_get_dev_from_conn(conn):  # noqa: ANN001, ANN201
     """Returns a device used by specified connection
     conn: networkmanager connection id(name) or uuid.
     """
     conn = str(conn)
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
 
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get device used by NM connection " + conn)
         print(output)
         return None
     return output
 
 
-def nm_conn_up(conn):
+def nm_conn_up(conn):  # noqa: ANN001, ANN201
     """Uses nmcli to activate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn up "{conn}"'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to activate the connection: {conn}")
         return False
     print(output)
     return True
 
 
-def nm_conn_down(conn):
+def nm_conn_down(conn):  # noqa: ANN001, ANN201
     """Uses nmcli to deactivate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn down "{conn}"'
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to deactivate the connection: {conn}")
         return False
     print(output)
     return True
 
 
-def nm_conn_reload():
+def nm_conn_reload():  # noqa: ANN201
     """Runs `nmcli conn reload`. Does not support RHEL6."""
     cmd = "nmcli conn reload"
     retcode = run(cmd, verbose=False).returncode
     if retcode != 0:
         print("FAIL: Unable to reload NetworkManager")
         return False
     return True
 
 
-def nm_conn_show(conn):
+def nm_conn_show(conn):  # noqa: ANN001, ANN201
     """Use nmcli conn to show all connection parameters. Does not support RHEL6
     conn: networkmanager connection id(name) or uuid.
     """
     if not conn:
         print("FAIL: No conn specified")
         return False
 
@@ -509,28 +508,28 @@
     if retcode != 0:
         print("FAIL: Unable to show conn")
         return False
     print(output)
     return True
 
 
-def nm_conn_del(conn):
+def nm_conn_del(conn):  # noqa: ANN001, ANN201
     """Deletes NetworkManager connection using nmcli
     conn: connection id(name) or uuid.
     """
     cmd = f"nmcli conn delete {conn}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to delete the conn {conn}")
         return False
     print(output)
     return True
 
 
-def nm_add_conn(name=None, nic_or_mac=None, nic_type="ethernet"):
+def nm_add_conn(name=None, nic_or_mac=None, nic_type="ethernet"):  # noqa: ANN001, ANN201
     """Use it to add new connection for devices without one
     cmd="nmcli con add type ethernet ifname enp5s0f1 con-name enp5s0f1 ".
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
         if not nic:
             print("FAIL: Couldn't find NIC from MAC.")
@@ -559,15 +558,15 @@
         print(f"FAIL: Unable to add con with cmd {cmd} ")
         print(output)
         return False
     nm_conn_reload()
     return True
 
 
-def nm_conn_mod(conn, key, value):
+def nm_conn_mod(conn, key, value):  # noqa: ANN001, ANN201
     """Modify one or more properties of the NetworkManager connection profile.
     nm_con_mod("enp17s0f1","connection.autoconnect", "yes")
     nmcli c modify ens2f1 connection.autoconnect yes
     Examples compared to network-scripts:
     ipv4.method manual     >> BOOTPROTO=none
     ipv4.method auto       >> BOOTPROTO=dhcp
     ipv4.address "192.168.0.10/24"   >> IPADDR=192.168.0.10
@@ -593,15 +592,15 @@
     if retcode != 0:
         print(f"FAIL: Unable to modify conn {conn} with cmd {cmd} ")
         print(output)
         return False
     return True
 
 
-def nm_dev_mod(dev, key, value):
+def nm_dev_mod(dev, key, value):  # noqa: ANN001, ANN201
     """Modify one or more properties that are currently active on the device without modifying
     the connection profile. The changes have immediate effect.
     nmcli dev modify em1 ipv4.method shared
     nmcli dev modify em1 ipv4.address xx.
     """
     cmd = f"nmcli device modify {dev}"
     cmd += f" {key} {value}"
@@ -609,15 +608,15 @@
     if retcode != 0:
         print(f"FAIL: Unable to modify dev {dev} with cmd {cmd} ")
         print(output)
         return False
     return True
 
 
-def nm_set_ip(conn, ip, netmask="24", activate=True):
+def nm_set_ip(conn, ip, netmask="24", activate=True):  # noqa: ANN001, ANN201
     """Uses nmcli to set static IP, netmask and activates connection.
     conn: networkmanager connection id(name) or uuid
     ip: IPv4 or IPv6.
     """
     ip = str(ip)
     ipver = get_ip_version(ip)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/qemu_img.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 """qemu_img.py: Module to manipulate disk image using QEMU disk image utility."""
 from pathlib import Path
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.cmdline import run
 
 _QCOW_SUPPORTED_OPTIONS = [
     "compat",
     "backing_file",
     "encryption",
     "cluster_size",
     "preallocation",
     "lazy_refcounts",
 ]
 
 
-def _get_package_name():
+def _get_package_name():  # noqa: ANN202
     return "qemu-img"
 
 
-def _get_image_file(name, image_path):
+def _get_image_file(name, image_path):  # noqa: ANN001, ANN202
     return f"{image_path}/{name}.img"
 
 
-def get_qcow_supported_options():
+def get_qcow_supported_options():  # noqa: ANN201
     """Return supported options for qcow image.
 
     Returns:
       List of strings.
     """
     return _QCOW_SUPPORTED_OPTIONS
 
 
-def install_qemu_img():
+def install_qemu_img():  # noqa: ANN201
     """Install qemu-img tool.
 
     Returns:
     True: If qemu-img is installed correctly
     False: If some problem happened
     """
     if not linux.install_package(_get_package_name()):
-        sts_print(f"FAIL: Could not install {_get_package_name()}")
+        print(f"FAIL: Could not install {_get_package_name()}")
         return False
     return True
 
 
-def qemu_create(filename, size="1024", fmt=None, img_path="/var/tmp", **options):
+def qemu_create(filename, size="1024", fmt=None, img_path="/var/tmp", **options):  # noqa: ANN001, ANN003, ANN201
     """Create the new disk image.
 
     Args:
       filename: is a disk image filename
       size: is the disk image size in bytes
       fmt: is the disk image format
       img_path: is the full path to output directory
@@ -60,48 +59,48 @@
     Returns:
     True: if success
     False: in case of failure
     """
     if not linux.is_installed(_get_package_name()):
         install_qemu_img()
     if not filename:
-        sts_print("FAIL: qemu_create() requires parameter filename")
+        print("FAIL: qemu_create() requires parameter filename")
         return False
     if img_path:
         filename = _get_image_file(filename, img_path)
     cmd = _get_package_name() + " create "
     if fmt is not None:
         cmd += f"-f {fmt}"
     if fmt == "qcow2" and options:
         cmd += " -o "
         option = [str(i) + "=" + str(options[i]) for i in options if i in _QCOW_SUPPORTED_OPTIONS]
         cmd += ",".join(option)
     cmd += f" {filename} {size}"
     if run(cmd).returncode != 0:
-        sts_print("FAIL: Could not create disk image.")
+        print("FAIL: Could not create disk image.")
         return False
     return True
 
 
-def delete_image(name, image_path="/var/tmp"):
+def delete_image(name, image_path="/var/tmp"):  # noqa: ANN001, ANN201
     """Delete the disk image.
 
     Args:
       name: is the image filename
       image_path: is the full path to the image directory
 
     Returns:
     True: if success
     False: in case of failure
     """
     if not name:
-        sts_print("FAIL: delete_image() - requires name parameter")
+        print("FAIL: delete_image() - requires name parameter")
         return False
 
     print(f"INFO: Deleting image device {name}")
     fname = _get_image_file(name, image_path)
     if Path(fname).is_file():
         cmd = f"rm -f {fname}"
         if run(cmd).returncode != 0:
-            sts_print(f"FAIL: Could not delete image disk file {fname}")
+            print(f"FAIL: Could not delete image disk file {fname}")
             return False
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 
 import os.path
 import re
 from os import readlink
 from pathlib import Path
 
 from sts import linux, lvm, md, mp, net
-from sts.utils import size, sts_print
+from sts.utils import size
 from sts.utils.cmdline import exists, run, run_ret_out
 
 # I'm still note sure whether to use /sys/class/scsi_disk or /sys/class/scsi_device
 
 sys_disk_path = "/sys/class/scsi_disk"
 host_path = "/sys/class/scsi_host"
 
 # add /lib/udev to PATH because scsi_id is located there on RHEL7
 os.environ["PATH"] += ":/lib/udev"
 
 
-def get_regex_scsi_id():
+def get_regex_scsi_id():  # noqa: ANN201
     return "([0-9]+):([0-9]+):([0-9]+):([0-9]+)"
 
 
-def is_scsi_device(scsi_device):
+def is_scsi_device(scsi_device):  # noqa: ANN001, ANN201
     return bool(re.match("^sd[a-z]+$", scsi_device))
 
 
-def get_scsi_disk_ids():
+def get_scsi_disk_ids():  # noqa: ANN201
     """Return an array of scsi_ids. If an scsi_device name is given as
     parameter, then just the id of the device is returned (TODO)
     The arguments are:
     None
     Device name: eg. sda
     Returns:
     array: Return an array of SCSI IDs.
@@ -41,51 +41,51 @@
     cmd = f"ls {sys_disk_path}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output.split()
 
 
-def get_scsi_disk_name(device_id):
+def get_scsi_disk_name(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        sts_print("FAIL: get_scsi_disk_name() requires scsi_device_id as parameter")
+        print("FAIL: get_scsi_disk_name() requires scsi_device_id as parameter")
         return None
 
     cmd = f"ls {sys_disk_path}/{device_id}/device/block"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
-def get_scsi_disk_vendor(device_id):
+def get_scsi_disk_vendor(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        sts_print("FAIL: get_scsi_disk_vendor() requires scsi_device_id as parameter")
+        print("FAIL: get_scsi_disk_vendor() requires scsi_device_id as parameter")
         return None
 
     cmd = f"cat {sys_disk_path}/{device_id}/device/vendor"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
-def get_scsi_disk_model(device_id):
+def get_scsi_disk_model(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        sts_print("FAIL: get_scsi_disk_model() requires scsi_device_id as parameter")
+        print("FAIL: get_scsi_disk_model() requires scsi_device_id as parameter")
         return None
 
     cmd = f"cat {sys_disk_path}/{device_id}/device/model"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
-def query_all_scsi_disks(scsi_disk=None):
+def query_all_scsi_disks(scsi_disk=None):  # noqa: ANN001, ANN201
     """Query information of all SCSI disks and return them as a dict
     SCSI id is the dict key.
     If an SCSI disk is given as argument, return its info
     Parameter:
     scsi_disk (option):        SCSI disk name. eg: 'sda'.
     """
     disk_ids = get_scsi_disk_ids()
@@ -96,15 +96,15 @@
     scsi_disks = {}
     for disk_id in disk_ids:
         scsi_name = get_scsi_disk_name(disk_id)
         if scsi_disk and scsi_name and scsi_disk != scsi_name:
             # optimization in case we requested specific disk, do not query all
             continue
         if not scsi_name:
-            sts_print(f"WARN: Could not get scsi_name for disk_id '{disk_id}'.")
+            print(f"WARN: Could not get scsi_name for disk_id '{disk_id}'.")
             scsi_wwid = scsi_wwn = udev_wwn = size_bytes = state = timeout = None
         else:
             scsi_wwid = wwid_of_disk(scsi_name)
             scsi_wwn = wwn_of_disk(scsi_name)
             udev_wwn = udev_wwn_of_disk(scsi_name)
             size_bytes = size_of_disk(scsi_name)
             state = disk_sys_check(scsi_name)
@@ -139,78 +139,78 @@
             if scsi_disk == scsi_disks[disk_id]["name"]:
                 return scsi_disks[disk_id]
         return None
 
     return scsi_disks
 
 
-def get_scsi_name_by_vendor(vendor):
+def get_scsi_name_by_vendor(vendor):  # noqa: ANN001, ANN201
     """Query information of all SCSI disks and return all scsi device names that
     are from the requested vendor
     Parameter:
     vendor:        SCSI disk Vendor. eg: 'LIO'
     Return:
     List:          List of SCSI names.
     """
     if not vendor:
-        sts_print("FAIL: get_scsi_name_by_vendor() - requires vendor parameter")
+        print("FAIL: get_scsi_name_by_vendor() - requires vendor parameter")
         return None
 
     all_scsi_disks_info = query_all_scsi_disks()
     if not all_scsi_disks_info:
         return None
     scsi_names = []
     for scsi_info in list(all_scsi_disks_info.values()):
         if "vendor" in list(scsi_info.keys()) and scsi_info["vendor"] == vendor:
             scsi_names.append(scsi_info["name"])
     return scsi_names
 
 
-def scsi_host_of_scsi_name(scsi_name):
+def scsi_host_of_scsi_name(scsi_name):  # noqa: ANN001, ANN201
     if not scsi_name:
-        sts_print("FAIL: scsi_host_of_scsi_name() - requires scsi_name parameter")
+        print("FAIL: scsi_host_of_scsi_name() - requires scsi_name parameter")
         return None
 
     scsi_disk_info = query_all_scsi_disks(scsi_name)
     if not scsi_disk_info:
-        sts_print(f"WARN: scsi_host_of_scsi_name() did not query info for {scsi_name}")
+        print(f"WARN: scsi_host_of_scsi_name() did not query info for {scsi_name}")
         return None
     return scsi_disk_info["host_id"]
 
 
-def scsi_name_2_scsi_id(scsi_name):
+def scsi_name_2_scsi_id(scsi_name):  # noqa: ANN001, ANN201
     if not scsi_name:
-        sts_print("FAIL: scsi_name_2_scsi_id() - requires scsi_name parameter")
+        print("FAIL: scsi_name_2_scsi_id() - requires scsi_name parameter")
         return None
 
     scsi_disk_info = query_all_scsi_disks(scsi_name)
     if not scsi_disk_info:
-        sts_print(f"WARN: scsi_name_2_scsi_id() did not query info for {scsi_name}")
+        print(f"WARN: scsi_name_2_scsi_id() did not query info for {scsi_name}")
         return None
     return scsi_disk_info["scsi_id"]
 
 
-def delete_disk(device_name):
+def delete_disk(device_name):  # noqa: ANN001, ANN201
     """device_name:    eg. sda."""
     if not device_name:
-        sts_print("FAIL: delete_disk() requires scsi_device_name as parameter")
+        print("FAIL: delete_disk() requires scsi_device_name as parameter")
         return None
 
     device_id = scsi_name_2_scsi_id(device_name)
     if not device_id:
-        sts_print(f"FAIL: delete_disk() could not find disk {device_name}")
+        print(f"FAIL: delete_disk() could not find disk {device_name}")
         return None
 
     cmd = f'echo "1" >  {sys_disk_path}/{device_id}/device/delete'
     if run(cmd, verbose=False).returncode != 0:
         return None
     return True
 
 
-def get_hosts(somethings=None):
+def get_hosts(somethings=None):  # noqa: ANN001, ANN201
     """Return a list with all SCSI hosts.
     The arguments are:
     None
     or
     scsi_disk     e.g. sda
     or
     scsi_id       e.g. 3:0:0:1
@@ -228,15 +228,15 @@
     if not somethings:
         return all_host_ids
 
     scsi_host_ids = None
     # If something is a single string, convert it to list
     for something in somethings if not isinstance(somethings, str) else [somethings]:
         if something is None:
-            sts_print("FAIL: get_hosts() - Invalid input")
+            print("FAIL: get_hosts() - Invalid input")
             print(somethings)
             return None
         m = re.match(get_regex_scsi_id(), something)
         if m and m.group(1) in all_host_ids:
             if not scsi_host_ids:
                 scsi_host_ids = []
             if m.group(1) not in scsi_host_ids:
@@ -249,19 +249,18 @@
                 if not scsi_host_ids:
                     scsi_host_ids = []
                 if m.group(1) not in scsi_host_ids:
                     scsi_host_ids.append(m.group(1))
 
     if not scsi_host_ids:
         return None
-    scsi_host_ids = list(set(scsi_host_ids))
-    return scsi_host_ids
+    return list(set(scsi_host_ids))
 
 
-def query_scsi_host_info(host_id):
+def query_scsi_host_info(host_id):  # noqa: ANN001, ANN201
     """Usage
         query_scsi_host_info(scsi_host_id)
     Purpose
         Save sysfs info of "/sys/class/scsi_host/host$scsi_host_id" to
             scsi_host_info
         We also check these folders:
             /sys/class/iscsi_host/host$scsi_host_id/
@@ -270,20 +269,20 @@
         scsi_host_id           # like '0' for host0
     Returns
         scsi_host_info
             or
         None.
     """
     if not host_id:
-        sts_print("FAIL: query_scsi_host_info() - requires host_id")
+        print("FAIL: query_scsi_host_info() - requires host_id")
         return None
 
     sysfs_folder = Path(f"/sys/class/scsi_host/host{host_id}")
     if not sysfs_folder.is_dir():
-        sts_print(f"FAIL: {host_id} is not a valid directory")
+        print(f"FAIL: {host_id} is not a valid directory")
         return None
 
     scsi_host_info = {
         "scsi_host_id": host_id,
         "pci_id": pci_id_of_host_id(host_id),
         "driver": scsi_driver_of_host_id(host_id),
     }
@@ -311,35 +310,34 @@
                 # For some reason could not read the file
                 continue
             scsi_host_info[param] = ", ".join(output.split("\n"))
 
     return scsi_host_info
 
 
-def scsi_driver_of_host_id(host_id):
+def scsi_driver_of_host_id(host_id):  # noqa: ANN001, ANN201
     if not host_id:
-        sts_print("FAIL: scsi_driver_of_host_id() - requires host_id parameter")
+        print("FAIL: scsi_driver_of_host_id() - requires host_id parameter")
         return None
     scsi_drv_sysfs = f"/sys/class/scsi_host/host{host_id}/proc_name"
     if not Path(scsi_drv_sysfs).is_file():
-        sts_print(f"FAIL: {scsi_drv_sysfs} is not a valid path")
+        print(f"FAIL: {scsi_drv_sysfs} is not a valid path")
         return None
 
     output = run(f"cat {scsi_drv_sysfs}", capture_output=True, verbose=False).output
     scsi_driver = output
     if scsi_driver == "(null)" or scsi_driver == "":
         # Driver information was not exported, let try to find it out some other way
         lpfc_sysfs_file = f"/sys/class/scsi_host/host{host_id}/lpfc_drvr_version"
         if Path(lpfc_sysfs_file).is_file():
             return "lpfc"
 
         driver_sysfs_file = f"/sys/class/scsi_host/host{host_id}/driver_name"
         if Path(driver_sysfs_file).is_file():
-            output = run(f"cat {driver_sysfs_file}", capture_output=True, verbose=False).output
-            return output
+            return run(f"cat {driver_sysfs_file}", capture_output=True, verbose=False).output
 
         model_sysfs_file = f"/sys/class/scsi_host/host{host_id}/model_name"
         if Path(model_sysfs_file).is_file():
             output = run(f"cat {model_sysfs_file}", capture_output=True, verbose=False).output
             if re.match("^QLE", output):
                 return "qla2xxx"
 
@@ -349,74 +347,74 @@
             if re.search("bnx2fc", output):
                 return "bnx2fc"
 
         pci_id = pci_id_of_host_id(host_id)
         if pci_id:
             lspci_regex = r"Kernel modules:\s+(\S+)"
             if not exists("lspci"):
-                sts_print("FAIL: pciutils is not installed. Can't query driver name using pci_id.")
+                print("FAIL: pciutils is not installed. Can't query driver name using pci_id.")
                 return None
             output = run(
                 f'lspci -s "{pci_id}" -v | grep "Kernel modules:"',
                 capture_output=True,
                 verbose=False,
             ).output
             if output:
                 m = re.search(lspci_regex, output)
                 if m:
                     return m.group(1)
 
-        sts_print(f"FAIL: Could not get driver name for SCSI host{host_id}")
+        print(f"FAIL: Could not get driver name for SCSI host{host_id}")
         return None
     if scsi_driver == "fcoe":
         drv_version_path = f"/sys/class/fc_host/host{host_id}/driver_version"
         output = run(f"cat {drv_version_path}", capture_output=True, verbose=False).output
         if re.search("ixgbe", output):
             return "ixgbe"
     return scsi_driver
 
 
-def pci_id_of_host_id(host_id):
+def pci_id_of_host_id(host_id):  # noqa: ANN001, ANN201
     """Usage
         pci_id_of(scsi_host_id);
     Purpose
         Find out which PCI id providing the SCSI Host via:
             readlink("/sys/class/scsi_host/host'scsi_host_id'");
     Parameter
         $scsi_host_id           # like '0' for host0
     Returns
         pci_id                 # like '0000:00:1c.0'.
     """
     if not host_id:
-        sts_print("FAIL: pci_id_of_host_id() - requires host_id parameter")
+        print("FAIL: pci_id_of_host_id() - requires host_id parameter")
         return None
     sys_path = f"/sys/class/scsi_host/host{host_id}"
     if not Path(sys_path).exists():
-        sts_print(f"FAIL: {sys_path} is not a valid path")
+        print(f"FAIL: {sys_path} is not a valid path")
         return None
 
     link_path = readlink(sys_path)
 
     regex_pci_id = linux.get_regex_pci_id()
     m = re.search(f"({regex_pci_id})/host{host_id}/scsi_host", link_path)
-    # sts_print("DEBUG: pci_id_of_host_id - %s" % link_path)
+    # print("DEBUG: pci_id_of_host_id - %s" % link_path)
     if m:
         return m.group(1)
 
     # for example ixgbe need to check the PCI id from the network device
     # check for network interface name
     net_regex = re.compile(r"devices/virtual/net/(.*)\.")
     m = net_regex.search(link_path)
     if m:
         return net.get_pci_id_of_nic(m.group(1))
 
     return None
 
 
-def rescan_host(host=None, verbose=True):
+def rescan_host(host=None, verbose=True):  # noqa: ANN001, ANN201
     """Rescan for devices for specific host
     If no host is given it will scan all SCSI hosts
     The arguments are:
     Host:      e.g. 1 for host1
     Returns:
     True if no problem executing command
     False if something went wrong.
@@ -428,32 +426,32 @@
         scsi_hosts = get_hosts()
         for host in scsi_hosts:
             host_list.append(host)
 
     error = 0
 
     if not host_list:
-        sts_print("WARN: No host found on server to rescan")
+        print("WARN: No host found on server to rescan")
         return True
 
     for host in host_list:
         if verbose:
-            sts_print(f"INFO: Rescanning host{host}")
+            print(f"INFO: Rescanning host{host}")
         cmd = f'echo "- - -" > {host_path}/host{host}/scan'
         if run(cmd, verbose=verbose).returncode != 0:
             error += 1
-            sts_print(f"FAIL: there was some problem scanning host{host}")
+            print(f"FAIL: there was some problem scanning host{host}")
 
     if error:
         return False
 
     return True
 
 
-def rescan_disk(scsi_disk=None):
+def rescan_disk(scsi_disk=None):  # noqa: ANN001, ANN201
     """Rescan a specific SCSI disk.
     If no disk is given, rescann all SCSI disks
     echo 1 > /sys/block/<scsi_disk>/device/rescan
     Host:      e.g. 1 for host1
     Returns:
     True if no problem executing command
     False if something went wrong.
@@ -467,24 +465,24 @@
         for _id in ids:
             scsi_disks.append(get_scsi_disk_name(_id))
 
     error = 0
     for scsi_disk in scsi_disks:
         cmd = f"echo 1 > /sys/block/{scsi_disk}/device/rescan"
         if run(cmd).returncode != 0:
-            sts_print(f"FAIL: Could not rescan {scsi_disk}")
+            print(f"FAIL: Could not rescan {scsi_disk}")
             error += 1
 
     if error:
         return False
 
     return True
 
 
-def size_of_disk(scsi_disk):
+def size_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
         size_of_disk(disk)
     Purpose
         Given an scsi_disk name. Eg. sda
     Parameter
         scsi_disk
     Returns
@@ -493,67 +491,67 @@
     """
     if not scsi_disk:
         return None
 
     cmd = f"cat /sys/block/{scsi_disk}/queue/logical_block_size"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: size_of_disk() - Could not get size for disk {scsi_disk}")
+        print(f"FAIL: size_of_disk() - Could not get size for disk {scsi_disk}")
         print(output)
         return None
     if not output:
         return None
     logical_block_size = output
 
     cmd = f"cat /sys/block/{scsi_disk}/size"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: size_of_disk() - Could not get sectore size for disk {scsi_disk}")
+        print(f"FAIL: size_of_disk() - Could not get sectore size for disk {scsi_disk}")
         print(output)
         return None
     if not output:
         return None
 
     sector_size = output
 
     return int(logical_block_size) * int(sector_size)
 
 
-def wwid_of_disk(scsi_disk=None):
+def wwid_of_disk(scsi_disk=None):  # noqa: ANN001, ANN201
     """Usage
         wwid_of_disk(disk)
     Purpose
         Given a scsi_disk name. E.g. sda, mpatha
     Parameter
         scsi_disk   device to get wwid for
     Returns
         wwid:       e.g. 360fff19abdd9f5fb943525d45126ca27.
     """
     if not scsi_disk:
-        sts_print("FAIL: wwid_of_disk() - requires scsi_disk parameter")
+        print("FAIL: wwid_of_disk() - requires scsi_disk parameter")
         return None
 
     if linux.is_dm_device(scsi_disk):
         return linux.get_udev_property(scsi_disk, "DM_SERIAL")
 
     return linux.get_udev_property(scsi_disk, "ID_SERIAL")
 
 
-def scsi_ids_of_wwid(wwid):
+def scsi_ids_of_wwid(wwid):  # noqa: ANN001, ANN201
     """Usage
         scsi_ids_of_wwid(wwid)
     Purpose
         Find out all SCSI id for WWID.
     Parameter
         wwid
     Returns
         scsi_ids.
     """
     if not wwid:
-        sts_print("FAIL: scsi_ids_of_wwid(): Got NULL input for WWID")
+        print("FAIL: scsi_ids_of_wwid(): Got NULL input for WWID")
         return None
 
     scsi_ids = []
     all_scsi_info = query_all_scsi_disks()
     if not all_scsi_info:
         # Could not find any SCSI device
         return None
@@ -562,139 +560,137 @@
         if all_scsi_info[_id]["wwid"] == wwid:
             scsi_ids.append(_id)
     if scsi_ids:
         scsi_ids = list(set(scsi_ids))  # dedup
     return scsi_ids
 
 
-def wwn_of_disk(scsi_disk):
+def wwn_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
         wwn_of_disk(disk)
     Purpose
         Given an scsi_disk name. Eg. sda
     Parameter
         scsi_disk
     Returns
         wwid:       eg. 0x60a980003246694a412b45673342616e.
     """
     if not scsi_disk:
-        sts_print("FAIL: wwn_of_disk() - requires scsi_disk parameter")
+        print("FAIL: wwn_of_disk() - requires scsi_disk parameter")
         return None
 
     key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
 
     # cmd = "udevadm info --name=%s --query=all" % scsi_disk
     # retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     # if (retcode != 0):
-    # #sts_print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
+    # #print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
     # #print output
 
     # return None
 
     # udev_wwn = None
     # lines = output.split("\n")
     # for line in lines:
     # m = re.search(key_regex, line)
     # if m:
     # udev_wwn = m.group(1)
 
     cmd = f"scsi_id --whitelisted --export /dev/{scsi_disk}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        # sts_print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
+        # print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
     lines = output.split("\n")
     for line in lines:
         m = re.search(key_regex, line)
         if m:
-            scsi_wwn = m.group(1)
-            return scsi_wwn
+            return m.group(1)
 
     # if udev_wwn and scsi_wwn:
     # if udev_wwn == scsi_wwn:
     # return udev_wwn
-    # sts_print("udevadm WWN is %s" % udev_wwn)
-    # sts_print("scsi_id WWN is %s" % scsi_wwn)
-    # sts_print("FAIL: wwn_of_disk() - udevadm WWN and scsi_id WWN for %s do not match" % scsi_disk)
+    # print("udevadm WWN is %s" % udev_wwn)
+    # print("scsi_id WWN is %s" % scsi_wwn)
+    # print("FAIL: wwn_of_disk() - udevadm WWN and scsi_id WWN for %s do not match" % scsi_disk)
     # return None
 
     return None
 
 
-def udev_wwn_of_disk(scsi_disk):
+def udev_wwn_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
         udev_wwn_of_disk(disk)
     Purpose
         Given an scsi_disk name. Eg. sda
     Parameter
         scsi_disk
     Returns
         wwid:       eg. 0x60a980003246694a412b45673342616e.
     """
     if not scsi_disk:
-        sts_print("FAIL: udev_wwn_of_disk() - requires scsi_disk parameter")
+        print("FAIL: udev_wwn_of_disk() - requires scsi_disk parameter")
         return None
 
     key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
 
     cmd = f"udevadm info --name={scsi_disk} --query=all"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        # sts_print("FAIL: udev_wwn_of_disk() - Could not query %s" % scsi_disk)
+        # print("FAIL: udev_wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
     lines = output.split("\n")
     for line in lines:
         m = re.search(key_regex, line)
         if m:
-            udev_wwn = m.group(1)
-            return udev_wwn
+            return m.group(1)
     return None
 
 
-def query_scsi_driver_info(driver):
+def query_scsi_driver_info(driver):  # noqa: ANN001, ANN201
     if not driver:
-        sts_print("FAIL: query_scsi_driver_info() - requires driver parameter")
+        print("FAIL: query_scsi_driver_info() - requires driver parameter")
         return None
 
     all_scsi_host_ids = get_hosts()
     if not all_scsi_host_ids:
-        sts_print("FAIL: query_scsi_driver_info() - Host does not have any SCSI host")
+        print("FAIL: query_scsi_driver_info() - Host does not have any SCSI host")
         return None
 
     driver_host_ids = []
     # Check which SCSI hosts are using the driver we want
     for host_id in all_scsi_host_ids:
         if scsi_driver_of_host_id(host_id) == driver:
             driver_host_ids.append(host_id)
 
     if not driver_host_ids:
-        sts_print(f"FAIL:  No SCSI disk found from driver {driver}")
+        print(f"FAIL:  No SCSI disk found from driver {driver}")
         return None
 
     scsi_driver_info = {"scsi_host": {}}
     for host_id in driver_host_ids:
         scsi_driver_info["scsi_host"][host_id] = query_scsi_host_info(host_id)
 
     scsi_driver_info["driver_name"] = driver
     # Add general driver info to this dict
     scsi_driver_info.update(linux.get_driver_info(driver))
 
     return scsi_driver_info
 
 
-def get_free_disks(
-    exclude_boot_device=True,
-    exclude_lvm_device=True,
-    exclude_mpath_device=True,
-    exclude_md_device=True,
-    filter_only=None,
+def get_free_disks(  # noqa: ANN201
+    exclude_boot_device=True,  # noqa: ANN001
+    exclude_lvm_device=True,  # noqa: ANN001
+    exclude_mpath_device=True,  # noqa: ANN001
+    exclude_md_device=True,  # noqa: ANN001
+    filter_only=None,  # noqa: ANN001
 ):
     """Return a dict of free SCSI devices.
     By default, it excludes devices used for boot, lvm or multipath
     Optional "filter_only" argument should be a dict. E.g. filter_only={'state': 'running'}.
     """
     all_scsi_disks = query_all_scsi_disks()
     if not all_scsi_disks:
@@ -718,46 +714,46 @@
             all_mp_info = None
 
     chosen_disks = {}
     for scsi_disk in list(all_scsi_disks.keys()):
         scsi_info = all_scsi_disks[scsi_disk]
         # Skip if mpath device is used for boot
         if boot_wwid == scsi_info["wwid"] and exclude_boot_device:
-            sts_print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for boot")
+            print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for boot")
             continue
 
         # Skip if disk is used by multipath
         if all_mp_info and scsi_info["wwid"] in list(all_mp_info["by_wwid"].keys()) and exclude_mpath_device:
-            sts_print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for mpath")
+            print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for mpath")
             continue
 
         # Skip if it is used by Soft RAID
         if md_devices and exclude_md_device:
             used_by_md = False
             for md_dev in md_devices:
                 storage_devs = md.md_get_storage_dev(md_dev)
                 if not storage_devs:
                     continue
                 for dev in storage_devs:
                     dev_wwid = wwid_of_disk(dev)
                     if not dev_wwid:
                         continue
                     if dev_wwid == scsi_info["wwid"]:
-                        sts_print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for md")
+                        print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for md")
                         used_by_md = True
                         continue
             if used_by_md:
                 continue
 
         # Skip if filter_only is specified
         filtered = False
         if filter_only is not None:
             for key in filter_only:
                 if scsi_info[key] != filter_only[key]:
-                    sts_print(
+                    print(
                         "DEBUG: get_free_disks() - filtered {} as {} is not {}".format(
                             scsi_info["name"],
                             key,
                             filter_only[key],
                         ),
                     )
                     filtered = True
@@ -767,21 +763,21 @@
 
         chosen_disks[scsi_info["name"]] = scsi_info
 
         # Skip if it is used by LVM
         if pvs and exclude_lvm_device:
             for pv in list(pvs.keys()):
                 if "/" + get_scsi_disk_name(scsi_disk) in pv:
-                    sts_print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for LVM")
+                    print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for LVM")
                     chosen_disks.pop(scsi_info["name"])
 
     return chosen_disks
 
 
-def scsi_device_2_scsi_name(scsi_device):
+def scsi_device_2_scsi_name(scsi_device):  # noqa: ANN001, ANN201
     """Convert an specific SCSI device to scsi_name
     Eg. /dev/sdap1 => sda.
     """
     scsi_dev_regex = r"/dev\/(sd.*)"
     m = re.match(scsi_dev_regex, scsi_device)
     if m:
         # remove partition if it has
@@ -790,15 +786,15 @@
         if m:
             device_name = m.group(1)
         return device_name
     # does not seem to be a valid SCSI device
     return None
 
 
-def disk_sys_trigger(scsi_disk, action):
+def disk_sys_trigger(scsi_disk, action):  # noqa: ANN001, ANN201
     """Usage
         disk_sys_trigger(scsi_disk, action)
     Purpose
         Bring disk online/offline, via
             /sys/block/sdX/device/state
         action could be 'UP|DOWN|other', for UP, we change it into 'running'.
         for DOWN, we change it into 'offline'.
@@ -807,100 +803,100 @@
         action         # 'UP|DOWN|other'
     Returns
         True               # got expected /sys/block/sdX/device/state
             or
         False.
     """
     if not scsi_disk or not action:
-        sts_print("FAIL: disk_sys_trigger() - requires scsi_disk and action parameters")
+        print("FAIL: disk_sys_trigger() - requires scsi_disk and action parameters")
         return False
 
     sys_path = f"/sys/block/{scsi_disk}/device/state"
     if not Path(sys_path).is_file():
-        sts_print(f"FAIL: No such file: {sys_path}")
+        print(f"FAIL: No such file: {sys_path}")
         return False
 
     if action == "UP":
         action = "running"
     if action == "DOWN":
         action = "offline"
 
     cmd = f"echo {action} > {sys_path}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
-        sts_print(f"FAIL: disk_sys_trigger() - Could not execute {cmd}")
+        print(f"FAIL: disk_sys_trigger() - Could not execute {cmd}")
         print(output)
         return None
 
     # cmd = "cat %s 2>/dev/null" % sys_path
     new_state = disk_sys_check(scsi_disk)
     if not new_state:
-        sts_print(f"FAIL: disk_sys_trigger() - Could not get state of {scsi_disk}")
+        print(f"FAIL: disk_sys_trigger() - Could not get state of {scsi_disk}")
         return False
 
     if action != new_state:
-        sts_print(f"FAIL: disk_sys_trigger() - Current state is '{new_state}' expected '{action}'")
+        print(f"FAIL: disk_sys_trigger() - Current state is '{new_state}' expected '{action}'")
         return False
 
     return True
 
 
-def disk_sys_check(scsi_disk):
+def disk_sys_check(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
         disk_sys_check(scsi_disk)
     Purpose
         Check state of specific disk
             /sys/block/sdX/device/state
     Parameter
         scsi_disk      # like 'sda'
     Returns
         running/offline       # got expected /sys/block/sdX/device/state
             or
         None.
     """
     if not scsi_disk:
-        sts_print("FAIL: disk_sys_check() - requires scsi_disk parameter")
+        print("FAIL: disk_sys_check() - requires scsi_disk parameter")
         return None
 
     sys_path = f"/sys/block/{scsi_disk}/device/state"
     if not Path(sys_path).is_file():
-        sts_print(f"FAIL: disk_sys_check() - No such file: {sys_path}")
+        print(f"FAIL: disk_sys_check() - No such file: {sys_path}")
         return None
 
     cmd = f"cat {sys_path} 2>/dev/null"
     state = run(cmd, capture_output=True, verbose=False).output
     if not state:
-        sts_print(f"FAIL: disk_sys_check() - Could not read from {sys_path}")
+        print(f"FAIL: disk_sys_check() - Could not read from {sys_path}")
         return None
 
     return state
 
 
-def timeout_of_disk(scsi_disk):
+def timeout_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
         timeout_of_disk(scsi_disk)
     Purpose
         Check timeout of specific disk
             /sys/block/sdX/device/timeout
     Parameter
         scsi_disk      # like 'sda'
     Returns
         timeout in seconds       # got expected /sys/block/sdX/device/timeout
             or
         None.
     """
     if not scsi_disk:
-        sts_print("FAIL: timeout_of_disk() - requires scsi_disk parameter")
+        print("FAIL: timeout_of_disk() - requires scsi_disk parameter")
         return None
 
     sys_path = f"/sys/block/{scsi_disk}/device/timeout"
     if not Path(sys_path).is_file():
-        sts_print(f"FAIL: timeout_of_disk() - No such file: {sys_path}")
+        print(f"FAIL: timeout_of_disk() - No such file: {sys_path}")
         return None
 
     cmd = f"cat {sys_path} 2>/dev/null"
     timeout = run(cmd, capture_output=True, verbose=False).output
     if not timeout:
-        sts_print(f"FAIL: timeout_of_disk() - Could not read from {sys_path}")
+        print(f"FAIL: timeout_of_disk() - Could not read from {sys_path}")
         return None
 
     return timeout
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi_debug.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """scsi_debug.py: Module to manipulate devices created by scsi_debug module."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 from sts import linux, mp
 from sts.scsi import get_scsi_name_by_vendor
-from sts.utils import sts_print
 from sts.utils.cmdline import run
 
 
-def scsi_debug_load_module(options=None):
+def scsi_debug_load_module(options=None):  # noqa: ANN001, ANN201
     module_cmd = "scsi_debug"
     if linux.is_module_loaded(module_cmd):
-        sts_print("WARN: scsi_debug_load_module() - Module is already loaded")
+        print("WARN: scsi_debug_load_module() - Module is already loaded")
         return True
 
     if options:
         module_cmd += f" {options}"
 
     if not linux.load_module(module_cmd):
-        sts_print(f"FAIL: scsi_debug_load_module() - Could not load {module_cmd}")
+        print(f"FAIL: scsi_debug_load_module() - Could not load {module_cmd}")
         return False
     # Wait a bit, for example for multipath to create the device
     linux.sleep(2)
     return True
 
 
-def scsi_debug_unload_module():
+def scsi_debug_unload_module():  # noqa: ANN201
     module_name = "scsi_debug"
     if not linux.is_module_loaded(module_name):
         # Module is not loaded, return success
         return True
 
     if mp.is_multipathd_running():
         mpaths = mp.mpath_names_of_vendor("Linux")
         for mpath in mpaths:
             mp.remove_mpath(mpath)
             # Wait a bit, for example for multipath to remove the device
             linux.sleep(2)
 
     if not linux.unload_module(module_name):
-        sts_print(f"FAIL: scsi_debug_load_module() - Could not unload {module_name}")
+        print(f"FAIL: scsi_debug_load_module() - Could not unload {module_name}")
         return False
     return True
 
 
-def get_scsi_debug_devices():
+def get_scsi_debug_devices():  # noqa: ANN201
     """Return a list of scsi_debug devices."""
     module_name = "scsi_debug"
     vendor = "Linux"
     if not linux.is_module_loaded(module_name):
         return None
 
     mpaths = mp.mpath_names_of_vendor(vendor)
@@ -59,33 +58,33 @@
     scsi_devices = get_scsi_name_by_vendor(vendor)
     if scsi_devices:
         return scsi_devices
 
     return None
 
 
-def scsi_debug_set_param(param, value):
+def scsi_debug_set_param(param, value):  # noqa: ANN001, ANN201
     """Set specific value to scsi debug parameter."""
     if param is None or value is None:
-        sts_print("FAIL: scsi_debug_set_param() - requires param_name and value")
+        print("FAIL: scsi_debug_set_param() - requires param_name and value")
         return False
 
     if (
         run(
             f"echo '{value}' > /sys/bus/pseudo/drivers/scsi_debug/{param}",
             verbose=False,
         )
         != 0
     ):
-        sts_print(f"FAIL: scsi_debug_set_param() - Could not set {param} with value {value}")
+        print(f"FAIL: scsi_debug_set_param() - Could not set {param} with value {value}")
         return False
     return True
 
 
-def scsi_debug_insert_failure(every_nth, opts):
+def scsi_debug_insert_failure(every_nth, opts):  # noqa: ANN001, ANN201
     """Purpose:
     Enable/Disable failure on scsi_debug device
     Parameter:
     A dictionary with all option to be set
     The supported parameters are defined at: http://sg.danny.cz/sg/sdebug26.html
     opts: 1 - "noisy"
     2-"medium error"
@@ -99,35 +98,35 @@
     """
     if not every_nth:
         every_nth = 0
     if not opts:
         opts = 0
 
     if not scsi_debug_set_param("every_nth", every_nth):
-        sts_print(f"FAIL: scsi_debug_insert_failure() - Could not set every_nth with value: {every_nth}")
+        print(f"FAIL: scsi_debug_insert_failure() - Could not set every_nth with value: {every_nth}")
         return False
     if not scsi_debug_set_param("opts", opts):
-        sts_print(f"FAIL: scsi_debug_insert_failure() - Could not set opts with value: {opts}")
+        print(f"FAIL: scsi_debug_insert_failure() - Could not set opts with value: {opts}")
         return False
     return True
 
 
-def self_test():
+def self_test():  # noqa: ANN201
     if not scsi_debug_load_module():
-        sts_print("FAIL: self_test() - Could not load the module")
+        print("FAIL: self_test() - Could not load the module")
         return False
 
     if not get_scsi_debug_devices():
-        sts_print("FAIL: self_test() - Could not find any scsi debug device")
+        print("FAIL: self_test() - Could not find any scsi debug device")
         scsi_debug_unload_module()
         return False
 
     if not scsi_debug_insert_failure(0, 0):
-        sts_print("FAIL: self_test() - Could not set parameters")
+        print("FAIL: self_test() - Could not set parameters")
         scsi_debug_unload_module()
         return False
 
     if not scsi_debug_unload_module():
-        sts_print("FAIL: self_test() - Could not unload the module")
+        print("FAIL: self_test() - Could not unload the module")
         return False
 
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/vdo.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import stat
 from difflib import context_diff
 from pathlib import Path
+from typing import Dict, List, Union
 
 from sts import linux
-from sts.utils import sts_print
 from sts.utils.atomic_run import atomic_run
 from sts.utils.cli_tools import (
     FailedCheckExceptionError,
     Wrapper,
     WrongArgumentExceptionError,
     WrongCommandExceptionError,
 )
 from sts.utils.cmdline import run, run_ret_out
 
 
-def restart_modify(vdo_object, vdo_name, errors):
+def restart_modify(vdo_object, vdo_name, errors):  # noqa: ANN001, ANN201
     # sometimes VDO needs to be restarted for changes to take effect
     print("Restarting VDO for changes to take effect.")
     commands = [
         {
             "message": "Stopping VDO to apply modification.",
             "command": vdo_object.stop,
             "expected_out": ["Stopping VDO"],
@@ -34,30 +34,30 @@
             "expected_out": ["Starting VDO", "VDO instance", "is ready"],
         },
     ]
     for command in commands:
         atomic_run(name=vdo_name, errors=errors, expected_ret=0, **command)
 
 
-def report_modify_difference(errors, status_old, status_new, changed_var, changed_argument):
+def report_modify_difference(errors, status_old, status_new, changed_var, changed_argument):  # noqa: ANN001, ANN201
     status_old = [x for x in status_old.splitlines() if changed_var in x]
     status_new = [x for x in status_new.splitlines() if changed_var in x]
     print(f"Before: {', '.join(status_old)}")
     print(f"After:  {', '.join(status_new)}")
     diff = list(context_diff(status_old, status_new))
     difference = "\n".join([x for x in diff if x.startswith("!")])
 
     if difference == "":
         error = f"WARN: Modifying VDO to {changed_argument} did nothing."
         print(error)
         errors.append(error)
 
 
-def minimum_slab_size(device, default_to_2g=True):
-    def _get_raid_device(device):
+def minimum_slab_size(device, default_to_2g=True):  # noqa: ANN001, ANN201
+    def _get_raid_device(device):  # noqa: ANN001, ANN202
         device_name = device.split("/").pop()
         ret, device_link = run_ret_out(cmd=f"ls -al /dev/md | grep {device_name}", return_output=True)
         if ret or device_link is None:
             print(f"WARN: Device {device_name} not found in /dev/md.")
             return None
         return device_link.split("../").pop()  # raid device
 
@@ -74,15 +74,15 @@
     if minimum_size < 128:
         minimum_size = 128
     if default_to_2g and minimum_size < 2048:
         return "2G"
     return str(minimum_size) + "M"
 
 
-def maximum_logical_size():
+def maximum_logical_size():  # noqa: ANN201
     """Returns maximum logical size based on memory.
 
     Returns:
       string max_size.
     """
     good_size = 4096
     memory = linux.get_memory()["mem"]["free"]
@@ -90,29 +90,28 @@
     if memory < 10000:
         size = 2 ** (((4096.0 / 10000) * float(memory)).__int__().bit_length() - 1)
         if size > good_size:
             size = good_size
     return size
 
 
-def is_block_device(device):
+def is_block_device(device):  # noqa: ANN001, ANN201
     try:
         mode = Path(device).stat().st_mode
     except OSError:
-        msg = f"Device {device} does not exist."
-        return msg
+        return f"Device {device} does not exist."
 
     if not stat.S_ISBLK(mode):
         msg = f"Device {device} is not block device, aborting."
         print(msg)
         return msg
     return True
 
 
-def get_underlying_device(name, conf_file="/etc/vdoconf.yml"):
+def get_underlying_device(name, conf_file="/etc/vdoconf.yml"):  # noqa: ANN001, ANN201
     vdo = VDO(disable_check=True)
     ret, data = vdo.status(name=name, return_output=True, verbosity=False, conf_file=conf_file)
     if ret != 0:
         msg = f"FAIL: Could not get status of VDO device '{name}'."
         print(msg)
         return None
     device = None
@@ -155,28 +154,28 @@
         device = f"/dev/mapper/{dev_name}"
     else:
         device = f"/dev/{device}"
 
     return device
 
 
-def get_replace_dict():
+def get_replace_dict():  # noqa: ANN201
     """Returns dict of keys to replace from fmf to sts.vdo.VDO.
 
     Returns:
       dict.
     """
     return {"vdo_name": "name"}
 
 
 class VDO(Wrapper):
-    def __init__(self, disable_check=False):
+    def __init__(self, disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
 
-        self.commands = {
+        self.commands: Dict[str, Union[str, List[str]]] = {
             "create": "create",
             "remove": "remove",
             "start": "start",
             "stop": "stop",
             "activate": "activate",
             "deactivate": "deactivate",
             "status": "status",
@@ -230,15 +229,15 @@
             "force_rebuild": [["start"], " --forceRebuild"],
             "force": [["stop", "remove", "create"], " --force"],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
-    def _check_size_format(size, return_size=False):
+    def _check_size_format(size, return_size=False):  # noqa: ANN001, ANN205
         # check if requested size format is in supported formats and the rest is numbers
         # FIXME: Is KiB and KB valid too?
         size = size.strip("'")
         try:
             if size[-3:] in ["KiB", "MiB", "GiB", "TiB"] and isinstance(int(size[:-3]), int):
                 if return_size:
                     return True, [size[:-3], size[-3:-2]]
@@ -257,43 +256,43 @@
                     return True, [size, "M"]
                 return True
         except ValueError:
             pass
         return False, []
 
     @staticmethod
-    def _is_positive_int(value):
+    def _is_positive_int(value):  # noqa: ANN001, ANN205
         try:
             port = int(value)
             if port < 1:
                 raise ValueError  # noqaTRY301
         except ValueError:
             return False
         return True
 
-    def _check(self, cmd):
+    def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check:
             # Do not check if checking is disabled
             return True
 
         if self._get_arg("all") in cmd and self._get_arg("name") in cmd:
-            sts_print("WARN: Use either 'name' or 'all', not both.")
+            print("WARN: Use either 'name' or 'all', not both.")
             raise FailedCheckExceptionError
 
         if self._get_arg("conf_file") in cmd:
             _file = self._get_value(cmd, self._get_arg("conf_file"))
             if not Path(_file).is_file():
-                sts_print(f"WARN: Config file {_file} is not a regular file.")
+                print(f"WARN: Config file {_file} is not a regular file.")
                 raise FailedCheckExceptionError(self._get_arg("conf_file"))
 
         if self._get_arg("log_file") in cmd:
             _file = self._get_value(cmd, self._get_arg("log_file"))
             f = Path(_file)
             if not f.is_file() and stat.S_ISBLK(f.stat().st_mode):
-                sts_print(f"WARN: Path {_file} exists and is not a regular file.")
+                print(f"WARN: Path {_file} exists and is not a regular file.")
                 raise FailedCheckExceptionError(self._get_arg("log_file"))
 
         if self._get_arg("name") in cmd:
             # FIXME: Check if VDO already exists
             pass
 
         for arg in [
@@ -302,64 +301,64 @@
             "deduplication",
             "emulate512",
             "sparse_index",
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
                 if _value not in ["enabled", "disabled"]:
-                    sts_print(f"WARN: {arg} value must be either 'enabled' or 'disabled'.")
+                    print(f"WARN: {arg} value must be either 'enabled' or 'disabled'.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
 
         for arg in [
             "logical_size",
             "slab_size",
             "block_map_cache_size",
             "max_discard_size",
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
                 ret, _ = self._check_size_format(_value, return_size=True)
                 if not ret:
-                    sts_print(f"WARN: VDO {' '.join(arg.split('_'))} value {_value} is in unknown format.")
+                    print(f"WARN: VDO {' '.join(arg.split('_'))} value {_value} is in unknown format.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
                 if arg == "slab_size":  # noqaSIM114
                     pass
                     # FIXME: Check if size is power of 2 between 128M and 32G
                 elif arg == "block_map_cache_size":
                     pass
                     # FIXME: Check if size is multiple of 4096
 
         if self._get_arg("index_mem") in cmd:
             _value = self._get_value(cmd, self._get_arg("index_mem"), return_type=float)
             if not (_value in [0, 0.25, 0.5, 0.75] or self._is_positive_int(_value)):
-                sts_print(f"WARN: Albireo mem value {_value} is not a 0, 0.25, 0.5, 0.75 or positive int.")
+                print(f"WARN: Albireo mem value {_value} is not a 0, 0.25, 0.5, 0.75 or positive int.")
                 raise FailedCheckExceptionError(self._get_arg("index_mem"))
 
         if self._get_arg("log_level") in cmd:
             _value = self._get_value(cmd, self._get_arg("log_level"))
             possible_values = [
                 "critical",
                 "error",
                 "warning",
                 "notice",
                 "info",
                 "debug",
             ]
             if _value not in possible_values:
-                sts_print(f"WARN: Unknown vdo log level value, must be one of {possible_values}.")
+                print(f"WARN: Unknown vdo log level value, must be one of {possible_values}.")
                 raise FailedCheckExceptionError(self._get_arg("log_level"))
 
         if self._get_arg("device") in cmd:
             _value = self._get_value(cmd, self._get_arg("device"))
             # FIXME: Check if device exists
 
         if self._get_arg("block_map_period") in cmd:
             _value = self._get_value(cmd, self._get_arg("block_map_period"))
             if not self._is_positive_int(_value):
-                sts_print("WARN: Block map period value must be a positive integer.")
+                print("WARN: Block map period value must be a positive integer.")
                 raise FailedCheckExceptionError(self._get_arg("block_map_period"))
             # FIXME: Can this be higher than 16380?
 
         for arg in [
             "ack_threads",
             "bio_rotation_interval",
             "bio_threads",
@@ -367,190 +366,190 @@
             "hash_zone_threads",
             "logical_threads",
             "physical_threads",
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
                 if not self._is_positive_int(_value):
-                    sts_print(f"WARN: VDO {' '.join(arg.split('_'))} value must be a positive integer.")
+                    print(f"WARN: VDO {' '.join(arg.split('_'))} value must be a positive integer.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
                     # FIXME: Is 0 valid?
 
         if self._get_arg("write_policy") in cmd:
             _value = self._get_value(cmd, self._get_arg("write_policy"))
             if _value not in ["sync", "async"]:
-                sts_print("WARN: VDO read cache value must be either 'sync' or 'async'.")
+                print("WARN: VDO read cache value must be either 'sync' or 'async'.")
                 raise FailedCheckExceptionError(self._get_arg("write_policy"))
 
         if self._get_arg("force_rebuild") in cmd and self._get_arg("upgrade") in cmd:
-            sts_print("WARN: Cannot use both force_rebuild and upgrade when starting VDO volume.")
+            print("WARN: Cannot use both force_rebuild and upgrade when starting VDO volume.")
             raise FailedCheckExceptionError
 
         return True
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):
+    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
 
         ret_fail = False
         if return_output:
             ret_fail = (False, None)
 
         try:
             command = self._add_command(cmd)
             command = self._add_arguments(command, **kwargs)
 
         except WrongCommandExceptionError as e:
-            sts_print(f"WARN: Given command '{e.command}' is not allowed in this VDO version.")
+            print(f"WARN: Given command '{e.command}' is not allowed in this VDO version.")
             return ret_fail
         except WrongArgumentExceptionError as e:
             message = f"WARN: Given argument '{e.argument}' is not allowed for given command."
             if e.command:
                 message = message[:-1] + " '" + e.command + "'."
             if e.arguments:
                 message += f"\nPlease use only these: {', '.join(e.arguments)}."
-            sts_print(message)
+            print(message)
             return ret_fail
 
         cmd = "vdo " + command
 
         try:
             self._check(cmd)
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
-            sts_print(f"WARN: Failed checking on argument {e.argument}")
+            print(f"WARN: Failed checking on argument {e.argument}")
             return ret_fail
 
         if return_output:
             ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
-                sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
         ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
-    def help():  # noqa: A003
+    def help():  # noqa: A003, ANN205
         if run("vdo --help", verbose=True) != 0:
-            sts_print("WARN: Running command: 'vdo --help' failed.")
+            print("WARN: Running command: 'vdo --help' failed.")
             return False
         return True
 
-    def create(self, **kwargs):
+    def create(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("create", **kwargs)
 
-    def remove(self, force=True, **kwargs):
+    def remove(self, force=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run("remove", force=force, **kwargs)
 
-    def start(self, **kwargs):
+    def start(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("start", **kwargs)
 
-    def stop(self, force=True, **kwargs):
+    def stop(self, force=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run("stop", force=force, **kwargs)
 
-    def activate(self, **kwargs):
+    def activate(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("activate", **kwargs)
 
-    def deactivate(self, **kwargs):
+    def deactivate(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("deactivate", **kwargs)
 
-    def status(self, **kwargs):
+    def status(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("status", **kwargs)
 
-    def list(self, **kwargs):  # noqa: A003
+    def list(self, **kwargs):  # noqa: A003, ANN003, ANN201
         return self._run("list", **kwargs)
 
-    def modify(self, **kwargs):
+    def modify(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("modify", **kwargs)
 
-    def change_write_policy(self, **kwargs):
+    def change_write_policy(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("change_write_policy", **kwargs)
 
-    def deduplication(self, enable=True, **kwargs):
+    def deduplication(self, enable=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run("enable_deduplication", **kwargs) if enable else self._run("disable_deduplication", **kwargs)
 
-    def compression(self, enable=True, **kwargs):
+    def compression(self, enable=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
         return self._run("enable_compression", **kwargs) if enable else self._run("disable_compression", **kwargs)
 
-    def grow(self, grow_type=None, **kwargs):
+    def grow(self, grow_type=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         if grow_type.upper() not in ["LOGICAL", "PHYSICAL"]:
-            sts_print("WARN: Please specify either 'logical' or 'physical' type for growing VDO.")
+            print("WARN: Please specify either 'logical' or 'physical' type for growing VDO.")
             if kwargs["return_output"]:
                 return False, None
             return False
 
         if grow_type.upper() == "LOGICAL":
             ret = self._run("grow_logical", **kwargs)
         else:
             ret = self._run("grow_physical", **kwargs)
         return ret
 
-    def print_config_file(self, **kwargs):
+    def print_config_file(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("print_config_file", **kwargs)
 
 
 class VDOStats:
-    def __init__(self, disable_check=False):
+    def __init__(self, disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
         self.command = "vdostats"
         self.arguments = {
             "help": " --help",
             "all": " --all",
             "human_readable": " --human-readable",
             "si": " --si",
             "verbose": " --verbose",
             "version": " --version",
         }
 
-    def _get_arg(self, name):
+    def _get_arg(self, name):  # noqa: ANN001, ANN202
         return self.arguments[name]
 
-    def _get_possible_arguments(self):
+    def _get_possible_arguments(self):  # noqa: ANN202
         # Returns possible arguments
         return list(self.arguments.keys())
 
-    def _add_argument(self, arg, command):
+    def _add_argument(self, arg, command):  # noqa: ANN001, ANN202
         # Checks if given argument is allowed and adds it to cmd string
         if arg not in self.arguments:
             return None
         argument = self._get_arg(arg)
         command += argument
         return command
 
-    def _add_arguments(self, cmd, **kwargs):
+    def _add_arguments(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         command = cmd
         for kwarg in kwargs:
             command = self._add_argument(kwarg, command)
             if command is None:
                 args = self._get_possible_arguments()
-                sts_print(f"WARN: Unknown argument '{kwarg}', please use only these: {args}.")
+                print(f"WARN: Unknown argument '{kwarg}', please use only these: {args}.")
                 return None
         return command
 
-    def _check(self, cmd):
+    def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check:
             # Do not check if checking is disabled
             return True
 
         # check if specified devices are block devices
         for block in cmd.split():
             file = Path(block)
             if (
                 (block not in list(self.arguments.values()) and block != self.command)
                 and file.exists()
                 and not stat.S_ISBLK(file.stat().st_mode)
             ):
-                sts_print(f"WARN: Device {block} is not a block device.")
+                print(f"WARN: Device {block} is not a block device.")
                 return False
 
         return True
 
-    def _run(self, **kwargs):
+    def _run(self, **kwargs):  # noqa: ANN003, ANN202
         # Constructs the command to run and runs it
         cmd = self.command
 
         if "devices" in kwargs:
             devices = kwargs.pop("devices")
             if isinstance(devices, list):
                 for device in devices:
@@ -563,25 +562,25 @@
             return False
 
         if not self._check(cmd):
             # Requested command did not pass checking, reason was already written by _check()
             return False
 
         if run(cmd, verbose=True).returncode != 0:
-            sts_print(f"WARN: Running command: '{cmd}' failed.")
+            print(f"WARN: Running command: '{cmd}' failed.")
             return False
         return True
 
-    def help(self):  # noqa: A003
+    def help(self):  # noqa: A003, ANN201
         if not self._run(help=True):
             return False
         return True
 
-    def version(self):
+    def version(self):  # noqa: ANN201
         if not self._run(version=True):
             return False
         return True
 
-    def stats(self, **kwargs):
+    def stats(self, **kwargs):  # noqa: ANN003, ANN201
         if not self._run(**kwargs):
             return False
         return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/atomic_run.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/atomic_run.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,74 +8,74 @@
 from time import localtime, strftime
 
 from sts import linux
 
 
 class Variables:
     # global variables persistent across libraries and instances
-    def __init__(self):
+    def __init__(self) -> None:
         pass
 
     logging_level = 20
     tests_to_run = "*"
     tier_to_test = 3
     no_run = False
     bz: list  # list of BZ numbers
 
 
 class Logger:
-    def __init__(self):
+    def __init__(self) -> None:
         pass
 
-    def debug(self, message):
+    def debug(self, message):  # noqa: ANN001, ANN201
         if Variables.logging_level < 20:
             if message.startswith("\n"):
                 print(f"\nDEBUG: [{self.get_time()}] " + message[1:])
             else:
                 print(f"DEBUG: [{self.get_time()}] " + message)
 
-    def info(self, message):
+    def info(self, message):  # noqa: ANN001, ANN201
         if message.startswith("\n"):
             print(f"\nINFO: [{self.get_time()}] " + message[1:])
         else:
             print(f"INFO: [{self.get_time()}] " + message)
 
-    def warn(self, message):
+    def warn(self, message):  # noqa: ANN001, ANN201
         if message.startswith("\n"):
             print(f"\nWARN: [{self.get_time()}] " + message[1:])
         else:
             print(f"WARN: [{self.get_time()}] " + message)
 
-    def fail(self, message):
+    def fail(self, message):  # noqa: ANN001, ANN201
         if message.startswith("\n"):
             print(f"\nFAIL: [{self.get_time()}] " + message[1:])
         else:
             print(f"FAIL: [{self.get_time()}] " + message)
 
     @staticmethod
-    def get_time():
+    def get_time():  # noqa: ANN205
         return strftime("%Y-%m-%d %H:%M:%S", localtime())
 
 
-def atomic_run(
-    message,
-    success=True,
-    return_output=False,
-    expected_ret=None,
-    expected_out=None,
-    **kwargs,
+def atomic_run(  # noqa: ANN201
+    message,  # noqa: ANN001
+    success=True,  # noqa: ANN001
+    return_output=False,  # noqa: ANN001
+    expected_ret=None,  # noqa: ANN001
+    expected_out=None,  # noqa: ANN001
+    **kwargs,  # noqa: ANN003
 ):
-    def log_error(error_message, errors_list):
+    def log_error(error_message, errors_list):  # noqa: ANN001, ANN202
         logger.fail(error_message)
         if isinstance(errors_list, list):
             errors_list.append(error_message)
         else:
             logger.fail("atomic_run got 'errors' value that is not list.")
 
-    def is_expected_out_in_out(out, exp_out):
+    def is_expected_out_in_out(out, exp_out):  # noqa: ANN001, ANN202
         out = out.replace("'", "").replace('"', "")
         if isinstance(exp_out, list):
             # check all from list are in output
             return bool(all(e in out for e in exp_out))
         if str(exp_out) in out:
             return True
         return False
@@ -157,15 +157,15 @@
         )
 
     if return_output:
         return ret, output
     return ret
 
 
-def parse_ret(errors):
+def parse_ret(errors):  # noqa: ANN001, ANN201
     if not errors:
         return 0
     # write errors to file for parsing at the end
     try:
         test_name = os.environ["FMF_NAME"]
     except KeyError:
         print("FAIL: Could not get test name though os.environ. Not running error parsing.")
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/beaker.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,83 +6,72 @@
 import os
 import re  # regex
 
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.restraint import is_restraint_job, log_submit
 
 
-def sts_print(string):
-    module_name = __name__
-    string = re.sub("DEBUG:", "DEBUG:(" + module_name + ") ", string)
-    string = re.sub("FAIL:", "FAIL:(" + module_name + ") ", string)
-    string = re.sub("FATAL:", "FATAL:(" + module_name + ") ", string)
-    string = re.sub("WARN:", "WARN:(" + module_name + ") ", string)
-    print(string)
-    if "FATAL:" in string:
-        raise RuntimeError(string)
-
-
-def get_task_timeout(task_id):
+def get_task_timeout(task_id):  # noqa: ANN001, ANN201
     """Get how much time the task still has
     Parameter:
     task_id:          Beaker Task id
     Return:
     None:             In case of some problem
     or
     int(value):       The remaining time in seconds.
     """
     if not is_restraint_job():
         return None
 
     if task_id is None:
-        sts_print("FAIL: beaker get_task_timeout() - requires task_id as parameter")
+        print("FAIL: beaker get_task_timeout() - requires task_id as parameter")
         return None
 
     cmd = f"bkr watchdog-show {task_id}"
     ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
-        sts_print("FAIL: beaker get_task_timeout() - Could not get beaker kill time")
+        print("FAIL: beaker get_task_timeout() - Could not get beaker kill time")
         print(output)
         return None
 
     output_regex = re.compile(r"%s: (\d+)" % task_id)
     m = output_regex.match(output)
     if m:
         return int(m.group(1))
-    sts_print("FAIL: beaker get_task_timeout() - Could not parse output:")
+    print("FAIL: beaker get_task_timeout() - Could not parse output:")
     print(output)
     return None
 
 
-def get_task_status(task_id):
+def get_task_status(task_id):  # noqa: ANN001, ANN201
     """Requires beaker-client package installed and configured."""
     if not is_restraint_job():
         return None
 
     if not task_id:
-        sts_print("FAIL: get_task_status() - requires task id")
+        print("FAIL: get_task_status() - requires task id")
         return None
 
     cmd = f"bkr job-results --prettyxml T:{task_id}"
     ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
-        sts_print(f"FAIL: get_task_status() - Could not get beaker task result for T:{task_id}")
+        print(f"FAIL: get_task_status() - Could not get beaker task result for T:{task_id}")
         print(output)
         return None
 
     lines = output.split("\n")
     status_regex = re.compile(r"<task.*status=\"(\S+)\"")
     for line in lines:
         m = status_regex.match(line)
         if m:
             return m.group(1)
     return None
 
 
-def console_log_check(error_mgs):
+def console_log_check(error_mgs):  # noqa: ANN001, ANN201
     """Checks for error messages on console log ("Call Trace and segfault")."""
     error = 0
     console_log_file = "/root/console.log"
     prev_console_log_file = "/root/console.log.prev"
     new_console_log_file = "/root/console.log.new"
 
     if not is_beaker_job():
@@ -121,11 +110,11 @@
     if error:
         return False
 
     print(f"PASS: No errors on {console_log_file} have been found.")
     return True
 
 
-def is_beaker_job():
+def is_beaker_job():  # noqa: ANN201
     """Checks if it is beaker job."""
     need_env = ["BEAKER", "BEAKER_RECIPE_ID", "LAB_CONTROLLER"]
     return all(not var not in os.environ for var in need_env)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cli_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,123 +1,121 @@
 """cli_tools.py: Module to provide tools of wrapping command line tools for further usage."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
-from sts.utils import sts_print
-
 
 class WrongCommandExceptionError(Exception):
-    def __init__(self, cmd):
+    def __init__(self, cmd) -> None:  # noqa: ANN001
         self.command = cmd
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return repr(WrongCommandExceptionError.__name__ + ", caused by " + repr(self.command))
 
 
 class WrongArgumentExceptionError(Exception):
-    def __init__(self, arg, cmd=None, args=None):
+    def __init__(self, arg, cmd=None, args=None) -> None:  # noqa: ANN001
         self.argument = arg
         self.command = cmd
         self.arguments = args
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return repr(WrongArgumentExceptionError.__name__ + ", caused by " + repr(self.argument))
 
 
 class FailedCheckExceptionError(Exception):
-    def __init__(self, arg=None):
+    def __init__(self, arg=None) -> None:  # noqa: ANN001
         self.argument = arg
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         message = repr(FailedCheckExceptionError.__name__)
         if self.argument:
             message += ", caused by " + repr(self.argument)
         return message
 
 
 class Wrapper:
-    def __init__(self, commands, arguments, disable_check):
+    def __init__(self, commands, arguments, disable_check) -> None:  # noqa: ANN001
         self.commands = commands
         self.arguments = arguments
         self.disable_check = disable_check
 
-    def _add_command(self, cmd):
+    def _add_command(self, cmd):  # noqa: ANN001, ANN202
         # Checks if given command is provided by CLI and returns its correct syntax
         if cmd in self.commands:
             return self.commands[cmd]
         raise WrongCommandExceptionError(cmd)
 
-    def _get_arg(self, name):
+    def _get_arg(self, name):  # noqa: ANN001, ANN202
         if not self.disable_check:
             if name in self.arguments:
                 return self.arguments[name][1]
             raise WrongArgumentExceptionError(name)
         return self.arguments[name][1]
 
-    def _get_cmd(self, name):
+    def _get_cmd(self, name):  # noqa: ANN001, ANN202
         if self.disable_check:
             return self.commands["all"]
         if name in self.arguments:
             return self.arguments[name][0]
         raise WrongCommandExceptionError(name)
 
     @staticmethod
-    def _get_value(string, command, return_type=str):
+    def _get_value(string, command, return_type=str):  # noqa: ANN001, ANN205
         _value = string.split(command)[1].split()[0]
         try:
             value = return_type(_value)
         except ValueError as e:
-            sts_print(f"WARN: Got ValueError: {e}.")
+            print(f"WARN: Got ValueError: {e}.")
             return None
         return value
 
-    def _get_possible_arguments(self, command=None):
+    def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
         # Returns possible arguments for said command if specified
         args = []
         if command:
             for key in list(self.arguments.keys()):
                 if list(self.commands.keys())[list(self.commands.values()).index(command)] in self._get_cmd(key):
                     args.append(key)
         else:
             args = list(self.arguments.keys())
         return args
 
     @staticmethod
-    def _add_value(value, command, argument):
+    def _add_value(value, command, argument):  # noqa: ANN001, ANN205
         if argument[-1:] in ["=", "&"]:
             if argument[-1:] == "&":
                 argument = argument[:-1] + " "
             if isinstance(value, list):
                 # allows to use repeatable arguments as a list of values
                 for val in value:
                     command += argument + "'" + str(val) + "'"
             else:
                 command += argument + "'" + str(value) + "'"
         else:
             command += argument
         return command
 
-    def _check_allowed_argument(self, arg, command):
+    def _check_allowed_argument(self, arg, command):  # noqa: ANN001, ANN202
         if arg not in self.arguments and not self.disable_check:
             raise WrongArgumentExceptionError(arg)
         cmd = command.split()[0]
         args = self._get_possible_arguments(cmd)
         if arg not in args:
             raise WrongArgumentExceptionError(arg, cmd, args)
 
-    def _add_argument(self, arg, value, command):
+    def _add_argument(self, arg, value, command):  # noqa: ANN001, ANN202
         # Checks if given argument is allowed for given command and adds it to cmd string
         self._check_allowed_argument(arg, command)
         return self._add_value(value, command, self._get_arg(arg))
 
-    def _add_arguments(self, cmd, **kwargs):
+    def _add_arguments(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         command = cmd
         for kwarg in kwargs:
             # skip adding this argument if the value is False
             if kwargs[kwarg] is False:
                 continue
             command = self._add_argument(kwarg, kwargs[kwarg], command)
         return command
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,18 @@
     Derived from subprocess.run()
 
     Attributes:
       returncode: The exit code of the process, negative for signals.
       output: stdout and stderr combined (None if not captured).
     """
 
-    def __init__(self, returncode, output=None):
+    def __init__(self, returncode: int, output: Optional[str] = None) -> None:
         self.returncode = returncode
         self.output = output
 
-    def __repr__(self):
-        args = [f"{self.returncode=}"]
-        if self.output is not None:
-            args.append(f"{self.output=}")
-
 
 def run(
     cmd: str,
     timeout: Optional[int] = None,
     capture_output: bool = False,
     use_popen: bool = False,
     verbose: bool = True,
@@ -76,15 +71,15 @@
                     output_str += output_line
                     if verbose:
                         print(output_line.rstrip())
 
             process.wait(timeout=timeout)
             retcode = process.poll()
             return StsCompletedProcess(
-                returncode=retcode,
+                returncode=retcode,  # type: ignore [arg-type]
                 output=output_str.rstrip() if output_str else None,
             )
         except subprocess.TimeoutExpired:
             if verbose:
                 print("WARN: Command timed out")
             return StsCompletedProcess(returncode=124, output=output_str if output_str else None)
 
@@ -106,15 +101,15 @@
 
         if not capture_output and verbose and ret_out.output:
             print(ret_out.output)
 
         return ret_out
 
     except subprocess.TimeoutExpired as e:
-        return StsCompletedProcess(returncode=124, output=e.stdout if e.stdout else None)
+        return StsCompletedProcess(returncode=124, output=e.output if e.output else None)
 
 
 def run_ret_out(
     cmd: str,
     timeout: Optional[int] = None,
     return_output: bool = False,
     use_popen: bool = False,
@@ -129,16 +124,16 @@
         timeout=timeout,
         use_popen=use_popen,
         verbose=verbose,
         capture_output=bool(return_output),
     )
 
     if return_output:
-        return completed_command.returncode, completed_command.output
+        return completed_command.returncode, completed_command.output  # type: ignore [return-value]
 
     return completed_command.returncode
 
 
-def exists(cmd):
+def exists(cmd):  # noqa: ANN001, ANN201
     if not which(str(cmd)):
         return False
     return True
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/logchecker.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Usage example:
         logging_start = journalctl_timestamp()
         failure_logs = run(f"journalctl -S {logging_start}, capture_output=True).output"
     """
     return datetime.now().isoformat(sep=" ", timespec="minutes")  # noqa: DTZ005 <- We want local timezone.
 
 
-def check_all():
+def check_all():  # noqa: ANN201
     """Check for error on the system
     Returns:
     Boolean:
     True is no error was found
     False if some error was found.
     """
     print("INFO: Checking for error on the system")
@@ -68,15 +68,15 @@
                 return False
             restraint.log_submit(sos_file)
         return False
 
     return True
 
 
-def abrt_check():
+def abrt_check():  # noqa: ANN201
     """Check if abrtd found any issue
     Returns:
     Boolean:
     True no error was found
     False some error was found.
     """
     print("INFO: Checking abrt for error")
@@ -119,15 +119,15 @@
         print("FAIL: Found abrt error")
         return False
 
     print("PASS: no Abrt entry has been found.")
     return True
 
 
-def kernel_check():
+def kernel_check():  # noqa: ANN201
     """Check if kernel got tainted.
     It checks /proc/sys/kernel/tainted which returns a bitmask.
     The values are defined in the kernel source file include/linux/kernel.h,
     and explained in kernel/panic.c
     cd /usr/src/kernels/`uname -r`/
     Sources are provided by kernel-devel
     Returns:
@@ -202,15 +202,15 @@
     run(f"echo {tainted} > {previous_tainted_file}", verbose=False)
     if found_issue:
         return False
 
     return True
 
 
-def _date2num(date):
+def _date2num(date):  # noqa: ANN001, ANN202
     date_map = {
         "Jan": "1",
         "Feb": "2",
         "Mar": "3",
         "Apr": "4",
         "May": "5",
         "Jun": "6",
@@ -232,15 +232,15 @@
 
     hour = m.group(3)
     hour = hour.replace(":", "")
 
     return month + day + hour
 
 
-def messages_dump_check():
+def messages_dump_check():  # noqa: ANN201
     previous_time_file = "/tmp/previous-dump-check"
 
     log_msg_file = "/var/log/messages"
     if not Path(log_msg_file).is_file():
         print(f"WARN: Could not open {log_msg_file}")
         return True
 
@@ -272,15 +272,15 @@
         print(m.group(1))
         # TODO
 
     print("PASS: No recent dump messages has been found.")
     return True
 
 
-def dmesg_check():
+def dmesg_check():  # noqa: ANN201
     """Check for error messages on dmesg ("Call Trace and segfault")."""
     print("INFO: Checking for errors on dmesg.")
     error = 0
     for msg in error_mgs:
         output = run(f"dmesg | grep -i '{msg}'", capture_output=True).output
         if output:
             print(f"FAIL: found {msg} on dmesg")
@@ -292,23 +292,23 @@
     if error:
         return False
 
     print("PASS: No errors on dmesg have been found.")
     return True
 
 
-def console_log_check():
+def console_log_check():  # noqa: ANN201
     """Checks for error messages on console log ("Call Trace and segfault")."""
     if not beaker.is_beaker_job():
         # skip check
         return True
     return beaker.console_log_check(error_mgs)
 
 
-def kdump_check():
+def kdump_check():  # noqa: ANN201
     """Check for kdump error messages.
     It assumes kdump is configured on /var/crash.
     """
     error = 0
 
     previous_kdump_check_file = "/tmp/previous-kdump-check"
     kdump_dir = "/var/crash"
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def exists_persistent_vars_file() -> bool:
     """Returns True if persistent vars filer exists, default /tmp/FILE_NAMES."""
     return Path(get_persistent_files_dir() + get_persistent_vars_file_name()).exists()
 
 
-def _check_0_start(value) -> bool:
+def _check_0_start(value) -> bool:  # noqa: ANN001
     """Checks if value starts with 0 but is not 0. This prevents from changing '02314' but allows changing '0'.
 
     Args:
       value (string): value to check
     """
     return all([value.startswith("0"), value != "0"])
 
@@ -114,15 +114,15 @@
 
     Returns:
       original string without quotes
     """
     return "".join([char for char in value if char not in ["'", '"']])
 
 
-def recursive_read_value(value: str) -> Any:
+def recursive_read_value(value: str) -> Any:  # noqa: ANN401
     """Given string tries to change type of the string to different types. Returns value of new type of possible.
     Supported new types: list, int, float, None, bool
     Example: str("21654") changes to int(21654).
 
     Args:
       value (string): value to be retyped
 
@@ -141,15 +141,15 @@
         if ret:
             if func == _read_to_list:
                 return [recursive_read_value(val) for val in value]
             return value
     return value
 
 
-def read_var(var: str) -> Any:
+def read_var(var: str) -> Any:  # noqa: ANN401
     """Args:
       var (string): variable name saved in file of the same name in get_persistent_files_dir() location.
 
     Returns:
       Any(_recursive_read_value): Value saved in the file with proper type
     """
     if not Path(get_persistent_files_dir() + var).is_file():
@@ -157,40 +157,40 @@
             print(f"WARN: File {get_persistent_files_dir() + var} does not exist.")
         return None
     with Path(get_persistent_files_dir() + var).open() as f:
         value = f.read()
     return recursive_read_value(value)
 
 
-def read_env(var: str) -> Any:
+def read_env(var: str) -> Any:  # noqa: ANN401
     """This does not handle KeyError, it is intentional.
 
     Args:
       var (string): os.environ variable
 
     Returns:
       Any(_recursive_read_value).: value of environ variable
     """
     return recursive_read_value(os.environ[var])
 
 
-def _write_to_string(value: Any) -> Tuple[bool, Union[str, Any]]:
+def _write_to_string(value: Any) -> Tuple[bool, Union[str, Any]]:  # noqa: ANN401
     """Args:
       value (Any): Value to try to change to string.
 
     Returns:
       tuple: (False, original value) or (True, str(value))
     """
     try:
         return True, str(value)
     except ValueError:
         return False, value
 
 
-def _write_from_list(value: Any) -> Tuple[bool, Union[str, Any]]:
+def _write_from_list(value: Any) -> Tuple[bool, Union[str, Any]]:  # noqa: ANN401
     """Args:
       value: Value to try to change to list.
 
     Returns:
       tuple.: (False, original value) or (True, str(list(value)) without '' or "").
     """
     if isinstance(value, list):
@@ -210,15 +210,15 @@
         return 1
     file_name = list(var.keys()).pop()
     write_file(file_name, list(var.values()).pop())
     add_file_to_list(file_name)
     return 0
 
 
-def write_file(file_name: str, value) -> None:
+def write_file(file_name: str, value) -> None:  # noqa: ANN001
     """Args:
       file_name (string): File name to write to location get_persistent_files_dir() + file_name
       value: value to write to the file.
 
     Returns:
       None: None
     """
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/restraint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 """restraint.py: Module to manage restraint."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import os
-import re
 from pathlib import Path
 
 from sts import linux
 from sts.utils.cmdline import run_ret_out
 
 
-def sts_print(string):
-    module_name = __name__
-    string = re.sub("DEBUG:", "DEBUG:(" + module_name + ") ", string)
-    string = re.sub("FAIL:", "FAIL:(" + module_name + ") ", string)
-    string = re.sub("FATAL:", "FATAL:(" + module_name + ") ", string)
-    string = re.sub("WARN:", "WARN:(" + module_name + ") ", string)
-    print(string)
-    if "FATAL:" in string:
-        raise RuntimeError(string)
-
-
-def update_killtime(kill_time):
+def update_killtime(kill_time):  # noqa: ANN001, ANN201
     """Change beaker watchdog kill time
     Parameter:
     kill_time     new kill time in hours
     Return:
     True
     or
     False.
@@ -49,69 +37,69 @@
         jobid,
         test,
         kill_time,
         testid,
     )
     ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
-        sts_print("FAIL: Could not update beaker kill time")
+        print("FAIL: Could not update beaker kill time")
         print(output)
         return False
-    sts_print("INFO: beaker_update_killtime() - Watchdog timer successfully updated to %d hours" % kill_time)
+    print("INFO: beaker_update_killtime() - Watchdog timer successfully updated to %d hours" % kill_time)
     return True
 
 
-def log_submit(log_file):
+def log_submit(log_file):  # noqa: ANN001, ANN201
     """Upload log file."""
     if not is_restraint_job():
         return True
 
     if not log_file:
-        sts_print("FAIL: log_submit() - requires log_file parameter")
+        print("FAIL: log_submit() - requires log_file parameter")
         return False
 
     if not Path(log_file).exists():
-        sts_print(f"FAIL: log_submit() - file ({log_file}) does not exist")
+        print(f"FAIL: log_submit() - file ({log_file}) does not exist")
         return False
 
     cmd = f'rhts-submit-log -l "{log_file}"'
     ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
-        sts_print(f"FAIL: Could not upload log {log_file}")
+        print(f"FAIL: Could not upload log {log_file}")
         print(output)
         return False
-    sts_print(f"INFO: log_submit() - {log_file} uploaded successfully")
+    print(f"INFO: log_submit() - {log_file} uploaded successfully")
     return True
 
 
-def get_recipe_id():
+def get_recipe_id():  # noqa: ANN201
     """Get current recipe id
     Parameter:
     None
     Return:
     recipe_id:          Restraint recipe id
     or
     None:               When not running using restraint.
     """
     if not is_restraint_job():
         return None
     return os.environ["RSTRNT_RECIPEID"]
 
 
-def get_task_id():
+def get_task_id():  # noqa: ANN201
     """Get current task id
     Parameter:
     None
     Return:
     task_id:          Beaker task id
     or
     None:             Some error occurred.
     """
     if not is_restraint_job():
         return None
     return os.environ["RSTRNT_TASKID"]
 
 
-def is_restraint_job():
+def is_restraint_job():  # noqa: ANN201
     """Checks if it is restraint job."""
     need_env = ["RSTRNT_TASKNAME", "RSTRNT_TASKID"]
     return all(not var not in os.environ for var in need_env)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/size.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """size.py: Module to convert human size <=> bytes."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 
-from sts.utils import sts_print
-
 size_human_regex = re.compile(r"([\-0-9\.]+)(Ki|Mi|Gi|Ti|Ei|Zi){0,1}B$")
 
 
-def size_human_check(size_human):
+def size_human_check(size_human):  # noqa: ANN001, ANN201
     size_human = str(size_human)
     m = size_human_regex.match(size_human)
     if not m:
-        sts_print(f"FAIL: size_human_check() - incorrect number format {size_human}")
+        print(f"FAIL: size_human_check() - incorrect number format {size_human}")
         return False
     return True
 
 
-def size_human_2_size_bytes(size_human):
+def size_human_2_size_bytes(size_human):  # noqa: ANN001, ANN201
     """Usage
         size_human_2_size_bytes(size_human)
     Purpose
         Convert human readable stander size to B
     Parameter
         size_human     # like '1KiB'
     Returns
@@ -39,15 +37,15 @@
         return None
 
     m = size_human_regex.match(size_human)
     if not m:
         if re.match(r"^\d+$", size_human):
             # Assume size is already in bytes
             return size_human
-        sts_print(f"FAIL: '{size_human}' is an invalid human size format")
+        print(f"FAIL: '{size_human}' is an invalid human size format")
         return None
 
     fraction = 0
     # check if number is fractional
     f = re.match(r"(\d+)\.(\d+)", m.group(1))
     if f:
         number = int(f.group(1))
@@ -67,25 +65,23 @@
             return int(number + fraction)
         number *= 1024
         fraction *= 1024
         fraction /= 10
     return int(number + fraction)
 
 
-def size_bytes_2_size_human(num):
+def size_bytes_2_size_human(num):  # noqa: ANN001, ANN201
     if not num:
         return None
 
     # Even if we receive string we , so we can process it
     num = int(num)
     for unit in ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB"]:
         if abs(num) < 1024.0:
             size_human = f"{num:3.1f}{unit}"
             # round it down removing decimal numbers
-            size_human = re.sub(r"\.\d+", "", size_human)
-            return size_human
+            return re.sub(r"\.\d+", "", size_human)
         num /= 1024.0
     # Very big number!!
     size_human = f"{num:.1f}Yi"
     # round it down removing decimal numbers
-    size_human = re.sub(r"\.\d+", "", size_human)
-    return size_human
+    return re.sub(r"\.\d+", "", size_human)
```

### Comparing `sts_libs-0.0.4/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/tmt.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,20 @@
 
 
 class GuestType(TypedDict):
     name: Optional[str]
     role: Optional[str]
 
 
+TmtResult = Literal["pass", "fail", "info", "warn", "error"]
+
+
 class CustomResults(TypedDict):
     name: str  # e.g. "/step-1" or "/setup/iscsi/target"
-    result: Literal["pass", "fail", "info", "warn", "error"]
+    result: TmtResult
     note: Optional[str]
     log: Optional[List[str]]  # path(s) to log file
     serialnumber: Optional[int]  # serial number of the test in the sequence of all tests of a plan.
     guest: Optional[GuestType]
     duration: Optional[str]
     ids: Optional[Dict[str, str]]
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/cmdline_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import unittest
 
 from sts.utils.cmdline import run, run_ret_out
 
 
 class TestCmdline(unittest.TestCase):
-    def test_run_verbose(self):
+    def test_run_verbose(self) -> None:
         test_msg = "run test message"
         # write to stderr, the message should be shown in the test
         test_cmd = f"echo {test_msg} >&2"
         running_string = f"Running command: '{test_cmd}'"
 
         new_callable = io.StringIO()
         sys.stdout = new_callable
@@ -28,40 +28,40 @@
         new_callable = io.StringIO()
         sys.stdout = new_callable
         assert run(test_cmd, verbose=False).returncode == 0
         sys.stdout = sys.__stdout__
         assert new_callable.getvalue() == ""
         sys.stdout = sys.__stdout__
 
-    def test_run_return_output(self):
+    def test_run_return_output(self) -> None:
         test_msg = "run test message"
         test_cmd = f"echo {test_msg}"
         ret_out = run(test_cmd, capture_output=True)
         assert ret_out.returncode == 0
         assert ret_out.output == test_msg
 
-    def test_run_return_output_legacy(self):
+    def test_run_return_output_legacy(self) -> None:
         test_msg = "run test message"
         test_cmd = f"echo {test_msg}"
         assert run_ret_out(test_cmd, return_output=True) == (0, test_msg)
 
-    def test_run_fail_return_output(self):
+    def test_run_fail_return_output(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
         test_cmd = "ls invalid_file"
         ret_out = run(test_cmd, capture_output=True)
         assert ret_out.returncode == 2
         assert ret_out.output == failure_msg
 
-    def test_run_fail_return_output_legacy(self):
+    def test_run_fail_return_output_legacy(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
         test_cmd = "ls invalid_file"
         assert run_ret_out(test_cmd, return_output=True) == (2, failure_msg)
 
-    def test_run_timeout(self):
+    def test_run_timeout(self) -> None:
         test_cmd = "sleep 9"
         expected_retcode = 124
         assert run(test_cmd, timeout=1).returncode == expected_retcode
 
-    def test_run_timeout_legacy(self):
+    def test_run_timeout_legacy(self) -> None:
         test_cmd = "sleep 9"
         expected_retcode = 124
         assert run_ret_out(test_cmd, return_output=True, timeout=1) == (expected_retcode, None)
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/fio_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/fio_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 
 from sts import fio
 from sts.utils.cmdline import run
 
 
-def test_fio():
+def test_fio() -> None:
     if not fio.install_fio():
         pytest.fail("Unable to install fio")
 
     output_file = "fio.test"
 
     # Create a file big enough to use by FIO
     run(f"dd if=/dev/zero of={output_file} count=20 bs=1024k")
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/iscsi_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import pytest
 
 from sts import iscsi
 
 target = "localhost"
 
 
-def test_install_initiator():
+def test_install_initiator() -> None:
     if not iscsi.install():
         pytest.fail("FAIL: Could not install iSCSI initiator package")
     assert 1
 
 
 @patch("sts.iscsi.run_ret_out")
-def test_query_discovery(iscsi_run_func):
+def test_query_discovery(iscsi_run_func) -> None:  # noqa: ANN001
     discovery_output = """
 SENDTARGETS:
 DiscoveryAddress: localhost,3260
 Target: iqn.2009-10.com.redhat:storage-0
     Portal: [::1]:3260,1
         Iface Name: default
 iSNS:
@@ -51,22 +51,22 @@
         "STATIC": {},
         "FIRMWARE": {},
     }
     assert iscsi.query_discovery() == expected_ret
 
 
 @patch("sts.iscsi.run_ret_out")
-def test_discovery(iscsi_run_func):
+def test_discovery(iscsi_run_func) -> None:  # noqa: ANN001
     discovery_output = "[::1]:3260,1 iqn.2009-10.com.redhat:storage-0"
     iscsi_run_func.return_value = (0, discovery_output)
 
     if not iscsi.discovery_st(target):
         pytest.fail("FAIL: Could not discovery iSCSI target")
     assert 1
 
 
 @patch("sts.linux.service_restart")
-def test_set_iscsid_parameter(service_restart_func):
+def test_set_iscsid_parameter(service_restart_func) -> None:  # noqa: ANN001
     service_restart_func.return_value = True
     if not iscsi.set_iscsid_parameter({"node.session.cmds_max": "4096", "node.session.queue_depth": "128"}):
         pytest.fail("FAIL: Unable to set iscsid parameter")
     assert 1
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/linux_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/linux_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from unittest.mock import patch
 
 import pytest
 
 from sts import linux, scsi_debug
 
 
-def test_os_info():
+def test_os_info():  # noqa: ANN201
     os_info = linux.query_os_info()
     if not os_info:
         pytest.fail("FAIL: Could not query OS info")
 
     for info in os_info:
         print(f"{info}: {os_info[info]}")
     assert 1
 
 
-def test_using_scsi_debug():
+def test_using_scsi_debug():  # noqa: ANN201
     if linux.is_docker():
         print("SKIP: Cannot create scsi_debug in container")
         return
     if not scsi_debug.scsi_debug_load_module():
         pytest.fail("FAIL: loading scsi_debug module")
 
     device = scsi_debug.get_scsi_debug_devices()[-1]
@@ -40,53 +40,53 @@
         pytest.fail("FAIL: scsi_debug device should not be mapped by DM")
 
     if not scsi_debug.scsi_debug_unload_module():
         pytest.fail("FAIL: loading scsi_debug module")
     assert 1
 
 
-def test_get_boot_device():
+def test_get_boot_device():  # noqa: ANN201
     get_boot = linux.get_boot_device()
     if get_boot is None and linux.is_docker() is False:
         pytest.fail("FAIL: Could not find '/boot' and '/'! ")
     print(f"INFO: Boot device is: {get_boot}")
     assert 1
 
 
-def test_get_dist_release():
+def test_get_dist_release():  # noqa: ANN201
     release = linux.dist_release()
     if not release:
         pytest.fail("FAIL: Could not find distribution release")
 
 
-def test_get_dist_ver():
+def test_get_dist_ver():  # noqa: ANN201
     version = linux.dist_ver()
     if not version:
         pytest.fail("FAIL: Could not find distribution version")
 
 
-def test_get_dist_name():
+def test_get_dist_name():  # noqa: ANN201
     name = linux.dist_name()
     if not name:
         pytest.fail("FAIL: Could not find distribution name")
 
 
 @patch("sts.linux.download_repo_file")
-def test_rpm_repo(get_mock):
+def test_rpm_repo(get_mock):  # noqa: ANN001, ANN201
     content = """[test-fedora-debuginfo]
 name=testrepo
 #baseurl=http://download.example/pub/fedora/linux/releases/$releasever/Everything/$basearch/debug/tree/
 metalink=https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch
 enabled=1
 repo_gpgcheck=0
 type=rpm
 skip_if_unavailable=False
 """
 
-    def create_repo_file(_):
+    def create_repo_file(_):  # noqa: ANN001, ANN202
         with Path("/etc/yum.repos.d/test2.repo").open("w") as f:
             f.write(content)
 
     get_mock.side_effect = create_repo_file
     repo_metalink = "https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch"
     repo_url = "https://testurl.com/test.repo"
     repo_name = "testrepo"
@@ -101,15 +101,15 @@
     if not linux.del_repo("test2"):
         pytest.fail("FAIL: Unable to delete repo")
     if Path("/etc/yum.repos.d/test2.repo").exists():
         pytest.fail("FAIL: repo file should have been deleted")
 
 
 @patch("sts.linux.run")
-def test_is_mounted(run_func):
+def test_is_mounted(run_func):  # noqa: ANN001, ANN201
     run_func.return_value = 0
     if not linux.is_mounted("testdev"):
         pytest.fail("FAIL: device should have been mounted")
     if not linux.is_mounted(mountpoint="testdir"):
         pytest.fail("FAIL: mountpoint should have been mounted")
     run_func.return_value = 1
     if linux.is_mounted("testdev"):
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/logchecker_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 # found segfault
 segfault_msg = (
     " segfault at 10 ip 00007f9bebcca90d sp 00007fffb62705f0 error 4 in libQtWebKit.so.4.5.2[7f9beb83a000+f6f000]"
 )
 calltrace_msg = " Call Trace: "
 
 
-def _run_dmesg_segfault(cmd, **kwargs):
+def _run_dmesg_segfault(cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
     if cmd.startswith("dmesg | grep"):
         cmd = cmd.replace("dmesg", f"echo '{segfault_msg}'")
         return run(cmd, verbose=False, **kwargs)
 
     return 0, ""
 
 
-def _run_dmesg_calltrace(cmd, **kwargs):
+def _run_dmesg_calltrace(cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
     if cmd.startswith("dmesg | grep"):
         cmd = cmd.replace("dmesg", f"echo '{calltrace_msg}'")
         return run(cmd, verbose=False, **kwargs)
 
     return 0, ""
 
 
 class Testlogchecker(unittest.TestCase):
     @patch("sts.utils.logchecker.run")
-    def test_kernel_check(self, run_func):
+    def test_kernel_check(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value.returncode = 0
         run_func.return_value.output = "0"
         assert log_checker.kernel_check() is True
         # already handled taint
         run_func.return_value.returncode = 0
         run_func.return_value.output = "1"
         assert log_checker.kernel_check() is True
 
     @patch("sts.utils.logchecker.run")
-    def test_dmesg_check(self, run_func):
+    def test_dmesg_check(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value.returncode = 0
         run_func.return_value.output = ""
         assert log_checker.dmesg_check() is True
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_segfault
         assert log_checker.dmesg_check() is False
@@ -69,10 +69,10 @@
             call("dmesg >> ./dmesg.log"),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
     @patch("sts.utils.logchecker.kernel_check")
-    def test_check_all(self, check_func):
+    def test_check_all(self, check_func):  # noqa: ANN001, ANN201
         check_func.return_value = False
         assert log_checker.check_all() is False
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/lvm_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,76 +5,76 @@
 from unittest.mock import patch
 
 from sts import lvm
 
 
 class TestPV(unittest.TestCase):
     pvs_output = "  /dev/vda1,lvm_test,lvm2,a--,98.41g,0"
-    pv_query_output = {
+    pv_query_output = {  # noqa: RUF012
         "/dev/vda1": {
             "vg": "lvm_test",
             "fmt": "lvm2",
             "attr": "a--",
             "psize": "98.41g",
             "pfree": "0",
         },
     }
 
-    def test_pv_query(self):
+    def test_pv_query(self) -> None:
         with patch("sts.lvm.run_ret_out") as run_func:
             run_func.return_value = [0, self.pvs_output]
             assert self.pv_query_output == lvm.pv_query()
 
-    def test_pv_create(self):
+    def test_pv_create(self) -> None:
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 0
             assert lvm.pv_create("/dev/vda1")
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 1
             assert not lvm.pv_create("/dev/vda1")
 
     @patch("sts.lvm.pv_query")
-    def test_pv_remove(self, mock):
+    def test_pv_remove(self, mock):  # noqa: ANN001, ANN201
         mock.return_value = self.pv_query_output
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 0
             assert lvm.pv_remove("/dev/vda1")
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 1
             assert not lvm.pv_remove("/dev/vda1")
 
 
 class TestVG(unittest.TestCase):
     vgs_output = "  lvm_test,1,3,0,wz--n-,98.41g,0"
-    vg_query_output = {
+    vg_query_output = {  # noqa: RUF012
         "lvm_test": {
             "num_pvs": "1",
             "num_lvs": "3",
             "num_sn": "0",
             "attr": "wz--n-",
             "vsize": "98.41g",
             "vfree": "0",
         },
     }
 
-    def test_vg_query(self):
+    def test_vg_query(self) -> None:
         with patch("sts.lvm.run_ret_out") as run_func:
             run_func.return_value = [0, self.vgs_output]
             assert self.vg_query_output == lvm.vg_query()
 
-    def test_pv_create(self):
+    def test_pv_create(self) -> None:
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 0
             assert lvm.vg_create("lvm_test", "/dev/vda1")
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 1
             assert not lvm.vg_create("lvm_test", "/dev/vda1")
 
     @patch("sts.lvm.pv_query")
-    def test_pv_remove(self, mock):
+    def test_pv_remove(self, mock):  # noqa: ANN001, ANN201
         mock.return_value = self.vg_query_output
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 0
             assert lvm.pv_remove("lvm_test")
         with patch("sts.lvm.run") as run_func:
             run_func.return_value.returncode = 1
             assert not lvm.pv_remove("lvm_test")
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/md_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/md_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,57 +80,57 @@
         },
     },
 }
 
 
 class TestMD(unittest.TestCase):
     @patch("sts.md.run_ret_out")
-    def test_md_query(self, run_func):
+    def test_md_query(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value = (0, mdstat_output)
 
         assert md.md_query() == ["md0"]
 
         assert run_func.call_count == 1
         run_calls = [call("cat /proc/mdstat", return_output=True, verbose=False)]
         run_func.assert_has_calls(run_calls)
 
     @patch("sts.md._mdadm_query")
     @patch("sts.md.md_query")
-    def test_md_get_info(self, md_query_func, mdadm_query_func):
+    def test_md_get_info(self, md_query_func, mdadm_query_func):  # noqa: ANN001, ANN201
         md_query_func.return_value = ["md0"]
         mdadm_query_func.return_value = mdadm_output
 
         assert md.md_get_info("md0", verbose=True) == md0_info
 
     @patch("sts.md.md_get_info")
-    def test_md_get_storage_dev(self, md_get_info_func):
+    def test_md_get_storage_dev(self, md_get_info_func):  # noqa: ANN001, ANN201
         md_get_info_func.return_value = md0_info
 
         storage_devs = md.md_get_storage_dev("md0")
         assert "/dev/sda" in storage_devs
         assert "/dev/sdb1" in storage_devs
 
     @patch("sts.md.run_ret_out")
-    def test_md_stop(self, run_func):
+    def test_md_stop(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value = (0, "")
         assert md.md_stop("md0")
         run_calls = [call("mdadm --stop /dev/md0", return_output=True, verbose=False)]
         run_func.assert_has_calls(run_calls)
 
     @patch("sts.md.run_ret_out")
-    def test_md_clean(self, run_func):
+    def test_md_clean(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value = (0, "")
         assert md.md_clean("/dev/sda")
         run_calls = [call("mdadm --zero-superblock /dev/sda", return_output=True, verbose=False)]
         run_func.assert_has_calls(run_calls)
 
     @patch("sts.md.run_ret_out")
     @patch("sts.md.md_stop")
     @patch("sts.md.md_get_storage_dev")
-    def test_md_remove(self, get_sto_func, md_stop_func, run_func):
+    def test_md_remove(self, get_sto_func, md_stop_func, run_func):  # noqa: ANN001, ANN201
         run_func.return_value = (0, "")
         md_stop_func.return_value = True
         get_sto_func.return_value = ["/dev/sda1", "/dev/sdb1"]
         assert md.md_remove("md0", clean=True)
         run_calls = [
             call("mdadm --remove /dev/md0", return_output=True, verbose=False),
             call("mdadm --zero-superblock /dev/sda1", return_output=True, verbose=False),
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/net_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/net_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,94 +16,94 @@
 NETMASK24 = "255.255.255.0"
 CIDR24 = "24"
 NOTIP = "256.256.256.256"
 IPV6 = "fd6f:60d2:2d9:0:b7e:b6e6:7bf5:c17e"
 
 
 class TestNet(unittest.TestCase):
-    def test_is_mac(self):
+    def test_is_mac(self) -> None:
         assert net.is_mac(MAC)
         assert not net.is_mac(NOTMAC)
 
-    def test_get_nics(self):
+    def test_get_nics(self) -> None:
         assert net.get_nics() is not None
 
-    def test_get_mac_of_nics(self):
+    def test_get_mac_of_nics(self) -> None:
         assert net.get_mac_of_nic(NOTVALID) is None
         assert net.get_mac_of_nic(net.get_nics()[-1]) is not None
 
-    def test_get_nic_of_mac(self):
+    def test_get_nic_of_mac(self) -> None:
         assert net.get_nic_of_mac(MAC) is None
         assert net.get_nic_of_mac(net.get_mac_of_nic(net.get_nics()[-1])) is not None
 
-    def test_get_ip_address_of_nic(self):
+    def test_get_ip_address_of_nic(self) -> None:
         assert net.get_ip_address_of_nic(NOTVALID) is None
         assert net.get_ip_address_of_nic(net.get_nics()[-1]) is not None
 
-    def test_get_ipv6_address_of_nic(self):
+    def test_get_ipv6_address_of_nic(self) -> None:
         assert net.get_ipv6_address_of_nic(NOTVALID) is None
         if not is_docker():
             assert net.get_ipv6_address_of_nic(net.get_nics()[-1]) is not None
 
-    def test_get_nic_of_ip(self):
+    def test_get_nic_of_ip(self) -> None:
         assert net.get_nic_of_ip(NOTIP) is None
         assert net.get_nic_of_ip(LOCALHOST) is not None
 
-    def test_driver_of_nic(self):
+    def test_driver_of_nic(self) -> None:
         assert net.driver_of_nic(NOTVALID) is None
 
-    def test_get_ip_version(self):
+    def test_get_ip_version(self) -> None:
         assert net.get_ip_version(LOCALHOST) == 4
         assert net.get_ip_version(IPV6) == 6
         assert net.get_ip_version(NOTIP) is None
 
-    def test_standardize_mac(self):
+    def test_standardize_mac(self) -> None:
         assert net.standardize_mac(BADMAC) == LOWMAC
         assert net.standardize_mac(NOTMAC) is None
 
-    def test_convert_netmask(self):
+    def test_convert_netmask(self) -> None:
         assert int(CIDR24) == net.convert_netmask(NETMASK24)
         assert int(CIDR24) == net.convert_netmask(CIDR24)
         assert net.convert_netmask(NOTVALID) is None
 
-    def test_nm_get_conn(self):
+    def test_nm_get_conn(self) -> None:
         assert net.nm_get_conn(MAC) is None
         assert net.nm_get_conn(NOTVALID) is None
 
-    def test_nm_get_conn_iface(self):
+    def test_nm_get_conn_iface(self) -> None:
         assert net.nm_get_conn_iface(NOTVALID) is None
 
-    def test_nm_get_conn_uuid(self):
+    def test_nm_get_conn_uuid(self) -> None:
         assert net.nm_get_conn_uuid(NOTVALID) is None
 
-    def test_nm_get_conn_from_dev(self):
+    def test_nm_get_conn_from_dev(self) -> None:
         assert net.nm_get_conn_from_dev(NOTVALID) is None
 
-    def test_nm_get_dev_from_conn(self):
+    def test_nm_get_dev_from_conn(self) -> None:
         assert net.nm_get_dev_from_conn(NOTVALID) is None
 
-    def test_nm_conn_up(self):
+    def test_nm_conn_up(self) -> None:
         assert not net.nm_conn_up(NOTVALID)
 
-    def test_nm_set_ip(self):
+    def test_nm_set_ip(self) -> None:
         assert not net.nm_set_ip(NOTVALID, NOTIP)
         assert not net.nm_set_ip(NOTVALID, IPV6)
 
-    def test_nm_dev_mod_success(self):
+    def test_nm_dev_mod_success(self) -> None:
         with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [0, ""]
             assert net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
 
-    def test_nm_dev_mod_failure(self):
+    def test_nm_dev_mod_failure(self) -> None:
         with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [1, "Mocked failure"]
             assert not net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
 
-    def test_nm_set_ip_success(self):
+    def test_nm_set_ip_success(self) -> None:
         with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [0, ""]
             assert net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
 
-    def test_nm_set_ip_failure(self):
+    def test_nm_set_ip_failure(self) -> None:
         with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [1, "Mocked failure"]
             assert not net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/persistent_vars_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 
 import unittest
 
 from sts.utils.persistent_vars import recursive_read_value
 
 
 class TestChangeType(unittest.TestCase):
-    def test_to_float(self):
+    def test_to_float(self) -> None:
         assert recursive_read_value("0.1") == 0.1
         assert recursive_read_value("1.0") == 1.0
         assert recursive_read_value("1.1") == 1.1
 
-    def test_to_int(self):
+    def test_to_int(self) -> None:
         assert recursive_read_value("0") == 0
         assert recursive_read_value("1") == 1
         assert recursive_read_value("1234") == 1234
 
-    def test_to_str(self):
+    def test_to_str(self) -> None:
         assert recursive_read_value("0123") == "0123"
         assert recursive_read_value("string") == "string"
 
-    def test_to_none(self):
+    def test_to_none(self) -> None:
         assert recursive_read_value("None") is None
 
-    def test_to_bool(self):
+    def test_to_bool(self) -> None:
         assert recursive_read_value("true") is True
         assert recursive_read_value("false") is False
         assert recursive_read_value("True") is True
         assert recursive_read_value("False") is False
         assert recursive_read_value("TRUE") is True
         assert recursive_read_value("FALSE") is False
 
-    def test_to_list(self):
+    def test_to_list(self) -> None:
         assert recursive_read_value("[1, string]") == [1, "string"]
         assert recursive_read_value("[None]") == [None]
         assert recursive_read_value("['string', 0.1]") == ["string", 0.1]
         assert recursive_read_value("['/dev/sda', '/dev/sdb', '/dev/sdc']") == [
             "/dev/sda",
             "/dev/sdb",
             "/dev/sdc",
```

### Comparing `sts_libs-0.0.4/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.5.dev0/sts_libs/tests/scsi_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import pytest
 
 from sts import scsi
 
 
-def test_query_scsi_hosts():
+def test_query_scsi_hosts() -> None:
     hosts = scsi.get_hosts()
     if not hosts:
         print("SKIP: Could not find scsi hosts")
         return
 
     for host in hosts:
         print(f"Querying info for host {host}")
@@ -19,15 +19,15 @@
             pytest.fail(f"Could not query info for host: {host}")
         for inf in info:
             print(f"\t{inf}: {info[inf]}")
 
     assert 1
 
 
-def test_query_scsi_disks():
+def test_query_scsi_disks() -> None:
     disks = scsi.query_all_scsi_disks()
     if not disks:
         print("SKIP: Could not find scsi disks")
         return
 
     for disk in disks:
         print(f"INFO: details for scsi id: {disk}")
```

### Comparing `sts_libs-0.0.4/.gitignore` & `sts_libs-0.0.5.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.4/LICENSE` & `sts_libs-0.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.4/pyproject.toml` & `sts_libs-0.0.5.dev0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,47 @@
 [project]
 name = "sts-libs"
 description = ""
 readme = "sts_libs/README.md"
 requires-python = ">=3.8"
 dynamic = ["version"]
 authors = [
-  { name = "Bruno Goncalves", email = "bgoncalv@redhat.com" },
-  { name = "Filip Suba", email = "fsuba@redhat.com" },
-  { name = "Jakub Krysl", email = "jkrysl@redhat.com" },
-  { name = "Martin Hoyer", email = "mhoyer@redhat.com" },
+  {name = "Bruno Goncalves", email = "bgoncalv@redhat.com"},
+  {name = "Filip Suba", email = "fsuba@redhat.com"},
+  {name = "Jakub Krysl", email = "jkrysl@redhat.com"},
+  {name = "Martin Hoyer", email = "mhoyer@redhat.com"},
 ]
 maintainers = [
-  { name = "Martin Hoyer", email = "mhoyer@redhat.com" },
-  { name = "Filip Suba", email = "fsuba@redhat.com" },
-  { name = "Bruno Goncalves", email = "bgoncalv@redhat.com" },
+  {name = "Martin Hoyer", email = "mhoyer@redhat.com"},
+  {name = "Filip Suba", email = "fsuba@redhat.com"},
+  {name = "Bruno Goncalves", email = "bgoncalv@redhat.com"},
 ]
 license = "GPL-3.0-or-later"
-license-files = { paths = ["LICENSE"] }
+license-files = {paths = ["LICENSE"]}
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Testing",
   "Topic :: Software Development :: Quality Assurance",
   "Intended Audience :: Developers",
   "Operating System :: POSIX :: Linux",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Framework :: Hatch",
 ]
-
 dependencies = [
-  "pytest",
+  "pytest>=6.2.2",
   "configobj==5.0.8",
   "netifaces2==0.0.16",
   "six==1.16.0",
-      # via configobj
-  "typing-extensions==4.5.0"
-      # via netifaces2
+    # via configobj
+  "typing-extensions==4.5.0",
+    # via netifaces2
 ]
 
 [project.urls]
 Repository = "https://gitlab.com/rh-kernel-stqe/sts/"
 
 [tool.hatch.version]
 path = "sts_libs/__about__.py"
@@ -72,15 +71,15 @@
   "W",  # pycodestyle
   #"C90",  # mccabe
   "I",  # isort
   "N",  # pep8-naming
   "D",  # pydocstyle
   "UP",  # pyupgrade
   "YTT",  # flake8-2020
-  #"ANN",  # flake8-annotations
+  "ANN",  # flake8-annotations
   #"BLE",  # flake8-blind-except
   "B",  # flake8-bugbear
   "A",  # flake8-builtins
   "COM",  # flake8-commas
   "C4",  # flake8-comprehensions
   "DTZ",  # flake8-datetimez
   "T10",  # flake8-debugger
@@ -105,23 +104,23 @@
   "PTH",  # flake8-use-pathlib
   #"ERA",  # eradicate
   "PGH",  # pygrep-hooks
   "PL",  # Pylint
   "TRY",  # tryceratops
   "RUF",  # Ruff-specific rules
 ]
-
 ignore = [
   "D10",  # Missing docstring
   "D205",  # 1 blank line required between summary line and description
   "D417",  # Missing argument descriptions -> Do not use docstring description for well type-annotated args
   "PLR09",  # pylint-refactor too-many
   "PLC1901",  # compare-to-empty-string
   "PLR2004",  # magic value
   "TRY300",  # Consider moving this statement to an `else` block. Seems to be broken?
+  "ANN101",  # Missing type annotation for `self` in method
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["INP001"]
 
 [tool.ruff.flake8-builtins]
 builtins-ignorelist = ["id"]
@@ -137,7 +136,12 @@
 omit = ["_test.py"]
 
 [tool.mypy]
 ignore_missing_imports = true
 # strict = true  # TODO -> Will require a lot of effort
 show_error_codes = true
 python_version = "3.8"
+
+[tool.yamlfix]
+explicit_start = "false"
+line_length = 120
+sequence_style = "block_style"
```

### Comparing `sts_libs-0.0.4/sts_libs/README.md` & `sts_libs-0.0.5.dev0/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.4/PKG-INFO` & `sts_libs-0.0.5.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.4
+Version: 0.0.5.dev0
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: configobj==5.0.8
 Requires-Dist: netifaces2==0.0.16
-Requires-Dist: pytest
+Requires-Dist: pytest>=6.2.2
 Requires-Dist: six==1.16.0
 Requires-Dist: typing-extensions==4.5.0
 Description-Content-Type: text/markdown
 
 # sts-libs
 
 Libs for testing storage drivers and userspace utilities on rpm-based operating systems.
```

