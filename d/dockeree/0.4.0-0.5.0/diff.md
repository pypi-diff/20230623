# Comparing `tmp/dockeree-0.4.0.tar.gz` & `tmp/dockeree-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockeree-0.4.0.tar", max compression
+gzip compressed data, was "dockeree-0.5.0.tar", max compression
```

## Comparing `dockeree-0.4.0.tar` & `dockeree-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    60340 2022-08-01 01:57:38.508534 dockeree-0.4.0/LICENSE
--rw-r--r--   0        0        0     6679 2022-08-01 01:57:38.508534 dockeree-0.4.0/dockeree/__init__.py
--rw-r--r--   0        0        0    25062 2022-08-01 01:57:38.508534 dockeree-0.4.0/dockeree/builder.py
--rw-r--r--   0        0        0     1330 2022-08-01 01:57:38.508534 dockeree-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      605 2022-08-01 01:57:38.508534 dockeree-0.4.0/readme.md
--rw-r--r--   0        0        0     1410 2022-08-01 01:58:01.325155 dockeree-0.4.0/setup.py
--rw-r--r--   0        0        0     1519 2022-08-01 01:58:01.325513 dockeree-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    60340 2023-06-23 08:04:28.689015 dockeree-0.5.0/LICENSE
+-rw-r--r--   0        0        0      488 2023-06-23 08:04:28.689015 dockeree-0.5.0/README.md
+-rw-r--r--   0        0        0     6799 2023-06-23 08:04:28.689015 dockeree-0.5.0/dockeree/__init__.py
+-rw-r--r--   0        0        0    24961 2023-06-23 08:04:28.689015 dockeree-0.5.0/dockeree/builder.py
+-rw-r--r--   0        0        0     1335 2023-06-23 08:04:28.689015 dockeree-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 dockeree-0.5.0/PKG-INFO
```

### Comparing `dockeree-0.4.0/LICENSE` & `dockeree-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockeree-0.4.0/dockeree/__init__.py` & `dockeree-0.5.0/dockeree/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,82 +35,86 @@
             for tag in image.tags:
                 data.append(
                     {
                         "repository": repository,
                         "tag": tag.split(":")[1],
                         "image_id": image_id,
                         "created": created,
-                        "size": size
+                        "size": size,
                     }
                 )
         else:
             data.append(
                 {
                     "repository": repository,
                     "tag": "<none>",
                     "image_id": image_id,
                     "created": created,
-                    "size": size
+                    "size": size,
                 }
             )
     frame = pd.DataFrame(data)
     frame.created = pd.to_datetime(frame.created)
     return frame
 
 
 def containers() -> pd.DataFrame:
-    """Return Docker containers as a pandas DataFrame.
-    """
+    """Return Docker containers as a pandas DataFrame."""
     data = [
         (
             cont.short_id,
             cont,
             cont.image.tags[0] if cont.image.tags else cont.image.short_id[7:],
             cont.attrs["Config"]["Cmd"],
             cont.attrs["Created"],
             cont.status,
             cont.ports,
             cont.name,
-        ) for cont in docker.from_env().containers.list(all=True)
+        )
+        for cont in docker.from_env().containers.list(all=True)
     ]
     columns = [
-        "container_id", "container_obj", "image", "command", "created", "status",
-        "ports", "name"
+        "container_id",
+        "container_obj",
+        "image",
+        "command",
+        "created",
+        "status",
+        "ports",
+        "name",
     ]
     return pd.DataFrame(data, columns=columns)
 
 
 def remove(aggressive: bool = False, choice: str = "") -> None:
-    """Remove exited Docker containers and images without tags.
-    """
+    """Remove exited Docker containers and images without tags."""
     docker.from_env().containers.prune()
     failures = remove_images(tag="none", aggressive=aggressive, choice=choice)
     if failures:
         logger.error(
             "Failed to remove the following Docker images:\n{}", "\n".join(failures)
         )
 
 
 def pull():
