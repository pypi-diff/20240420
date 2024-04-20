# Comparing `tmp/pulumi_proxmoxve-6.3.1.tar.gz` & `tmp/pulumi_proxmoxve-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.3.1.tar", last modified: Fri Apr 12 07:15:50 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.4.0.tar", last modified: Sat Apr 20 07:06:16 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.3.1.tar` & `pulumi_proxmoxve-6.4.0.tar`

### file list

```diff
@@ -1,94 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.234657 pulumi_proxmoxve-6.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-12 07:15:50.234657 pulumi_proxmoxve-6.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.222657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55933 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.230657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.230657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.234657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.234657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   122141 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:15:50.226657 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 07:15:50.000000 pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:15:50.234657 pulumi_proxmoxve-6.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 07:15:49.000000 pulumi_proxmoxve-6.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.330602 pulumi_proxmoxve-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-20 07:06:16.330602 pulumi_proxmoxve-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.318602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14356 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.318602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/get_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.322602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.326602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.326602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.330602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.330602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:06:16.318602 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 07:06:16.330602 pulumi_proxmoxve-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-20 07:06:16.000000 pulumi_proxmoxve-6.4.0/setup.py
```

### Comparing `pulumi_proxmoxve-6.3.1/PKG-INFO` & `pulumi_proxmoxve-6.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 6.3.1
+Version: 6.4.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.3.1/README.md` & `pulumi_proxmoxve-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Export this package's modules as members:
 from .certifi import *
 from .dns import *
 from .get_node import *
 from .hosts import *
 from .provider import *
 from .time import *
+from .vm2 import *
 from ._inputs import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumi_proxmoxve.cluster as __cluster
     cluster = __cluster
@@ -22,28 +23,31 @@
     config = __config
     import pulumi_proxmoxve.ct as __ct
     ct = __ct
     import pulumi_proxmoxve.download as __download
     download = __download
     import pulumi_proxmoxve.ha as __ha
     ha = __ha
+    import pulumi_proxmoxve.hardware as __hardware
+    hardware = __hardware
     import pulumi_proxmoxve.network as __network
     network = __network
     import pulumi_proxmoxve.permission as __permission
     permission = __permission
     import pulumi_proxmoxve.storage as __storage
     storage = __storage
     import pulumi_proxmoxve.vm as __vm
     vm = __vm
 else:
     cluster = _utilities.lazy_import('pulumi_proxmoxve.cluster')
     config = _utilities.lazy_import('pulumi_proxmoxve.config')
     ct = _utilities.lazy_import('pulumi_proxmoxve.ct')
     download = _utilities.lazy_import('pulumi_proxmoxve.download')
     ha = _utilities.lazy_import('pulumi_proxmoxve.ha')
+    hardware = _utilities.lazy_import('pulumi_proxmoxve.hardware')
     network = _utilities.lazy_import('pulumi_proxmoxve.network')
     permission = _utilities.lazy_import('pulumi_proxmoxve.permission')
     storage = _utilities.lazy_import('pulumi_proxmoxve.storage')
     vm = _utilities.lazy_import('pulumi_proxmoxve.vm')
 
 _utilities.register(
     resource_modules="""
@@ -86,14 +90,30 @@
   "fqn": "pulumi_proxmoxve.ha",
   "classes": {
    "proxmoxve:HA/hAResource:HAResource": "HAResource"
   }
  },
  {
   "pkg": "proxmoxve",
+  "mod": "Hardware/mapping/pci",
+  "fqn": "pulumi_proxmoxve.hardware.mapping",
+  "classes": {
+   "proxmoxve:Hardware/mapping/pci:Pci": "Pci"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "Hardware/mapping/usb",
+  "fqn": "pulumi_proxmoxve.hardware.mapping",
+  "classes": {
+   "proxmoxve:Hardware/mapping/usb:Usb": "Usb"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
   "mod": "Network/firewall",
   "fqn": "pulumi_proxmoxve.network",
   "classes": {
    "proxmoxve:Network/firewall:Firewall": "Firewall"
   }
  },
  {
@@ -227,14 +247,22 @@
  {
   "pkg": "proxmoxve",
   "mod": "index/time",
   "fqn": "pulumi_proxmoxve",
   "classes": {
    "proxmoxve:index/time:Time": "Time"
   }
+ },
+ {
+  "pkg": "proxmoxve",
+  "mod": "index/vm2",
+  "fqn": "pulumi_proxmoxve",
+  "classes": {
+   "proxmoxve:index/vm2:Vm2": "Vm2"
+  }
  }
 ]
 """,
     resource_packages="""
 [
  {
   "pkg": "proxmoxve",
```

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,256 +3,307 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from ... import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = [
-    'HostsEntryArgs',
-    'ProviderSshArgs',
-    'ProviderSshNodeArgs',
-]
+__all__ = ['PciArgs', 'Pci']
 
 @pulumi.input_type
-class HostsEntryArgs:
+class PciArgs:
     def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] address: The IP address.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] hostnames: The hostnames.
-        """
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "hostnames", hostnames)
+                 maps: pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]],
+                 comment: Optional[pulumi.Input[str]] = None,
+                 mediated_devices: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Pci resource.
+        :param pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]] maps: The actual map of devices for the PCI hardware mapping.
+        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
+        :param pulumi.Input[str] name: The name of this PCI hardware mapping.
+        """
+        pulumi.set(__self__, "maps", maps)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if mediated_devices is not None:
+            pulumi.set(__self__, "mediated_devices", mediated_devices)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
+    def maps(self) -> pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]:
         """
