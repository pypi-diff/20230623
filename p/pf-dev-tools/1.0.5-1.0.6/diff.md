# Comparing `tmp/pf_dev_tools-1.0.5.tar.gz` & `tmp/pf_dev_tools-1.0.6.tar.gz`

## Comparing `pf_dev_tools-1.0.5.tar` & `pf_dev_tools-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.flake8
--rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.nova/Artwork
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.nova/Configuration.json
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/CoreConfig.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Exceptions.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Git.py
--rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/OpenFPGACore.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Paths.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/SCons.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Utils.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/__about__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clean.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clone.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Convert.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Delete.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/DryRun.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Eject.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Install.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Make.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Package.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Qfs.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Reverse.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/__main__.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/LICENSE
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.nova/Configuration.json
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/CoreConfig.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Git.py
+-rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/OpenFPGACore.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Paths.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/SCons.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Utils.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clean.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clone.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Convert.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Delete.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/DryRun.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Eject.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Install.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Make.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Package.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Qfs.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Reverse.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/LICENSE
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.5/.nova/Artwork` & `pf_dev_tools-1.0.6/.nova/Artwork`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/CoreConfig.py` & `pf_dev_tools-1.0.6/pfDevTools/CoreConfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,16 +112,13 @@
         return self._getConfigParam('Video', 'mirror')
 
     def fullPlatformName(self) -> str:
         return f'{self.authorName()}.{self.platformShortName()}'
 
     @classmethod
     def coreInstallVolumePath(cls) -> str:
-        volume_path: str = os.environ.get('PF_CORE_INSTALL_VOLUME', None)
-        if volume_path is None:
-            if platform == "darwin":
-                # -- On macOS, if PF_CORE_INSTALL_VOLUME is not defined, we default to POCKET
-                volume_path = os.path.join('/Volumes', 'POCKET')
-            else:
-                raise RuntimeError('PF_CORE_INSTALL_VOLUME is not defined in the environment.')
-
-        return volume_path
+        # -- On macOS, if PF_CORE_INSTALL_VOLUME is not defined, we default to POCKET
+        volume_name: str = os.environ.get('PF_CORE_INSTALL_VOLUME', "POCKET")
+        if platform == "darwin":
+            return os.path.join('/Volumes', volume_name)
+        else:
+            raise RuntimeError('PF_CORE_INSTALL_VOLUME is not defined in the environment.')
```

### Comparing `pf_dev_tools-1.0.5/pfDevTools/Git.py` & `pf_dev_tools-1.0.6/pfDevTools/Git.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/OpenFPGACore.py` & `pf_dev_tools-1.0.6/pfDevTools/OpenFPGACore.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 import shutil
 import pfDevTools
 
 from typing import List
 from pathlib import Path
+from distutils.dir_util import copy_tree
 
 
 # -- Classes
 class OpenFPGACore:
     """A SCons action to build on openFPGA core."""
 
     @classmethod
@@ -23,19 +24,38 @@
         if url is not None:
             command_line.append(url)
 
         tag = env.get('PF_CORE_TEMPLATE_REPO_TAG', None)
         if tag is not None:
             command_line.append(f'tag={tag}')
 
-        command_line.append(env['PF_BUILD_FOLDER'])
+        repo_folder = env['PF_CORE_TEMPLATE_FOLDER']
+        command_line.append(repo_folder)
+
+        if os.path.exists(repo_folder):
+            pfDevTools.Utils.deleteFolder(repo_folder, force_delete=True)
 
         pfDevTools.Clone(command_line).run()
 
     @classmethod
+    def _copyRepo(cls, target, source, env):
+        src_folder = os.path.expanduser(env['PF_CORE_TEMPLATE_REPO_FOLDER'])
+        dest_folder = env['PF_CORE_TEMPLATE_FOLDER']
+
+        if not os.path.exists(src_folder) or not os.path.isdir(src_folder):
+            raise RuntimeError(f'Cannot find \'{src_folder}\' to copy core tmeplate repo from.')
+
+        print(f'Copying core template repo from \'{src_folder}\'.')
+
+        if os.path.exists(dest_folder):
+            pfDevTools.Utils.deleteFolder(dest_folder, force_delete=True)
+
+        copy_tree(src_folder, dest_folder)
+
+    @classmethod
     def _runDockerCommand(cls, image: str, command: str, build_folder: str = None, quiet: bool = True):
         try:
             pfDevTools.Utils.requireCommand('docker')
 
             if not OpenFPGACore._dockerIsRunning():
                 raise RuntimeError('Docker engine does not seem to be running.')
 