-    """Automatically pull all valid images.
-    """
+    """Automatically pull all valid images."""
     client = docker.from_env()
     imgs = images()
     imgs = imgs[imgs.repository != "<None>" & imgs.tag != "<None>"]
     for _, (repo, tag, *_) in imgs.iterrows():
         client.images.pull(repo, tag)
 
 
 def remove_images(
     id_: str = "",
     name: str = "",
     tag: str = "",
     aggressive: bool = False,
     frame: Union[pd.DataFrame, None] = None,
-    choice: str = ""
+    choice: str = "",
 ) -> list[str]:
     """Remove specified Docker images.
     :param id_: The id of the image to remove.
     :param name: A (regex) pattern of names of images to remove.
     :param tag: Remove images whose tags containing specified tag.
     :return: A list of images failed to be removed.
     """
@@ -123,17 +127,22 @@
     if name:
         frames.append(imgs[imgs.repository.str.contains(name, case=False)])
     if tag:
         frames.append(imgs[imgs.tag.str.contains(tag, case=False)])
     if aggressive:
         frames.append(imgs[imgs.tag.str.contains(r"[a-z]*_?\d{4,}", case=False)])
         frames.append(
-            imgs[~imgs.tag.str.contains(r"\d{4,}")].groupby("image_id").apply(  # pylint: disable=E1101
-            lambda frame: frame.query("tag == 'next'") if frame.shape[0] > 1 else None
-        ))
+            imgs[~imgs.tag.str.contains(r"\d{4,}")]
+            .groupby("image_id")
+            .apply(  # pylint: disable=E1101
+                lambda frame: frame.query("tag == 'next'")
+                if frame.shape[0] > 1
+                else None
+            )
+        )
     return _remove_images_frame(pd.concat(frames, ignore_index=True), choice=choice)
 
 
 def _remove_images_frame(imgs, choice: str = "") -> list[str]:
     if imgs.empty:
         return []
     imgs = imgs.drop_duplicates().sort_values("created", ascending=False)
```

### Comparing `dockeree-0.4.0/dockeree/builder.py` & `dockeree-0.5.0/dockeree/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,24 +51,27 @@
     :param tag: The tag of the Docker image to push.
     :return: The time (in seconds) used to push the Docker image.
     """
     logger.info("Pushing Docker image {}:{} ...", repo, tag)
     time_begin = time.perf_counter_ns()
     try:
         retry(
-            lambda: sp.run(f"docker push {repo}:{tag}", shell=True, check=True),
-            times=3
+            lambda: sp.run(f"docker push {repo}:{tag}", shell=True, check=True), times=3
         )
         return DockerActionResult(
-            True, "", repo, tag, "push", (time.perf_counter_ns() - time_begin) / 1E9
+            True, "", repo, tag, "push", (time.perf_counter_ns() - time_begin) / 1e9
         )
     except Exception as err:
         return DockerActionResult(
-            False, str(err), repo, tag, "push",
-            (time.perf_counter_ns() - time_begin) / 1E9
+            False,
+            str(err),
+            repo,
+            tag,
+            "push",
+            (time.perf_counter_ns() - time_begin) / 1e9,
         )
 
 
 def _ignore_socket(dir_, files):
     dir_ = Path(dir_)
     return [file for file in files if (dir_ / file).is_socket()]
 
@@ -104,45 +107,45 @@
     if Path(kaniko).is_file():
         return kaniko
     return ""
 
 
 @dataclass(frozen=True)
 class Node:
-    """A class similar to DockerImage for simplifying code.
-    """
+    """A class similar to DockerImage for simplifying code."""
+
     git_url: str
     branch: str
 
     def __str__(self):
         rindex = self.git_url.rindex("/")
         # HTTP urls, e.g., https://github.com/dclong/docker-jupyterhub-ds
         index = self.git_url.rfind("/", 0, rindex)
         if index < 0:
             # SSH urls, e.g., git@github.com:dclong/docker-jupyterhub-ds
             index = self.git_url.rindex(":", 0, rindex)
-        return self.git_url[(index + 1):] + f"<{self.branch}>"
+        return self.git_url[(index + 1) :] + f"<{self.branch}>"
 
 
 DockerActionResult = namedtuple(
     "DockerActionResult", ["succeed", "err_msg", "image", "tag", "action", "seconds"]
 )
 
 
 class DockerImage:
-    """Class representing a Docker Image.
-    """
+    """Class representing a Docker Image."""
+
     DOCKERFILE = "Dockerfile"
 
     def __init__(
         self,
         git_url: str,
         branch: str = "dev",
         branch_fallback: str = "dev",
-        repo_path: Optional[dict[str, str]] = None
+        repo_path: Optional[dict[str, str]] = None,
     ):
         """Initialize a DockerImage object.
 
         :param git_url: URL of the remote Git repository.
         :param branch: The branch of the GitHub repository to use.
         """
         self._git_url = git_url[:-4] if git_url.endswith(".git") else git_url
@@ -151,43 +154,43 @@
         self._repo_path = {} if repo_path is None else repo_path
         self._path = None
         self._name = ""
         self._base_image = ""
         self._git_url_base = ""
 
     def is_root(self) -> bool:
-        """Check whether this DockerImage is a root DockerImage.
-        """
+        """Check whether this DockerImage is a root DockerImage."""
         return not self._git_url_base
 
     def clone_repo(self) -> None:
         """Clone the Git repository to a local directory.
 
         :param repo_branch: A dick containing mapping of git_url to its local path.
         """
         if self._path:
             return
         if self._git_url in self._repo_path:
             self._path = self._repo_path[self._git_url]
             repo = pygit2.Repository(self._path)
             logger.info(
-                "{} has already been cloned into {} previously.", self._git_url,
-                self._path
+                "{} has already been cloned into {} previously.",
+                self._git_url,
+                self._path,
             )
         else:
             self._path = Path(tempfile.mkdtemp())
             logger.info("Cloning {} into {}", self._git_url, self._path)
             repo = pygit2.clone_repository(self._git_url, self._path)
             self._repo_path[self._git_url] = self._path
         self._checkout_branch(repo)
         self._parse_dockerfile()
 
     def _checkout_branch(self, repo) -> None:
         """Checkout the branch self._branch from repo if the branch exists.
