# Comparing `tmp/sigstore-1.1.2rc1.tar.gz` & `tmp/sigstore-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-1.1.2rc1.tar", last modified: Wed Mar 15 21:25:46 2023, max compression
+gzip compressed data, was "sigstore-2.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-1.1.2rc1.tar` & `sigstore-2.0.0rc1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0    11358 2023-03-15 21:25:33.169977 sigstore-1.1.2rc1/LICENSE
--rw-r--r--   0        0        0    20574 2023-03-15 21:25:33.169977 sigstore-1.1.2rc1/README.md
--rw-r--r--   0        0        0     4125 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0      958 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/__main__.py
--rw-r--r--   0        0        0    34542 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      774 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/ctfe.py
--rw-r--r--   0        0        0      833 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    11677 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     3395 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/keyring.py
--rw-r--r--   0        0        0     4544 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0     2576 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15958 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0      687 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     9313 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     8229 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/sct.py
--rw-r--r--   0        0        0     1513 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/set.py
--rw-r--r--   0        0        0     7790 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/root.json
--rw-r--r--   0        0        0     2482 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/staging-root.json
--rw-r--r--   0        0        0     4481 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_utils.py
--rw-r--r--   0        0        0     2874 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/errors.py
--rw-r--r--   0        0        0     8054 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/oidc.py
--rw-r--r--   0        0        0     8732 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/sign.py
--rw-r--r--   0        0        0     4679 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/transparency.py
--rw-r--r--   0        0        0     1932 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/__init__.py
--rw-r--r--   0        0        0    10469 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/models.py
--rw-r--r--   0        0        0     9824 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/policy.py
--rw-r--r--   0        0        0    10444 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    22863 1970-01-01 00:00:00.000000 sigstore-1.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    20790 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     4131 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      958 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/__main__.py
+-rw-r--r--   0        0        0    34259 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      774 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/ctfe.py
+-rw-r--r--   0        0        0      883 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    11831 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     3891 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/keyring.py
+-rw-r--r--   0        0        0     4544 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0      653 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15958 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0      748 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     7301 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/checkpoint.py
+-rw-r--r--   0        0        0     9313 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     9162 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0     1508 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/set.py
+-rw-r--r--   0        0        0     9403 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/prod/root.json
+-rw-r--r--   0        0        0     4567 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/prod/trusted_root.json
+-rw-r--r--   0        0        0     1876 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/staging/root.json
+-rw-r--r--   0        0        0     4521 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/staging/trusted_root.json
+-rw-r--r--   0        0        0    10657 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_utils.py
+-rw-r--r--   0        0        0     3247 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/errors.py
+-rw-r--r--   0        0        0    15934 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/oidc.py
+-rw-r--r--   0        0        0    12380 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/sign.py
+-rw-r--r--   0        0        0     4735 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/transparency.py
+-rw-r--r--   0        0        0     1932 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0    13404 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/models.py
+-rw-r--r--   0        0        0     9824 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    11219 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    23085 1970-01-01 00:00:00.000000 sigstore-2.0.0rc1/PKG-INFO
```

### Comparing `sigstore-1.1.2rc1/LICENSE` & `sigstore-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/README.md` & `sigstore-2.0.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,24 @@
 
 Top-level:
 
 <!-- @begin-sigstore-help@ -->
 ```
 usage: sigstore [-h] [-V] [-v] [--staging] [--rekor-url URL]
                 [--rekor-root-pubkey FILE]
-                {sign,verify,get-identity-token} ...
+                COMMAND ...
 
 a tool for signing and verifying Python package distributions
 
 positional arguments:
-  {sign,verify,get-identity-token}
+  COMMAND               the operation to perform
+    sign                sign one or more inputs
+    verify              verify one or more inputs
+    get-identity-token  retrieve and return a Sigstore-compatible OpenID
+                        Connect token
 
 optional arguments:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -v, --verbose         run with additional debug logging; supply multiple
                         times to increase verbosity (default: 0)
 
@@ -126,19 +130,19 @@
 ### Signing
 
 <!-- @begin-sigstore-sign-help@ -->
 ```
 usage: sigstore sign [-h] [--identity-token TOKEN] [--oidc-client-id ID]
                      [--oidc-client-secret SECRET]
                      [--oidc-disable-ambient-providers] [--oidc-issuer URL]
-                     [--no-default-files] [--signature FILE]
-                     [--certificate FILE] [--bundle FILE] [--no-bundle]
-                     [--overwrite] [--staging] [--rekor-url URL]
-                     [--rekor-root-pubkey FILE] [--fulcio-url URL]
-                     [--ctfe FILE]
+                     [--oauth-force-oob] [--no-default-files]
+                     [--signature FILE] [--certificate FILE] [--bundle FILE]
+                     [--output-directory DIR] [--overwrite] [--staging]
+                     [--rekor-url URL] [--rekor-root-pubkey FILE]
+                     [--fulcio-url URL] [--ctfe FILE]
                      FILE [FILE ...]
 
 positional arguments:
   FILE                  The file to sign
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -152,29 +156,33 @@
                         The custom OpenID Connect client secret to use during
                         OAuth2 (default: None)
   --oidc-disable-ambient-providers
                         Disable ambient OpenID Connect credential detection
                         (e.g. on GitHub Actions) (default: False)
   --oidc-issuer URL     The OpenID Connect issuer to use (conflicts with
                         --staging) (default: https://oauth2.sigstore.dev/auth)
+  --oauth-force-oob     Force an out-of-band OAuth flow and do not
+                        automatically start the default web browser (default:
+                        False)
 
 Output options:
-  --no-default-files    Don't emit the default output files ({input}.sig,
-                        {input}.crt, {input}.rekor) (default: False)
+  --no-default-files    Don't emit the default output files ({input}.sigstore)
+                        (default: False)
   --signature FILE, --output-signature FILE
                         Write a single signature to the given file; does not
                         work with multiple input files (default: None)
   --certificate FILE, --output-certificate FILE
                         Write a single certificate to the given file; does not
                         work with multiple input files (default: None)
   --bundle FILE         Write a single Sigstore bundle to the given file; does
                         not work with multiple input files (default: None)
-  --no-bundle           Don't emit {input}.sigstore files for each input; this
-                        option is experimental and may change between releases
-                        until stabilized (default: False)
+  --output-directory DIR
+                        Write default outputs to the given directory
+                        (conflicts with --signature, --certificate, --bundle)
+                        (default: None)
   --overwrite           Overwrite preexisting signature and certificate
                         outputs, if present (default: False)
 
 Sigstore instance options:
   --staging             Use sigstore's staging instances, instead of the
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
@@ -253,18 +261,14 @@
   --certificate-chain FILE
                         Path to a list of CA certificates in PEM format which
                         will be needed when building the certificate chain for
                         the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-identity-help@ -->
 
-For backwards compatibility, `sigstore verify [args ...]` is equivalent to
-`sigstore verify identity [args ...]`, but the latter form is **strongly**
-preferred.
-
 #### Signatures from GitHub Actions
 
 If your signatures are coming from GitHub Actions (e.g., a workflow
 that uses its [ambient credentials](#signing-with-ambient-credentials)),
 then you can use the `sigstore verify github` subcommand to verify
 claims more precisely than `sigstore verify identity` allows:
```

### Comparing `sigstore-1.1.2rc1/pyproject.toml` & `sigstore-2.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   "importlib_resources ~= 5.7; python_version < '3.11'",
   "pydantic ~= 1.10",
   "pyjwt >= 2.1",
   "pyOpenSSL >= 23.0.0",
   "requests",
   "securesystemslib",
   "sigstore-protobuf-specs ~= 0.1.0",
-  "tuf ~= 2.1",
+  "tuf >= 2.1,< 4.0",
 ]
 requires-python = ">=3.7"
 
 [project.scripts]
 sigstore = "sigstore._cli:main"
 
 [project.urls]
@@ -60,15 +60,15 @@
   "bandit",
   "black",
   "isort",
   "interrogate",
   "mypy ~= 1.1",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.0.256",
+  "ruff < 0.0.275",
   "types-requests",
   # Needed for protocol typing in 3.7; remove when our minimum Python is 3.8.
   "typing-extensions; python_version < '3.8'",
   # TODO(ww): Re-enable once dependency on types-cryptography is dropped.
   # See: https://github.com/python/typeshed/issues/8699
   # "types-pyOpenSSL",
 ]
```

### Comparing `sigstore-1.1.2rc1/sigstore/__main__.py` & `sigstore-2.0.0rc1/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_cli.py` & `sigstore-2.0.0rc1/sigstore/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,39 +17,44 @@
 import argparse
 import base64
 import logging
 import os
 import sys
 from pathlib import Path
 from textwrap import dedent
-from typing import Optional, TextIO, Union, cast
+from typing import NoReturn, Optional, TextIO, Union, cast
 
 from cryptography.x509 import load_pem_x509_certificates
 from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import Bundle
 
 from sigstore import __version__
 from sigstore._internal.ctfe import CTKeyring
-from sigstore._internal.fulcio.client import DEFAULT_FULCIO_URL, FulcioClient
+from sigstore._internal.fulcio.client import (
+    DEFAULT_FULCIO_URL,
+    ExpiredCertificate,
+    FulcioClient,
+)
 from sigstore._internal.keyring import Keyring
-from sigstore._internal.oidc import DEFAULT_AUDIENCE
 from sigstore._internal.rekor.client import (
     DEFAULT_REKOR_URL,
     RekorClient,
     RekorKeyring,
 )
 from sigstore._internal.tuf import TrustUpdater
 from sigstore._utils import PEMCert
 from sigstore.errors import Error
 from sigstore.oidc import (
     DEFAULT_OAUTH_ISSUER_URL,
     STAGING_OAUTH_ISSUER_URL,
+    ExpiredIdentity,
+    IdentityToken,
     Issuer,
     detect_credential,
 )
