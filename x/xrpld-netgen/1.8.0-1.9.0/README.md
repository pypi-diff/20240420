# Comparing `tmp/xrpld_netgen-1.8.0.tar.gz` & `tmp/xrpld_netgen-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpld_netgen-1.8.0.tar", max compression
+gzip compressed data, was "xrpld_netgen-1.9.0.tar", max compression
```

## Comparing `xrpld_netgen-1.8.0.tar` & `xrpld_netgen-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      768 2023-12-15 09:14:58.763233 xrpld_netgen-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-10-25 12:02:59.993204 xrpld_netgen-1.8.0/xrpld_netgen/__init__
--rw-r--r--   0        0        0    13799 2023-12-15 09:12:15.572152 xrpld_netgen-1.8.0/xrpld_netgen/cli.py
--rw-r--r--   0        0        0     2031 2023-11-23 14:37:16.371752 xrpld_netgen-1.8.0/xrpld_netgen/deploykit/config.json
--rwxr-xr-x   0        0        0      970 2023-11-17 00:21:06.280112 xrpld_netgen-1.8.0/xrpld_netgen/deploykit/entrypoint
--rw-r--r--   0        0        0       72 2023-11-17 00:21:06.280726 xrpld_netgen-1.8.0/xrpld_netgen/deploykit/nginx.dockerfile
--rw-r--r--   0        0        0     1611 2023-11-23 12:29:16.077445 xrpld_netgen-1.8.0/xrpld_netgen/libs/github.py
--rw-r--r--   0        0        0    14323 2023-12-15 08:13:49.820648 xrpld_netgen-1.8.0/xrpld_netgen/main.py
--rw-r--r--   0        0        0    14862 2023-12-15 08:27:53.149794 xrpld_netgen-1.8.0/xrpld_netgen/network.py
--rw-r--r--   0        0        0    11126 2023-12-13 14:37:33.492886 xrpld_netgen-1.8.0/xrpld_netgen/rippled_cfg.py
--rw-r--r--   0        0        0     4133 2023-12-14 11:45:46.435391 xrpld_netgen-1.8.0/xrpld_netgen/utils/deploy_kit.py
--rw-r--r--   0        0        0     4411 2023-12-15 08:11:57.719686 xrpld_netgen-1.8.0/xrpld_netgen/utils/misc.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 xrpld_netgen-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      768 2024-01-21 17:13:13.266390 xrpld_netgen-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-10-25 12:02:59.993204 xrpld_netgen-1.9.0/xrpld_netgen/__init__.py
+-rw-r--r--   0        0        0    13857 2024-01-21 17:12:47.651703 xrpld_netgen-1.9.0/xrpld_netgen/cli.py
+-rw-r--r--   0        0        0     2031 2023-11-23 14:37:16.371752 xrpld_netgen-1.9.0/xrpld_netgen/deploykit/config.json
+-rwxr-xr-x   0        0        0      970 2023-11-17 00:21:06.280112 xrpld_netgen-1.9.0/xrpld_netgen/deploykit/entrypoint
+-rw-r--r--   0        0        0       72 2023-11-17 00:21:06.280726 xrpld_netgen-1.9.0/xrpld_netgen/deploykit/nginx.dockerfile
+-rw-r--r--   0        0        0     1611 2023-11-23 12:29:16.077445 xrpld_netgen-1.9.0/xrpld_netgen/libs/github.py
+-rw-r--r--   0        0        0    14267 2024-01-21 17:12:24.370985 xrpld_netgen-1.9.0/xrpld_netgen/main.py
+-rw-r--r--   0        0        0    15445 2024-01-21 17:12:38.188742 xrpld_netgen-1.9.0/xrpld_netgen/network.py
+-rw-r--r--   0        0        0    12764 2024-01-15 19:15:00.296464 xrpld_netgen-1.9.0/xrpld_netgen/rippled_cfg.py
+-rw-r--r--   0        0        0     4133 2023-12-27 13:54:25.649254 xrpld_netgen-1.9.0/xrpld_netgen/utils/deploy_kit.py
+-rw-r--r--   0        0        0     4656 2023-12-27 17:47:31.084655 xrpld_netgen-1.9.0/xrpld_netgen/utils/misc.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 xrpld_netgen-1.9.0/PKG-INFO
```

### Comparing `xrpld_netgen-1.8.0/pyproject.toml` & `xrpld_netgen-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xrpld-netgen"
-version = "1.8.0"
+version = "1.9.0"
 description = "Xrpld network generator"
 authors = ["Denis Angell <dangell@transia.co>"]
 
 [tool.poetry.dependencies]
 python = "^3.9.6"
 pytest = "^7.2.1"
 pyyaml = "^6.0.1"
 requests = "^2.31.0"