-            Otherwise, create a new branch named self._branch in repo and checkout it.
+        Otherwise, create a new branch named self._branch in repo and checkout it.
         """
         repo.reset(repo.head.peel().oid, pygit2.GIT_RESET_HARD)  # pylint: disable=E1101
         if repo.branches.get(self._branch) is None:
             for ref in [
                 f"refs/remotes/origin/{self._branch}",
                 f"refs/heads/{self._branch_fallback}",
                 f"refs/remotes/origin/{self._branch_fallback}",
@@ -224,29 +227,31 @@
         :param repo_branch: A set-like collection containing tuples of (git_url, branch).
         :param repo_branch: A dick containing mapping of git_url to its local path.
         :return: A deque containing dependency images.
         """
         self.clone_repo()
         deps = deque([self])
         obj = self
-        while (obj._git_url_base, obj._branch) not in repo_branch:  # pylint: disable=W0212
+        while (
+            obj._git_url_base,
+            obj._branch,
+        ) not in repo_branch:  # pylint: disable=W0212
             if not obj._git_url_base:  # pylint: disable=W0212
                 break
             obj = obj.base_image()
             deps.appendleft(obj)
         return deps
 
     def base_image(self) -> DockerImage:
-        """Get the base DockerImage of this DockerImage.
-        """
+        """Get the base DockerImage of this DockerImage."""
         image = DockerImage(
             git_url=self._git_url_base,
             branch=self._branch,
             branch_fallback=self._branch_fallback,
-            repo_path=self._repo_path
+            repo_path=self._repo_path,
         )
         image.clone_repo()
         return image
 
     def _copy_ssh(self, copy_ssh_to: str):
         if copy_ssh_to:
             ssh_src = Path.home() / ".ssh"
@@ -272,15 +277,15 @@
         :param tags: The tags of the Docker image to build.
             If None (default), then it is determined by the branch name.
             When the branch is master the "latest" tag is used,
             otherwise the next tag is used.
             If an empty string is specifed for tags,
             it is also treated as the latest tag.
         :param copy_ssh_to: If True, SSH keys are copied into a directory named ssh