-from sigstore.sign import Signer
+from sigstore.sign import SigningContext
 from sigstore.transparency import LogEntry
 from sigstore.verify import (
     CertificateVerificationFailure,
     LogEntryMissing,
     VerificationMaterials,
     Verifier,
     policy,
@@ -61,14 +66,23 @@
 
 # NOTE: We configure the top package logger, rather than the root logger,
 # to avoid overly verbose logging in third-party code by default.
 package_logger = logging.getLogger("sigstore")
 package_logger.setLevel(os.environ.get("SIGSTORE_LOGLEVEL", "INFO").upper())
 
 
+def _die(args: argparse.Namespace, message: str) -> NoReturn:
+    """
+    An `argparse` helper that fixes up the type hints on our use of
+    `ArgumentParser.error`.
+    """
+    args._parser.error(message)
+    raise ValueError("unreachable")
+
+
 def _boolify_env(envvar: str) -> bool:
     """
     An `argparse` helper for turning an environment variable into a boolean.
 
     The semantics here closely mirror `distutils.util.strtobool`.
 
     See: <https://docs.python.org/3/distutils/apiref.html#distutils.util.strtobool>
@@ -82,50 +96,14 @@
         return True
     elif val in {"n", "no", "false", "f", "off", "0"}:
         return False
     else:
         raise ValueError(f"can't coerce '{val}' to a boolean")
 
 
-def _set_default_verify_subparser(parser: argparse.ArgumentParser, name: str) -> None:
-    """
-    An argparse patch for configuring a default subparser for `sigstore verify`.
-
-    Adapted from <https://stackoverflow.com/a/26379693>
-    """
-    subparser_found = False
-    for arg in sys.argv[1:]:
-        if arg in ["-h", "--help"]:  # global help if no subparser
-            break
-    else:
-        for x in parser._subparsers._actions:  # type: ignore[union-attr]
-            if not isinstance(x, argparse._SubParsersAction):
-                continue
-            for sp_name in x._name_parser_map.keys():
-                if sp_name in sys.argv[1:]:
-                    subparser_found = True
-        if not subparser_found:
-            try:
-                # If `sigstore verify identity` wasn't passed explicitly, we need
-                # to insert the `identity` subcommand into the correct position
-                # within `sys.argv`. To do that, we get the index of the `verify`
-                # subcommand, and insert it directly after it.
-                verify_idx = sys.argv.index("verify")
-                sys.argv.insert(verify_idx + 1, name)
-                logger.warning(
-                    "`sigstore verify` without a subcommand will be treated as "
-                    "`sigstore verify identity`, but this behavior will be deprecated "
-                    "in a future release"
-                )
-            except ValueError:
-                # This happens when we invoke `sigstore sign`, since there's no
-                # `verify` subcommand to insert under. We do nothing in this case.
-                pass
-
-
 def _add_shared_instance_options(group: argparse._ArgumentGroup) -> None:
     """
     Common Sigstore instance options, shared between all `sigstore` subcommands.
     """
     group.add_argument(
         "--staging",
         dest="__deprecated_staging",
@@ -244,14 +222,20 @@
     group.add_argument(
         "--oidc-issuer",
         metavar="URL",
         type=str,
         default=os.getenv("SIGSTORE_OIDC_ISSUER", DEFAULT_OAUTH_ISSUER_URL),
         help="The OpenID Connect issuer to use (conflicts with --staging)",
     )
+    group.add_argument(
+        "--oauth-force-oob",
+        action="store_true",
+        default=_boolify_env("SIGSTORE_OAUTH_FORCE_OOB"),
+        help="Force an out-of-band OAuth flow and do not automatically start the default web browser",
+    )
 
 
 def _parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog="sigstore",
         description="a tool for signing and verifying Python package distributions",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -285,19 +269,26 @@
         "--rekor-root-pubkey",
         metavar="FILE",
         type=argparse.FileType("rb"),
         help="A PEM-encoded root public key for Rekor itself (conflicts with --staging)",
         default=os.getenv("SIGSTORE_REKOR_ROOT_PUBKEY"),
     )
 
-    subcommands = parser.add_subparsers(required=True, dest="subcommand")
+    subcommands = parser.add_subparsers(
+        required=True,
+        dest="subcommand",
+        metavar="COMMAND",
+        help="the operation to perform",
+    )
 
     # `sigstore sign`
     sign = subcommands.add_parser(
-        "sign", formatter_class=argparse.ArgumentDefaultsHelpFormatter
+        "sign",
+        help="sign one or more inputs",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     oidc_options = sign.add_argument_group("OpenID Connect options")
     oidc_options.add_argument(
         "--identity-token",
         metavar="TOKEN",
         type=str,
@@ -307,15 +298,15 @@
     _add_shared_oidc_options(oidc_options)
 
     output_options = sign.add_argument_group("Output options")
     output_options.add_argument(
         "--no-default-files",
         action="store_true",
         default=_boolify_env("SIGSTORE_NO_DEFAULT_FILES"),
-        help="Don't emit the default output files ({input}.sig, {input}.crt, {input}.rekor)",
+        help="Don't emit the default output files ({input}.sigstore)",
     )
     output_options.add_argument(
         "--signature",
         "--output-signature",
         metavar="FILE",
         type=Path,
         default=os.getenv("SIGSTORE_OUTPUT_SIGNATURE"),
@@ -340,20 +331,21 @@
         default=os.getenv("SIGSTORE_BUNDLE"),
         help=(
             "Write a single Sigstore bundle to the given file; does not work with multiple input "
             "files"
         ),
     )
     output_options.add_argument(
-        "--no-bundle",
-        action="store_true",
-        default=False,
+        "--output-directory",
+        metavar="DIR",
+        type=Path,
+        default=os.getenv("SIGSTORE_OUTPUT_DIRECTORY"),
         help=(
-            "Don't emit {input}.sigstore files for each input; this option is experimental "
-            "and may change between releases until stabilized"
+            "Write default outputs to the given directory (conflicts with --signature, --certificate"
+            ", --bundle)"
         ),
     )
     output_options.add_argument(
         "--overwrite",
         action="store_true",
         default=_boolify_env("SIGSTORE_OVERWRITE"),
         help="Overwrite preexisting signature and certificate outputs, if present",
@@ -384,17 +376,23 @@
         nargs="+",
         help="The file to sign",
     )
 
     # `sigstore verify`
     verify = subcommands.add_parser(
         "verify",
+        help="verify one or more inputs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    verify_subcommand = verify.add_subparsers(dest="verify_subcommand")
+    verify_subcommand = verify.add_subparsers(
+        required=True,
+        dest="verify_subcommand",
+        metavar="COMMAND",
+        help="the kind of verification to perform",
+    )
 
     # `sigstore verify identity`
     verify_identity = verify_subcommand.add_parser(
         "identity",
         help="verify against a known identity and identity provider",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
@@ -485,20 +483,20 @@
         type=argparse.FileType("r"),
         help=(
             "Path to a list of CA certificates in PEM format which will be needed when building "
             "the certificate chain for the Fulcio signing certificate"
         ),
     )
 
-    # `sigstore verify` defaults to `sigstore verify identity`, for backwards
-    # compatibility.
-    _set_default_verify_subparser(verify, "identity")
-
     # `sigstore get-identity-token`
-    get_identity_token = subcommands.add_parser("get-identity-token")
+    get_identity_token = subcommands.add_parser(
+        "get-identity-token",
+        help="retrieve and return a Sigstore-compatible OpenID Connect token",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     _add_shared_oidc_options(get_identity_token)
 
     return parser
 
 
 def main() -> None:
     parser = _parser()
@@ -543,108 +541,107 @@
         if args.subcommand == "sign":
             _sign(args)
         elif args.subcommand == "verify":
             if args.verify_subcommand == "identity":
                 _verify_identity(args)
             elif args.verify_subcommand == "github":
                 _verify_github(args)
-            else:
-                parser.error(f"Unknown verify subcommand: {args.verify_subcommand}")
         elif args.subcommand == "get-identity-token":
-            token = _get_identity_token(args)
-            if token:
-                print(token)
+            identity = _get_identity(args)
+            if identity:
+                print(identity)
             else:
-                args._parser.error("No identity token supplied or detected!")
+                _die(args, "No identity token supplied or detected!")
 
         else:
-            parser.error(f"Unknown subcommand: {args.subcommand}")
+            _die(args, f"Unknown subcommand: {args.subcommand}")
     except Error as e:
         e.print_and_exit(args.verbose >= 1)
 
 
 def _sign(args: argparse.Namespace) -> None:
-    if args.bundle:
-        logger.warning(
-            "--bundle support is experimental; the behaviour of this flag may change "
-            "between releases until stabilized."
-        )
-
-    if args.no_bundle:
-        logger.warning(
-            "--no-bundle support is experimental; the behaviour of this flag may change "
-            "between releases until stabilized."
-        )
-
-    # `--no-default-files` has no effect on `--{signature,certificate,bundle}`,
-    # but we forbid it because it indicates user confusion.
-    if args.no_default_files and (args.signature or args.certificate or args.bundle):
-        args._parser.error(
-            "--no-default-files may not be combined with --signature, "
-            "--certificate, or --bundle",
-        )
-
-    # Fail if `--bundle` and `--no-bundle` are both specified.
-    if args.bundle and args.no_bundle:
-        args._parser.error("--bundle may not be combined with --no-bundle")
+    has_sig = bool(args.signature)
+    has_crt = bool(args.certificate)
+    has_bundle = bool(args.bundle)
+
+    # `--no-default-files` has no effect on `--bundle`, but we forbid it because
+    # it indicates user confusion.
+    if args.no_default_files and has_bundle:
+        _die(args, "--no-default-files may not be combined with --bundle.")
 
     # Fail if `--signature` or `--certificate` is specified *and* we have more
     # than one input.
-    if (args.signature or args.certificate) and len(args.files) > 1:
-        args._parser.error(
-            "Error: --signature and --certificate can't be used "
-            "with explicit outputs for multiple inputs",
-        )
+    if (has_sig or has_crt or has_bundle) and len(args.files) > 1:
+        _die(
+            args,
+            "Error: --signature, --certificate, and --bundle can't be used with "
+            "explicit outputs for multiple inputs.",
+        )
+
+    if args.output_directory and (has_sig or has_crt or has_bundle):
+        _die(
+            args,
+            "Error: --signature, --certificate, and --bundle can't be used with "
+            "an explicit output directory.",
+        )
+
+    # Fail if either `--signature` or `--certificate` is specified, but not both.
+    if has_sig ^ has_crt:
+        _die(args, "Error: --signature and --certificate must be used together.")
 
     # Build up the map of inputs -> outputs ahead of any signing operations,
     # so that we can fail early if overwriting without `--overwrite`.
     output_map = {}
     for file in args.files:
         if not file.is_file():
-            args._parser.error(f"Input must be a file: {file}")
+            _die(args, f"Input must be a file: {file}")
 
         sig, cert, bundle = (
             args.signature,
             args.certificate,
             args.bundle,
         )
-        if not sig and not cert and not bundle and not args.no_default_files:
-            sig = file.parent / f"{file.name}.sig"
-            cert = file.parent / f"{file.name}.crt"
-            if not args.no_bundle:
-                bundle = file.parent / f"{file.name}.sigstore"
+
+        output_dir = args.output_directory if args.output_directory else file.parent
+        if output_dir.exists() and not output_dir.is_dir():
+            _die(args, f"Output directory exists and is not a directory: {output_dir}")
+        output_dir.mkdir(parents=True, exist_ok=True)
+
+        if not bundle and not args.no_default_files:
+            bundle = output_dir / f"{file.name}.sigstore"
 
         if not args.overwrite:
             extants = []
             if sig and sig.exists():
                 extants.append(str(sig))
             if cert and cert.exists():
                 extants.append(str(cert))
             if bundle and bundle.exists():
                 extants.append(str(bundle))
 
             if extants:
-                args._parser.error(
+                _die(
+                    args,
                     "Refusing to overwrite outputs without --overwrite: "
-                    f"{', '.join(extants)}"
+                    f"{', '.join(extants)}",
                 )
 
         output_map[file] = {
             "cert": cert,
             "sig": sig,
             "bundle": bundle,
         }
 
-    # Select the signer to use.
+    # Select the signing context to use.
     if args.staging:
         logger.debug("sign: staging instances requested")
-        signer = Signer.staging()
+        signing_ctx = SigningContext.staging()
         args.oidc_issuer = STAGING_OAUTH_ISSUER_URL
     elif args.fulcio_url == DEFAULT_FULCIO_URL and args.rekor_url == DEFAULT_REKOR_URL:
-        signer = Signer.production()
+        signing_ctx = SigningContext.production()
     else:
         # Assume "production" keys if none are given as arguments
         updater = TrustUpdater.production()
         if args.ctfe_pem is not None:
             ctfe_keys = [args.ctfe_pem.read()]
         else:
             ctfe_keys = updater.get_ctfe_keys()
@@ -652,61 +649,73 @@
             rekor_keys = [args.rekor_root_pubkey.read()]
         else:
             rekor_keys = updater.get_rekor_keys()
 
         ct_keyring = CTKeyring(Keyring(ctfe_keys))
         rekor_keyring = RekorKeyring(Keyring(rekor_keys))
 
-        signer = Signer(
+        signing_ctx = SigningContext(
             fulcio=FulcioClient(args.fulcio_url),
             rekor=RekorClient(args.rekor_url, rekor_keyring, ct_keyring),
         )
 
-    # The order of precedence is as follows:
+    # The order of precedence for identities is as follows:
     #
     # 1) Explicitly supplied identity token
     # 2) Ambient credential detected in the environment, unless disabled
     # 3) Interactive OAuth flow
-    if not args.identity_token:
-        args.identity_token = _get_identity_token(args)
-    if not args.identity_token:
-        args._parser.error("No identity token supplied or detected!")
+    identity: IdentityToken | None
+    if args.identity_token:
+        identity = IdentityToken(args.identity_token)
+    else:
+        identity = _get_identity(args)
 
-    for file, outputs in output_map.items():
-        logger.debug(f"signing for {file.name}")
-        with file.open(mode="rb", buffering=0) as io:
-            result = signer.sign(
-                input_=io,
-                identity_token=args.identity_token,
-            )
+    if not identity:
+        _die(args, "No identity token supplied or detected!")
 
-        print("Using ephemeral certificate:")
-        print(result.cert_pem)
+    with signing_ctx.signer(identity) as signer:
+        for file, outputs in output_map.items():
+            logger.debug(f"signing for {file.name}")
+            with file.open(mode="rb", buffering=0) as io:
+                try:
+                    result = signer.sign(input_=io)
+                except ExpiredIdentity as exp_identity:
+                    print("Signature failed: identity token has expired")
+                    raise exp_identity
+
+                except ExpiredCertificate as exp_certificate:
+                    print("Signature failed: Fulcio signing certificate has expired")
+                    raise exp_certificate
 
-        print(f"Transparency log entry created at index: {result.log_entry.log_index}")
+            print("Using ephemeral certificate:")
+            print(result.cert_pem)
 
-        sig_output: TextIO
-        if outputs["sig"] is not None:
-            sig_output = outputs["sig"].open("w")
-        else:
-            sig_output = sys.stdout
+            print(
+                f"Transparency log entry created at index: {result.log_entry.log_index}"
+            )
 
-        print(result.b64_signature, file=sig_output)
-        if outputs["sig"] is not None:
-            print(f"Signature written to {outputs['sig']}")
-
-        if outputs["cert"] is not None:
-            with outputs["cert"].open(mode="w") as io:
-                print(result.cert_pem, file=io)
-            print(f"Certificate written to {outputs['cert']}")
-
-        if outputs["bundle"] is not None:
-            with outputs["bundle"].open(mode="w") as io:
-                print(result._to_bundle().to_json(), file=io)
-            print(f"Sigstore bundle written to {outputs['bundle']}")
+            sig_output: TextIO
+            if outputs["sig"] is not None:
+                sig_output = outputs["sig"].open("w")
+            else:
+                sig_output = sys.stdout
+
+            print(result.b64_signature, file=sig_output)
+            if outputs["sig"] is not None:
+                print(f"Signature written to {outputs['sig']}")
+
+            if outputs["cert"] is not None:
+                with outputs["cert"].open(mode="w") as io:
+                    print(result.cert_pem, file=io)
+                print(f"Certificate written to {outputs['cert']}")
+
+            if outputs["bundle"] is not None:
+                with outputs["bundle"].open(mode="w") as io:
+                    print(result._to_bundle().to_json(), file=io)
+                print(f"Sigstore bundle written to {outputs['bundle']}")
 
 
 def _collect_verification_state(
     args: argparse.Namespace,
 ) -> tuple[Verifier, list[tuple[Path, VerificationMaterials]]]:
     """
     Performs CLI functionality common across all `sigstore verify` subcommands.
@@ -715,29 +724,30 @@
     tuples, where `file` is the path to the file being verified (for display
     purposes) and `materials` is the `VerificationMaterials` to verify with.
     """
 
     # Fail if --certificate, --signature, or --bundle is specified and we
     # have more than one input.
     if (args.certificate or args.signature or args.bundle) and len(args.files) > 1:
-        args._parser.error(
+        _die(
+            args,
             "--certificate, --signature, or --bundle can only be used "
-            "with a single input file"
+            "with a single input file",
         )
 
     # Fail if `--certificate` or `--signature` is used with `--bundle`.
     if args.bundle and (args.certificate or args.signature):
-        args._parser.error("--bundle cannot be used with --certificate or --signature")
+        _die(args, "--bundle cannot be used with --certificate or --signature")
 
     # The converse of `sign`: we build up an expected input map and check
     # that we have everything so that we can fail early.
     input_map = {}
     for file in args.files:
         if not file.is_file():
-            args._parser.error(f"Input must be a file: {file}")
+            _die(args, f"Input must be a file: {file}")
 
         sig, cert, bundle = (
             args.signature,
             args.certificate,
             args.bundle,
         )
         if sig is None:
@@ -759,35 +769,34 @@
             # `--rekor-bundle`, we expect a bundle either supplied via `--bundle` or with the
             # default `{input}.sigstore` name.
             if not bundle.is_file():
                 missing.append(str(bundle))
             input_map[file] = {"bundle": bundle}
 
         if missing:
-            args._parser.error(
-                f"Missing verification materials for {(file)}: {', '.join(missing)}"
+            _die(
+                args,
+                f"Missing verification materials for {(file)}: {', '.join(missing)}",
             )
 
     if args.staging:
         logger.debug("verify: staging instances requested")
         verifier = Verifier.staging()
     elif args.rekor_url == DEFAULT_REKOR_URL:
         verifier = Verifier.production()
     else:
         if not args.certificate_chain:
-            args._parser.error(
-                "Custom Rekor URL used without specifying --certificate-chain"
-            )
+            _die(args, "Custom Rekor URL used without specifying --certificate-chain")
 
         try:
             certificate_chain = load_pem_x509_certificates(
                 args.certificate_chain.read()
             )
         except ValueError as error:
-            args._parser.error(f"Invalid certificate chain: {error}")
+            _die(args, f"Invalid certificate chain: {error}")
 
         if args.rekor_root_pubkey is not None:
             rekor_keys = [args.rekor_root_pubkey.read()]
         else:
             updater = TrustUpdater.production()
             rekor_keys = updater.get_rekor_keys()
 
@@ -950,28 +959,33 @@
         if result:
             print(f"OK: {file}")
         else:
             print(f"FAIL: {file}")
             raise VerificationError(cast(VerificationFailure, result))
 
 
-def _get_identity_token(args: argparse.Namespace) -> Optional[str]:
+def _get_identity(args: argparse.Namespace) -> Optional[IdentityToken]:
     token = None
     if not args.oidc_disable_ambient_providers:
-        token = detect_credential(DEFAULT_AUDIENCE)
+        token = detect_credential()
 
-    if not token:
-        if args.staging:
-            issuer = Issuer.staging()
-        elif args.oidc_issuer == DEFAULT_OAUTH_ISSUER_URL:
-            issuer = Issuer.production()
-        else:
-            issuer = Issuer(args.oidc_issuer)
+    # Happy path: we've detected an ambient credential, so we can return early.
+    if token:
+        return IdentityToken(token)
+
+    if args.staging:
+        issuer = Issuer.staging()
+    elif args.oidc_issuer == DEFAULT_OAUTH_ISSUER_URL:
+        issuer = Issuer.production()
+    else:
+        issuer = Issuer(args.oidc_issuer)
 
-        if args.oidc_client_secret is None:
-            args.oidc_client_secret = ""  # nosec: B105
+    if args.oidc_client_secret is None:
+        args.oidc_client_secret = ""  # nosec: B105
 
-        token = issuer.identity_token(
-            client_id=args.oidc_client_id, client_secret=args.oidc_client_secret
-        )
+    token = issuer.identity_token(
+        client_id=args.oidc_client_id,
+        client_secret=args.oidc_client_secret,
+        force_oob=args.oauth_force_oob,
+    )
 
     return token
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/__init__.py` & `sigstore-2.0.0rc1/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/ctfe.py` & `sigstore-2.0.0rc1/sigstore/_internal/ctfe.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/fulcio/__init__.py` & `sigstore-2.0.0rc1/sigstore/_internal/fulcio/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 """
 APIs for interacting with Fulcio.
 """
 
 
 from .client import (
     DetachedFulcioSCT,
+    ExpiredCertificate,
     FulcioCertificateSigningResponse,
     FulcioClient,
 )
 
 __all__ = [
     "DetachedFulcioSCT",
+    "ExpiredCertificate",
     "FulcioCertificateSigningResponse",
     "FulcioClient",
 ]
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/fulcio/client.py` & `sigstore-2.0.0rc1/sigstore/_internal/fulcio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     SignatureAlgorithm,
     SignedCertificateTimestamp,
     Version,
 )
 from pydantic import BaseModel, Field, validator
 
 from sigstore._utils import B64Str
+from sigstore.oidc import IdentityToken
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_FULCIO_URL = "https://fulcio.sigstore.dev"
 STAGING_FULCIO_URL = "https://fulcio.sigstage.dev"
 SIGNING_CERT_ENDPOINT = "/api/v2/signingCert"
 TRUST_BUNDLE_ENDPOINT = "/api/v2/trustBundle"
@@ -159,14 +160,18 @@
 
 
 # SignedCertificateTimestamp is an ABC, so register our DetachedFulcioSCT as
 # virtual subclass.
 SignedCertificateTimestamp.register(DetachedFulcioSCT)
 
 
+class ExpiredCertificate(Exception):
+    """An error raised when the Certificate is expired."""
+
+
 @dataclass(frozen=True)
 class FulcioCertificateSigningResponse:
     """Certificate response"""
 
     cert: Certificate
     chain: List[Certificate]
     sct: SignedCertificateTimestamp
@@ -204,22 +209,22 @@
 
 class FulcioSigningCert(_Endpoint):
     """
     Fulcio REST API signing certificate functionality.
     """
 
     def post(
-        self, req: CertificateSigningRequest, token: str
+        self, req: CertificateSigningRequest, identity: IdentityToken
     ) -> FulcioCertificateSigningResponse:
         """
         Get the signing certificate, using an X.509 Certificate
         Signing Request.
         """
         headers = {
-            "Authorization": f"Bearer {token}",
+            "Authorization": f"Bearer {identity}",
             "Content-Type": "application/json",
             "Accept": "application/pem-certificate-chain",
         }
         resp: requests.Response = self.session.post(
             url=self.url, data=_serialize_cert_request(req), headers=headers
         )
         try:
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/keyring.py` & `sigstore-2.0.0rc1/sigstore/_internal/keyring.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,22 @@
 from typing import List
 
 import cryptography.hazmat.primitives.asymmetric.padding as padding
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 
-from sigstore._utils import KeyID, key_id, load_pem_public_key
+from sigstore._utils import (
+    InvalidKeyError,
+    KeyID,
+    UnexpectedKeyFormatError,
+    key_id,
+    load_der_public_key,
+    load_pem_public_key,
+)
 
 
 class KeyringError(Exception):
     """
     Raised on failure by `Keyring.verify()`.
     """
 
@@ -40,30 +47,44 @@
     A specialization of `KeyringError`, indicating that the specified
     key ID wasn't found in the keyring.
     """
 
     pass
 
 
+class KeyringSignatureError(KeyringError):
+    """
+    Raised when `Keyring.verify()` is passed an invalid signature.
+    """
+
+
 class Keyring:
     """
     Represents a set of CT signing keys, each of which is a potentially
     valid signer for a Signed Certificate Timestamp (SCT).
 
     This structure exists to facilitate key rotation in a CT log.
     """
 
     def __init__(self, keys: List[bytes] = []):
         """
         Create a new `Keyring`, with `keys` as the initial set of signing
-        keys.
+        keys. These `keys` can be in either DER format or PEM encoded.
         """
         self._keyring = {}
         for key_bytes in keys:
-            key = load_pem_public_key(key_bytes)
+            key = None
+
+            try:
+                key = load_pem_public_key(key_bytes)
+            except UnexpectedKeyFormatError as e:
+                raise e
+            except InvalidKeyError:
+                key = load_der_public_key(key_bytes)
+
             self._keyring[key_id(key)] = key
 
     def add(self, key_pem: bytes) -> None:
         """
         Adds a PEM-encoded key to the current keyring.
         """
         key = load_pem_public_key(key_pem)
@@ -97,8 +118,8 @@
                     data=data,
                     signature_algorithm=ec.ECDSA(hashes.SHA256()),
                 )
             else:
                 # NOTE(ww): Unreachable without API misuse.
                 raise KeyringError(f"unsupported key type: {key}")
         except InvalidSignature as exc:
-            raise KeyringError("invalid signature") from exc
+            raise KeyringSignatureError("invalid signature") from exc
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/merkle.py` & `sigstore-2.0.0rc1/sigstore/_internal/merkle.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/oidc/oauth.py` & `sigstore-2.0.0rc1/sigstore/_internal/oidc/oauth.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/rekor/__init__.py` & `sigstore-2.0.0rc1/sigstore/_internal/oidc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,13 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-APIs for interacting with Rekor.
+Internal OIDC and OAuth functionality for sigstore-python.
 """
-
-from .client import RekorClient
-
-__all__ = ["RekorClient"]
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/rekor/client.py` & `sigstore-2.0.0rc1/sigstore/_internal/rekor/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/sct.py` & `sigstore-2.0.0rc1/sigstore/_internal/sct.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignedCertificateTimestamp,
 )
 from cryptography.x509.oid import ExtendedKeyUsageOID
 
 from sigstore._internal.ctfe import CTKeyring
-from sigstore._internal.keyring import KeyringError, KeyringLookupError
+from sigstore._internal.keyring import (
+    KeyringError,
+    KeyringLookupError,
+    KeyringSignatureError,
+)
 from sigstore._utils import DERCert, KeyID, key_id
 from sigstore.errors import Error
 
 logger = logging.getLogger(__name__)
 
 
 def _pack_signed_entry(
@@ -138,36 +142,76 @@
 class InvalidSCTError(Error):
     """
     Raised during SCT verification if an SCT is invalid in some way.
     """
 
     def diagnostics(self) -> str:
         """Returns diagnostics for the error."""
-        # We specialize this error case, since it usually indicates one of
-        # two conditions: either the current sigstore client is out-of-date,
-        # or that the SCT is well-formed but invalid for the current configuration
-        # (indicating that the user has asked for the wrong instance).
-        if isinstance(self.__cause__, KeyringLookupError):
-            return dedent(
-                f"""
+
+        ctx = f"\nContext: {self.__context__}" if self.__context__ else ""
+        return dedent(
+            f"""
+            SCT verification failed.
+
+            Additional context:
+
+            Message: {str(self)}
+            """
+            + ctx
+        )
+
+
+class InvalidSCTKeyError(InvalidSCTError):
+    """
+    Raised during SCT verification if the SCT can't be validated against the given keyring.
+
+    We specialize this error case, since it usually indicates one of
+    two conditions: either the current sigstore client is out-of-date,
+    or that the SCT is well-formed but invalid for the current configuration
+    (indicating that the user has asked for the wrong instance).
+    """
+
+    def diagnostics(self) -> str:
+        """Returns diagnostics for the error."""
+        return dedent(
+            f"""
                 Invalid key ID in SCT: not found in current keyring.
 
                 This may be a result of an outdated `sigstore` installation.
 
                 Consider upgrading with:
 
                     python -m pip install --upgrade sigstore
 
                 Additional context:
 
                 {self.__cause__}
                 """
-            )
+        )
+
+
+class SCTSignatureError(InvalidSCTError):
+    """
+    Raised during SCT verification if the signature of the SCT is invalid.
+    """
+
+    def diagnostics(self) -> str:
+        """Returns diagnostics for the error."""
+        return dedent(
+            f"""
+            Invalid signature on SCT.
+
+            If validating a certificate, the certificate associated with this
+            SCT should not be trusted.
 
-        return str(self)
+            Additional context:
+
+            {self.__cause__}
+            """
+        )
 
 
 def verify_sct(
     sct: SignedCertificateTimestamp,
     cert: Certificate,
     chain: List[Certificate],
     ct_keyring: CTKeyring,
@@ -210,12 +254,12 @@
         # singular `opaque key_id[32]`. Cryptography's APIs don't bother
         # to expose this trivial single member, so we use the `log_id`
         # attribute directly.
         ct_keyring.verify(
             key_id=KeyID(sct.log_id), signature=sct.signature, data=digitally_signed
         )
     except KeyringLookupError as exc:
-        raise InvalidSCTError(
-            "Invalid key ID in SCT: not found in current keyring"
-        ) from exc
+        raise InvalidSCTKeyError from exc
+    except KeyringSignatureError as exc:
+        raise SCTSignatureError from exc
     except KeyringError as exc:
         raise InvalidSCTError from exc
```

### Comparing `sigstore-1.1.2rc1/sigstore/_internal/set.py` & `sigstore-2.0.0rc1/sigstore/_internal/set.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 def verify_set(client: RekorClient, entry: LogEntry) -> None:
     """
     Verify the Signed Entry Timestamp for a given Rekor `entry` using the given `client`.
     """
 
-    signed_entry_ts = base64.b64decode(entry.signed_entry_timestamp)
+    signed_entry_ts = base64.b64decode(entry.inclusion_promise)
 
     try:
         client._rekor_keyring.verify(
             key_id=KeyID(bytes.fromhex(entry.log_id)),
             signature=signed_entry_ts,
             data=entry.encode_canonical(),
         )
```

### Comparing `sigstore-1.1.2rc1/sigstore/_store/__init__.py` & `sigstore-2.0.0rc1/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/_store/root.json` & `sigstore-2.0.0rc1/sigstore/_store/prod/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/errors.py` & `sigstore-2.0.0rc1/sigstore/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         {self.__cause__}
         """
             if self.__cause__
             else ""
         )
 
         return (
-            """A network issue occurred.
+            """\
+        A network issue occurred.
 
         Check your internet connection and try again.
         """
             + cause_ctx
         )
 
 