-xrpld-publisher = "^1.0.5"
+xrpld-publisher = "^2.0.0"
 xrpl-helpers = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.8.4"
 black = "22.10.0"
 flake8-black = "^0.3.3"
 flake8-docstrings = "^1.5.0"
```

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/cli.py` & `xrpld_netgen-1.9.0/xrpld_netgen/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 # NETWORK
 # create:network
-# xrpld-netgen create:network --protocol "xahau" --version "2023.11.10-dev+549"
+# xrpld-netgen create:network --protocol "xahau" --build_version "2023.11.10-dev+549"
 # add:peer
 # xrpld-netgen add:peer --network_name xrpld-2023.11.10-dev+549 --protocol "xahau" --version "2023.11.10-dev+549"
 # remove:peer
 # xrpld-netgen remove:peer --network_name xrpld-2023.11.10-dev+549 --protocol "xahau" --version "2023.11.10-dev+549"
 # update:version
 # xrpld-netgen update:version --node --version xrpld-2023.11.10-dev+549
 # enable:amendment
@@ -38,26 +38,26 @@
 import argparse
 from xrpld_netgen.main import (
     create_standalone_binary,
     create_standalone_image,
     start_local,
 )
 from xrpld_netgen.network import (
-    create_network_binary,
+    create_network,
     update_node_binary,
     enable_node_amendment,
 )
 from xrpld_netgen.utils.misc import (
     run_file,
     remove_directory,
 )
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 
-XAHAU_RELEASE: str = "2023.11.10-dev+549"
+XAHAU_RELEASE: str = "2023.12.29-release+689"
 XRPL_RELEASE: str = "1.12.0"
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="A python cli to build xrpld networks and standalone ledgers."
     )
@@ -93,14 +93,15 @@
 
     # NETWORK
 
     # create:network
     parser_cn = subparsers.add_parser("create:network", help="Create Network")
     parser_cn.add_argument(
         "--protocol",
+        type=str,
         required=False,
         help="The protocol of the network",
         default="xahau",
     )
     parser_cn.add_argument(
         "--num_validators",
         type=int,
@@ -112,41 +113,71 @@
         "--num_peers",
         type=int,
         required=False,
         help="The number of peers in the network",
         default=1,
     )
     parser_cn.add_argument(
-        "--network_id", type=int, required=False, help="The network id", default=21339
+        "--network_id",
+        type=int,
+        required=False,
+        help="The id of the network",
+        default=21339,
+    )
+    parser_cn.add_argument(
+        "--build_server",
+        type=str,
+        required=False,
+        help="The build server for the network",
     )
     parser_cn.add_argument(
-        "--build_server", required=False, help="The build server for the network"
+        "--build_version",
+        type=str,
+        required=False,
+        help="The build version for the network",
     )
     parser_cn.add_argument(
-        "--build_version", required=False, help="The build version for the network"
+        "--genesis",
+        type=bool,
+        required=False,
+        help="Is this a genesis network?",
+        default=False,
+    )
+    parser_cn.add_argument(
+        "--quorum",
+        type=int,
+        required=False,
+        help="The quorum required for the network",
     )
     # update:node
     parser_un = subparsers.add_parser("update:node", help="Update Node Version")
-    parser_un.add_argument("--name", required=True, help="The name of the network")
+    parser_un.add_argument(
+        "--name", type=str, required=True, help="The name of the network"
+    )
     parser_un.add_argument(
         "--node_id",
+        type=str,
         required=True,
         help="The node id you want to update",
     )
     parser_un.add_argument(
         "--node_type",
+        type=str,
         required=True,
         help="The node type you want to update",
         choices=["validator", "peer"],
     )
     parser_un.add_argument(
-        "--build_server", required=False, help="The build server for the node"
+        "--build_server", type=str, required=False, help="The build server for the node"
     )
     parser_un.add_argument(
-        "--build_version", required=False, help="The build version for the node"
+        "--build_version",
+        type=str,
+        required=False,
+        help="The build version for the node",
     )
     # enable:amendment
     parser_ea = subparsers.add_parser("enable:amendment", help="Enable Amendment")
     parser_ea.add_argument("--name", required=True, help="The name of the network")
     parser_ea.add_argument(
         "--amendment_name",
         required=True,
@@ -303,45 +334,40 @@
     if args.command == "create:network":
         PROTOCOL = args.protocol
         NUM_VALIDATORS = args.num_validators
         NUM_PEERS = args.num_peers
         NETWORK_ID = args.network_id
         BUILD_SERVER = args.build_server
         BUILD_VERSION = args.build_version
+        GENESIS = args.genesis
+        QUORUM = args.quorum
 
-        public_key: str = (
-            "ED87E0EA91AAFFA130B78B75D2CC3E53202AA1BD8AB3D5E7BAC530C8440E328501"
-        )
         import_vl_key: str = (
             "ED87E0EA91AAFFA130B78B75D2CC3E53202AA1BD8AB3D5E7BAC530C8440E328501"
         )
-        private_key: str = (
-            "A232AD54A29466CDE4A3D99C651B332F89D25B5ACE3D8BD6ABD4748DA67159B2"
-        )
-        manifest: str = "JAAAAAFxIe2H4OqRqv+hMLeLddLMPlMgKqG9irPV57rFMMhEDjKFAXMh7eP2BCI6nc9g/k66bj7ksWmKuwZOKJeFx1emXip6dXxCdkB/0p6s8BzkgY7AXQxJh47pGP+vVtgcVJ44y2FK9H7xMsGOhdrbl0KUWY1Y15ZHd/R/QmvLhNC05psAX1+76YkNcBJAytrEazBhxQAEZSSLkfLwNTj3MewH1l1BjZhuIARiJNzh90dkV6AFqFW2m9VyVNLJX8EKl6yau/NET8KV2oFhAQ=="
 
         if not BUILD_SERVER:
             BUILD_SERVER: str = "https://build.xahau.tech"
 
         if not BUILD_VERSION:
             BUILD_VERSION: str = XAHAU_RELEASE
 
-        create_network_binary(
-            public_key,
+        if not QUORUM:
+            QUORUM = NUM_VALIDATORS - 1
+
+        create_network(
             import_vl_key,
-            private_key,
-            manifest,
             PROTOCOL,
             NUM_VALIDATORS,
             NUM_PEERS,
             NETWORK_ID,
             BUILD_SERVER,
             BUILD_VERSION,
-            True,
-            3,
+            GENESIS,
+            QUORUM,
         )
 
     if args.command == "update:node":
         NAME = args.name
         NODE_ID = args.node_id
         NODE_VERSION = args.node_version
         BUILD_SERVER = args.build_server
```

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/deploykit/config.json` & `xrpld_netgen-1.9.0/xrpld_netgen/deploykit/config.json`

 * *Files identical despite different names*

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/deploykit/entrypoint` & `xrpld_netgen-1.9.0/xrpld_netgen/deploykit/entrypoint`

 * *Files identical despite different names*

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/libs/github.py` & `xrpld_netgen-1.9.0/xrpld_netgen/libs/github.py`

 * *Files identical despite different names*

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/main.py` & `xrpld_netgen-1.9.0/xrpld_netgen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,14 @@
 from xrpl_helpers.rippled.utils import (
     update_amendments,
     parse_rippled_amendments,
     get_feature_lines_from_content,
     get_feature_lines_from_path,
 )
 
-
-from xrpld_publisher.publisher import PublisherClient
-from xrpld_publisher.validator import ValidatorClient
-
 basedir = os.path.abspath(os.path.dirname(__file__))
 
 
 def generate_validator_config(protocol: str, network: str):
     try:
         config = read_json(f"{basedir}/deploykit/config.json")
         return config[protocol][network]
@@ -105,14 +101,15 @@
     if vl_key:
         vl_config["validator_list_keys"] = [vl_key]
 
     if ivl_key:
         vl_config["import_vl_keys"] = [ivl_key]
 
     configs: List[RippledBuild] = gen_config(
+        protocol,
         name,
         vl_config["network_id"],
         0,
         rpc_public,
         rpc_admin,
         ws_public,
         ws_admin,
@@ -259,14 +256,15 @@
     if vl_key:
         vl_config["validator_list_keys"] = [vl_key]
 
     if ivl_key:
         vl_config["import_vl_keys"] = [ivl_key]
 
     configs: List[RippledBuild] = gen_config(
+        protocol,
         name,
         vl_config["network_id"],
         0,
         rpc_public,
         rpc_admin,
         ws_public,
         ws_admin,
@@ -417,14 +415,15 @@
     if vl_key:
         vl_config["validator_list_keys"] = [vl_key]
 
     if ivl_key:
         vl_config["import_vl_keys"] = [ivl_key]
 
     configs: List[RippledBuild] = gen_config(
+        protocol,
         name,
         vl_config["network_id"],
         0,
         rpc_public,
         rpc_admin,
         ws_public,
         ws_admin,
```

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/network.py` & `xrpld_netgen-1.9.0/xrpld_netgen/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,40 +17,35 @@
     update_dockerfile,
 )
 from xrpld_netgen.libs.github import (
     get_commit_hash_from_server_version,
     download_file_at_commit,
 )
 from xrpld_netgen.utils.misc import (
-    run_file,
+    download_json,
+    parse_image_name,
     run_command,
     generate_ports,
     save_local_config,
     get_node_port,
+    sha512_half,
 )
 
 from xrpl_helpers.common.utils import write_file, read_json
 from xrpl_helpers.rippled.utils import (
     update_amendments,
     parse_rippled_amendments,
     get_feature_lines_from_content,
-    get_feature_lines_from_path,
 )
 
 from xrpld_publisher.publisher import PublisherClient
 from xrpld_publisher.validator import ValidatorClient
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 
-RPC_PUBLIC: int = 5005
-RPC_ADMIN: int = 5015
-WS_PUBLIC: int = 6016
-WS_ADMIN: int = 6018
-PEER: int = 51235
-
 deploykit_path: str = ""
 
 
 def generate_validator_config(protocol: str, network: str):
     try:
         config = read_json(f"{basedir}/deploykit/config.json")
         return config[protocol][network]