@@ -164,28 +184,32 @@
     src_folder: str = env['PF_SRC_FOLDER']
 
     env.SetDefault(PF_BUILD_FOLDER='_build')
     build_folder: str = env['PF_BUILD_FOLDER']
 
     env.Replace(PF_CORE_CONFIG_FILE=config_file)
 
-    core_template_folder: str = os.path.join(build_folder, 'pfCoreTemplate')
+    core_template_folder: str = os.path.join(build_folder, '_core_template_repo')
+    env.Replace(PF_CORE_TEMPLATE_FOLDER=core_template_folder)
 
     core_fpga_folder: str = os.path.join(core_template_folder, 'src', 'fpga')
     env.Replace(PF_CORE_FPGA_FOLDER=core_fpga_folder)
 
     core_input_qsf_file = os.path.join(core_fpga_folder, 'ap_core.qsf')
     core_output_qsf_file = os.path.join(core_fpga_folder, 'pf_core.qsf')
 
     core_output_bitstream_file = os.path.join(core_fpga_folder, 'output_files', 'pf_core.rbf')
     env.Replace(PF_CORE_BITSTREAM_FILE=core_output_bitstream_file)
 
     dest_verilog_folder: str = os.path.join(core_fpga_folder, 'core')
 
-    env.Command(core_input_qsf_file, '', OpenFPGACore._cloneRepo)
+    if env.get('PF_CORE_TEMPLATE_REPO_FOLDER', None) is None:
+        env.Command(core_input_qsf_file, '', OpenFPGACore._cloneRepo)
+    else:
+        env.Command(core_input_qsf_file, '', OpenFPGACore._copyRepo)
 
     dest_verilog_files: List[str] = OpenFPGACore._searchSourceFiles(env, src_folder, dest_verilog_folder)
     extra_dest_files: List[str] = OpenFPGACore._addExtraFiles(env, src_folder, dest_verilog_folder, extra_files)
 
     env.Command(core_output_qsf_file, [core_input_qsf_file] + dest_verilog_files, OpenFPGACore._updateQsfFile)
     env.Command(core_output_bitstream_file, [core_output_qsf_file] + dest_verilog_files + extra_dest_files, OpenFPGACore._compileBitStream)