-            under the current local Git repository. 
+            under the current local Git repository.
         :param builder: The tool to use to build Docker images.
         :return: A tuple of the format (image_name_built, tag_built, time_taken, "build").
         """
         time_begin = time.perf_counter_ns()
         self.clone_repo()
         self._copy_ssh(copy_ssh_to)
         tags = _reg_tag(tags, self._branch)
@@ -291,23 +296,24 @@
         images = docker.from_env().images
         try:
             images.remove(image_tag, force=True)
         except:
             pass
         try:
             if builder == "docker":
-                for msg in docker.APIClient(base_url="unix://var/run/docker.sock"
-                                           ).build(
-                                               path=str(self._path),
-                                               tag=image_tag,
-                                               rm=True,
-                                               pull=self.is_root(),
-                                               cache_from=None,
-                                               decode=True
-                                           ):
+                for msg in docker.APIClient(
+                    base_url="unix://var/run/docker.sock"
+                ).build(
+                    path=str(self._path),
+                    tag=image_tag,
+                    rm=True,
+                    pull=self.is_root(),
+                    cache_from=None,
+                    decode=True,
+                ):
                     if "stream" in msg:
                         print(f"[{image_tag}] {msg['stream']}", end="")
                 # add additional tags for the image
                 image = images.get(image_tag)
                 for tag in tags[1:]:
                     image.tag(self._name, tag, force=True)
             elif builder == "/kaniko/executor":
@@ -325,43 +331,43 @@
                 succeed=False,
                 err_msg="\n".join(
                     line.get("stream", line.get("error")) for line in err.build_log
                 ),
                 image=self._name,
                 tag="",
                 action="build",
-                seconds=(time.perf_counter_ns() - time_begin) / 1E9,
+                seconds=(time.perf_counter_ns() - time_begin) / 1e9,
             )
         except docker.errors.ImageNotFound:
             return DockerActionResult(
                 succeed=False,
                 err_msg="",
                 image=self._name,
                 tag="",
                 action="build",
-                seconds=(time.perf_counter_ns() - time_begin) / 1E9,
+                seconds=(time.perf_counter_ns() - time_begin) / 1e9,
             )
         finally:
             self._remove_ssh(copy_ssh_to)
         if self._test_built_image():
             return DockerActionResult(
                 succeed=True,
                 err_msg="",
                 image=self._name,
                 tag=tag0,
                 action="build",
-                seconds=(time.perf_counter_ns() - time_begin) / 1E9,
+                seconds=(time.perf_counter_ns() - time_begin) / 1e9,
             )
         return DockerActionResult(
             succeed=False,
             err_msg="Built image failed to pass tests.",
             image=self._name,
             tag=tag0,
             action="build",
-            seconds=(time.perf_counter_ns() - time_begin) / 1E9,
+            seconds=(time.perf_counter_ns() - time_begin) / 1e9,
         )
 
     def _test_built_image(self) -> bool:
         code = pytest.main([str(self._path)])
         return code in (pytest.ExitCode.OK, pytest.ExitCode.NO_TESTS_COLLECTED, 0)
 
     def _remove_ssh(self, copy_ssh_to: str):
@@ -375,30 +381,28 @@
         if not self._git_url_base:  # self is a root image
             return
         dockerfile = self._path / DockerImage.DOCKERFILE
         with dockerfile.open() as fin:
             lines = fin.readlines()
         for idx, line in enumerate(lines):
             if line.startswith("FROM "):
-                lines[idx] = line[:line.rfind(":")] + f":{tag_build}\n"
+                lines[idx] = line[: line.rfind(":")] + f":{tag_build}\n"
                 break
         with dockerfile.open("w") as fout:
             fout.writelines(lines)
 
     def node(self):
-        """Convert this DockerImage to a Node.
-        """
+        """Convert this DockerImage to a Node."""
         return Node(
             git_url=self._git_url,
             branch=self._branch,
         )
 
     def base_node(self):
-        """Convert the base image of this DockerImage to a Node.
-        """
+        """Convert the base image of this DockerImage to a Node."""
         return self.base_image().node()
 
     def docker_servers(self) -> set[str]:
         """Get 3rd-party Docker image hosts associated with this DockerImage and its base DockerImage.
 
         :return: A set of 3rdd-party Docker image hosts.
         """
@@ -411,16 +415,16 @@
 
 
 class DockerImageBuilderError(Exception):
     """Exception due to Docker image building."""
 
 
 class DockerImageBuilder:
-    """A class for build many Docker images at once.
-    """
+    """A class for build many Docker images at once."""
+
     def __init__(
         self,
         branch_urls: Union[dict[str, list[str]], str, Path],
         branch_fallback: str = "dev",
         builder: str = _get_docker_builder(),
     ):
         if isinstance(branch_urls, (str, Path)):
@@ -442,15 +446,15 @@
 
     def _build_graph_branch(self, branch, urls):
         for url in urls:
             deps: deque[DockerImage] = DockerImage(
                 git_url=url,
                 branch=branch,
                 branch_fallback=self._branch_fallback,
-                repo_path=self._repo_path
+                repo_path=self._repo_path,
             ).get_deps(self._graph.nodes)
             self._record_docker_servers(deps)
             dep0 = deps.popleft()
             if dep0.is_root():
                 node_prev = self._add_root_node(dep0.node())
             else:
                 node_prev = self._find_identical_node(dep0.base_node())
@@ -459,15 +463,15 @@
             for dep in deps:
                 node_prev = self._add_edge(node_prev, dep.node())
 
     def _find_identical_node(self, node: Node) -> Union[Node, None]:
         """Find node in the graph which has identical branch as the specified dependency.
         Notice that a node in the graph is represented as (git_url, branch).
 