-        The IP address.
+        The actual map of devices for the PCI hardware mapping.
         """
-        return pulumi.get(self, "address")
+        return pulumi.get(self, "maps")
 
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+    @maps.setter
+    def maps(self, value: pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]):
+        pulumi.set(self, "maps", value)
 
     @property
     @pulumi.getter
-    def hostnames(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The hostnames.
+        The comment of the mapped PCI device.
         """
-        return pulumi.get(self, "hostnames")
-
-    @hostnames.setter
-    def hostnames(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "hostnames", value)
+        return pulumi.get(self, "comment")
 
-
-@pulumi.input_type
-class ProviderSshArgs:
-    def __init__(__self__, *,
-                 agent: Optional[pulumi.Input[bool]] = None,
-                 agent_socket: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 private_key: Optional[pulumi.Input[str]] = None,
-                 socks5_password: Optional[pulumi.Input[str]] = None,
-                 socks5_server: Optional[pulumi.Input[str]] = None,
-                 socks5_username: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[bool] agent: Whether to use the SSH agent for authentication. Takes precedence over the `private_key` and `password` fields. Defaults to the value of the `PROXMOX_VE_SSH_AGENT` environment variable, or `false` if not set.
-        :param pulumi.Input[str] agent_socket: The path to the SSH agent socket. Defaults to the value of the `SSH_AUTH_SOCK` environment variable.
-        :param pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]] nodes: Overrides for SSH connection configuration for a Proxmox VE node.
-        :param pulumi.Input[str] password: The password used for the SSH connection. Defaults to the value of the `password` field of the `provider` block.
-        :param pulumi.Input[str] private_key: The unencrypted private key (in PEM format) used for the SSH connection. Defaults to the value of the `PROXMOX_VE_SSH_PRIVATE_KEY` environment variable.
-        :param pulumi.Input[str] socks5_password: The password for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_PASSWORD` environment variable.
-        :param pulumi.Input[str] socks5_server: The address:port of the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_SERVER` environment variable.
-        :param pulumi.Input[str] socks5_username: The username for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_USERNAME` environment variable.
-        :param pulumi.Input[str] username: The username used for the SSH connection. Defaults to the value of the `username` field of the `provider` block.
-        """
-        if agent is not None:
-            pulumi.set(__self__, "agent", agent)
-        if agent_socket is not None:
-            pulumi.set(__self__, "agent_socket", agent_socket)
-        if nodes is not None:
-            pulumi.set(__self__, "nodes", nodes)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if private_key is not None:
-            pulumi.set(__self__, "private_key", private_key)
-        if socks5_password is not None:
-            pulumi.set(__self__, "socks5_password", socks5_password)
-        if socks5_server is not None:
-            pulumi.set(__self__, "socks5_server", socks5_server)
-        if socks5_username is not None:
-            pulumi.set(__self__, "socks5_username", socks5_username)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
-    @pulumi.getter
-    def agent(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="mediatedDevices")
+    def mediated_devices(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to use the SSH agent for authentication. Takes precedence over the `private_key` and `password` fields. Defaults to the value of the `PROXMOX_VE_SSH_AGENT` environment variable, or `false` if not set.
+        Indicates whether to enable mediated devices.
         """
-        return pulumi.get(self, "agent")
+        return pulumi.get(self, "mediated_devices")
 
-    @agent.setter
-    def agent(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "agent", value)
+    @mediated_devices.setter
+    def mediated_devices(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mediated_devices", value)
 
     @property
-    @pulumi.getter(name="agentSocket")
-    def agent_socket(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The path to the SSH agent socket. Defaults to the value of the `SSH_AUTH_SOCK` environment variable.
+        The name of this PCI hardware mapping.
         """
-        return pulumi.get(self, "agent_socket")
+        return pulumi.get(self, "name")
 
-    @agent_socket.setter
-    def agent_socket(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "agent_socket", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @property
-    @pulumi.getter
-    def nodes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]:
-        """
-        Overrides for SSH connection configuration for a Proxmox VE node.
-        """
-        return pulumi.get(self, "nodes")
 
-    @nodes.setter
-    def nodes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]):
-        pulumi.set(self, "nodes", value)
+@pulumi.input_type
+class _PciState:
+    def __init__(__self__, *,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 maps: Optional[pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]] = None,
+                 mediated_devices: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Pci resources.
+        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]] maps: The actual map of devices for the PCI hardware mapping.
+        :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
+        :param pulumi.Input[str] name: The name of this PCI hardware mapping.
+        """
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if maps is not None:
+            pulumi.set(__self__, "maps", maps)
+        if mediated_devices is not None:
+            pulumi.set(__self__, "mediated_devices", mediated_devices)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
+    def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The password used for the SSH connection. Defaults to the value of the `password` field of the `provider` block.
+        The comment of the mapped PCI device.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "comment")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
-    @pulumi.getter(name="privateKey")
-    def private_key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def maps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]]:
         """
-        The unencrypted private key (in PEM format) used for the SSH connection. Defaults to the value of the `PROXMOX_VE_SSH_PRIVATE_KEY` environment variable.
+        The actual map of devices for the PCI hardware mapping.
         """
-        return pulumi.get(self, "private_key")
+        return pulumi.get(self, "maps")
 
-    @private_key.setter
-    def private_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "private_key", value)
+    @maps.setter
+    def maps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]]):
+        pulumi.set(self, "maps", value)
 
     @property
-    @pulumi.getter(name="socks5Password")
-    def socks5_password(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="mediatedDevices")
+    def mediated_devices(self) -> Optional[pulumi.Input[bool]]:
         """
-        The password for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_PASSWORD` environment variable.
+        Indicates whether to enable mediated devices.
         """
-        return pulumi.get(self, "socks5_password")
+        return pulumi.get(self, "mediated_devices")
 
-    @socks5_password.setter
-    def socks5_password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_password", value)
+    @mediated_devices.setter
+    def mediated_devices(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mediated_devices", value)
 
     @property
-    @pulumi.getter(name="socks5Server")
-    def socks5_server(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The address:port of the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_SERVER` environment variable.
+        The name of this PCI hardware mapping.
         """