```

### Comparing `pf_dev_tools-1.0.5/pfDevTools/Utils.py` & `pf_dev_tools-1.0.6/pfDevTools/Utils.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/__init__.py` & `pf_dev_tools-1.0.6/pfDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clean.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clean.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clone.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clone.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,49 +12,46 @@
 # -- Classes
 class Clone:
     """A tool to clone the Github core template."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
+        self._destination_folder: str = None
         self._tag_name: str = None
         self._url: str = 'github.com/DidierMalenfant/pfCoreTemplate'
 
         nb_of_arguments = len(arguments)
-        if nb_of_arguments == 1 or nb_of_arguments == 3:
-            self._url: str = arguments[0]
-            nb_of_arguments -= 1
-            arguments = arguments[1:]
-
-        if nb_of_arguments == 0:
-            self._destination_folder: str = arguments[0]
-        elif nb_of_arguments == 2:
-            if arguments[0].startswith('tag='):
+        while nb_of_arguments:
+            if nb_of_arguments == 1:
+                self._destination_folder: str = arguments[0]
+            elif arguments[0].startswith('tag='):
                 self._tag_name = arguments[0][4:]
             else:
-                raise ArgumentError('Invalid cloning arguments. Maybe start with `pf --help?')
+                self._url: str = arguments[0]
+
+            nb_of_arguments -= 1
+            arguments = arguments[1:]
 
-            self._destination_folder: str = arguments[1]
-        else:
+        if self._destination_folder is None:
             raise ArgumentError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        repo_folder = os.path.join(self._destination_folder, 'pfCoreTemplate')
-        if os.path.exists(repo_folder):
-            pfDevTools.Utils.deleteFolder(repo_folder, force_delete=True)
+        if os.path.exists(self._destination_folder):
+            raise RuntimeError('Folder \'' + self._destination_folder + '\' already exists.')
 
-        print('Cloning core template in \'' + repo_folder + '\'.')
+        print(f'Cloning core template in \'{self._destination_folder}\'.')
 
-        pfDevTools.Git(self._url).cloneIn(repo_folder, self._tag_name)
+        pfDevTools.Git(self._url).cloneIn(self._destination_folder, self._tag_name)
 
-        git_folder = os.path.join(repo_folder, '.git')
+        git_folder = os.path.join(self._destination_folder, '.git')
         if os.path.exists(git_folder):
             pfDevTools.Utils.deleteFolder(git_folder, force_delete=True)
 
     @classmethod
     def name(cls) -> str:
         return 'clone'
 
     @classmethod
     def usage(cls) -> None:
-        print('   clone <url> <tag=name> dest_folder    - Clone repo at url, optionally at a given tag/branch.')
+        print('   clone <url> <tag=name> dest_folder    - Clone core template repo or repo at url optionally at a given tag/branch.')
         print('                                           (url defaults to pfCoreTemplate\'s repo if missing).')
```

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Convert.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Convert.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Delete.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Delete.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/DryRun.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/DryRun.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Eject.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Eject.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Install.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Install.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Make.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Make.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Package.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Package.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Qfs.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Qfs.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Reverse.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Reverse.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/pfDevTools/pfCommand/pfCommand.py` & `pf_dev_tools-1.0.6/pfDevTools/pfCommand/pfCommand.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/LICENSE` & `pf_dev_tools-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/README.md` & `pf_dev_tools-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 ```
 
 The following variables are currently supported:
 
 - `PF_DOCKER_IMAGE` - Name of the **Docker** image used to compile the core's bitstream. Defaults to `didiermalenfant/quartus:22.1-apple-silicon`.
 - `PF_SRC_FOLDER` - Root folder for all the **Verilog** source files for the project. Defaults to the folder where the `toml` config [file]](#core-config-file-format) is located.
 - `PF_BUILD_FOLDER` - Folder where intermediate build files are created. Defaults to `_build`.
+- `PF_CORE_TEMPLATE_REPO_URL` - Repo url to use instead of the default core template repo at `github.com/DidierMalenfant/pfCoreTemplate`.
+- `PF_CORE_TEMPLATE_REPO_TAG` - Repo tag to use to clone the core template repo.
+- `PF_CORE_TEMPLATE_REPO_FOLDER` - Path to a local core template folder to copy instead of cloning a repo.
 
 ### Core config file format
 
 Core configuration is done via a single `toml` file like this one:
 
 ```
 [Platform]
```

### Comparing `pf_dev_tools-1.0.5/pyproject.toml` & `pf_dev_tools-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.5/PKG-INFO` & `pf_dev_tools-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-dev-tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: A collection of tools for Project Freedom projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfDevTools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfDevTools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfDevTools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -165,14 +165,17 @@
 ```
 
 The following variables are currently supported:
 
 - `PF_DOCKER_IMAGE` - Name of the **Docker** image used to compile the core's bitstream. Defaults to `didiermalenfant/quartus:22.1-apple-silicon`.
 - `PF_SRC_FOLDER` - Root folder for all the **Verilog** source files for the project. Defaults to the folder where the `toml` config [file]](#core-config-file-format) is located.
 - `PF_BUILD_FOLDER` - Folder where intermediate build files are created. Defaults to `_build`.
+- `PF_CORE_TEMPLATE_REPO_URL` - Repo url to use instead of the default core template repo at `github.com/DidierMalenfant/pfCoreTemplate`.
+- `PF_CORE_TEMPLATE_REPO_TAG` - Repo tag to use to clone the core template repo.
+- `PF_CORE_TEMPLATE_REPO_FOLDER` - Path to a local core template folder to copy instead of cloning a repo.
 
 ### Core config file format
 
 Core configuration is done via a single `toml` file like this one:
 
 ```
 [Platform]
```