@@ -88,19 +89,31 @@
     def diagnostics(self) -> str:
         """Returns diagnostics specialized to the wrapped TUF error."""
         details = TUFError._details.get(
             type(self.__context__),
             "Please report this issue at <https://github.com/sigstore/sigstore-python/issues/new>.",
         )
 
-        return f"""{self.message}.
+        return f"""\
+        {self.message}.
 
         {details}
         """
 
 
 class MetadataError(Error):
     """Raised when TUF metadata does not conform to the expected structure."""
 
     def diagnostics(self) -> str:
         """Returns diagnostics for the error."""
         return f"""{str(self)}."""
+
+
+class RootError(Error):
+    """Raised when TUF cannot establish its root of trust."""
+
+    def diagnostics(self) -> str:
+        """Returns diagnostics for the error."""
+        return """\
+        Unable to establish root of trust.
+
+        This error may occur when the resources embedded in this distribution of sigstore-python are out of date."""
```

### Comparing `sigstore-1.1.2rc1/sigstore/sign.py` & `sigstore-2.0.0rc1/sigstore/_internal/tuf.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,266 +9,266 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-API for signing artifacts.
+TUF functionality for `sigstore-python`.
+"""
+
+from __future__ import annotations
 
-Example:
-```python
+import logging
+from datetime import datetime, timezone
+from functools import lru_cache
 from pathlib import Path
+from typing import Iterable
+from urllib import parse
 
-from sigstore.sign import Signer
-from sigstore.oidc import Issuer
+import appdirs
+from cryptography.x509 import Certificate, load_der_x509_certificate
+from sigstore_protobuf_specs.dev.sigstore.common.v1 import TimeRange
+from sigstore_protobuf_specs.dev.sigstore.trustroot.v1 import (
+    CertificateAuthority,
+    TransparencyLogInstance,
+    TrustedRoot,
+)
+from tuf.api import exceptions as TUFExceptions
+from tuf.ngclient import RequestsFetcher, Updater
 
-issuer = Issuer.production()
-token = issuer.identity_token()
+from sigstore._utils import read_embedded
+from sigstore.errors import MetadataError, RootError, TUFError
 
-# The artifact to sign
-artifact = Path("foo.txt")
+logger = logging.getLogger(__name__)
 
-with artifact.open("rb") as a:
-    signer = Signer.production()
-    result = signer.sign(input_=a, identity_token=token)
-    print(result)
-```
-"""
+DEFAULT_TUF_URL = "https://tuf-repo-cdn.sigstore.dev"
+STAGING_TUF_URL = "https://tuf-repo-cdn.sigstage.dev"
 
-from __future__ import annotations
 
-import base64
-import logging
-from typing import IO
+@lru_cache()
+def _get_fetcher() -> RequestsFetcher:
+    # NOTE: We poke into the underlying fetcher here to set a more reasonable timeout.
+    # The default timeout is 4 seconds, which can cause spurious timeout errors on
+    # CI systems like GitHub Actions (where traffic may be delayed/deprioritized due
+    # to network load).
+    fetcher = RequestsFetcher()
+    fetcher.socket_timeout = 30
 
-import cryptography.x509 as x509
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import ec
-from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
-from cryptography.x509.oid import NameOID
-from pydantic import BaseModel
-from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import (
-    Bundle,
-    VerificationMaterial,
-)
-from sigstore_protobuf_specs.dev.sigstore.common.v1 import (
-    HashAlgorithm,
-    HashOutput,
-    LogId,
-    MessageSignature,
-    X509Certificate,
-    X509CertificateChain,
-)
-from sigstore_protobuf_specs.dev.sigstore.rekor.v1 import (
-    InclusionPromise,
-    InclusionProof,
-    KindVersion,
-    TransparencyLogEntry,
-)
+    return fetcher
 
-from sigstore._internal.fulcio import FulcioClient
-from sigstore._internal.oidc import Identity
-from sigstore._internal.rekor.client import RekorClient
-from sigstore._internal.sct import verify_sct
-from sigstore._internal.tuf import TrustUpdater
-from sigstore._utils import B64Str, HexStr, PEMCert, sha256_streaming
-from sigstore.transparency import LogEntry
 
-logger = logging.getLogger(__name__)
+def _get_dirs(url: str) -> tuple[Path, Path]:
+    """
+    Given a TUF repository URL, return suitable local metadata and cache directories.
 
