# Comparing `tmp/walt-virtual-7.tar.gz` & `tmp/walt-virtual-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walt-virtual-7.tar", last modified: Mon Feb  1 15:17:01 2021, max compression
+gzip compressed data, was "walt-virtual-8.0.tar", last modified: Fri Jun 23 07:38:05 2023, max compression
```

## Comparing `walt-virtual-7.tar` & `walt-virtual-8.0.tar`

### file list

```diff
@@ -1,38 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/
--rw-r--r--   0 root         (0) root         (0)      163 2020-09-24 12:01:14.000000 walt-virtual-7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      304 2021-02-01 15:17:01.000000 walt-virtual-7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      139 2020-09-24 12:01:14.000000 walt-virtual-7/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-01 15:17:01.000000 walt-virtual-7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      342 2020-09-24 12:01:14.000000 walt-virtual-7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2020-09-24 12:01:14.000000 walt-virtual-7/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt/virtual/
--rw-r--r--   0 root         (0) root         (0)       44 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/__init__.py
--rw-r--r--   0 root         (0) root         (0)      998 2021-02-01 15:16:44.000000 walt-virtual-7/walt/virtual/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt/virtual/node/
--rwxr-xr-x   0 root         (0) root         (0)       39 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6477 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/node/fakeipxe.py
--rwxr-xr-x   0 root         (0) root         (0)     6829 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/node/node.py
--rw-r--r--   0 root         (0) root         (0)     3316 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/node/udhcpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt/virtual/setup/
--rwxr-xr-x   0 root         (0) root         (0)     1818 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/setup/S51waltvpnclient
--rwxr-xr-x   0 root         (0) root         (0)     2031 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/setup/S52waltvirtualnode
--rwxr-xr-x   0 root         (0) root         (0)     3316 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/setup/walt-vpn-server.service
--rw-r--r--   0 root         (0) root         (0)       82 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/setup/walt-vpn-server.socket
--rw-r--r--   0 root         (0) root         (0)     1231 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt/virtual/vpn/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      390 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/authtool.py
--rwxr-xr-x   0 root         (0) root         (0)     7625 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/client.py
--rwxr-xr-x   0 root         (0) root         (0)       63 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/const.py
--rwxr-xr-x   0 root         (0) root         (0)     1103 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/endpoint.py
--rwxr-xr-x   0 root         (0) root         (0)     3632 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/server.py
--rwxr-xr-x   0 root         (0) root         (0)     1672 2020-09-24 12:01:14.000000 walt-virtual-7/walt/virtual/vpn/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/
--rw-r--r--   0 root         (0) root         (0)      304 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      430 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-02-01 15:17:01.000000 walt-virtual-7/walt_virtual.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.324741 walt-virtual-8.0/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-21 15:19:09.000000 walt-virtual-8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-23 07:38:05.324741 walt-virtual-8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      139 2022-03-29 14:58:03.000000 walt-virtual-8.0/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:05.324741 walt-virtual-8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      893 2023-06-23 07:37:56.000000 walt-virtual-8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/sh/
+-rwxr-xr-x   0 root         (0) root         (0)       66 2023-06-21 15:19:09.000000 walt-virtual-8.0/sh/walt-vnode-ifdown
+-rwxr-xr-x   0 root         (0) root         (0)      174 2023-06-21 15:19:09.000000 walt-virtual-8.0/sh/walt-vnode-ifup
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/node/
+-rwxr-xr-x   0 root         (0) root         (0)       58 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16206 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/node.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/udhcpc.py
+-rwxr-xr-x   0 root         (0) root         (0)      889 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/walt-vnode-ifdown
+-rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/walt-vnode-ifup
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/setup/
+-rwxr-xr-x   0 root         (0) root         (0)     2215 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/S52waltvirtualnode
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      434 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.324741 walt-virtual-8.0/walt_virtual.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      581 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `walt-virtual-7/walt/virtual/node/udhcpc.py` & `walt-virtual-8.0/walt/virtual/node/udhcpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,110 @@
-import time, sys, os, tempfile, traceback
+import os
+import sys
+import tempfile
+import time
+import traceback
+from contextlib import contextmanager
 from pathlib import Path
 from subprocess import check_call, check_output
-from contextlib import contextmanager
 
 BRIDGE_INTF = "walt-net"
 
+
 @contextmanager
 def temporary_network_pipe():
     # generate a unique name
-    pipe_name = 'pipe-%d' %  os.getpid()
-    pipe = ('%s-0' % pipe_name, '%s-1' % pipe_name)
+    pipe_name = "pipe-%d" % os.getpid()
+    pipe = ("%s-0" % pipe_name, "%s-1" % pipe_name)
     # create pipe
-    check_call('ip link add %(pipe0)s type veth peer name %(pipe1)s' % dict(
-        pipe0 = pipe[0],
-        pipe1 = pipe[1]
-    ), shell = True)
+    check_call(
+        "ip link add %(pipe0)s type veth peer name %(pipe1)s"
+        % dict(pipe0=pipe[0], pipe1=pipe[1]),
+        shell=True,
+    )
     try:
         yield pipe
     finally:
         # release pipe (note: the other end is automatically removed)
-        check_call('ip link del ' + pipe[0], shell = True)
+        check_call("ip link del " + pipe[0], shell=True)
+
 
-UDHCPC_SCRIPT = '''\
+UDHCPC_SCRIPT = """\
 #!/bin/sh
 if [ "$ip" = "" ]
 then
     exit 0
 fi
 echo VAR hostname $hostname
 echo VAR ip $ip
 echo VAR server_ip $serverid
 echo VAR gateway $router
 echo VAR netmask $subnet
-'''
+"""
+
 
 def udhcpc_get_vars(env, interface):
     with tempfile.TemporaryDirectory() as tmpdir:
         tmpdir = Path(tmpdir)
-        script = tmpdir / 'script.sh'
+        script = tmpdir / "script.sh"
         script.write_text(UDHCPC_SCRIPT)
-        script.chmod(0o755) # make it executable
-        info = check_output('udhcpc -V %(vci)s -f -q -n -i %(interface)s -s %(script)s' % dict(
-            vci = env['vci'],
-            interface = interface,
-            script = str(script)
-        ), shell=True).decode(sys.getdefaultencoding())
+        script.chmod(0o755)  # make it executable
+        info = check_output(
+            "udhcpc -V %(vci)s -f -q -n -i %(interface)s -s %(script)s"
+            % dict(vci=env["vci"], interface=interface, script=str(script)),
+            shell=True,
+        ).decode(sys.getdefaultencoding())
         for line in info.splitlines():
             words = line.split()
-            if words[0] != 'VAR':
+            if words[0] != "VAR":
                 continue
             if len(words) == 3:
                 var_name, value = words[1], words[2]
             else:
-                var_name, value = words[1], ''
+                var_name, value = words[1], ""
             env[var_name] = value
 
+
 def udhcpc_setup_interface(env, interface):
-    check_call('udhcpc -V %(vci)s -f -q -n -i %(interface)s' % dict(
-            vci = env['vci'],
-            interface = interface
-            ), shell=True)
+    check_call(
+        "udhcpc -V %(vci)s -f -q -n -i %(interface)s"
+        % dict(vci=env["vci"], interface=interface),
+        shell=True,
+    )
+
 
 # 1. We create a set of temporary "veth" interfaces. One end is linked to
 #    walt-net bridge. The other end is configured with the mac address we
 #    will use later for the walt node.
 # 2. We use udhcpc to get the network parameters we were missing.
 #    Because of the mac address, the server will consider this request comes
 #    from the node.
 # 3. We clean things up by removing temporary "veth" interfaces.
 
+
 @contextmanager
 def udhcpc_fake_netboot(env):
-    bridge_dev_dir = Path('/sys/class/net') / BRIDGE_INTF
+    bridge_dev_dir = Path("/sys/class/net") / BRIDGE_INTF
     while not bridge_dev_dir.is_dir():
         print("'%s' not available yet. Will retry in a moment." % BRIDGE_INTF)
         time.sleep(3)
     with temporary_network_pipe() as pipe:
-        check_call('ip link set dev %(pipe0)s master %(bridge)s up' % dict(
-            pipe0 = pipe[0],
-            bridge = BRIDGE_INTF
-        ), shell=True)
-        check_call('ip link set dev %(pipe1)s address %(mac)s up' % dict(
-            pipe1 = pipe[1],
-            mac = env['mac']
-        ), shell=True)
+        check_call(
+            "ip link set dev %(pipe0)s master %(bridge)s up"
+            % dict(pipe0=pipe[0], bridge=BRIDGE_INTF),
+            shell=True,
+        )
+        check_call(
+            "ip link set dev %(pipe1)s address %(mac)s up"
+            % dict(pipe1=pipe[1], mac=env["mac"]),
+            shell=True,
+        )
         try:
             # we need to save env variables retrieved through DHCP
             # (they are needed to interpret ipxe scripts)
             udhcpc_get_vars(env, pipe[1])
             # we also need to setup the interface to handle TFTP transfers
             udhcpc_setup_interface(env, pipe[1])
             yield True
-        except:
+        except Exception:
             traceback.print_exc()
             yield False
```