-        :param node: A dependency of the type DockerImage. 
+        :param node: A dependency of the type DockerImage.
         """
         logger.debug("Finding identical node of {} in the graph ...", node)
         nodes: list[Node] = self._repo_nodes.get(node.git_url, [])
         logger.debug("Nodes associated with the repo {}: {}", node.git_url, str(nodes))
         if not nodes:
             return None
         path = self._repo_path[node.git_url]
@@ -487,17 +491,18 @@
         """
         logger.debug("Comparing branches {} and {} of the local repo {}", b1, b2, path)
         if b1 == b2:
             return True
         repo = pygit2.Repository(path)
         diff = repo.diff(f"refs/heads/{b1}", f"refs/heads/{b2}")
         return not any(
-            True for delta in diff.deltas
-            if not Path(delta.old_file.path).parts[0] in ("test", "tests") and
-            not Path(delta.new_file.path).parts[0] in ("test", "tests")
+            True
+            for delta in diff.deltas
+            if not Path(delta.old_file.path).parts[0] in ("test", "tests")
+            and not Path(delta.new_file.path).parts[0] in ("test", "tests")
         )
 
     def _add_root_node(self, node) -> Node:
         logger.debug("Adding root node {} into the graph ...", node)
         inode = self._find_identical_node(node)
         if inode is None:
             self._graph.add_node(node)
@@ -544,16 +549,15 @@
         if self._graph is not None:
             return
         self._graph = nx.DiGraph()
         for branch, urls in self._branch_urls.items():
             self._build_graph_branch(branch, urls)
 
     def save_graph(self, output="graph.yaml") -> None:
-        """Save the underlying graph structure to files.
-        """
+        """Save the underlying graph structure to files."""
         with open(output, "w", encoding="utf-8") as fout:
             # nodes and attributes
             fout.write("nodes:\n")
             for node in self._graph.nodes:
                 fout.write(f"  {node}: {list(self._get_identical_branches(node))}\n")
             # edges
             fout.write("edges:\n")
@@ -577,15 +581,15 @@
         push: bool = True,
         remove: bool = False,
     ) -> pd.DataFrame:
         """Build all Docker images in self.docker_images in order.
 
         :param tag_build: The tag of built images.
         :param copy_ssh_to: If True, SSH keys are copied into a directory named ssh
-            under each of the local Git repositories. 
+            under each of the local Git repositories.
         :param push: If True, push the built Docker images to DockerHub.
         :return: A pandas DataFrame summarizing building information.
         """
         self.build_graph()
         if self._builder == "docker":
             self._login_servers()
         for node in self._roots:
@@ -596,17 +600,20 @@
                 push=push,
                 remove=remove,
             )
         if self.failures:
             raise DockerImageBuilderError(self._build_error_msg())
 
     def _build_error_msg(self):