-        return pulumi.get(self, "socks5_server")
+        return pulumi.get(self, "name")
 
-    @socks5_server.setter
-    def socks5_server(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_server", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @property
-    @pulumi.getter(name="socks5Username")
-    def socks5_username(self) -> Optional[pulumi.Input[str]]:
-        """
-        The username for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_USERNAME` environment variable.
-        """
-        return pulumi.get(self, "socks5_username")
 
-    @socks5_username.setter
-    def socks5_username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_username", value)
+class Pci(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 maps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]]] = None,
+                 mediated_devices: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Manages a PCI hardware mapping in a Proxmox VE cluster.
+
+        ## Import
+
+        #!/usr/bin/env sh
+
+        A PCI hardware mapping can be imported using their name, e.g.:
+
+        ```sh
+        $ pulumi import proxmoxve:Hardware/mapping/pci:Pci example example
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]] maps: The actual map of devices for the PCI hardware mapping.
+        :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
+        :param pulumi.Input[str] name: The name of this PCI hardware mapping.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: PciArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Manages a PCI hardware mapping in a Proxmox VE cluster.
+
+        ## Import
+
+        #!/usr/bin/env sh
+
+        A PCI hardware mapping can be imported using their name, e.g.:
+
+        ```sh
+        $ pulumi import proxmoxve:Hardware/mapping/pci:Pci example example
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param PciArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(PciArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 maps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]]] = None,
+                 mediated_devices: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = PciArgs.__new__(PciArgs)
+
+            __props__.__dict__["comment"] = comment
+            if maps is None and not opts.urn:
+                raise TypeError("Missing required property 'maps'")
+            __props__.__dict__["maps"] = maps
+            __props__.__dict__["mediated_devices"] = mediated_devices
+            __props__.__dict__["name"] = name
+        super(Pci, __self__).__init__(
+            'proxmoxve:Hardware/mapping/pci:Pci',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            comment: Optional[pulumi.Input[str]] = None,
+            maps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]]] = None,
+            mediated_devices: Optional[pulumi.Input[bool]] = None,
+            name: Optional[pulumi.Input[str]] = None) -> 'Pci':
+        """
+        Get an existing Pci resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]] maps: The actual map of devices for the PCI hardware mapping.
+        :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
+        :param pulumi.Input[str] name: The name of this PCI hardware mapping.
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _PciState.__new__(_PciState)
+
+        __props__.__dict__["comment"] = comment
+        __props__.__dict__["maps"] = maps
+        __props__.__dict__["mediated_devices"] = mediated_devices
+        __props__.__dict__["name"] = name
+        return Pci(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        The username used for the SSH connection. Defaults to the value of the `username` field of the `provider` block.
+        The comment of the mapped PCI device.
         """
-        return pulumi.get(self, "username")
-
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
-
-
-@pulumi.input_type
-class ProviderSshNodeArgs:
-    def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 port: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[str] address: The address of the Proxmox VE node.
-        :param pulumi.Input[str] name: The name of the Proxmox VE node.
-        :param pulumi.Input[int] port: The port of the Proxmox VE node.
-        """
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "name", name)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
+        return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
+    def maps(self) -> pulumi.Output[Sequence['outputs.PciMap']]:
         """
-        The address of the Proxmox VE node.
+        The actual map of devices for the PCI hardware mapping.
         """
-        return pulumi.get(self, "address")
-
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+        return pulumi.get(self, "maps")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="mediatedDevices")
+    def mediated_devices(self) -> pulumi.Output[bool]:
         """
-        The name of the Proxmox VE node.
+        Indicates whether to enable mediated devices.
         """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+        return pulumi.get(self, "mediated_devices")
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
+    def name(self) -> pulumi.Output[str]:
         """