@@ -58,27 +53,26 @@
         return None
 
 
 import requests
 import os
 import json
 
-
 services: Dict[str, Dict] = {}
 
 
 def create_node_folders(
     binary: bool,
     name: str,
     image: str,
     feature_content: str,
     num_validators: int,
     num_peers: int,
     network_id: int,
-    genesis: bool,
+    enable_all: bool,
     quorum: int,
     vl_key: str,
     ivl_key: str,
     protocol: str,
 ):
     # Create directories for validator nodes
     ips_fixed: List[str] = []
@@ -93,23 +87,23 @@
         cfg_path = f"{basedir}/{name}-cluster/{node_dir}/config"
         # GENERATE VALIDATOR KEY
         client = ValidatorClient(node_dir)
         client.create_keys()
         client.set_domain(f"xahau.{node_dir}.transia.co")
         client.create_token()
         token = client.read_token()
-        client.create_manifest()
         manifest = client.read_manifest()
         manifests.append(manifest)
         # GENERATE PORTS
         rpc_public, rpc_admin, ws_public, ws_admin, peer = generate_ports(
             i, "validator"
         )
         # GENERATE CONFIG
         configs: List[RippledBuild] = gen_config(
+            protocol,
             name,
             network_id,
             i,
             rpc_public,
             rpc_admin,
             ws_public,
             ws_admin,
@@ -125,44 +119,56 @@
             [ips for ips in ips_fixed if ips != f"{node_dir} {peer}"],
         )
 
         os.makedirs(f"{basedir}/{name}-cluster/{node_dir}", exist_ok=True)
         os.makedirs(f"{basedir}/{name}-cluster/{node_dir}/config", exist_ok=True)
         save_local_config(cfg_path, configs[0].data, configs[1].data)
 