+    These directories are not guaranteed to already exist.
+    """
 
-class Signer:
+    builder = appdirs.AppDirs("sigstore-python", "sigstore")
+    repo_base = parse.quote(url, safe="")
+
+    tuf_data_dir = Path(builder.user_data_dir) / "tuf"
+    tuf_cache_dir = Path(builder.user_cache_dir) / "tuf"
+
+    return (tuf_data_dir / repo_base), (tuf_cache_dir / repo_base)
+
+
+def _is_timerange_valid(period: TimeRange | None, *, allow_expired: bool) -> bool:
     """
-    The primary API for signing operations.
+    Given a `period`, checks that the the current time is not before `start`. If
+    `allow_expired` is `False`, also checks that the current time is not after
+    `end`.
     """
+    now = datetime.now(timezone.utc)
 
-    def __init__(self, *, fulcio: FulcioClient, rekor: RekorClient):
-        """
-        Create a new `Signer`.
+    # If there was no validity period specified, the key is always valid.
+    if not period:
+        return True
+
+    # Active: if the current time is before the starting period, we are not yet
+    # valid.
+    if now < period.start:
+        return False
+
+    # If we want Expired keys, the key is valid at this point. Otherwise, check
+    # that we are within range.
+    return allow_expired or (period.end is None or now <= period.end)
 
-        `fulcio` is a `FulcioClient` capable of connecting to a Fulcio instance
-        and returning signing certificates.
 
-        `rekor` is a `RekorClient` capable of connecting to a Rekor instance
-        and creating transparency log entries.
+class TrustUpdater:
+    """Internal trust root (certificates and keys) downloader.
+
+    TrustUpdater discovers the currently valid certificates and keys and
+    securely downloads them from the remote TUF repository at 'url'.
+
+    TrustUpdater expects to find an initial root.json in either the local
+    metadata directory for this URL, or (as special case for the sigstore.dev
+    production and staging instances) in the application resources.
+    """
+
+    def __init__(self, url: str) -> None:
         """
-        self._fulcio = fulcio
-        self._rekor = rekor
+        Create a new `TrustUpdater`, pulling from the given `url`.
+
+        The URL is expected to match one of `sigstore-python`'s known TUF
+        roots, i.e. for the production or staging Sigstore TUF repos.
+        """
+        self._repo_url = url
+        self._metadata_dir, self._targets_dir = _get_dirs(url)
+
+        rsrc_prefix: str
+        if self._repo_url == DEFAULT_TUF_URL:
+            rsrc_prefix = "prod"
+        elif self._repo_url == STAGING_TUF_URL:
+            rsrc_prefix = "staging"
+        else:
+            raise RootError
+
+        # Initialize metadata dir
+        self._metadata_dir.mkdir(parents=True, exist_ok=True)
+        tuf_root = self._metadata_dir / "root.json"
+
+        if not tuf_root.exists():
+            try:
+                root_json = read_embedded("root.json", rsrc_prefix)
+            except FileNotFoundError as e:
+                raise RootError from e
+
+            tuf_root.write_bytes(root_json)
+
+        # Initialize targets cache dir
+        self._targets_dir.mkdir(parents=True, exist_ok=True)
+        trusted_root_target = self._targets_dir / "trusted_root.json"
+
+        if not trusted_root_target.exists():
+            try:
+                trusted_root_json = read_embedded("trusted_root.json", rsrc_prefix)
+            except FileNotFoundError as e:
+                raise RootError from e
+
+            trusted_root_target.write_bytes(trusted_root_json)
+
+        logger.debug(f"TUF metadata: {self._metadata_dir}")
+        logger.debug(f"TUF targets cache: {self._targets_dir}")
 
     @classmethod
-    def production(cls) -> Signer:
+    def production(cls) -> TrustUpdater:
         """
-        Return a `Signer` instance configured against Sigstore's production-level services.
+        Returns a `TrustUpdater` for the Sigstore production instances.
         """
-        updater = TrustUpdater.production()
-        rekor = RekorClient.production(updater)
-        return cls(fulcio=FulcioClient.production(), rekor=rekor)
+        return cls(DEFAULT_TUF_URL)
 
     @classmethod
-    def staging(cls) -> Signer:
+    def staging(cls) -> TrustUpdater:
         """
-        Return a `Signer` instance configured against Sigstore's staging-level services.
+        Returns a `TrustUpdater` for the Sigstore staging instances.
         """
-        updater = TrustUpdater.staging()
-        rekor = RekorClient.staging(updater)
-        return cls(fulcio=FulcioClient.staging(), rekor=rekor)
-
-    def sign(
-        self,
-        input_: IO[bytes],
-        identity_token: str,
-    ) -> SigningResult:
-        """Public API for signing blobs"""
-        input_digest = sha256_streaming(input_)
-
-        logger.debug("Generating ephemeral keys...")
-        private_key = ec.generate_private_key(ec.SECP384R1())
-
-        logger.debug("Retrieving signed certificate...")
-
-        oidc_identity = Identity(identity_token)
-        logger.debug(f"cert-identity: {oidc_identity.proof}")
-        logger.debug(f"cert-oidc-issuer: {oidc_identity.issuer}")
-
-        # Build an X.509 Certificiate Signing Request
-        builder = (
-            x509.CertificateSigningRequestBuilder()
-            .subject_name(
-                x509.Name(
-                    [
-                        x509.NameAttribute(NameOID.EMAIL_ADDRESS, oidc_identity.proof),
-                    ]
-                )
-            )
-            .add_extension(
-                x509.BasicConstraints(ca=False, path_length=None),
-                critical=True,
-            )
-        )
-        certificate_request = builder.sign(private_key, hashes.SHA256())
+        return cls(STAGING_TUF_URL)
 