-        The port of the Proxmox VE node.
+        The name of this PCI hardware mapping.
         """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
-
+        return pulumi.get(self, "name")
```

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,19 @@
                  operating_system: Optional[pulumi.Input['ContainerOperatingSystemArgs']] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  start_on_boot: Optional[pulumi.Input[bool]] = None,
                  started: Optional[pulumi.Input[bool]] = None,
                  startup: Optional[pulumi.Input['ContainerStartupArgs']] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
+                 timeout_clone: Optional[pulumi.Input[int]] = None,
                  timeout_create: Optional[pulumi.Input[int]] = None,
+                 timeout_delete: Optional[pulumi.Input[int]] = None,
                  timeout_start: Optional[pulumi.Input[int]] = None,
+                 timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Container resource.
         :param pulumi.Input[str] node_name: The name of the node to assign the container to.
         :param pulumi.Input['ContainerCloneArgs'] clone: The cloning configuration.
         :param pulumi.Input['ContainerConsoleArgs'] console: Console.
@@ -62,16 +65,19 @@
         :param pulumi.Input['ContainerStartupArgs'] startup: Defines startup and shutdown behavior of the container.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags the container tags. This is only meta
                information (defaults to `[]`). Note: Proxmox always sorts the container tags.
                If the list in template is not sorted, then Proxmox will always report a
                difference on the resource. You may use the `ignore_changes` lifecycle
                meta-argument to ignore changes to this attribute.
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
+        :param pulumi.Input[int] timeout_clone: Timeout for cloning a container in seconds (defaults to 1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a container in seconds (defaults to 1800).
-        :param pulumi.Input[int] timeout_start: Timeout for starting a container in seconds (defaults to 300).
+        :param pulumi.Input[int] timeout_delete: Timeout for deleting a container in seconds (defaults to 60).
+        :param pulumi.Input[int] timeout_start: Start container timeout
+        :param pulumi.Input[int] timeout_update: Timeout for updating a container in seconds (defaults to 1800).
         :param pulumi.Input[bool] unprivileged: Whether the container runs as unprivileged on
                the host (defaults to `false`).
         :param pulumi.Input[int] vm_id: The container identifier
         """
         pulumi.set(__self__, "node_name", node_name)
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
@@ -105,18 +111,27 @@
             pulumi.set(__self__, "started", started)
         if startup is not None:
             pulumi.set(__self__, "startup", startup)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template is not None:
             pulumi.set(__self__, "template", template)
+        if timeout_clone is not None:
+            pulumi.set(__self__, "timeout_clone", timeout_clone)
         if timeout_create is not None:
             pulumi.set(__self__, "timeout_create", timeout_create)
