# Comparing `tmp/ABOTP-1.0.tar.gz` & `tmp/ABOTP-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ABOTP-1.0.tar", last modified: Sat Jun 17 17:56:01 2023, max compression
+gzip compressed data, was "ABOTP-2.0.tar", last modified: Thu Jun 22 22:06:42 2023, max compression
```

## Comparing `ABOTP-1.0.tar` & `ABOTP-2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 17:56:01.133769 ABOTP-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-17 17:56:01.123778 ABOTP-1.0/ABOTP/
--rw-rw-rw-   0        0        0     3359 2023-06-17 17:47:23.000000 ABOTP-1.0/ABOTP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 17:56:01.132771 ABOTP-1.0/ABOTP.egg-info/
--rw-rw-rw-   0        0        0      183 2023-06-17 17:56:00.000000 ABOTP-1.0/ABOTP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-17 17:56:00.000000 ABOTP-1.0/ABOTP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 17:56:00.000000 ABOTP-1.0/ABOTP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-17 17:56:00.000000 ABOTP-1.0/ABOTP.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-17 17:56:00.000000 ABOTP-1.0/ABOTP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      183 2023-06-17 17:56:01.133769 ABOTP-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-17 17:56:01.135769 ABOTP-1.0/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-06-17 17:52:24.000000 ABOTP-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:06:42.990833 ABOTP-2.0/
+drwxrwxrwx   0        0        0        0 2023-06-22 22:06:42.966856 ABOTP-2.0/ABOTP/
+-rw-rw-rw-   0        0        0       95 2023-06-22 21:23:26.000000 ABOTP-2.0/ABOTP/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-06-22 21:49:07.000000 ABOTP-2.0/ABOTP/client.py
+-rw-rw-rw-   0        0        0     4115 2023-06-22 21:51:27.000000 ABOTP-2.0/ABOTP/server.py
+-rw-rw-rw-   0        0        0     1983 2023-06-22 21:56:54.000000 ABOTP-2.0/ABOTP/storages.py
+-rw-rw-rw-   0        0        0      153 2023-06-22 21:37:57.000000 ABOTP-2.0/ABOTP/support.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:06:42.973844 ABOTP-2.0/ABOTP.egg-info/
+-rw-rw-rw-   0        0        0      574 2023-06-22 22:06:42.000000 ABOTP-2.0/ABOTP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-06-22 22:06:42.000000 ABOTP-2.0/ABOTP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 22:06:42.000000 ABOTP-2.0/ABOTP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 22:06:42.000000 ABOTP-2.0/ABOTP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      574 2023-06-22 22:06:42.991833 ABOTP-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 22:06:42.992832 ABOTP-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-06-22 21:06:37.000000 ABOTP-2.0/setup.py
```

### Comparing `ABOTP-1.0/ABOTP/__init__.py` & `ABOTP-2.0/ABOTP/server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,122 @@
 import socket
 import struct
-from typing import Optional, List
-
-
-class Client:
-
-    def __init__(self, family: Optional[int] = socket.AF_INET):
-        self.address = None
-        self.status = False
-        self.sock = socket.socket(family, socket.SOCK_STREAM)
-
-    def connect(self, address: tuple) -> None:
-        self.sock.connect(address)
-        self.status = True
-
-    def recv(self) -> List[bytes]:
-        def picking(n):
-            data = b''
-            while len(data) < n:
-                packet = self.sock.recv(n - len(data))
-                if not packet:
-                    return None
-                data += packet
-            return data
-
-        num_objects = struct.unpack('>I', picking(4))[0]
-        objects = []
-        for _ in range(num_objects):
-            len_data = struct.unpack('>I', picking(4))[0]
-            obj_data = picking(len_data)
-            objects.append(obj_data)
-        return objects
-
-    def send(self, objects: List[bytes]) -> None:
-        num_objects = len(objects)
-        packet = struct.pack('>I', num_objects)
-        for obj in objects:
-            packet += struct.pack('>I', len(obj)) + obj
-        self.sock.sendall(packet)
-
-    def close(self):
-        self.sock.close()
-        self.status = False
-
-    def __del__(self):
-        self.sock.close()
+import support
 
 
 class Server:
+
     class Client:
-        def __init__(self, conn):
-            self.conn = conn
+        def __init__(self, sock, addr):
+            self.socket = sock
+            self.addr = addr
 