-        lines: List[str] = get_feature_lines_from_content(feature_content)
-        features_json: Dict[str, Any] = parse_rippled_amendments(lines)
-        if genesis:
-            genesis_json: Any = update_amendments(features_json, protocol)
-            write_file(
-                f"{basedir}/{name}-cluster/{node_dir}/genesis.json",
-                json.dumps(genesis_json, indent=4, sort_keys=True),
-            )
+        # default features
+        features_json: Any = read_json(f"default.{protocol}d.features.json")
+
+        # genesis (enable all features)
+        if enable_all:
+            if protocol == "xahau":
+                lines: List[str] = get_feature_lines_from_content(feature_content)
+                features_json: Dict[str, Any] = parse_rippled_amendments(lines)
+
+            if protocol == "ripple":
+                features_json: Dict[str, Any] = download_json(
+                    feature_content, f"{basedir}/{name}-cluster"
+                )
+
+        genesis_json: Any = update_amendments(features_json, protocol)
+        write_file(
+            f"{basedir}/{name}-cluster/{node_dir}/genesis.json",
+            json.dumps(genesis_json, indent=4, sort_keys=True),
+        )
 
         write_file(
             f"{basedir}/{name}-cluster/{node_dir}/features.json",
             json.dumps(features_json, indent=4, sort_keys=True),
         )
 