-        return "Failed to build Docker images corresponding to the following nodes:\n" + "\n".join(
-            f"{node} {list(self._get_identical_branches(node))}:\n{self._graph.nodes[node]['build_err_msg']}"
-            for node in self.failures
+        return (
+            "Failed to build Docker images corresponding to the following nodes:\n"
+            + "\n".join(
+                f"{node} {list(self._get_identical_branches(node))}:\n{self._graph.nodes[node]['build_err_msg']}"
+                for node in self.failures
+            )
         )
 
     def _build_images_graph(
         self,
         node,
         tag_build: str,
         copy_ssh_to: str,
@@ -650,26 +657,26 @@
         copy_ssh_to: str,
         push: bool,
     ) -> None:
         succeed, err_msg, name, tag, _, _ = DockerImage(
             git_url=node.git_url,
             branch=node.branch,
             branch_fallback=self._branch_fallback,
-            repo_path=self._repo_path
+            repo_path=self._repo_path,
         ).build(tags=tags, copy_ssh_to=copy_ssh_to, builder=self._builder)
         attr = self._graph.nodes[node]
         attr["build_succeed"] = succeed
         attr["build_err_msg"] = err_msg
         attr["image_name"] = name
         if self._builder == "docker" and succeed and push:
             for tag in tags:
                 _push_image_timing(name, tag)
 
-    #@staticmethod
-    #def _push_images(name, action_time):
+    # @staticmethod
+    # def _push_images(name, action_time):
     #    for idx in range(len(action_time)):
     #        tag, *_ = action_time[idx]
     #        _, *tas = _push_image_timing(name, tag)
     #        action_time.append(tas)
 
     def _gen_add_tags(self, tag_build, node) -> list:
         tag_build = _reg_tag(tag_build, node.branch)[0]
```

### Comparing `dockeree-0.4.0/pyproject.toml` & `dockeree-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "dockeree"
-version = "0.4.0"
+version = "0.5.0"
 description = "Make it easy to build and manager Docker images."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "GPLv2"
-readme = "readme.md"
+readme = "README.md"
 repository = "https://github.com/legendu-net/dockeree"
 keywords = ["Docker", "container", "build", "management"]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = ">=3.8,<3.12"
 pandas = ">=1.2.0"
 networkx = ">=2.5"
-docker = ">=4.4.0"
+docker = ">=6.1.0"
 requests = ">=2.20.0"
 loguru = ">=0.6.0"
 PyYAML = ">=6.0"
 pygit2 = ">=1.9.1"
 pytest = ">=3.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+black = ">=23.3.0"
 pylint = ">=2.7.0"
 flake8 = ">=3.8.4"
 pytype = { version = ">=2020.08.10", python = "<3.9" }
 darglint = ">=1.5.8"
-yapf = ">=0.32.0"
 
 [tool.yapf]
 based_on_style = "facebook"
 column_limit = 88
 
 [tool.yapfignore]
 ignore_patterns = [
```

### Comparing `dockeree-0.4.0/PKG-INFO` & `dockeree-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dockeree
-Version: 0.4.0
+Version: 0.5.0
 Summary: Make it easy to build and manager Docker images.
 Home-page: https://github.com/legendu-net/dockeree
 License: GPLv2
 Keywords: Docker,container,build,management
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0)
-Requires-Dist: docker (>=4.4.0)
+Requires-Dist: docker (>=6.1.0)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: networkx (>=2.5)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: pygit2 (>=1.9.1)
 Requires-Dist: pytest (>=3.0)
 Requires-Dist: requests (>=2.20.0)
 Project-URL: Repository, https://github.com/legendu-net/dockeree
@@ -26,19 +27,18 @@
 
 # [dockeree](https://github.com/dclong/dockeree)
 
 Make it easy to build and manager Docker images.
     
 ## Supported Operating Systems and Python Versions
 
-| OS      | Python 3.7 | Python 3.8 | Python 3.9 | Python 3.10 |
-|---------|------------|------------|------------|-------------|
-| Linux   | Y          | Y          | Y          | Y           |
-| macOS   | Y          | Y          | Y          | Y           |
-| Windows | Y          | Y          | Y          | Y           |
+| OS      | Python 3.8 | Python 3.9 | Python 3.10 |
+|---------|------------|------------|-------------|
+| Linux   | Y          | Y          | Y           |
+| macOS   | Y          | Y          | Y           |
 
 ## Installation
 
 You can download a copy of the latest release and install it using pip.
 ```bash
 pip3 install dockeree
 ```
```