-        certificate_response = self._fulcio.signing_cert.post(
-            certificate_request, identity_token
+    @lru_cache()
+    def _updater(self) -> Updater:
+        """Initialize and update the toplevel TUF metadata"""
+        updater = Updater(
+            metadata_dir=str(self._metadata_dir),
+            metadata_base_url=self._repo_url,
+            target_base_url=parse.urljoin(f"{self._repo_url}/", "targets/"),
+            target_dir=str(self._targets_dir),
+            fetcher=_get_fetcher(),
         )
 
-        # TODO(alex): Retrieve the public key via TUF
-        #
-        # Verify the SCT
-        sct = certificate_response.sct  # noqa
-        cert = certificate_response.cert  # noqa
-        chain = certificate_response.chain
-
-        verify_sct(sct, cert, chain, self._rekor._ct_keyring)
-
-        logger.debug("Successfully verified SCT...")
-
-        # Sign artifact
-        artifact_signature = private_key.sign(
-            input_digest, ec.ECDSA(Prehashed(hashes.SHA256()))
-        )
-        b64_artifact_signature = B64Str(base64.b64encode(artifact_signature).decode())
+        # NOTE: we would like to avoid refresh if the toplevel metadata is valid.
+        # https://github.com/theupdateframework/python-tuf/issues/2225
+        try:
+            updater.refresh()
+        except Exception as e:
+            raise TUFError("Failed to refresh TUF metadata") from e
+
+        return updater
+
+    @lru_cache()
+    def _get_trusted_root(self) -> TrustedRoot:
+        root_info = self._updater().get_targetinfo("trusted_root.json")
+        if root_info is None:
+            raise TUFError("Unsupported TUF configuration: no trusted root")
+        path = self._updater().find_cached_target(root_info)
+        if path is None:
+            try:
+                path = self._updater().download_target(root_info)
+            except (
+                TUFExceptions.DownloadError,
+                TUFExceptions.RepositoryError,
+            ) as e:
+                raise TUFError("Failed to download trusted key bundle") from e
+
+        logger.debug("Found trusted root")
+        return TrustedRoot().from_json(Path(path).read_bytes())
+
+    def _get_tlog_keys(self, tlogs: list[TransparencyLogInstance]) -> Iterable[bytes]:
+        """Return public key contents given transparency log instances."""
+
+        for key in tlogs:
+            if not _is_timerange_valid(key.public_key.valid_for, allow_expired=False):
+                continue
+            key_bytes = key.public_key.raw_bytes
+            if key_bytes:
+                yield key_bytes
+
+    def _get_ca_keys(
+        self, cas: list[CertificateAuthority], *, allow_expired: bool
+    ) -> Iterable[bytes]:
+        """Return public key contents given certificate authorities."""
+
+        for ca in cas:
+            if not _is_timerange_valid(ca.valid_for, allow_expired=allow_expired):
+                continue
+            for cert in ca.cert_chain.certificates:
+                yield cert.raw_bytes
 
-        # Prepare inputs
-        b64_cert = base64.b64encode(
-            cert.public_bytes(encoding=serialization.Encoding.PEM)
-        )
+    def get_ctfe_keys(self) -> list[bytes]:
+        """Return the active CTFE public keys contents.
 
-        # Create the transparency log entry
-        entry = self._rekor.log.entries.post(
-            b64_artifact_signature=B64Str(b64_artifact_signature),
-            sha256_artifact_hash=input_digest.hex(),
-            b64_cert=B64Str(b64_cert.decode()),
-        )
+        May download files from the remote repository.
+        """
+        ctfes: list[bytes]
 
-        logger.debug(f"Transparency log entry created with index: {entry.log_index}")
+        trusted_root = self._get_trusted_root()
+        ctfes = list(self._get_tlog_keys(trusted_root.ctlogs))
 
-        return SigningResult(
-            input_digest=HexStr(input_digest.hex()),
-            cert_pem=PEMCert(
-                cert.public_bytes(encoding=serialization.Encoding.PEM).decode()
-            ),
-            b64_signature=B64Str(b64_artifact_signature),
-            log_entry=entry,
-        )
+        if not ctfes:
+            raise MetadataError("CTFE keys not found in TUF metadata")
+        return ctfes
 
+    def get_rekor_keys(self) -> list[bytes]:
+        """Return the rekor public key content.
 
-class SigningResult(BaseModel):
-    """
-    Represents the artifacts of a signing operation.
-    """
-
-    input_digest: HexStr
-    """
-    The hex-encoded SHA256 digest of the input that was signed for.
-    """
+        May download files from the remote repository.
+        """
+        keys: list[bytes]
 
-    cert_pem: PEMCert
-    """
-    The PEM-encoded public half of the certificate used for signing.
-    """
+        trusted_root = self._get_trusted_root()
+        keys = list(self._get_tlog_keys(trusted_root.tlogs))
 
-    b64_signature: B64Str
-    """
-    The base64-encoded signature.
-    """
+        if len(keys) != 1:
+            raise MetadataError("Did not find one active Rekor key in TUF metadata")
+        return keys
 
-    log_entry: LogEntry
-    """
-    A record of the Rekor log entry for the signing operation.
-    """
+    def get_fulcio_certs(self) -> list[Certificate]:
+        """Return the Fulcio certificates.
 
-    def _to_bundle(self) -> Bundle:
-        """
-        Creates a Sigstore bundle (as defined by Sigstore's protobuf specs)
-        from this `SigningResult`.
+        May download files from the remote repository.
         """
+        certs: list[Certificate]
 
-        # TODO: Include the current Fulcio intermediate and root in the
-        # chain as well.
-        cert = x509.load_pem_x509_certificate(self.cert_pem.encode())
-        cert_der = cert.public_bytes(encoding=serialization.Encoding.DER)
-        chain = X509CertificateChain(certificates=[X509Certificate(raw_bytes=cert_der)])
-
-        inclusion_proof: InclusionProof | None = None
-        if self.log_entry.inclusion_proof is not None:
-            inclusion_proof = InclusionProof(
-                log_index=self.log_entry.inclusion_proof.log_index,
-                root_hash=bytes.fromhex(self.log_entry.inclusion_proof.root_hash),
-                tree_size=self.log_entry.inclusion_proof.tree_size,
-                hashes=[
-                    bytes.fromhex(h) for h in self.log_entry.inclusion_proof.hashes
-                ],
+        trusted_root = self._get_trusted_root()
+        # Return expired certificates too: they are expired now but may have
+        # been active when the certificate was used to sign.
+        certs = [
+            load_der_x509_certificate(c)
+            for c in self._get_ca_keys(
+                trusted_root.certificate_authorities, allow_expired=True
             )
+        ]
 
-        tlog_entry = TransparencyLogEntry(
-            log_index=self.log_entry.log_index,
-            log_id=LogId(key_id=bytes.fromhex(self.log_entry.log_id)),
-            kind_version=KindVersion(kind="hashedrekord", version="0.0.1"),
-            integrated_time=self.log_entry.integrated_time,
-            inclusion_promise=InclusionPromise(
-                signed_entry_timestamp=base64.b64decode(
-                    self.log_entry.signed_entry_timestamp
-                )
-            ),
-            inclusion_proof=inclusion_proof,
-            canonicalized_body=base64.b64decode(self.log_entry.body),
-        )
-
-        material = VerificationMaterial(
-            x509_certificate_chain=chain,
-            tlog_entries=[tlog_entry],
-        )
-
-        bundle = Bundle(
-            media_type="application/vnd.dev.sigstore.bundle+json;version=0.1",
-            verification_material=material,
-            message_signature=MessageSignature(
-                message_digest=HashOutput(
-                    algorithm=HashAlgorithm.SHA2_256,
-                    digest=bytes.fromhex(self.input_digest),
-                ),
-                signature=base64.b64decode(self.b64_signature),
-            ),
-        )
-
-        return bundle
+        if not certs:
+            raise MetadataError("Fulcio certificates not found in TUF metadata")
+        return certs
```

### Comparing `sigstore-1.1.2rc1/sigstore/transparency.py` & `sigstore-2.0.0rc1/sigstore/transparency.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,49 +62,49 @@
     """
 
     log_index: int
     """
     The index of this entry within the log.
     """
 
-    inclusion_proof: Optional["LogInclusionProof"]
+    inclusion_proof: Optional[LogInclusionProof]
     """
     An optional inclusion proof for this log entry.
-
-    Only present for entries retrieved from online logs.
     """
 
-    signed_entry_timestamp: B64Str
+    inclusion_promise: B64Str
     """
-    The base64-encoded Signed Entry Timestamp (SET) for this log entry.
+    An inclusion promise for this log entry.
+
+    Internally, this is a base64-encoded Signed Entry Timestamp (SET) for this
+    log entry.
     """
 
     @classmethod
     def _from_response(cls, dict_: dict[str, Any]) -> LogEntry:
         """
         Create a new `LogEntry` from the given API response.
         """
 
         # Assumes we only get one entry back
         entries = list(dict_.items())
         if len(entries) != 1:
             raise ValueError("Received multiple entries in response")
 
         uuid, entry = entries[0]
-
         return LogEntry(
             uuid=uuid,
             body=entry["body"],
             integrated_time=entry["integratedTime"],
             log_id=entry["logID"],
             log_index=entry["logIndex"],
             inclusion_proof=LogInclusionProof.parse_obj(
                 entry["verification"]["inclusionProof"]
             ),
-            signed_entry_timestamp=entry["verification"]["signedEntryTimestamp"],
+            inclusion_promise=entry["verification"]["signedEntryTimestamp"],
         )
 
     def encode_canonical(self) -> bytes:
         """
         Returns a canonicalized JSON (RFC 8785) representation of the transparency log entry.
 
         This encoded representation is suitable for verification against
@@ -121,18 +121,19 @@
 
 
 class LogInclusionProof(BaseModel):
     """
     Represents an inclusion proof for a transparency log entry.
     """
 
+    checkpoint: StrictStr = Field(..., alias="checkpoint")
+    hashes: List[StrictStr] = Field(..., alias="hashes")
     log_index: StrictInt = Field(..., alias="logIndex")
     root_hash: StrictStr = Field(..., alias="rootHash")
     tree_size: StrictInt = Field(..., alias="treeSize")
-    hashes: List[StrictStr] = Field(..., alias="hashes")
 
     class Config:
         allow_population_by_field_name = True
 
     @validator("log_index")
     def _log_index_positive(cls, v: int) -> int:
         if v < 0:
```

### Comparing `sigstore-1.1.2rc1/sigstore/verify/__init__.py` & `sigstore-2.0.0rc1/sigstore/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2rc1/sigstore/verify/models.py` & `sigstore-2.0.0rc1/sigstore/verify/policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,329 +9,300 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Common (base) models for the verification APIs.
+APIs for describing identity verification "policies", which describe how the identities
+passed into an individual verification step are verified.
 """
 
 from __future__ import annotations
 
-import base64
-import json
 import logging
-from dataclasses import dataclass
-from typing import IO
+from abc import ABC, abstractmethod
+from typing import cast
+
+try:
+    from typing import Protocol
+except ImportError:  # pragma: no cover
+    # TODO(ww): Remove when our minimum Python is 3.8.
+    from typing_extensions import Protocol  # type: ignore[assignment]
 
-from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.x509 import (
     Certificate,
-    load_der_x509_certificate,
-    load_pem_x509_certificate,
+    ExtensionNotFound,
+    ObjectIdentifier,
+    OtherName,
+    RFC822Name,
+    SubjectAlternativeName,
+    UniformResourceIdentifier,
 )
-from pydantic import BaseModel
-from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import Bundle
 
-from sigstore._internal.rekor import RekorClient
-from sigstore._utils import (
-    B64Str,
-    PEMCert,
-    base64_encode_pem_cert,
-    sha256_streaming,
+from sigstore.verify.models import (
+    VerificationFailure,
+    VerificationResult,
+    VerificationSuccess,
 )
-from sigstore.transparency import LogEntry, LogInclusionProof
 
 logger = logging.getLogger(__name__)
 
+# From: https://github.com/sigstore/fulcio/blob/main/docs/oid-info.md
+_OIDC_ISSUER_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.1")
+_OIDC_GITHUB_WORKFLOW_TRIGGER_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.2")
+_OIDC_GITHUB_WORKFLOW_SHA_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.3")
+_OIDC_GITHUB_WORKFLOW_NAME_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.4")
+_OIDC_GITHUB_WORKFLOW_REPOSITORY_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.5")
+_OIDC_GITHUB_WORKFLOW_REF_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.6")
+_OTHERNAME_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.7")
 
-class VerificationResult(BaseModel):
-    """
-    Represents the result of a verification operation.
 
-    Results are boolish, and failures contain a reason (and potentially
-    some additional context).
+class _SingleX509ExtPolicy(ABC):
+    """
+    An ABC for verification policies that boil down to checking a single
+    X.509 extension's value.
     """
 
-    success: bool
+    oid: ObjectIdentifier
     """
-    Represents the status of this result.
+    The OID of the extension being checked.
     """
 
-    def __bool__(self) -> bool:
+    def __init__(self, value: str) -> None:
+        """
+        Creates the new policy, with `value` as the expected value during
+        verification.
         """
-        Returns a boolean representation of this result.
+        self._value = value
 
-        `VerificationSuccess` is always `True`, and `VerificationFailure`
-        is always `False`.
+    def verify(self, cert: Certificate) -> VerificationResult:
         """
-        return self.success
+        Verify this policy against `cert`.
+        """
+        try:
+            ext = cert.extensions.get_extension_for_oid(self.oid).value
+        except ExtensionNotFound:
+            return VerificationFailure(
+                reason=(
+                    f"Certificate does not contain {self.__class__.__name__} "
+                    f"({self.oid.dotted_string}) extension"
+                )
+            )
 
+        # NOTE(ww): mypy is confused by the `Extension[ExtensionType]` returned
+        # by `get_extension_for_oid` above.
+        ext_value = ext.value.decode()  # type: ignore[attr-defined]
+        if ext_value != self._value:
+            return VerificationFailure(
+                reason=(
+                    f"Certificate's {self.__class__.__name__} does not match "
+                    f"(got {ext_value}, expected {self._value})"
+                )
+            )
+
+        return VerificationSuccess()
 
-class VerificationSuccess(VerificationResult):
-    """
-    The verification completed successfully,
-    """
 
-    success: bool = True
+class OIDCIssuer(_SingleX509ExtPolicy):
     """
-    See `VerificationResult.success`.
+    Verifies the certificate's OIDC issuer, identified by
+    an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.1`.
     """
 
+    oid = _OIDC_ISSUER_OID
 
-class VerificationFailure(VerificationResult):
-    """
-    The verification failed, due to `reason`.
-    """
 
-    success: bool = False
+class GitHubWorkflowTrigger(_SingleX509ExtPolicy):
     """
-    See `VerificationResult.success`.
+    Verifies the certificate's GitHub Actions workflow trigger,
+    identified by an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.2`.
     """
 
-    reason: str
-    """
-    A human-readable explanation or description of the verification failure.
-    """
+    oid = _OIDC_GITHUB_WORKFLOW_TRIGGER_OID
 
 
-class InvalidMaterials(Exception):
+class GitHubWorkflowSHA(_SingleX509ExtPolicy):
     """
-    The associated `VerificationMaterials` are invalid in some way.
+    Verifies the certificate's GitHub Actions workflow commit SHA,
+    identified by an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.3`.
     """
 
+    oid = _OIDC_GITHUB_WORKFLOW_SHA_OID
 
-class RekorEntryMissing(Exception):
-    """
-    Raised if `VerificationMaterials.rekor_entry()` fails to find an entry
-    in the Rekor log.
 
-    This is an internal exception; users should not see it.
+class GitHubWorkflowName(_SingleX509ExtPolicy):
+    """
+    Verifies the certificate's GitHub Actions workflow name,
+    identified by an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.4`.
     """
 
-    pass
+    oid = _OIDC_GITHUB_WORKFLOW_NAME_OID
 
 
-class InvalidRekorEntry(InvalidMaterials):
+class GitHubWorkflowRepository(_SingleX509ExtPolicy):
     """
-    Raised if the effective Rekor entry in `VerificationMaterials.rekor_entry()`
-    does not match the other materials in `VerificationMaterials`.
-
-    This can only happen in two scenarios:
-
-    * A user has supplied the wrong offline entry, potentially maliciously;
-    * The Rekor log responded with the wrong entry, suggesting a server error.
+    Verifies the certificate's GitHub Actions workflow repository,
+    identified by an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.5`.
     """
 
-    pass
+    oid = _OIDC_GITHUB_WORKFLOW_REPOSITORY_OID
 
 
-@dataclass(init=False)
-class VerificationMaterials:
+class GitHubWorkflowRef(_SingleX509ExtPolicy):
     """
-    Represents the materials needed to perform a Sigstore verification.
+    Verifies the certificate's GitHub Actions workflow ref,
+    identified by an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.6`.
     """
 
-    input_digest: bytes
+    oid = _OIDC_GITHUB_WORKFLOW_REF_OID
+
+
+class VerificationPolicy(Protocol):
     """
-    The SHA256 hash of the verification input, as raw bytes.
+    A protocol type describing the interface that all verification policies
+    conform to.
     """
 
-    certificate: Certificate
-    """
-    The certificate that attests to and contains the public signing key.
+    @abstractmethod
+    def verify(self, cert: Certificate) -> VerificationResult:
+        """
+        Verify the given `cert` against this policy, returning a `VerificationResult`.
+        """
+        raise NotImplementedError  # pragma: no cover
 
-    # TODO: Support a certificate chain here, with optional intermediates.
-    """
 
-    signature: bytes
-    """
-    The raw signature.
+class AnyOf:
     """
+    The "any of" policy, corresponding to a logical OR between child policies.
 
-    _offline: bool
+    An empty list of child policies is considered trivially invalid.
     """
-    Whether to do offline Rekor entry verification.
 
-    NOTE: This is intentionally not a public field, since it's slightly
-    mismatched against the other members of `VerificationMaterials` -- it's
-    more of an option than a piece of verification material.
-    """
+    def __init__(self, children: list[VerificationPolicy]):
+        """
+        Create a new `AnyOf`, with the given child policies.
+        """
+        self._children = children
 
-    _rekor_entry: LogEntry | None
-    """
-    An optional Rekor entry.
+    def verify(self, cert: Certificate) -> VerificationResult:
+        """
+        Verify `cert` against the policy.
+        """
+        verified = any(child.verify(cert) for child in self._children)
+        if verified:
+            return VerificationSuccess()
+        else:
+            return VerificationFailure(
+                reason=f"0 of {len(self._children)} policies succeeded"
+            )
 
-    If a Rekor entry is supplied **and** `offline` is set to `True`,
-    verification will be done against this entry rather than the against the
-    online transparency log. If not provided **or** `offline` is `False` (the
-    default), then the online transparency log will be used.
 
-    NOTE: This is **intentionally not a public field**. The `rekor_entry()`
-    method should be used to access a Rekor log entry for these materials,
-    as it performs the online lookup if an offline entry is not provided
-    and, **critically**, validates that the entry's contents match the other
-    signing materials. Without this check an adversary could present a
-    **valid but unrelated** Rekor entry during verification, similar
-    to CVE-2022-36056 in cosign.
+class AllOf:
+    """
+    The "all of" policy, corresponding to a logical AND between child
+    policies.
 
-    TODO: Support multiple entries here, with verification contingent on
-    all being valid.
+    An empty list of child policies is considered trivially invalid.
     """
 
-    def __init__(
-        self,
-        *,
-        input_: IO[bytes],
-        cert_pem: PEMCert,
-        signature: bytes,
-        offline: bool = False,
-        rekor_entry: LogEntry | None,
-    ):
+    def __init__(self, children: list[VerificationPolicy]):
+        """
+        Create a new `AllOf`, with the given child policies.
         """
-        Create a new `VerificationMaterials` from the given materials.
 
-        `offline` controls the behavior of any subsequent verification over
-        these materials: if `True`, the supplied Rekor entry (which must
-        be supplied) will be verified via its Signed Entry Timestamp, but
-        its proof of inclusion will not be checked. This is a slightly weaker
-        verification mode, as it demonstrates that an entry has been signed by
-        the log but not necessarily included in it.
+        self._children = children
 
-        Effect: `input_` is consumed as part of construction.
+    def verify(self, cert: Certificate) -> VerificationResult:
+        """
+        Verify `cert` against the policy.
         """
 
-        self.input_digest = sha256_streaming(input_)
-        self.certificate = load_pem_x509_certificate(cert_pem.encode())
-        self.signature = signature
+        # Without this, we'd consider empty lists of child policies trivially valid.
+        # This is almost certainly not what the user wants and is a potential
+        # source of API misuse, so we explicitly disallow it.
+        if len(self._children) < 1:
+            return VerificationFailure(reason="no child policies to verify")
+
+        # NOTE(ww): We need the cast here because MyPy can't tell that
+        # `VerificationResult.__bool__` is invariant with
+        # `VerificationSuccess | VerificationFailure`.
+        results = [child.verify(cert) for child in self._children]
+        failures = [
+            cast(VerificationFailure, result).reason for result in results if not result
+        ]
+        if len(failures) > 0:
+            inner_reasons = ", ".join(failures)
+            return VerificationFailure(
+                reason=f"{len(failures)} of {len(self._children)} policies failed: {inner_reasons}"
+            )
+        return VerificationSuccess()
 
-        # Invariant: requesting offline verification means that a Rekor entry
-        # *must* be provided.
-        if offline and not rekor_entry:
-            raise InvalidMaterials("offline verification requires a Rekor entry")
 
-        self._offline = offline
-        self._rekor_entry = rekor_entry
+class UnsafeNoOp:
+    """
+    The "no-op" policy, corresponding to a no-op "verification".
 
-    @classmethod
-    def from_bundle(
-        cls, *, input_: IO[bytes], bundle: Bundle, offline: bool = False
-    ) -> VerificationMaterials:
-        """
-        Create a new `VerificationMaterials` from the given Sigstore bundle.
+    **This policy is fundamentally insecure. You cannot use it safely.
+    It must not be used to verify any sort of certificate identity, because
+    it cannot do so. Using this policy is equivalent to reducing the
+    verification proof down to an integrity check against a completely
+    untrusted and potentially attacker-created signature. It must only
+    be used for testing purposes.**
+    """
 
-        Effect: `input_` is consumed as part of construction.
+    def verify(self, cert: Certificate) -> VerificationResult:
+        """
+        Verify `cert` against the policy.
         """
-        certs = bundle.verification_material.x509_certificate_chain.certificates
-        if len(certs) == 0:
-            raise InvalidMaterials("expected non-empty certificate chain in bundle")
-        cert_pem = PEMCert(
-            load_der_x509_certificate(certs[0].raw_bytes)
-            .public_bytes(Encoding.PEM)
-            .decode()
-        )
-
-        signature = bundle.message_signature.signature
-
-        tlog_entries = bundle.verification_material.tlog_entries
-        if len(tlog_entries) != 1:
-            raise InvalidMaterials(
-                f"expected exactly one log entry, got {len(tlog_entries)}"
-            )
-        tlog_entry = tlog_entries[0]
 
-        inclusion_proof = LogInclusionProof(
-            log_index=tlog_entry.inclusion_proof.log_index,
-            root_hash=tlog_entry.inclusion_proof.root_hash.hex(),
-            tree_size=tlog_entry.inclusion_proof.tree_size,
-            hashes=[h.hex() for h in tlog_entry.inclusion_proof.hashes],
-        )
-        entry = LogEntry(
-            uuid=None,
-            body=B64Str(base64.b64encode(tlog_entry.canonicalized_body).decode()),
-            integrated_time=tlog_entry.integrated_time,
-            log_id=tlog_entry.log_id.key_id.hex(),
-            log_index=tlog_entry.log_index,
-            inclusion_proof=inclusion_proof,
-            signed_entry_timestamp=B64Str(
-                base64.b64encode(
-                    tlog_entry.inclusion_promise.signed_entry_timestamp
-                ).decode()
-            ),
+        logger.warning(
+            "unsafe (no-op) verification policy used! no verification performed!"
         )
+        return VerificationSuccess()
 
-        return cls(
-            input_=input_,
-            cert_pem=PEMCert(cert_pem),
-            signature=signature,
-            offline=offline,
-            rekor_entry=entry,
-        )
 
-    @property
-    def has_rekor_entry(self) -> bool:
-        """
-        Returns whether or not these `VerificationMaterials` contain a Rekor
-        entry.
+class Identity:
+    """
+    Verifies the certificate's "identity", corresponding to the X.509v3 SAN.
+    Identities are verified modulo an OIDC issuer, so the issuer's URI
+    is also required.
 
-        If false, `VerificationMaterials.rekor_entry()` performs an online lookup.
-        """
-        return self._rekor_entry is not None
+    Supported SAN types include emails, URIs, and Sigstore-specific "other names".
+    """
 
-    def rekor_entry(self, client: RekorClient) -> LogEntry:
+    def __init__(self, *, identity: str, issuer: str):
         """
-        Returns a `RekorEntry` for the current signing materials.
+        Create a new `Identity`, with the given expected identity and issuer values.
         """
-        entry: LogEntry | None
-        if self._offline and self.has_rekor_entry:
-            logger.debug("using offline rekor entry")
-            entry = self._rekor_entry
-        else:
-            logger.debug("retrieving rekor entry")
-            entry = client.log.entries.retrieve.post(
-                self.signature,
-                self.input_digest.hex(),
-                self.certificate,
-            )
 
-        if entry is None:
-            raise RekorEntryMissing
+        self._identity = identity
+        self._issuer = OIDCIssuer(issuer)
 
-        # To verify that an entry matches our other signing materials,
-        # we transform our signature, artifact hash, and certificate
-        # into a "hashedrekord" style payload and compare it against the
-        # entry's own body.
-        #
-        # This is done by:
-        #
-        # * Serializing the certificate as PEM, and then base64-encoding it;
-        # * base64-encoding the signature;
-        # * Packing the resulting cert, signature, and hash into the
-        #   hashedrekord body format;
-        # * Comparing that body against the entry's own body, which
-        #   is extracted from its base64(json(...)) encoding.
-
-        logger.debug("Rekor entry: ensuring contents match signing materials")
-
-        expected_body = {
-            "kind": "hashedrekord",
-            "apiVersion": "0.0.1",
-            "spec": {
-                "signature": {
-                    "content": B64Str(base64.b64encode(self.signature).decode()),
-                    "publicKey": {
-                        "content": B64Str(base64_encode_pem_cert(self.certificate))
-                    },
-                },
-                "data": {
-                    "hash": {"algorithm": "sha256", "value": self.input_digest.hex()}
-                },
-            },
-        }
+    def verify(self, cert: Certificate) -> VerificationResult:
+        """
+        Verify `cert` against the policy.
+        """
 
-        actual_body = json.loads(base64.b64decode(entry.body))
+        issuer_verified: VerificationResult = self._issuer.verify(cert)
+        if not issuer_verified:
+            return issuer_verified
+
+        # Build a set of all valid identities.
+        san_ext = cert.extensions.get_extension_for_class(SubjectAlternativeName).value
+        all_sans = set(san_ext.get_values_for_type(RFC822Name))
+        all_sans.update(san_ext.get_values_for_type(UniformResourceIdentifier))
+        all_sans.update(
+            [
+                on.value.decode()
+                for on in san_ext.get_values_for_type(OtherName)
+                if on.type_id == _OTHERNAME_OID
+            ]
+        )
 
-        if expected_body != actual_body:
-            raise InvalidRekorEntry
+        verified = self._identity in all_sans
+        if not verified:
+            return VerificationFailure(
+                reason=f"Certificate's SANs do not match {self._identity}; actual SANs: {all_sans}"
+            )
 
-        return entry
+        return VerificationSuccess()
```

### Comparing `sigstore-1.1.2rc1/sigstore/verify/verifier.py` & `sigstore-2.0.0rc1/sigstore/verify/verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     X509StoreContextError,
 )
 
 from sigstore._internal.merkle import (
     InvalidInclusionProofError,
     verify_merkle_inclusion,
 )
+from sigstore._internal.rekor.checkpoint import (
+    CheckpointError,
+    verify_checkpoint,
+)
 from sigstore._internal.rekor.client import RekorClient
 from sigstore._internal.set import InvalidSETError, verify_set
 from sigstore._internal.tuf import TrustUpdater
 from sigstore._utils import B64Str, HexStr
 from sigstore.verify.models import InvalidRekorEntry as InvalidRekorEntryError
 from sigstore.verify.models import RekorEntryMissing as RekorEntryMissingError
 from sigstore.verify.models import (
@@ -242,38 +246,52 @@
         except InvalidRekorEntryError:
             return VerificationFailure(
                 reason="Rekor entry contents do not match other signing materials"
             )
 
         # 5) Verify the inclusion proof supplied by Rekor for this artifact.
         #
-        # We skip the inclusion proof only if explicitly requested.
-        if not materials._offline:
+        # The inclusion proof should always be present in the online case. In
+        # the offline case, if it is present, we verify it.
+        if entry.inclusion_proof:
             try:
                 verify_merkle_inclusion(entry)
             except InvalidInclusionProofError as exc:
                 return VerificationFailure(
                     reason=f"invalid Rekor inclusion proof: {exc}"
                 )
+
+            try:
+                verify_checkpoint(self._rekor, entry)
+            except CheckpointError as exc:
+                return VerificationFailure(reason=f"invalid Rekor root hash: {exc}")
+
+            logger.debug("Successfully verified inclusion proof...")
+        elif not materials._offline:
+            # Paranoia: if we weren't given an inclusion proof, then
+            # this *must* have been offline verification. If it was online
+            # then we've somehow entered an invalid state, so fail.
+            return VerificationFailure(reason="missing Rekor inclusion proof")
         else:
-            logger.debug(
-                "offline verification requested: skipping Merkle inclusion proof"
+            logger.warning(
+                "inclusion proof not present in bundle: skipping due to offline verification"
             )
 
         # 6) Verify the Signed Entry Timestamp (SET) supplied by Rekor for this artifact
         try:
             verify_set(self._rekor, entry)
         except InvalidSETError as inval_set:
             return VerificationFailure(reason=f"invalid Rekor entry SET: {inval_set}")
 
         # 7) Verify that the signing certificate was valid at the time of signing
         integrated_time = datetime.datetime.utcfromtimestamp(entry.integrated_time)
-        if (
-            integrated_time < materials.certificate.not_valid_before
-            or integrated_time >= materials.certificate.not_valid_after
+        if not (
+            materials.certificate.not_valid_before
+            <= integrated_time
+            <= materials.certificate.not_valid_after
         ):
             return VerificationFailure(
                 reason="invalid signing cert: expired at time of Rekor entry"
             )
 
         logger.debug(f"Successfully verified Rekor entry at index {entry.log_index}")
         return VerificationSuccess()
```

### Comparing `sigstore-1.1.2rc1/PKG-INFO` & `sigstore-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore
-Version: 1.1.2rc1
+Version: 2.0.0rc1
 Summary: A tool for signing Python package distributions
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -23,25 +23,25 @@
 Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
 Requires-Dist: pydantic ~= 1.10
 Requires-Dist: pyjwt >= 2.1
 Requires-Dist: pyOpenSSL >= 23.0.0
 Requires-Dist: requests
 Requires-Dist: securesystemslib
 Requires-Dist: sigstore-protobuf-specs ~= 0.1.0
-Requires-Dist: tuf ~= 2.1
+Requires-Dist: tuf >= 2.1,< 4.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump >= 1.3.2 ; extra == "dev"
 Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ~= 1.1 ; extra == "lint"
-Requires-Dist: ruff < 0.0.256 ; extra == "lint"
+Requires-Dist: ruff < 0.0.275 ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: typing-extensions ; extra == "lint" and ( python_version < '3.8')
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
@@ -149,20 +149,24 @@
 
 Top-level:
 
 <!-- @begin-sigstore-help@ -->
 ```
 usage: sigstore [-h] [-V] [-v] [--staging] [--rekor-url URL]
                 [--rekor-root-pubkey FILE]
-                {sign,verify,get-identity-token} ...
+                COMMAND ...
 
 a tool for signing and verifying Python package distributions
 
 positional arguments:
-  {sign,verify,get-identity-token}
+  COMMAND               the operation to perform
+    sign                sign one or more inputs
+    verify              verify one or more inputs
+    get-identity-token  retrieve and return a Sigstore-compatible OpenID
+                        Connect token
 
 optional arguments:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -v, --verbose         run with additional debug logging; supply multiple
                         times to increase verbosity (default: 0)
 
@@ -181,19 +185,19 @@
 ### Signing
 
 <!-- @begin-sigstore-sign-help@ -->
 ```
 usage: sigstore sign [-h] [--identity-token TOKEN] [--oidc-client-id ID]
                      [--oidc-client-secret SECRET]
                      [--oidc-disable-ambient-providers] [--oidc-issuer URL]
-                     [--no-default-files] [--signature FILE]
-                     [--certificate FILE] [--bundle FILE] [--no-bundle]
-                     [--overwrite] [--staging] [--rekor-url URL]
-                     [--rekor-root-pubkey FILE] [--fulcio-url URL]
-                     [--ctfe FILE]
+                     [--oauth-force-oob] [--no-default-files]
+                     [--signature FILE] [--certificate FILE] [--bundle FILE]
+                     [--output-directory DIR] [--overwrite] [--staging]
+                     [--rekor-url URL] [--rekor-root-pubkey FILE]
+                     [--fulcio-url URL] [--ctfe FILE]
                      FILE [FILE ...]
 
 positional arguments:
   FILE                  The file to sign
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -207,29 +211,33 @@
                         The custom OpenID Connect client secret to use during
                         OAuth2 (default: None)
   --oidc-disable-ambient-providers
                         Disable ambient OpenID Connect credential detection
                         (e.g. on GitHub Actions) (default: False)
   --oidc-issuer URL     The OpenID Connect issuer to use (conflicts with
                         --staging) (default: https://oauth2.sigstore.dev/auth)
+  --oauth-force-oob     Force an out-of-band OAuth flow and do not
+                        automatically start the default web browser (default:
+                        False)
 
 Output options:
-  --no-default-files    Don't emit the default output files ({input}.sig,
-                        {input}.crt, {input}.rekor) (default: False)
+  --no-default-files    Don't emit the default output files ({input}.sigstore)
+                        (default: False)
   --signature FILE, --output-signature FILE
                         Write a single signature to the given file; does not
                         work with multiple input files (default: None)
   --certificate FILE, --output-certificate FILE
                         Write a single certificate to the given file; does not
                         work with multiple input files (default: None)
   --bundle FILE         Write a single Sigstore bundle to the given file; does
                         not work with multiple input files (default: None)
-  --no-bundle           Don't emit {input}.sigstore files for each input; this
-                        option is experimental and may change between releases
-                        until stabilized (default: False)
+  --output-directory DIR
+                        Write default outputs to the given directory
+                        (conflicts with --signature, --certificate, --bundle)
+                        (default: None)
   --overwrite           Overwrite preexisting signature and certificate
                         outputs, if present (default: False)
 
 Sigstore instance options:
   --staging             Use sigstore's staging instances, instead of the
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
@@ -308,18 +316,14 @@
   --certificate-chain FILE
                         Path to a list of CA certificates in PEM format which
                         will be needed when building the certificate chain for
                         the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-identity-help@ -->
 
-For backwards compatibility, `sigstore verify [args ...]` is equivalent to
-`sigstore verify identity [args ...]`, but the latter form is **strongly**
-preferred.
-
 #### Signatures from GitHub Actions
 
 If your signatures are coming from GitHub Actions (e.g., a workflow
 that uses its [ambient credentials](#signing-with-ambient-credentials)),
 then you can use the `sigstore verify github` subcommand to verify
 claims more precisely than `sigstore verify identity` allows:
```