-        shutil.copyfile(
-            f"{basedir}/{name}-cluster/rippled.{name}",
-            f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}",
-        )
-        os.chmod(f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}", 0o755)
+        if protocol == "xahau":
+            shutil.copyfile(
+                f"{basedir}/{name}-cluster/rippled.{name}",
+                f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}",
+            )
+            os.chmod(f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}", 0o755)
 
         dockerfile: str = create_dockerfile(
-            binary,
+            binary and protocol == "xahau",
             name,
             image,
             rpc_public,
             rpc_admin,
             ws_public,
             ws_admin,
             peer,
-            genesis,
+            True,
             quorum,
             "",
         )
         with open(f"{basedir}/{name}-cluster/{node_dir}/Dockerfile", "w") as file:
             file.write(dockerfile)
 
         shutil.copyfile(
@@ -187,30 +193,21 @@
             ],
             "volumes": [
                 f"{pwd_str}/vnode{i}/log:/var/log/rippled",
                 f"{pwd_str}/vnode{i}/lib:/var/lib/rippled",
             ],
             "networks": [f"{name}-network"],
         }
-        services[f"vnode{i}-explorer"] = {
-            "image": "transia/explorer:latest",
-            "container_name": f"vnode{i}-explorer",
-            "environment": [
-                f"PORT=410{i}",
-                f"VUE_APP_WSS_ENDPOINT=ws://0.0.0.0:{ws_admin}",
-            ],
-            "ports": [f"410{i}:410{i}"],
-            "networks": [f"{name}-network"],
-        }
 
-    for i in range(1, num_peers + 1):
+    for i in range(0, num_peers):
         node_dir = f"pnode{i}"
         cfg_path = f"{basedir}/{name}-cluster/{node_dir}/config"
         rpc_public, rpc_admin, ws_public, ws_admin, peer = generate_ports(i, "peer")
         configs: List[RippledBuild] = gen_config(
+            protocol,
             name,
             network_id,
             i,
             rpc_public,
             rpc_admin,
             ws_public,
             ws_admin,
@@ -226,44 +223,56 @@
             ips_fixed,
         )
         # print(f'CONFIG: {configs}')
         os.makedirs(f"{basedir}/{name}-cluster/{node_dir}", exist_ok=True)
         os.makedirs(f"{basedir}/{name}-cluster/{node_dir}/config", exist_ok=True)
         save_local_config(cfg_path, configs[0].data, configs[1].data)
 
-        lines: List[str] = get_feature_lines_from_content(feature_content)
-        features_json: Dict[str, Any] = parse_rippled_amendments(lines)
-        if genesis:
-            genesis_json: Any = update_amendments(features_json, protocol)
-            write_file(
-                f"{basedir}/{name}-cluster/{node_dir}/genesis.json",
-                json.dumps(genesis_json, indent=4, sort_keys=True),
-            )
+        # default features
+        features_json: Any = read_json("default.xahaud.features.json")
+
+        # genesis (enable all features)
+        if enable_all:
+            if protocol == "xahau":
+                lines: List[str] = get_feature_lines_from_content(feature_content)
+                features_json: Dict[str, Any] = parse_rippled_amendments(lines)
+
+            if protocol == "ripple":
+                features_json: Dict[str, Any] = download_json(
+                    feature_content, f"{basedir}/{name}-cluster"
+                )
+
+        genesis_json: Any = update_amendments(features_json, protocol)
+        write_file(
+            f"{basedir}/{name}-cluster/{node_dir}/genesis.json",
+            json.dumps(genesis_json, indent=4, sort_keys=True),
+        )
 
         write_file(
             f"{basedir}/{name}-cluster/{node_dir}/features.json",
             json.dumps(features_json, indent=4, sort_keys=True),
         )
 
-        shutil.copyfile(
-            f"{basedir}/{name}-cluster/rippled.{name}",
-            f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}",
-        )
-        os.chmod(f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}", 0o755)
+        if protocol == "xahau":
+            shutil.copyfile(
+                f"{basedir}/{name}-cluster/rippled.{name}",
+                f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}",
+            )
+            os.chmod(f"{basedir}/{name}-cluster/{node_dir}/rippled.{name}", 0o755)
 
         dockerfile: str = create_dockerfile(
-            binary,
+            binary and protocol == "xahau",
             name,
             image,
             rpc_public,
             rpc_admin,
             ws_public,
             ws_admin,
             peer,
-            genesis,
+            True,
             quorum,
             "",
         )
         with open(f"{basedir}/{name}-cluster/{node_dir}/Dockerfile", "w") as file:
             file.write(dockerfile)
 
         shutil.copyfile(
@@ -287,24 +296,14 @@
             ],
             "volumes": [
                 f"{pwd_str}/pnode{i}/log:/var/log/rippled",
                 f"{pwd_str}/pnode{i}/lib:/var/lib/rippled",
             ],
             "networks": [f"{name}-network"],
         }