+        if timeout_delete is not None:
+            pulumi.set(__self__, "timeout_delete", timeout_delete)
+        if timeout_start is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""", DeprecationWarning)
+            pulumi.log.warn("""timeout_start is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""")
         if timeout_start is not None:
             pulumi.set(__self__, "timeout_start", timeout_start)
+        if timeout_update is not None:
+            pulumi.set(__self__, "timeout_update", timeout_update)
         if unprivileged is not None:
             pulumi.set(__self__, "unprivileged", unprivileged)
         if vm_id is not None:
             pulumi.set(__self__, "vm_id", vm_id)
 
     @property
     @pulumi.getter(name="nodeName")
@@ -349,38 +364,77 @@
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "template", value)
 
     @property
+    @pulumi.getter(name="timeoutClone")
+    def timeout_clone(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for cloning a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_clone")
+
+    @timeout_clone.setter
+    def timeout_clone(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_clone", value)
+
+    @property
     @pulumi.getter(name="timeoutCreate")
     def timeout_create(self) -> Optional[pulumi.Input[int]]:
         """
         Timeout for creating a container in seconds (defaults to 1800).
         """
         return pulumi.get(self, "timeout_create")
 
     @timeout_create.setter
     def timeout_create(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_create", value)
 
     @property
+    @pulumi.getter(name="timeoutDelete")
+    def timeout_delete(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for deleting a container in seconds (defaults to 60).
+        """
+        return pulumi.get(self, "timeout_delete")
+
+    @timeout_delete.setter
+    def timeout_delete(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_delete", value)
+
+    @property
     @pulumi.getter(name="timeoutStart")
     def timeout_start(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout for starting a container in seconds (defaults to 300).
+        Start container timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_start is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""")
+
         return pulumi.get(self, "timeout_start")
 
     @timeout_start.setter
     def timeout_start(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_start", value)
 
     @property
+    @pulumi.getter(name="timeoutUpdate")
+    def timeout_update(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for updating a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_update")
+
+    @timeout_update.setter
+    def timeout_update(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_update", value)
+
+    @property
     @pulumi.getter
     def unprivileged(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether the container runs as unprivileged on
         the host (defaults to `false`).
         """
         return pulumi.get(self, "unprivileged")
@@ -420,16 +474,19 @@
                  operating_system: Optional[pulumi.Input['ContainerOperatingSystemArgs']] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  start_on_boot: Optional[pulumi.Input[bool]] = None,
                  started: Optional[pulumi.Input[bool]] = None,
                  startup: Optional[pulumi.Input['ContainerStartupArgs']] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
+                 timeout_clone: Optional[pulumi.Input[int]] = None,
                  timeout_create: Optional[pulumi.Input[int]] = None,
+                 timeout_delete: Optional[pulumi.Input[int]] = None,
                  timeout_start: Optional[pulumi.Input[int]] = None,
+                 timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Container resources.
         :param pulumi.Input['ContainerCloneArgs'] clone: The cloning configuration.
         :param pulumi.Input['ContainerConsoleArgs'] console: Console.
         :param pulumi.Input['ContainerCpuArgs'] cpu: The CPU configuration.
@@ -451,16 +508,19 @@
         :param pulumi.Input['ContainerStartupArgs'] startup: Defines startup and shutdown behavior of the container.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags the container tags. This is only meta
                information (defaults to `[]`). Note: Proxmox always sorts the container tags.
                If the list in template is not sorted, then Proxmox will always report a
                difference on the resource. You may use the `ignore_changes` lifecycle
                meta-argument to ignore changes to this attribute.
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
+        :param pulumi.Input[int] timeout_clone: Timeout for cloning a container in seconds (defaults to 1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a container in seconds (defaults to 1800).
-        :param pulumi.Input[int] timeout_start: Timeout for starting a container in seconds (defaults to 300).
+        :param pulumi.Input[int] timeout_delete: Timeout for deleting a container in seconds (defaults to 60).
+        :param pulumi.Input[int] timeout_start: Start container timeout
+        :param pulumi.Input[int] timeout_update: Timeout for updating a container in seconds (defaults to 1800).
         :param pulumi.Input[bool] unprivileged: Whether the container runs as unprivileged on
                the host (defaults to `false`).
         :param pulumi.Input[int] vm_id: The container identifier
         """
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
         if console is not None:
@@ -495,18 +555,27 @@
             pulumi.set(__self__, "started", started)
         if startup is not None:
             pulumi.set(__self__, "startup", startup)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template is not None:
             pulumi.set(__self__, "template", template)
+        if timeout_clone is not None:
+            pulumi.set(__self__, "timeout_clone", timeout_clone)
         if timeout_create is not None:
             pulumi.set(__self__, "timeout_create", timeout_create)
+        if timeout_delete is not None:
+            pulumi.set(__self__, "timeout_delete", timeout_delete)
+        if timeout_start is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""", DeprecationWarning)
+            pulumi.log.warn("""timeout_start is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""")
         if timeout_start is not None:
             pulumi.set(__self__, "timeout_start", timeout_start)
+        if timeout_update is not None:
+            pulumi.set(__self__, "timeout_update", timeout_update)
         if unprivileged is not None:
             pulumi.set(__self__, "unprivileged", unprivileged)
         if vm_id is not None:
             pulumi.set(__self__, "vm_id", vm_id)
 
     @property
     @pulumi.getter
@@ -739,38 +808,77 @@
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "template", value)
 
     @property
+    @pulumi.getter(name="timeoutClone")
+    def timeout_clone(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for cloning a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_clone")
+
+    @timeout_clone.setter
+    def timeout_clone(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_clone", value)
+
+    @property
     @pulumi.getter(name="timeoutCreate")
     def timeout_create(self) -> Optional[pulumi.Input[int]]:
         """
         Timeout for creating a container in seconds (defaults to 1800).
         """
         return pulumi.get(self, "timeout_create")
 
     @timeout_create.setter
     def timeout_create(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_create", value)
 
     @property
+    @pulumi.getter(name="timeoutDelete")
+    def timeout_delete(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for deleting a container in seconds (defaults to 60).
+        """
+        return pulumi.get(self, "timeout_delete")
+
+    @timeout_delete.setter
+    def timeout_delete(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_delete", value)
+
+    @property
     @pulumi.getter(name="timeoutStart")
     def timeout_start(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout for starting a container in seconds (defaults to 300).
+        Start container timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_start is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""")
+
         return pulumi.get(self, "timeout_start")
 
     @timeout_start.setter
     def timeout_start(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_start", value)
 
     @property
+    @pulumi.getter(name="timeoutUpdate")
+    def timeout_update(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout for updating a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_update")
+
+    @timeout_update.setter
+    def timeout_update(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout_update", value)
+
+    @property
     @pulumi.getter
     def unprivileged(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether the container runs as unprivileged on
         the host (defaults to `false`).
         """
         return pulumi.get(self, "unprivileged")
@@ -812,16 +920,19 @@
                  operating_system: Optional[pulumi.Input[pulumi.InputType['ContainerOperatingSystemArgs']]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  start_on_boot: Optional[pulumi.Input[bool]] = None,
                  started: Optional[pulumi.Input[bool]] = None,
                  startup: Optional[pulumi.Input[pulumi.InputType['ContainerStartupArgs']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
+                 timeout_clone: Optional[pulumi.Input[int]] = None,
                  timeout_create: Optional[pulumi.Input[int]] = None,
+                 timeout_delete: Optional[pulumi.Input[int]] = None,
                  timeout_start: Optional[pulumi.Input[int]] = None,
+                 timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manages a container.
 
         ## Import
@@ -857,16 +968,19 @@
         :param pulumi.Input[pulumi.InputType['ContainerStartupArgs']] startup: Defines startup and shutdown behavior of the container.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags the container tags. This is only meta
                information (defaults to `[]`). Note: Proxmox always sorts the container tags.
                If the list in template is not sorted, then Proxmox will always report a
                difference on the resource. You may use the `ignore_changes` lifecycle
                meta-argument to ignore changes to this attribute.
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
+        :param pulumi.Input[int] timeout_clone: Timeout for cloning a container in seconds (defaults to 1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a container in seconds (defaults to 1800).
-        :param pulumi.Input[int] timeout_start: Timeout for starting a container in seconds (defaults to 300).
+        :param pulumi.Input[int] timeout_delete: Timeout for deleting a container in seconds (defaults to 60).
+        :param pulumi.Input[int] timeout_start: Start container timeout
+        :param pulumi.Input[int] timeout_update: Timeout for updating a container in seconds (defaults to 1800).
         :param pulumi.Input[bool] unprivileged: Whether the container runs as unprivileged on
                the host (defaults to `false`).
         :param pulumi.Input[int] vm_id: The container identifier
         """
         ...
     @overload
     def __init__(__self__,
@@ -916,16 +1030,19 @@
                  operating_system: Optional[pulumi.Input[pulumi.InputType['ContainerOperatingSystemArgs']]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  start_on_boot: Optional[pulumi.Input[bool]] = None,
                  started: Optional[pulumi.Input[bool]] = None,
                  startup: Optional[pulumi.Input[pulumi.InputType['ContainerStartupArgs']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
+                 timeout_clone: Optional[pulumi.Input[int]] = None,
                  timeout_create: Optional[pulumi.Input[int]] = None,
+                 timeout_delete: Optional[pulumi.Input[int]] = None,
                  timeout_start: Optional[pulumi.Input[int]] = None,
+                 timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -950,16 +1067,19 @@
             __props__.__dict__["operating_system"] = operating_system
             __props__.__dict__["pool_id"] = pool_id
             __props__.__dict__["start_on_boot"] = start_on_boot
             __props__.__dict__["started"] = started
             __props__.__dict__["startup"] = startup
             __props__.__dict__["tags"] = tags
             __props__.__dict__["template"] = template
+            __props__.__dict__["timeout_clone"] = timeout_clone
             __props__.__dict__["timeout_create"] = timeout_create
+            __props__.__dict__["timeout_delete"] = timeout_delete
             __props__.__dict__["timeout_start"] = timeout_start
+            __props__.__dict__["timeout_update"] = timeout_update
             __props__.__dict__["unprivileged"] = unprivileged
             __props__.__dict__["vm_id"] = vm_id
         super(Container, __self__).__init__(
             'proxmoxve:CT/container:Container',
             resource_name,
             __props__,
             opts)
@@ -983,16 +1103,19 @@
             operating_system: Optional[pulumi.Input[pulumi.InputType['ContainerOperatingSystemArgs']]] = None,
             pool_id: Optional[pulumi.Input[str]] = None,
             start_on_boot: Optional[pulumi.Input[bool]] = None,
             started: Optional[pulumi.Input[bool]] = None,
             startup: Optional[pulumi.Input[pulumi.InputType['ContainerStartupArgs']]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             template: Optional[pulumi.Input[bool]] = None,
+            timeout_clone: Optional[pulumi.Input[int]] = None,
             timeout_create: Optional[pulumi.Input[int]] = None,
+            timeout_delete: Optional[pulumi.Input[int]] = None,
             timeout_start: Optional[pulumi.Input[int]] = None,
+            timeout_update: Optional[pulumi.Input[int]] = None,
             unprivileged: Optional[pulumi.Input[bool]] = None,
             vm_id: Optional[pulumi.Input[int]] = None) -> 'Container':
         """
         Get an existing Container resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
@@ -1019,16 +1142,19 @@
         :param pulumi.Input[pulumi.InputType['ContainerStartupArgs']] startup: Defines startup and shutdown behavior of the container.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags the container tags. This is only meta
                information (defaults to `[]`). Note: Proxmox always sorts the container tags.
                If the list in template is not sorted, then Proxmox will always report a
                difference on the resource. You may use the `ignore_changes` lifecycle
                meta-argument to ignore changes to this attribute.
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
+        :param pulumi.Input[int] timeout_clone: Timeout for cloning a container in seconds (defaults to 1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a container in seconds (defaults to 1800).
-        :param pulumi.Input[int] timeout_start: Timeout for starting a container in seconds (defaults to 300).
+        :param pulumi.Input[int] timeout_delete: Timeout for deleting a container in seconds (defaults to 60).
+        :param pulumi.Input[int] timeout_start: Start container timeout
+        :param pulumi.Input[int] timeout_update: Timeout for updating a container in seconds (defaults to 1800).
         :param pulumi.Input[bool] unprivileged: Whether the container runs as unprivileged on
                the host (defaults to `false`).
         :param pulumi.Input[int] vm_id: The container identifier
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ContainerState.__new__(_ContainerState)
@@ -1048,16 +1174,19 @@
         __props__.__dict__["operating_system"] = operating_system
         __props__.__dict__["pool_id"] = pool_id
         __props__.__dict__["start_on_boot"] = start_on_boot
         __props__.__dict__["started"] = started
         __props__.__dict__["startup"] = startup
         __props__.__dict__["tags"] = tags
         __props__.__dict__["template"] = template
+        __props__.__dict__["timeout_clone"] = timeout_clone
         __props__.__dict__["timeout_create"] = timeout_create
+        __props__.__dict__["timeout_delete"] = timeout_delete
         __props__.__dict__["timeout_start"] = timeout_start
+        __props__.__dict__["timeout_update"] = timeout_update
         __props__.__dict__["unprivileged"] = unprivileged
         __props__.__dict__["vm_id"] = vm_id
         return Container(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def clone(self) -> pulumi.Output[Optional['outputs.ContainerClone']]:
@@ -1213,30 +1342,57 @@
     def template(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to create a template (defaults to `false`).
         """
         return pulumi.get(self, "template")
 
     @property
+    @pulumi.getter(name="timeoutClone")
+    def timeout_clone(self) -> pulumi.Output[Optional[int]]:
+        """
+        Timeout for cloning a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_clone")
+
+    @property
     @pulumi.getter(name="timeoutCreate")
     def timeout_create(self) -> pulumi.Output[Optional[int]]:
         """
         Timeout for creating a container in seconds (defaults to 1800).
         """
         return pulumi.get(self, "timeout_create")
 
     @property
+    @pulumi.getter(name="timeoutDelete")
+    def timeout_delete(self) -> pulumi.Output[Optional[int]]:
+        """
+        Timeout for deleting a container in seconds (defaults to 60).
+        """
+        return pulumi.get(self, "timeout_delete")
+
+    @property
     @pulumi.getter(name="timeoutStart")
     def timeout_start(self) -> pulumi.Output[Optional[int]]:
         """
-        Timeout for starting a container in seconds (defaults to 300).
+        Start container timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_start is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (`timeout_create` / `timeout_clone`) is used instead.""")
+
         return pulumi.get(self, "timeout_start")
 
     @property
+    @pulumi.getter(name="timeoutUpdate")
+    def timeout_update(self) -> pulumi.Output[Optional[int]]:
+        """
+        Timeout for updating a container in seconds (defaults to 1800).
+        """
+        return pulumi.get(self, "timeout_update")
+
+    @property
     @pulumi.getter
     def unprivileged(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the container runs as unprivileged on
         the host (defaults to `false`).
         """
         return pulumi.get(self, "unprivileged")
```

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
         :param pulumi.Input[int] timeout_clone: Timeout for cloning a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_migrate: Timeout for migrating the VM (defaults to
                1800).
-        :param pulumi.Input[int] timeout_move_disk: Timeout for moving the disk of a VM in
-               seconds (defaults to 1800).
+        :param pulumi.Input[int] timeout_move_disk: MoveDisk timeout
         :param pulumi.Input[int] timeout_reboot: Timeout for rebooting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_shutdown_vm: Timeout for shutting down a VM in seconds (
                defaults to 1800).
         :param pulumi.Input[int] timeout_start_vm: Timeout for starting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_stop_vm: Timeout for stopping a VM in seconds (defaults
@@ -218,14 +217,17 @@
         if timeout_clone is not None:
             pulumi.set(__self__, "timeout_clone", timeout_clone)
         if timeout_create is not None:
             pulumi.set(__self__, "timeout_create", timeout_create)
         if timeout_migrate is not None:
             pulumi.set(__self__, "timeout_migrate", timeout_migrate)
         if timeout_move_disk is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""", DeprecationWarning)
+            pulumi.log.warn("""timeout_move_disk is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""")
+        if timeout_move_disk is not None:
             pulumi.set(__self__, "timeout_move_disk", timeout_move_disk)
         if timeout_reboot is not None:
             pulumi.set(__self__, "timeout_reboot", timeout_reboot)
         if timeout_shutdown_vm is not None:
             pulumi.set(__self__, "timeout_shutdown_vm", timeout_shutdown_vm)
         if timeout_start_vm is not None:
             pulumi.set(__self__, "timeout_start_vm", timeout_start_vm)
@@ -748,17 +750,19 @@
     def timeout_migrate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_migrate", value)
 
     @property
     @pulumi.getter(name="timeoutMoveDisk")
     def timeout_move_disk(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout for moving the disk of a VM in
-        seconds (defaults to 1800).
+        MoveDisk timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_move_disk is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""")
+
         return pulumi.get(self, "timeout_move_disk")
 
     @timeout_move_disk.setter
     def timeout_move_disk(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_move_disk", value)
 
     @property
@@ -979,16 +983,15 @@
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
         :param pulumi.Input[int] timeout_clone: Timeout for cloning a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_migrate: Timeout for migrating the VM (defaults to
                1800).
-        :param pulumi.Input[int] timeout_move_disk: Timeout for moving the disk of a VM in
-               seconds (defaults to 1800).
+        :param pulumi.Input[int] timeout_move_disk: MoveDisk timeout
         :param pulumi.Input[int] timeout_reboot: Timeout for rebooting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_shutdown_vm: Timeout for shutting down a VM in seconds (
                defaults to 1800).
         :param pulumi.Input[int] timeout_start_vm: Timeout for starting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_stop_vm: Timeout for stopping a VM in seconds (defaults
@@ -1083,14 +1086,17 @@
         if timeout_clone is not None:
             pulumi.set(__self__, "timeout_clone", timeout_clone)
         if timeout_create is not None:
             pulumi.set(__self__, "timeout_create", timeout_create)
         if timeout_migrate is not None:
             pulumi.set(__self__, "timeout_migrate", timeout_migrate)
         if timeout_move_disk is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""", DeprecationWarning)
+            pulumi.log.warn("""timeout_move_disk is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""")
+        if timeout_move_disk is not None:
             pulumi.set(__self__, "timeout_move_disk", timeout_move_disk)
         if timeout_reboot is not None:
             pulumi.set(__self__, "timeout_reboot", timeout_reboot)
         if timeout_shutdown_vm is not None:
             pulumi.set(__self__, "timeout_shutdown_vm", timeout_shutdown_vm)
         if timeout_start_vm is not None:
             pulumi.set(__self__, "timeout_start_vm", timeout_start_vm)
@@ -1652,17 +1658,19 @@
     def timeout_migrate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_migrate", value)
 
     @property
     @pulumi.getter(name="timeoutMoveDisk")
     def timeout_move_disk(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout for moving the disk of a VM in
-        seconds (defaults to 1800).
+        MoveDisk timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_move_disk is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""")
+
         return pulumi.get(self, "timeout_move_disk")
 
     @timeout_move_disk.setter
     def timeout_move_disk(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_move_disk", value)
 
     @property
@@ -1892,16 +1900,15 @@
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
         :param pulumi.Input[int] timeout_clone: Timeout for cloning a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_migrate: Timeout for migrating the VM (defaults to
                1800).
-        :param pulumi.Input[int] timeout_move_disk: Timeout for moving the disk of a VM in
-               seconds (defaults to 1800).
+        :param pulumi.Input[int] timeout_move_disk: MoveDisk timeout
         :param pulumi.Input[int] timeout_reboot: Timeout for rebooting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_shutdown_vm: Timeout for shutting down a VM in seconds (
                defaults to 1800).
         :param pulumi.Input[int] timeout_start_vm: Timeout for starting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_stop_vm: Timeout for stopping a VM in seconds (defaults
@@ -2190,16 +2197,15 @@
         :param pulumi.Input[bool] template: Whether to create a template (defaults to `false`).
         :param pulumi.Input[int] timeout_clone: Timeout for cloning a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_create: Timeout for creating a VM in seconds (defaults to
                1800).
         :param pulumi.Input[int] timeout_migrate: Timeout for migrating the VM (defaults to
                1800).
-        :param pulumi.Input[int] timeout_move_disk: Timeout for moving the disk of a VM in
-               seconds (defaults to 1800).
+        :param pulumi.Input[int] timeout_move_disk: MoveDisk timeout
         :param pulumi.Input[int] timeout_reboot: Timeout for rebooting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_shutdown_vm: Timeout for shutting down a VM in seconds (
                defaults to 1800).
         :param pulumi.Input[int] timeout_start_vm: Timeout for starting a VM in seconds (defaults
                to 1800).
         :param pulumi.Input[int] timeout_stop_vm: Timeout for stopping a VM in seconds (defaults
@@ -2639,17 +2645,19 @@
         """
         return pulumi.get(self, "timeout_migrate")
 
     @property
     @pulumi.getter(name="timeoutMoveDisk")
     def timeout_move_disk(self) -> pulumi.Output[Optional[int]]:
         """
-        Timeout for moving the disk of a VM in
-        seconds (defaults to 1800).
+        MoveDisk timeout
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""", DeprecationWarning)
+        pulumi.log.warn("""timeout_move_disk is deprecated: This field is deprecated and will be removed in a future release. An overall operation timeout (timeout_create / timeout_clone / timeout_migrate) is used instead.""")
+
         return pulumi.get(self, "timeout_move_disk")
 
     @property
     @pulumi.getter(name="timeoutReboot")
     def timeout_reboot(self) -> pulumi.Output[Optional[int]]:
         """
         Timeout for rebooting a VM in seconds (defaults
```

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 6.3.1
+Version: 6.4.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.3.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.4.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pulumi_proxmoxve/get_node.py
 pulumi_proxmoxve/hosts.py
 pulumi_proxmoxve/outputs.py
 pulumi_proxmoxve/provider.py
 pulumi_proxmoxve/pulumi-plugin.json
 pulumi_proxmoxve/py.typed
 pulumi_proxmoxve/time.py
+pulumi_proxmoxve/vm2.py
 pulumi_proxmoxve.egg-info/PKG-INFO
 pulumi_proxmoxve.egg-info/SOURCES.txt
 pulumi_proxmoxve.egg-info/dependency_links.txt
 pulumi_proxmoxve.egg-info/not-zip-safe
 pulumi_proxmoxve.egg-info/requires.txt
 pulumi_proxmoxve.egg-info/top_level.txt
 pulumi_proxmoxve/cluster/__init__.py
@@ -33,14 +34,24 @@
 pulumi_proxmoxve/ha/__init__.py
 pulumi_proxmoxve/ha/get_ha_group.py
 pulumi_proxmoxve/ha/get_ha_groups.py
 pulumi_proxmoxve/ha/get_ha_resource.py
 pulumi_proxmoxve/ha/get_ha_resources.py
 pulumi_proxmoxve/ha/ha_group.py
 pulumi_proxmoxve/ha/ha_resource.py
+pulumi_proxmoxve/hardware/__init__.py
+pulumi_proxmoxve/hardware/get_mappings.py
+pulumi_proxmoxve/hardware/outputs.py
+pulumi_proxmoxve/hardware/mapping/__init__.py
+pulumi_proxmoxve/hardware/mapping/_inputs.py
+pulumi_proxmoxve/hardware/mapping/get_pci.py
+pulumi_proxmoxve/hardware/mapping/get_usb.py
+pulumi_proxmoxve/hardware/mapping/outputs.py
+pulumi_proxmoxve/hardware/mapping/pci.py
+pulumi_proxmoxve/hardware/mapping/usb.py
 pulumi_proxmoxve/network/__init__.py
 pulumi_proxmoxve/network/_inputs.py
 pulumi_proxmoxve/network/firewall.py
 pulumi_proxmoxve/network/firewall_alias.py
 pulumi_proxmoxve/network/firewall_ip_set.py
 pulumi_proxmoxve/network/firewall_options.py
 pulumi_proxmoxve/network/firewall_rules.py
```

### Comparing `pulumi_proxmoxve-6.3.1/setup.py` & `pulumi_proxmoxve-6.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.3.1"
+VERSION = "6.4.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

