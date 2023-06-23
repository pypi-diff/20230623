# Comparing `tmp/dockerlab-0.3.5.tar.gz` & `tmp/dockerlab-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerlab-0.3.5.tar", max compression
+gzip compressed data, was "dockerlab-0.3.7.tar", max compression
```

## Comparing `dockerlab-0.3.5.tar` & `dockerlab-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1073 2023-03-22 13:56:39.899119 dockerlab-0.3.5/LICENSE
--rw-r--r--   0        0        0     5070 2023-03-22 13:56:39.899119 dockerlab-0.3.5/README.md
--rw-r--r--   0        0        0       84 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/__init__.py
--rw-r--r--   0        0        0     1226 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/asset.py
--rw-r--r--   0        0        0       43 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/assets/.gitignore
--rw-r--r--   0        0        0     1546 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/assets/docker-compose.yml
--rw-r--r--   0        0        0     6239 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/assets/docker.py
--rwxr-xr-x   0        0        0     1608 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/assets/misc/init_workspace
--rw-r--r--   0        0        0     1872 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/assets/requirements.txt
--rw-r--r--   0        0        0     5023 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/cli.py
--rw-r--r--   0        0        0     1209 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/post_templates/default.txt
--rw-r--r--   0        0        0      318 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/post_templates/node.txt
--rw-r--r--   0        0        0     1500 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/post_templates/python.txt
--rw-r--r--   0        0        0     3047 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/template.py
--rw-r--r--   0        0        0     3493 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/README.md
--rw-r--r--   0        0        0      194 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/runtime_node_lts/Dockerfile
--rw-r--r--   0        0        0     1468 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/settting.py
--rw-r--r--   0        0        0     4544 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_base/Dockerfile
--rw-r--r--   0        0        0     4577 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_cuda_11_1/Dockerfile
--rw-r--r--   0        0        0     4468 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_cuda_11_7/Dockerfile
--rw-r--r--   0        0        0     4571 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_protein/Dockerfile
--rw-r--r--   0        0        0      493 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_pytorch_1_13/Dockerfile
--rw-r--r--   0        0        0      488 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/templates/workspace_pytorch_2_0/Dockerfile
--rw-r--r--   0        0        0     2294 2023-03-22 13:56:39.899119 dockerlab-0.3.5/dockerlab/utils.py
--rw-r--r--   0        0        0      477 2023-03-22 13:56:39.903119 dockerlab-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 dockerlab-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-08 09:00:58.887390 dockerlab-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4831 2023-04-11 06:49:49.518450 dockerlab-0.3.7/README.md
+-rw-r--r--   0        0        0       35 2023-06-23 02:10:29.294390 dockerlab-0.3.7/dockerlab/__init__.py
+-rw-r--r--   0        0        0     1226 2023-03-22 12:19:12.078158 dockerlab-0.3.7/dockerlab/asset.py
+-rw-r--r--   0        0        0       43 2023-03-15 13:02:22.919974 dockerlab-0.3.7/dockerlab/assets/.gitignore
+-rw-r--r--   0        0        0     1534 2023-04-15 12:34:28.706070 dockerlab-0.3.7/dockerlab/assets/docker-compose.yml
+-rw-r--r--   0        0        0     6386 2023-06-23 01:50:53.760930 dockerlab-0.3.7/dockerlab/assets/docker.py
+-rwxr-xr-x   0        0        0     1608 2023-03-22 08:50:55.864206 dockerlab-0.3.7/dockerlab/assets/misc/init_workspace
+-rw-r--r--   0        0        0     1872 2023-03-22 11:41:34.374529 dockerlab-0.3.7/dockerlab/assets/requirements.txt
+-rw-r--r--   0        0        0     5619 2023-04-11 06:45:22.077237 dockerlab-0.3.7/dockerlab/cli.py
+-rw-r--r--   0        0        0     1198 2023-04-15 12:32:08.444974 dockerlab-0.3.7/dockerlab/post_templates/default.txt
+-rw-r--r--   0        0        0      318 2023-03-21 10:22:18.340920 dockerlab-0.3.7/dockerlab/post_templates/node.txt
+-rw-r--r--   0        0        0     1500 2023-03-22 07:53:54.516620 dockerlab-0.3.7/dockerlab/post_templates/python.txt
+-rw-r--r--   0        0        0     3201 2023-04-15 11:22:30.799781 dockerlab-0.3.7/dockerlab/template.py
+-rw-r--r--   0        0        0     3876 2023-06-23 01:55:35.435053 dockerlab-0.3.7/dockerlab/templates/README.md
+-rw-r--r--   0        0        0      204 2023-04-15 11:46:28.517882 dockerlab-0.3.7/dockerlab/templates/runtime_node_lts/Dockerfile
+-rw-r--r--   0        0        0     1780 2023-06-23 01:54:23.053192 dockerlab-0.3.7/dockerlab/templates/settting.py
+-rw-r--r--   0        0        0     4544 2023-03-22 07:50:22.159814 dockerlab-0.3.7/dockerlab/templates/workspace_base/Dockerfile
+-rw-r--r--   0        0        0     4577 2023-03-20 12:51:22.275231 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_1/Dockerfile
+-rw-r--r--   0        0        0     4468 2023-06-23 01:54:00.258144 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_3/Dockerfile
+-rw-r--r--   0        0        0     4468 2023-03-20 12:51:22.268004 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_7/Dockerfile
+-rw-r--r--   0        0        0     4571 2023-03-21 12:01:20.782551 dockerlab-0.3.7/dockerlab/templates/workspace_protein/Dockerfile
+-rw-r--r--   0        0        0      493 2023-03-20 14:19:33.075541 dockerlab-0.3.7/dockerlab/templates/workspace_pytorch_1_13/Dockerfile
+-rw-r--r--   0        0        0      488 2023-03-20 14:19:33.075321 dockerlab-0.3.7/dockerlab/templates/workspace_pytorch_2_0/Dockerfile
+-rw-r--r--   0        0        0     2294 2023-03-22 12:19:37.232253 dockerlab-0.3.7/dockerlab/utils.py
+-rw-r--r--   0        0        0      593 2023-06-23 02:10:29.293458 dockerlab-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 dockerlab-0.3.7/PKG-INFO
```

### Comparing `dockerlab-0.3.5/LICENSE` & `dockerlab-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/README.md` & `dockerlab-0.3.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,115 +5,118 @@
 
 [![Package Building Status](https://img.shields.io/github/actions/workflow/status/hughplay/dockerlab/poetry-publish.yml?label=Package%20Build&style=flat-square)](https://github.com/hughplay/dockerlab/actions)
 [![pypi](https://img.shields.io/pypi/v/dockerlab?color=blue&label=pypi&style=flat-square)](https://pypi.org/project/dockerlab/)
 [![Image Building Status](https://img.shields.io/github/actions/workflow/status/hughplay/dockerlab/images-build.yml?label=Image%20Build&style=flat-square)](https://github.com/hughplay/dockerlab/actions)
 [![](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square&labelColor=gray)](#license)
 [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/engine/)
 
-*Build a docker container as your workspace.*
+*用Docker搭建你的工作区。*
+
 
 
 </div>
 
 <br>
 
-## Pre-requirements
+Read this in [English](README.en.md).
+
+## 环境要求
 
 - [Docker](https://docs.docker.com/engine/install)
 
 
-## Features
+## 特点
 
-- **Easy to use**: Just a few commands to build and start a docker container.
-- **Customizable**: You can customize the docker image and the python packages you want to install in the container.
-- **Reproducible**: You can build the same docker image on different machines. Say bye bye to the ["It works on my machine"](https://www.reddit.com/r/ProgrammerHumor/comments/70we66/it_works_on_my_machine/) problem.
-- **Convenient**: We made some convenient setups for you, including tools and functions:
-  - tools: [oh-my-zsh](https://ohmyz.sh/), [docker within docker](https://www.docker.com/blog/docker-can-now-run-within-docker/), [tmux](https://github.com/tmux/tmux/wiki), [lightvim](https://github.com/hughplay/lightvim)
-  - free of permission problems: same uid and gid as the host
-  - reversely mounting $HOME directory from container to host
-    - easy to share `~/.ssh` and `~/.gitconfig`
-    - files will not be lost even if the container is removed, e.g., zsh history, configuration files, model checkpoints, ...
-  - free of port mapping: sharing network with the host
-- **Pre-built Images**: We provide several basic [pre-built images](dockerlab/templates/) for quickly setting up your own workspace environment.
+- **易于使用**：只需几个命令即可构建和启动 Docker 容器。
+- **可定制**：可以自定义要安装在容器中的 Docker 镜像和 Python 包。
+- **可重现**：可以在不同的计算机上构建相同的 Docker 镜像。告别[“这在我的机器上可以运行”](https://www.reddit.com/r/ProgrammerHumor/comments/70we66/it_works_on_my_machine/)的问题。
+- **方便**：Dockerlab提供了一些方便的设置，包括工具和功能：
+  - 工具：[oh-my-zsh](https://ohmyz.sh/)，[docker within docker](https://www.docker.com/blog/docker-can-now-run-within-docker/)，[tmux](https://github.com/tmux/tmux/wiki)，[lightvim](https://github.com/hughplay/lightvim)
+  - 解决权限问题：与主机相同的 uid 和 gid。
+  - 将 $HOME 目录从容器反向挂载到主机
+    - 轻松共享 `~/.ssh` 和 `~/.gitconfig`
+    - 即使删除容器，配置文件也不会丢失，例如：zsh历史记录、配置文件、模型检查点等
+  - 解决端口映射问题：与主机共享网络
+- **预构建镜像**：Dockerlab提供了几个基本的[预构建镜像](dockerlab/templates/)，可快速设置工作区环境。
 
 
-## Quick Start
+## 快速开始
 
-**1. Install dockerlab**
+**1. 安装dockerlab**
 
-Install dockerlab with pip:
+用pip安装dockerlab：
 
 ```bash
 pip install dockerlab
 ```
 
-Or install the latest version from source:
+或者从源码安装最新版本：
 
 ```bash
 pip install git+https://github.com/hughplay/dockerlab.git
 ```
 
 
-**2. Setup a dockerlab project**
+**2. 设置dockerlab项目**
 
-Create a new dockerlab project:
+创建一个新的dockerlab项目：
 
 ```bash
 dockerlab new <project_name>
 ```
 
-Or init a dockerlab environment for the existing project:
+或者为现有项目初始化一个dockerlab环境：
 
 ```bash
 dockerlab init .
 ```
 
-This will setup a few files and directories, the structure is as follows:
+这将设置一些文件和目录，其结构如下：
 
 ```bash
 .
 ├── docker/
 │   ├── Dockerfile
 │   └── misc/
 ├── docker-compose.yml
 ├── docker.py
 └── .gitignore
 ```
 
 
-**3. DIY your own workspace environment**
+**3. 自定义工作环境**
 
-In general, you only need to modify `docker/Dockerfile` to customize your own workspace environment. Files you may care about:
+通常情况下，只需要修改`docker/Dockerfile`文件来自定义自己的工作环境。可能关心的文件:
 
-- `docker/Dockerfile`: The dockerfile for building the docker image.
-- `docker-compose.yml`: The docker-compose file for building the docker container.
-- `docker.py`: The python script for building and starting the container.
+- `docker/Dockerfile`: 用于构建docker镜像的dockerfile。
+- `docker-compose.yml`: 用于构建docker容器的docker-compose文件。
+- `docker.py`: 用于构建和启动容器的python脚本。
 
 
-We have prepared several templates and pre-built docker images for you. You can replace the default `docker/Dockerfile` with the template you like by running the following command:
+dockerlab准备了几个模板和预构建的docker镜像。可以通过运行以下命令将默认的`docker/Dockerfile`替换为需要的模板:
 
 ```bash
 dockerlab use <template_name>
 ```
 
-The available templates can be listed by `dockerlab ls`, and the details of each template can be found in [dockerlab/templates](dockerlab/templates).
+可用的模板可以通过 `dockerlab ls`列出，每个模板的详细信息可以在[dockerlab/templates](dockerlab/templates)找到。
 
-By default, the generated `docker/Dockerfile` will use pre-built docker images if there exists. You can also get the full dockerfile by running the following command:
+默认情况下，生成的`docker/Dockerfile`将使用预构建的docker镜像（如果存在）。也可以通过运行以下命令获取完整的dockerfile：
 
 ```bash
 dockerlab use <template_name> --full
 ```
 
-**4. Build and start the container**
+**4. 构建和启动容器**
 
 ```bash
 python docker.py startd
 ```
 
-When you first execute the above command, it will ask you to enter information related to the container and store them in `.env`. The example of prompt and the output are as follows:
+当你第一次执行上述命令时，它将要求你输入与容器相关的信息，并将它们存储在`.env`中。提示和输出示例如下：
 
 ```bash
 # prompts
 Give a project name [dockerlab]: dockerlab
 Code root to be mounted at /project [.]:
 Data root to be mounted at /data [data]:
 `/home/hongxin/code/dockerlab/data` does not exist in your machine. Create? [yes]:
@@ -131,16 +134,17 @@
   CODE_ROOT: .
   DATA_ROOT: /home/hongxin/code/dockerlab/data
   LOG_ROOT: /home/hongxin/code/dockerlab/log
   CONTAINER_HOME: /home/hongxin/code/dockerlab/container_home
   COMPOSE_PROJECT_NAME: dockerlab_hongxin
 ```
 
-**5. Get in the container and start your journey.**
+**5. 进入容器开启旅程**
+
 
 ```bash
 python docker.py
 ```
 
-## License
+## 许可证
 
-DockerLab is released under the [MIT license](LICENSE).
+Dockerlab使用[MIT许可证](LICENSE)。
```

### Comparing `dockerlab-0.3.5/dockerlab/asset.py` & `dockerlab-0.3.7/dockerlab/asset.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/assets/docker-compose.yml` & `dockerlab-0.3.7/dockerlab/assets/docker-compose.yml`

 * *Files 10% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 
     working_dir: /project
 
     # command: ["sleep", "infinity"]
     command: >
       bash -c
       "sudo rsync -a --stats --chown=${USER_NAME}:${USER_NAME} --ignore-existing
-      /${USER_NAME}_home_bak/ /home/${USER_NAME}
-      && . /home/${USER_NAME}/.bashrc
+      /${USER_NAME}_home_bak/ ${TARGET_HOME}
+      && . ${TARGET_HOME}/.bashrc
       && sleep infinity"
 
     # mount the <directory in host> to the <directory in container>
     # add more mounts here if you need
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock # run docker in docker
       - ${CODE_ROOT}:/project
       - ${DATA_ROOT}:/data
       - ${LOG_ROOT}:/log
       - type: bind
         source: ${CONTAINER_HOME}
-        target: /home/${USER_NAME}
+        target: ${TARGET_HOME}
```

### Comparing `dockerlab-0.3.5/dockerlab/assets/docker.py` & `dockerlab-0.3.7/dockerlab/assets/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,18 @@
                     f"`{container_home}` does not exist in your machine. Create?",
                     default="yes",
                 )
                 == "yes"
             ):
                 container_home.mkdir(parents=True, exist_ok=True)
         e["CONTAINER_HOME"] = str(container_home)
+        if e["USER_NAME"] != "root":
+            e["TARGET_HOME"] = f"/home/{e['USER_NAME']}"
+        else:
+            e["TARGET_HOME"] = "/root"
 
     e["COMPOSE_PROJECT_NAME"] = f"{e['PROJECT']}_{e['USER_NAME']}".lower()
     e.save()
 
     if verbose:
         print(f"Your setting ({env_path}):\n{e}\n")
     return e
```

### Comparing `dockerlab-0.3.5/dockerlab/assets/misc/init_workspace` & `dockerlab-0.3.7/dockerlab/assets/misc/init_workspace`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/assets/requirements.txt` & `dockerlab-0.3.7/dockerlab/assets/requirements.txt`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/cli.py` & `dockerlab-0.3.7/dockerlab/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,19 @@
     write_file(
         project_dir / TARGET_DOCKER_DIR / "Dockerfile",
         assemble_template(template, full, post),
     )
     print(
         f"Project {name} created. Build the container and get started with:"
         f"\n> cd {name}"
+        "\n\n# Customize Dockerfile or use default templates."
+        "\n  # List available templates. Details can be found at: https://github.com/hughplay/dockerlab/tree/main/dockerlab/templates"
+        "\n  > dockerlab ls"
+        "\n  # Use template."
+        "\n  > dockerlab use <template>"
         "\n\n# Build and start the container."
         "\n> python docker.py startd"
         "\n\n# Get into the container."
         "\n> python docker.py"
     )
 
 
@@ -101,14 +106,19 @@
     copy_targets(get_copy_list(template, project_dir))
     write_file(
         project_dir / TARGET_DOCKER_DIR / "Dockerfile",
         assemble_template(template, full, post),
     )
     print(
         "Project initialized."
+        "\n\n# Customize Dockerfile or use default templates."
+        "\n  # List available templates. Details can be found at: https://github.com/hughplay/dockerlab/tree/main/dockerlab/templates"
+        "\n  > dockerlab ls"
+        "\n  # Use template."
+        "\n  > dockerlab use <template>"
         "\n\n# Build and start the container."
         "\n> python docker.py startd"
         "\n\n# Get into the container."
         "\n> python docker.py"
     )
```

### Comparing `dockerlab-0.3.5/dockerlab/post_templates/default.txt` & `dockerlab-0.3.7/dockerlab/post_templates/default.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Copy installed configuration files from root to user
 COPY misc/init_workspace /usr/local/bin
 RUN chmod +x /usr/local/bin/init_workspace
 RUN /usr/local/bin/init_workspace --user ${USER_NAME} --home /home/${USER_NAME}
 
 
 # backup $HOME for reverse mounting $HOME
-RUN rsync -a /home/${USER_NAME}/ /${USER_NAME}_home_bak
+RUN rsync -a ${HOME}/ /${USER_NAME}_home_bak
 
 
 # Switch to the created user
 USER ${USER_NAME}
 
 
 # Set working directory to /project
```

### Comparing `dockerlab-0.3.5/dockerlab/post_templates/python.txt` & `dockerlab-0.3.7/dockerlab/post_templates/python.txt`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/template.py` & `dockerlab-0.3.7/dockerlab/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from pathlib import Path
 from typing import List
 
-from .templates.settting import (
-    DEFAULT_TEMPLATE,
-    PREBUILT_TEMPLATES,
-    TEMPLATE_SETTING,
-)
+from .templates.settting import DEFAULT_TEMPLATE, TEMPLATE_SETTING
 
 TEMPLATES_DIR = Path(__file__).parent.resolve() / "templates"
 POST_TEMPLATES_DIR = Path(__file__).parent.resolve() / "post_templates"
 OFFICIAL_HUB = "deepbase/dockerlab"
 IGNORE_TEMPLATE_NAME = ["__pycache__"]
 
 
@@ -23,20 +19,23 @@
     templates = [
         (t.name, t)
         for t in TEMPLATES_DIR.iterdir()
         if t.is_dir() and t.name not in IGNORE_TEMPLATE_NAME
     ]
     templates.sort(key=lambda x: (not x[1].is_symlink(), x[0]))
     if verbose:
-        print("Available templates:")
+        print("Available templates (* is default):")
         for name, t in templates:
-            if name == DEFAULT_TEMPLATE:
-                print(f"  - {name} (default)")
-            else:
-                print(f"  - {name}")
+            str_template = (
+                f"  {'*' if name == DEFAULT_TEMPLATE else '-'} {name}"
+            )
+            cuda = TEMPLATE_SETTING[name].get("cuda", False)
+            if cuda:
+                str_template += f" [cuda {cuda}]"
+            print(str_template)
     return [name for name, _ in templates]
 
 
 def get_post_templates(verbose=False):
     # iterate files with .txt extension
     templates = [
         t.stem
@@ -50,19 +49,20 @@
     return templates
 
 
 def assemble_template(
     name: str, full: bool = False, post_templates: List[str] = None
 ):
     name = resolve_template(name)
+    templates = get_templates()
 
-    if name in PREBUILT_TEMPLATES:
-        temp_text = f"FROM {PREBUILT_TEMPLATES[name]}"
+    prebuilt_image = TEMPLATE_SETTING[name].get("prebuilt", False)
+    if prebuilt_image:
+        temp_text = f"FROM {prebuilt_image}"
     else:
-        templates = get_templates()
         if name not in templates:
             raise ValueError(f"Template {name} not found.")
         temp = TEMPLATES_DIR / name / "Dockerfile"
         temp_text = temp.read_text().strip()
 
     if full:
         temp_text = extend_template(temp_text, templates)
```

### Comparing `dockerlab-0.3.5/dockerlab/templates/README.md` & `dockerlab-0.3.7/dockerlab/templates/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 [![](http://github-actions.40ants.com/hughplay/dockerlab/matrix.svg)](https://github.com/hughplay/dockerlab?only=images-build)
 
 
 | Name | Description | Dockerfile |
 | --- | --- | --- |
-| `FROM workspace_base` | Image includes: <ul><li>Ubuntu 20.04</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
-| `FROM workspace_cuda_11_1` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.1.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
-| `FROM workspace_cuda_11_7` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.7.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
-| `FROM workspace_pytorch_1_13` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.4.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>Pytorch 1.13.1</li><li>Pytorch Lightning 1.9.4</li></ul> | [Dockerfile](workspace_pytorch_1_13/Dockerfile) |
-| `FROM workspace_pytorch_2_0` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.4.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>Pytorch 2.0</li><li>Pytorch Lightning 2.0.0</li></ul> | [Dockerfile](workspace_pytorch_2_0/Dockerfile) |
-| `FROM workspace_protein` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.1.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>FFindex</li><li>CCMpred</li><li>HH-suite3</li><li>HMMER</li><li>BLAST</li><li>MMseqs2</li><li>Align toools: Clustal-Omega, EMBOSS, ProbCons, Kalign 3</li></ul> | [Dockerfile](workspace_protein/Dockerfile) |
-| `FROM runtime_node` | Image includes: <ul><li>Node LTS</li><li>yrm</li></ul> | [Dockerfile](runtime_node/Dockerfile) |
+| `workspace_base` | Image includes: <ul><li>Ubuntu 20.04</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
+| `workspace_cuda_11_1` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.1.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
+| `workspace_cuda_11_3` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.3.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_3/Dockerfile) |
+| `workspace_cuda_11_7` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.7.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul></ul> | [Dockerfile](workspace_cuda_11_1/Dockerfile) |
+| `workspace_pytorch_1_13` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.4.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>Pytorch 1.13.1</li><li>Pytorch Lightning 1.9.4</li></ul> | [Dockerfile](workspace_pytorch_1_13/Dockerfile) |
+| `workspace_pytorch_2_0` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.4.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>Pytorch 2.0</li><li>Pytorch Lightning 2.0.0</li></ul> | [Dockerfile](workspace_pytorch_2_0/Dockerfile) |
+| `workspace_protein` | Image includes: <ul><li>Ubuntu 20.04</li><li>CUDA 11.1.1</li><li>cuDNN 8</li><li>Miniconda (Python 3.8)</li><li>ZSH (Oh-My-ZSH)</li><li>Docker (docker in docker)</li><li>Tmux (tmux-config)</li><li>Common used fonts for plotting</li><ul><li>Arial (recommended)</li><li>Helvetica</li><li>Palatino Linotype</li><li>Times New Roman</li></ul><li>FFindex</li><li>CCMpred</li><li>HH-suite3</li><li>HMMER</li><li>BLAST</li><li>MMseqs2</li><li>Align toools: Clustal-Omega, EMBOSS, ProbCons, Kalign 3</li></ul> | [Dockerfile](workspace_protein/Dockerfile) |
+| `runtime_node` | Image includes: <ul><li>Node LTS</li><li>yrm</li></ul> | [Dockerfile](runtime_node/Dockerfile) |
```

### Comparing `dockerlab-0.3.5/dockerlab/templates/workspace_base/Dockerfile` & `dockerlab-0.3.7/dockerlab/templates/workspace_base/Dockerfile`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/templates/workspace_cuda_11_1/Dockerfile` & `dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_1/Dockerfile`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/templates/workspace_cuda_11_7/Dockerfile` & `dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_7/Dockerfile`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/templates/workspace_protein/Dockerfile` & `dockerlab-0.3.7/dockerlab/templates/workspace_protein/Dockerfile`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/dockerlab/utils.py` & `dockerlab-0.3.7/dockerlab/utils.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.5/PKG-INFO` & `dockerlab-0.3.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerlab
-Version: 0.3.5
+Version: 0.3.7
 Summary: Build a docker container as your workspace.
 Home-page: https://github.com/hughplay/dockerlab
 License: MIT
 Author: Mr.Blue
 Author-email: silverhugh.77@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,115 +24,118 @@
 
 [![Package Building Status](https://img.shields.io/github/actions/workflow/status/hughplay/dockerlab/poetry-publish.yml?label=Package%20Build&style=flat-square)](https://github.com/hughplay/dockerlab/actions)
 [![pypi](https://img.shields.io/pypi/v/dockerlab?color=blue&label=pypi&style=flat-square)](https://pypi.org/project/dockerlab/)
 [![Image Building Status](https://img.shields.io/github/actions/workflow/status/hughplay/dockerlab/images-build.yml?label=Image%20Build&style=flat-square)](https://github.com/hughplay/dockerlab/actions)
 [![](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square&labelColor=gray)](#license)
 [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/engine/)
 
-*Build a docker container as your workspace.*
+*用Docker搭建你的工作区。*
+
 
 
 </div>
 
 <br>
 
-## Pre-requirements
+Read this in [English](README.en.md).
+
+## 环境要求
 
 - [Docker](https://docs.docker.com/engine/install)
 
 
-## Features
+## 特点
 
-- **Easy to use**: Just a few commands to build and start a docker container.
-- **Customizable**: You can customize the docker image and the python packages you want to install in the container.
-- **Reproducible**: You can build the same docker image on different machines. Say bye bye to the ["It works on my machine"](https://www.reddit.com/r/ProgrammerHumor/comments/70we66/it_works_on_my_machine/) problem.
-- **Convenient**: We made some convenient setups for you, including tools and functions:
-  - tools: [oh-my-zsh](https://ohmyz.sh/), [docker within docker](https://www.docker.com/blog/docker-can-now-run-within-docker/), [tmux](https://github.com/tmux/tmux/wiki), [lightvim](https://github.com/hughplay/lightvim)
-  - free of permission problems: same uid and gid as the host
-  - reversely mounting $HOME directory from container to host
-    - easy to share `~/.ssh` and `~/.gitconfig`
-    - files will not be lost even if the container is removed, e.g., zsh history, configuration files, model checkpoints, ...
-  - free of port mapping: sharing network with the host
-- **Pre-built Images**: We provide several basic [pre-built images](dockerlab/templates/) for quickly setting up your own workspace environment.
+- **易于使用**：只需几个命令即可构建和启动 Docker 容器。
+- **可定制**：可以自定义要安装在容器中的 Docker 镜像和 Python 包。
+- **可重现**：可以在不同的计算机上构建相同的 Docker 镜像。告别[“这在我的机器上可以运行”](https://www.reddit.com/r/ProgrammerHumor/comments/70we66/it_works_on_my_machine/)的问题。
+- **方便**：Dockerlab提供了一些方便的设置，包括工具和功能：
+  - 工具：[oh-my-zsh](https://ohmyz.sh/)，[docker within docker](https://www.docker.com/blog/docker-can-now-run-within-docker/)，[tmux](https://github.com/tmux/tmux/wiki)，[lightvim](https://github.com/hughplay/lightvim)
+  - 解决权限问题：与主机相同的 uid 和 gid。
+  - 将 $HOME 目录从容器反向挂载到主机
+    - 轻松共享 `~/.ssh` 和 `~/.gitconfig`
+    - 即使删除容器，配置文件也不会丢失，例如：zsh历史记录、配置文件、模型检查点等
+  - 解决端口映射问题：与主机共享网络
+- **预构建镜像**：Dockerlab提供了几个基本的[预构建镜像](dockerlab/templates/)，可快速设置工作区环境。
 
 
-## Quick Start
+## 快速开始
 
-**1. Install dockerlab**
+**1. 安装dockerlab**
 
-Install dockerlab with pip:
+用pip安装dockerlab：
 
 ```bash
 pip install dockerlab
 ```
 
-Or install the latest version from source:
+或者从源码安装最新版本：
 
 ```bash
 pip install git+https://github.com/hughplay/dockerlab.git
 ```
 
 
-**2. Setup a dockerlab project**
+**2. 设置dockerlab项目**
 
-Create a new dockerlab project:
+创建一个新的dockerlab项目：
 
 ```bash
 dockerlab new <project_name>
 ```
 
-Or init a dockerlab environment for the existing project:
+或者为现有项目初始化一个dockerlab环境：
 
 ```bash
 dockerlab init .
 ```
 
-This will setup a few files and directories, the structure is as follows:
+这将设置一些文件和目录，其结构如下：
 
 ```bash
 .
 ├── docker/
 │   ├── Dockerfile
 │   └── misc/
 ├── docker-compose.yml
 ├── docker.py
 └── .gitignore
 ```
 
 
-**3. DIY your own workspace environment**
+**3. 自定义工作环境**
 
-In general, you only need to modify `docker/Dockerfile` to customize your own workspace environment. Files you may care about:
+通常情况下，只需要修改`docker/Dockerfile`文件来自定义自己的工作环境。可能关心的文件:
 
-- `docker/Dockerfile`: The dockerfile for building the docker image.
-- `docker-compose.yml`: The docker-compose file for building the docker container.
-- `docker.py`: The python script for building and starting the container.
+- `docker/Dockerfile`: 用于构建docker镜像的dockerfile。
+- `docker-compose.yml`: 用于构建docker容器的docker-compose文件。
+- `docker.py`: 用于构建和启动容器的python脚本。
 
 
-We have prepared several templates and pre-built docker images for you. You can replace the default `docker/Dockerfile` with the template you like by running the following command:
+dockerlab准备了几个模板和预构建的docker镜像。可以通过运行以下命令将默认的`docker/Dockerfile`替换为需要的模板:
 
 ```bash
 dockerlab use <template_name>
 ```
 
-The available templates can be listed by `dockerlab ls`, and the details of each template can be found in [dockerlab/templates](dockerlab/templates).
+可用的模板可以通过 `dockerlab ls`列出，每个模板的详细信息可以在[dockerlab/templates](dockerlab/templates)找到。
 
-By default, the generated `docker/Dockerfile` will use pre-built docker images if there exists. You can also get the full dockerfile by running the following command:
+默认情况下，生成的`docker/Dockerfile`将使用预构建的docker镜像（如果存在）。也可以通过运行以下命令获取完整的dockerfile：
 
 ```bash
 dockerlab use <template_name> --full
 ```
 
-**4. Build and start the container**
+**4. 构建和启动容器**
 
 ```bash
 python docker.py startd
 ```
 
-When you first execute the above command, it will ask you to enter information related to the container and store them in `.env`. The example of prompt and the output are as follows:
+当你第一次执行上述命令时，它将要求你输入与容器相关的信息，并将它们存储在`.env`中。提示和输出示例如下：
 
 ```bash
 # prompts
 Give a project name [dockerlab]: dockerlab
 Code root to be mounted at /project [.]:
 Data root to be mounted at /data [data]:
 `/home/hongxin/code/dockerlab/data` does not exist in your machine. Create? [yes]:
@@ -150,17 +153,18 @@
   CODE_ROOT: .
   DATA_ROOT: /home/hongxin/code/dockerlab/data
   LOG_ROOT: /home/hongxin/code/dockerlab/log
   CONTAINER_HOME: /home/hongxin/code/dockerlab/container_home
   COMPOSE_PROJECT_NAME: dockerlab_hongxin
 ```
 
-**5. Get in the container and start your journey.**
+**5. 进入容器开启旅程**
+
 
 ```bash
 python docker.py
 ```
 
-## License
+## 许可证
 
-DockerLab is released under the [MIT license](LICENSE).
+Dockerlab使用[MIT许可证](LICENSE)。
```