-        services[f"pnode{i}-explorer"] = {
-            "image": "transia/explorer:latest",
-            "container_name": f"pnode{i}-explorer",
-            "environment": [
-                f"PORT=401{i}",
-                f"VUE_APP_WSS_ENDPOINT=ws://0.0.0.0:{ws_admin}",
-            ],
-            "ports": [f"401{i}:401{i}"],
-            "networks": [f"{name}-network"],
-        }
 
     return manifests
 
 
 def update_stop_sh(
     protocol: str,
     name: str,
@@ -336,65 +335,88 @@
         stop_sh_content = f"#! /bin/bash\ndocker compose -f docker-compose.yml down --remove-orphans\n"
         stop_sh_content += f"rm -r db\n"
         stop_sh_content += f"rm -r debug.log\n"
 
     return stop_sh_content
 
 
-def create_network_binary(
-    public_key: str,
+def create_network(
     import_key: str,
-    private_key: str,
-    manifest: str,
     protocol: str,
     num_validators: int,
     num_peers: int,
     network_id: int,
     build_server: str,
     build_version: str,
     genesis: bool = False,
     quorum: int = None,
 ) -> None:
-    name: str = build_version
-    os.makedirs(f"{basedir}/{name}-cluster", exist_ok=True)
-    # Usage
-    owner = "Xahau"
-    repo = "xahaud"
-    commit_hash = get_commit_hash_from_server_version(build_server, build_version)
-    content: str = download_file_at_commit(
-        owner, repo, commit_hash, "src/ripple/protocol/impl/Feature.cpp"
-    )
-    url: str = f"{build_server}/{build_version}"
-    download_binary(url, f"{basedir}/{name}-cluster/rippled.{build_version}")
-    image: str = "ubuntu:jammy"
+    if protocol == "xahau":
+        name: str = build_version
+        os.makedirs(f"{basedir}/{name}-cluster", exist_ok=True)
+        # Usage
+        owner = "Xahau"
+        repo = "xahaud"
+        commit_hash = get_commit_hash_from_server_version(build_server, build_version)
+        content: str = download_file_at_commit(
+            owner, repo, commit_hash, "src/ripple/protocol/impl/Feature.cpp"
+        )
+        url: str = f"{build_server}/{build_version}"
+        download_binary(url, f"{basedir}/{name}-cluster/rippled.{build_version}")
+        image: str = "ubuntu:jammy"
+
+    if protocol == "ripple":
+        name: str = build_version.replace(":", "-")
+        os.makedirs(f"{basedir}/{name}-cluster", exist_ok=True)
+        image_name, version = parse_image_name(build_version)
+        root_url = f"https://storage.googleapis.com/thelab-builds/"
+        content: str = (
+            root_url
+            + f"{image_name.split('-')[0]}/{image_name.split('-')[1]}/{version}/features.json"
+        )
+        image: str = f"{build_server}/{build_version}"
+
+    client = PublisherClient()
+    client.create_keys()
+    keys = client.get_keys()
     manifests: List[str] = create_node_folders(
         True,
         name,
         image,
         content,
         num_validators,
         num_peers,
         network_id,
         genesis,
         quorum,
-        public_key,
+        keys["publicKey"],
         import_key,
         protocol,
     )
 
     services["vl"] = {
         "build": {
             "context": "vl",
             "dockerfile": "Dockerfile",
         },
         "container_name": "vl",
         "ports": ["80:80"],
         "networks": [f"{name}-network"],
     }
 
+    services[f"network-explorer"] = {
+        "image": "transia/explorer-main:latest",
+        "container_name": f"network-explorer",
+        "environment": [
+            f"PORT=4000",
+        ],
+        "ports": [f"4000:4000"],
+        "networks": [f"{name}-network"],
+    }
+
     compose = {
         "version": "3.9",
         "services": services,
         "networks": {f"{name}-network": {"driver": "bridge"}},
     }
     with open(f"{basedir}/{name}-cluster/docker-compose.yml", "w") as f:
         yaml.dump(compose, f, default_flow_style=False)
@@ -406,21 +428,17 @@
 docker compose -f {basedir}/{name}-cluster/docker-compose.yml up --build --force-recreate -d
 """,
     )
     stop_sh_content: str = update_stop_sh(protocol, name, num_validators, num_peers)
     write_file(f"{basedir}/{name}-cluster/stop.sh", stop_sh_content)
 
     os.makedirs(f"{basedir}/{name}-cluster/vl", exist_ok=True)
-    client = PublisherClient(manifest)
     for manifest in manifests:
         client.add_validator(manifest)
-    print(private_key)
-    print(f"{basedir}/{name}-cluster/vl/vl.json")
-    print(os.getenv("BIN_PATH"))
-    client.sign_unl(private_key, f"{basedir}/{name}-cluster/vl/vl.json")
+    client.sign_unl(f"{basedir}/{name}-cluster/vl/vl.json")
     shutil.copyfile(
         f"{basedir}/deploykit/nginx.dockerfile",
         f"{basedir}/{name}-cluster/vl/Dockerfile",
     )
 
     os.chmod(f"{basedir}/{name}-cluster/start.sh", 0o755)
     os.chmod(f"{basedir}/{name}-cluster/stop.sh", 0o755)
@@ -451,17 +469,15 @@
 
 def enable_node_amendment(
     name: str,
     amendment_name: str,
     node_id: str,
     node_type: str,
 ) -> None:
-    node_dir: str = f"{'v' if node_type == 'validator' else 'p'}node{node_id}"
-    features: Dict[str, Any] = read_json(f"{basedir}/{name}/{node_dir}/features.json")
-    amendment_hash: str = features[amendment_name]
+    amendment_hash: str = sha512_half(amendment_name.encode("utf-8").hex())
     command: Dict[str, Any] = {
         "method": "feature",
         "params": [
             {
                 "feature": amendment_hash,
                 "vetoed": False,
             }
```

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/rippled_cfg.py` & `xrpld_netgen-1.9.0/xrpld_netgen/rippled_cfg.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,23 @@
     validator_list_sites: List[str] = [],
     validator_list_keys: List[str] = [],
     import_vl_keys: List[str] = [],
     ips_fixed_urls: List[str] = [],
     ips_urls: List[str] = [],
     amendment_majority_time: str = None,
     amendments_dict: Dict[str, str] = {},
+    max_transactions: int = 1000,
+    ledgers_in_queue: int = 200,
+    minimum_queue_size: int = 10000,
+    minimum_txn_in_ledger: int = 500,
+    target_txn_in_ledger: int = 10000,
+    normal_consensus_increase_percent: int = 50,
+    slow_consensus_decrease_percent: int = 10,
+    maximum_txn_in_ledger: int = 10000,
+    maximum_txn_per_account: int = 10000,
 ):
     try:
         node_config_path: str = build_path + "/config"
 
         cfg_out: str = ""
 
         server_cfg: str = "[server]" + "\n"
@@ -133,15 +142,15 @@
         cfg_out += f"{size_node}" + "\n"
         cfg_out += "\n"
 
         cfg_out += "[node_db]" + "\n"
         cfg_out += "type=NuDB" + "\n"
         cfg_out += f"path={nudb_path}" + "\n"
         cfg_out += "advisory_delete=0" + "\n"
-        # cfg_out += f"""online_delete={num_ledgers}""" + "\n"
+        cfg_out += f"online_delete={num_ledgers}" + "\n"
         cfg_out += "\n"
 
         fee_account_reserve: int = 5000000
         cfg_out += "[fee_account_reserve]" + "\n"
         cfg_out += f"{fee_account_reserve}" + "\n"
         cfg_out += "\n"
 
@@ -222,14 +231,35 @@
         else:
             cfg_out += '{ "command": "log_level", "severity": "info" }' + "\n"
 
         cfg_out += "\n"
         cfg_out += "[ssl_verify]" + "\n"
         cfg_out += f"{ssl_verify}" + "\n"
 
+        cfg_out += "\n"
+        cfg_out += "[max_transactions]" + "\n"
+        cfg_out += f"{max_transactions}" + "\n"
+
+        cfg_out += "\n"
+        cfg_out += "[transaction_queue]" + "\n"
+        cfg_out += f"ledgers_in_queue = {ledgers_in_queue}" + "\n"
+        cfg_out += f"minimum_queue_size = {minimum_queue_size}" + "\n"
+        cfg_out += f"minimum_txn_in_ledger = {minimum_txn_in_ledger}" + "\n"
+        cfg_out += f"target_txn_in_ledger = {target_txn_in_ledger}" + "\n"
+        cfg_out += (
+            f"normal_consensus_increase_percent = {normal_consensus_increase_percent}"
+            + "\n"
+        )
+        cfg_out += (
+            f"slow_consensus_decrease_percent = {slow_consensus_decrease_percent}"
+            + "\n"
+        )
+        cfg_out += f"maximum_txn_in_ledger = {maximum_txn_in_ledger}" + "\n"
+        cfg_out += f"maximum_txn_per_account = {maximum_txn_per_account}" + "\n"
+
         if amendment_majority_time:
             cfg_out += "\n"
             cfg_out += "[amendment_majority_time]" + "\n"
             cfg_out += amendment_majority_time + "\n"
 
         if amendments_dict and len(amendments_dict) > 0:
             cfg_out += "\n"
@@ -301,17 +331,26 @@
         print(cluster_nodes)
         print(validator_list_sites)
         print(validator_list_keys)
         print(import_vl_keys)
         print(ips_fixed_urls)
         print(ips_urls)
         print(amendments_dict)
+        print(max_transactions)
+        print(ledgers_in_queue)
+        print(minimum_txn_in_ledger)
+        print(target_txn_in_ledger)
+        print(normal_consensus_increase_percent)
+        print(slow_consensus_decrease_percent)
+        print(maximum_txn_in_ledger)
+        print(maximum_txn_per_account)
 
 
 def gen_config(
+    protocol: str,
     name: str,
     network_id: int,
     index: int,
     rpc_public: int,
     rpc_admin: int,
     ws_public: int,
     ws_admin: int,
@@ -344,26 +383,26 @@
         is_peer=True,
         peer_port=peer,
         # ssl_verify=1 if _node.ssl_verify else 0,
         ssl_verify=0,
         is_ssl=True,
         key_path=None,
         crt_path=None,
-        size_node="medium",
+        size_node="huge",
         nudb_path=nudb_path,
         db_path=db_path,
         num_ledgers=256,
         debug_path=debug_path,
         log_level="trace",
         # private_peer=1 if _node.private_peer and i == 1 else 0,
         private_peer=0,
         genesis=False,
         v_token=v_token,
         validator_list_sites=vl_sites,
         validator_list_keys=vl_keys,
         import_vl_keys=ivl_keys,
         ips_urls=ips_urls,
         ips_fixed_urls=ips_fixed_urls,
-        amendment_majority_time=None,
+        amendment_majority_time="5 minutes" if protocol == 'xahau' else '15 minutes',
         amendments_dict={},
     )
     return configs
```

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/utils/deploy_kit.py` & `xrpld_netgen-1.9.0/xrpld_netgen/utils/deploy_kit.py`

 * *Files identical despite different names*

### Comparing `xrpld_netgen-1.8.0/xrpld_netgen/utils/misc.py` & `xrpld_netgen-1.9.0/xrpld_netgen/utils/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import os
 import json
 import requests
 import shutil
 import subprocess
 import shlex
+import hashlib
 
 from xrpl_helpers.common.utils import read_json
 
 
 def remove_directory(directory_path: str):
     try:
         shutil.rmtree(directory_path)
@@ -99,18 +100,18 @@
     # Get the image name
     name = image_name.split(":")[0]
     # Get the version
     version = image_name.split(":")[1]
     return name, version
 
 
-RPC_PUBLIC: int = 5005
-RPC_ADMIN: int = 5015
-WS_PUBLIC: int = 6016
-WS_ADMIN: int = 6018
+RPC_PUBLIC: int = 5007
+RPC_ADMIN: int = 5005
+WS_PUBLIC: int = 6008
+WS_ADMIN: int = 6006
 PEER: int = 51235
 
 
 def get_node_port(index, node_type):
     if node_type == "validator":
         return RPC_ADMIN + (index * 100)
     elif node_type == "peer":
@@ -136,7 +137,15 @@
         ws_public = 6008
         ws_admin = 6006
         peer = PEER
     else:
         raise ValueError("Invalid node type. Must be 'validator' or 'peer'.")
 
     return rpc_public, rpc_admin, ws_public, ws_admin, peer
+
+
+def sha512_half(hex_string):
+    hash_obj = hashlib.sha512()
+    hash_obj.update(bytes.fromhex(hex_string))
+    full_digest = hash_obj.hexdigest().upper()
+    hash_size = len(full_digest) // 2
+    return full_digest[:hash_size]
```

### Comparing `xrpld_netgen-1.8.0/PKG-INFO` & `xrpld_netgen-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xrpld-netgen
-Version: 1.8.0
+Version: 1.9.0
 Summary: Xrpld network generator
 Author: Denis Angell
 Author-email: dangell@transia.co
 Requires-Python: >=3.9.6,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: xrpl-helpers (>=1.0.4,<2.0.0)
-Requires-Dist: xrpld-publisher (>=1.0.5,<2.0.0)
+Requires-Dist: xrpld-publisher (>=2.0.0,<3.0.0)
```