-        def recv(self) -> List[Optional[bytes]]:
+        def recv(self) -> list[bytes, ...] | None:
             def picking(n):
                 data = b''
                 while len(data) < n:
-                    packet = self.conn.recv(n - len(data))
+                    try:
+                        packet, _ = self.socket.recv(n - len(data))
+                    except socket.error as e:
+                        raise socket.error(f"Error receiving data: {e}")
                     if not packet:
                         return None
                     data += packet
                 return data
-            num_objects = struct.unpack('>I', picking(4))[0]
+
+            num_objects_data = picking(4)
+            if num_objects_data is None:
+                return None
+
+            num_objects = struct.unpack('>I', num_objects_data)[0]
             objects = []
             for _ in range(num_objects):
-                len_data = struct.unpack('>I', picking(4))[0]
-                obj_data = picking(len_data)
+                len_data = picking(4)
+                if len_data is None:
+                    return None
+
+                len_data_value = struct.unpack('>I', len_data)[0]
+                obj_data = picking(len_data_value)
+                if obj_data is None:
+                    return None
+
                 objects.append(obj_data)
             return objects
 
-        def send(self, objects: List[bytes]) -> None:
-            num_objects = len(objects)
+        def send(self, data: list[bytes, ...]) -> None:
+            num_objects = len(data)
+            len_objects = [len(obj) for obj in data]
             packet = struct.pack('>I', num_objects)
-            for obj in objects:
-                packet += struct.pack('>I', len(obj)) + obj
-            self.conn.sendall(packet)
+            for len_obj, obj in zip(len_objects, data):
+                packet += struct.pack('>I', len_obj) + obj
+            self.socket.sendall(packet)
 
-        def close(self):
-            self.conn.close()
+        def close(self) -> None:
+            self.socket.close()
 
         def __del__(self):
             self.close()
 
-    def __init__(self, family: Optional[int] = socket.AF_INET):
-        self.address = None
-        self.sock = socket.socket(family, socket.SOCK_STREAM)
-
-    def bind(self, param: tuple) -> None:
-        try:
-            self.sock.bind(param)
-        except TypeError as error:
-            raise error
-        except socket.gaierror as error:
-            raise error
+    def __init__(self, IP: str, TCP_port: int, UDP_port: int):
+        self.address = {
+            'TCP': (IP, TCP_port),
+            'UDP': (IP, UDP_port)
+        }
+        self.TCP = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.UDP = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.status = False
+
+    def start(self) -> None:
+        if not self.status:
+            self.UDP.bind(self.address['UDP'])
+            self.TCP.bind(self.address['TCP'])
+            self.TCP.listen()
+            self.status = True
         else:
-            self.address = param
+            raise support.ConnectionStatusError('Attempt to start an already working socket')
 
-    def accept(self) -> tuple:
-        conn, addr = self.sock.accept()
-        conn = self.Client(conn)
-        return conn, addr
-
-    def listen(self, backlog: Optional[int] = None) -> None:
-        if backlog is None:
-            self.sock.listen()
+    def recv(self) -> list[bytes, ...]:
+        if self.status:
+            def picking(n):
+                data = b''
+                while len(data) < n:
+                    try:
+                        packet, _ = self.UDP.recvfrom(n - len(data))
+                    except socket.error as e:
+                        print(f"Error receiving data: {e}")
+                        return None
+                    if not packet:
+                        return None
+                    data += packet
+                return data
+
+            num_objects_data = picking(4)
+            if num_objects_data is None:
+                return None
+
+            num_objects = struct.unpack('>I', num_objects_data)[0]
+            objects = []
+            for _ in range(num_objects):
+                len_data = picking(4)
+                if len_data is None:
+                    return None
+
+                len_data_value = struct.unpack('>I', len_data)[0]
+                obj_data = picking(len_data_value)
+                if obj_data is None:
+                    return None
+
+                objects.append(obj_data)
+            return objects
         else:
-            self.sock.listen(backlog)
+            raise support.ConnectionStatusError('Attempt to read data via UDP on an inactive socket')
 
-    def close(self):
-        self.sock.close()
+    def accept(self) -> Client:
+        if self.status:
+            sock, addr = self.TCP.accept()
+            return self.Client(sock, addr)
+        else:
+            raise support.ConnectionStatusError('Attempt to capture a client via TCP in an inactive socket')
 
     def __del__(self):
-        self.close()
+        self.TCP.close()
+        self.UDP.close()
```