### Comparing `walt-virtual-7/walt/virtual/setup/S52waltvirtualnode` & `walt-virtual-8.0/walt/virtual/setup/S52waltvirtualnode`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/bin/sh
 #
 # walt-virtual-node       Start a walt virtual node
 #
 
 CONF=/etc/default/walt-vpn-node
+CONSOLE=/dev/tty1    # HDMI console
+WRITEFS="writefs"
 
 msg() {
-	echo "[walt-virtual-node] $1" | tee /dev/tty0
+	echo "[walt-virtual-node] $1" | tee $CONSOLE
 }
 
 # Make sure the conf is OK
 [ -f $CONF ] || {
     msg "Missing file '$CONF'." >&2
     exit 1
 }
@@ -19,17 +21,15 @@
     msg "File $CONF should define var WALT_VPN_ENTRYPOINT." >&2
     exit 1
 }
 
 [ -z "$WALT_VIRTUAL_NODE_MAC" ] && {
     # generate and save random mac address for virtual node
     WALT_VIRTUAL_NODE_MAC="$(printf '52:54:00:%02x:%02x:%02x' $((RANDOM%256)) $((RANDOM%256)) $((RANDOM%256)))"
-    mount -o remount,rw /
-    echo "WALT_VIRTUAL_NODE_MAC='$WALT_VIRTUAL_NODE_MAC'" >> $CONF
-    mount -o remount,ro /
+    echo "WALT_VIRTUAL_NODE_MAC='$WALT_VIRTUAL_NODE_MAC'" | $WRITEFS tee -a $CONF
 }
 
 umask 077
 
 start() {
     msg "Starting virtual node..."
     # note: when the virtual node reboots, USB peripherals plugged on the host
@@ -37,17 +37,19 @@
     # cause issues.
     # thus, we use option --on-vm-reboot 'reboot', which will make the host
     # reboot too, whenever the virtual node reboots.
     screen -S walt.virtual.node -d -m   \
             walt-virtual-node --attach-usb \
                               --net-conf-udhcpc \
                               --mac $WALT_VIRTUAL_NODE_MAC \
-                              --model qemu-arm \
+                              --model qemu-arm-64 \
                               --on-vm-reboot 'reboot' \
-                              --log-file /dev/tty0 \
+                              --log-file $CONSOLE \
+                              --pid-path "/var/run/walt-virtual-node.pid" \
+                              --screen-session-path "/var/run/walt-virtual-node.screen" \
                               --log-prefix "walt-virtual-node"
     status=$?
     if [ "$status" -eq 0 ]; then
         msg "OK"
     else
         msg "FAIL"
     fi
```

