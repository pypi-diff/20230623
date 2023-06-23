# Comparing `tmp/commitizen-3.4.1.tar.gz` & `tmp/commitizen-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.4.1.tar", max compression
+gzip compressed data, was "commitizen-3.5.0.tar", max compression
```

## Comparing `commitizen-3.4.1.tar` & `commitizen-3.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-23 09:22:51.472965 commitizen-3.4.1/LICENSE
--rw-r--r--   0        0        0      609 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__version__.py
--rw-r--r--   0        0        0     4609 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/bump.py
--rw-r--r--   0        0        0    11712 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    17490 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13971 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7142 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5075 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/info.py
--rw-r--r--   0        0        0    12966 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3176 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/factory.py
--rw-r--r--   0        0        0     6900 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/out.py
--rw-r--r--   0        0        0     7109 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9732 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-06-23 09:22:51.476965 commitizen-3.4.1/docs/README.md
--rw-r--r--   0        0        0     4200 2023-06-23 09:22:51.488965 commitizen-3.4.1/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-23 09:44:24.137200 commitizen-3.5.0/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     4609 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11712 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    17750 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14245 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7142 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5075 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12966 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3176 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6900 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/out.py
+-rw-r--r--   0        0        0     7109 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9732 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-06-23 09:44:24.141200 commitizen-3.5.0/docs/README.md
+-rw-r--r--   0        0        0     4200 2023-06-23 09:44:24.153200 commitizen-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.0/PKG-INFO
```

### Comparing `commitizen-3.4.1/LICENSE` & `commitizen-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/__init__.py` & `commitizen-3.5.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/bump.py` & `commitizen-3.5.0/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/changelog.py` & `commitizen-3.5.0/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/changelog_parser.py` & `commitizen-3.5.0/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cli.py` & `commitizen-3.5.0/commitizen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,20 @@
                     {
                         "name": ["--changelog-to-stdout"],
                         "action": "store_true",
                         "default": False,
                         "help": "Output changelog to the stdout",
                     },
                     {
+                        "name": ["--git-output-to-stderr"],
+                        "action": "store_true",
+                        "default": False,
+                        "help": "Redirect git output to stderr",
+                    },
+                    {
                         "name": ["--retry"],
                         "action": "store_true",
                         "default": False,
                         "help": "retry commit if it fails the 1st time",
                     },
                     {
                         "name": ["--major-version-zero"],
```

### Comparing `commitizen-3.4.1/commitizen/cmd.py` & `commitizen-3.5.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/commands/bump.py` & `commitizen-3.5.0/commitizen/commands/bump.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             },
         }
         self.cz = factory.commiter_factory(self.config)
         self.changelog = arguments["changelog"] or self.config.settings.get(
             "update_changelog_on_bump"
         )
         self.changelog_to_stdout = arguments["changelog_to_stdout"]
+        self.git_output_to_stderr = arguments["git_output_to_stderr"]
         self.no_verify = arguments["no_verify"]
         self.check_consistency = arguments["check_consistency"]
         self.retry = arguments["retry"]
         self.pre_bump_hooks = self.config.settings["pre_bump_hooks"]
         self.post_bump_hooks = self.config.settings["post_bump_hooks"]
         deprecated_version_type = arguments.get("version_type")
         if deprecated_version_type:
@@ -325,17 +326,23 @@
             logger.info("1st commit attempt failed; retrying once")
             cmd.run(git_add_changelog_and_version_files_command)
             c = git.commit(message, args=self._get_commit_args())
         if c.return_code != 0:
             raise BumpCommitFailedError(f'2nd git.commit error: "{c.err.strip()}"')
 
         if c.out:
-            out.write(c.out)
+            if self.git_output_to_stderr:
+                out.diagnostic(c.out)
+            else:
+                out.write(c.out)
         if c.err:
-            out.write(c.err)
+            if self.git_output_to_stderr:
+                out.diagnostic(c.err)
+            else:
+                out.write(c.err)
 
         c = git.tag(
             new_tag_version,
             signed=self.bump_settings.get("gpg_sign", False)
             or bool(self.config.settings.get("gpg_sign", False)),
             annotated=self.bump_settings.get("annotated_tag", False)
             or bool(self.config.settings.get("annotated_tag", False)),
```

### Comparing `commitizen-3.4.1/commitizen/commands/changelog.py` & `commitizen-3.5.0/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/commands/check.py` & `commitizen-3.5.0/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/commands/commit.py` & `commitizen-3.5.0/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/commands/init.py` & `commitizen-3.5.0/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/commands/version.py` & `commitizen-3.5.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/config/__init__.py` & `commitizen-3.5.0/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/config/base_config.py` & `commitizen-3.5.0/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/config/json_config.py` & `commitizen-3.5.0/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/config/toml_config.py` & `commitizen-3.5.0/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/config/yaml_config.py` & `commitizen-3.5.0/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/__init__.py` & `commitizen-3.5.0/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/base.py` & `commitizen-3.5.0/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/customize/customize.py` & `commitizen-3.5.0/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/jira/jira.py` & `commitizen-3.5.0/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/cz/jira/jira_info.txt` & `commitizen-3.5.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/defaults.py` & `commitizen-3.5.0/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/exceptions.py` & `commitizen-3.5.0/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/factory.py` & `commitizen-3.5.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/git.py` & `commitizen-3.5.0/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/hooks.py` & `commitizen-3.5.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/out.py` & `commitizen-3.5.0/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/providers.py` & `commitizen-3.5.0/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/commitizen/version_schemes.py` & `commitizen-3.5.0/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/docs/README.md` & `commitizen-3.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.1/pyproject.toml` & `commitizen-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.4.1"
+version = "3.5.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.4.1"
+version = "3.5.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
```

### Comparing `commitizen-3.4.1/PKG-INFO` & `commitizen-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.4.1
+Version: 3.5.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

