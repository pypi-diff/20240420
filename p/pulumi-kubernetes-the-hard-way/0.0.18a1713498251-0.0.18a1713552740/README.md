# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713498251.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713552740.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713498251.tar", last modified: Fri Apr 19 03:48:12 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713552740.tar", last modified: Fri Apr 19 18:54:56 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251.tar` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.722100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 03:48:12.722100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.706100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4080 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.710100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.714100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      940 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    15965 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15536 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)     9915 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.718100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3157 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     3101 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.718100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      545 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3142 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22577 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    97822 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15129 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    24623 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    30857 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:12.722100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 03:48:12.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-19 03:48:12.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:48:12.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 03:48:12.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 03:48:12.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-04-19 03:48:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:48:12.722100 pulumi_kubernetes_the_hard_way-0.0.18a1713498251/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.668998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 18:54:56.668998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.656998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4080 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.660998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.664998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8426 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.664998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.668998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      545 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    22577 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    97822 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    14986 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    24623 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14032 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    16572 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    25981 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    16828 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    30857 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    13649 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    19232 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    17062 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    19599 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:54:56.668998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 18:54:56.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-19 18:54:56.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:54:56.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 18:54:56.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 18:54:56.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-04-19 18:54:47.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:54:56.668998 pulumi_kubernetes_the_hard_way-0.0.18a1713552740/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713498251
+Version: 0.0.18a1713552740
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/README.md` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,33 +19,37 @@
 @pulumi.input_type
 class SystemdServiceArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  service: pulumi.Input['SystemdServiceSectionArgs'],
                  directory: Optional[pulumi.Input[str]] = None,
                  install: Optional[pulumi.Input['SystemdInstallSectionArgs']] = None,
-                 unit: Optional[pulumi.Input['SystemdUnitSectionArgs']] = None):
+                 unit: Optional[pulumi.Input['SystemdUnitSectionArgs']] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SystemdService resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input['SystemdServiceSectionArgs'] service: Describes the [Service] section of a systemd service file.
         :param pulumi.Input[str] directory: The location to create the service file.
         :param pulumi.Input['SystemdInstallSectionArgs'] install: Describes the [Install] section of a systemd service file.
         :param pulumi.Input['SystemdUnitSectionArgs'] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
         pulumi.set(__self__, "connection", connection)
         pulumi.set(__self__, "service", service)
         if directory is None:
             directory = '/etc/systemd/system'
         if directory is not None:
             pulumi.set(__self__, "directory", directory)
         if install is not None:
             pulumi.set(__self__, "install", install)
         if unit is not None:
             pulumi.set(__self__, "unit", unit)
+        if unit_name is not None:
+            pulumi.set(__self__, "unit_name", unit_name)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
@@ -99,36 +103,50 @@
         """
         return pulumi.get(self, "unit")
 
     @unit.setter
     def unit(self, value: Optional[pulumi.Input['SystemdUnitSectionArgs']]):
         pulumi.set(self, "unit", value)
 
+    @property
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the systemd unit.
+        """
+        return pulumi.get(self, "unit_name")
+
+    @unit_name.setter
+    def unit_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "unit_name", value)
+
 
 class SystemdService(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
                  install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
                  service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
                  unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A systemd service on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input[str] directory: The location to create the service file.
         :param pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']] install: Describes the [Install] section of a systemd service file.
         :param pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']] service: Describes the [Service] section of a systemd service file.
         :param pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SystemdServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -151,14 +169,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
                  install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
                  service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
                  unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -173,14 +192,15 @@
                 directory = '/etc/systemd/system'
             __props__.__dict__["directory"] = directory
             __props__.__dict__["install"] = install
             if service is None and not opts.urn:
                 raise TypeError("Missing required property 'service'")
             __props__.__dict__["service"] = service
             __props__.__dict__["unit"] = unit
+            __props__.__dict__["unit_name"] = unit_name
             __props__.__dict__["file"] = None
         super(SystemdService, __self__).__init__(
             'kubernetes-the-hard-way:remote:SystemdService',
             resource_name,
             __props__,
             opts,
             remote=True)
@@ -229,7 +249,15 @@
     @pulumi.getter
     def unit(self) -> pulumi.Output[Optional['outputs.SystemdUnitSection']]:
         """
         Describes the [Unit] section of a systemd service file.
         """
         return pulumi.get(self, "unit")
 
+    @property
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> pulumi.Output[Optional[str]]:
+        """
+        Name of the systemd unit.
+        """
+        return pulumi.get(self, "unit_name")
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,44 +67,42 @@
     def key_pem(self, value: pulumi.Input[str]):
         pulumi.set(self, "key_pem", value)
 
 
 @pulumi.input_type
 class ClusterPkiNodeArgs:
     def __init__(__self__, *,
-                 ip: Optional[pulumi.Input[str]] = None,
-                 role: Optional[pulumi.Input['NodeRole']] = None):
+                 ip: pulumi.Input[str],
+                 role: pulumi.Input['NodeRole']):
         """
         TODO
         :param pulumi.Input[str] ip: The IP address of the node
         :param pulumi.Input['NodeRole'] role: The role a node should be configured for
         """
-        if ip is not None:
-            pulumi.set(__self__, "ip", ip)
-        if role is not None:
-            pulumi.set(__self__, "role", role)
+        pulumi.set(__self__, "ip", ip)
+        pulumi.set(__self__, "role", role)
 
     @property
     @pulumi.getter
-    def ip(self) -> Optional[pulumi.Input[str]]:
+    def ip(self) -> pulumi.Input[str]:
         """
         The IP address of the node
         """
         return pulumi.get(self, "ip")
 
     @ip.setter
-    def ip(self, value: Optional[pulumi.Input[str]]):
+    def ip(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip", value)
 
     @property
     @pulumi.getter
-    def role(self) -> Optional[pulumi.Input['NodeRole']]:
+    def role(self) -> pulumi.Input['NodeRole']:
         """
         The role a node should be configured for
         """
         return pulumi.get(self, "role")
 
     @role.setter
-    def role(self, value: Optional[pulumi.Input['NodeRole']]):
+    def role(self, value: pulumi.Input['NodeRole']):
         pulumi.set(self, "role", value)
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,36 +82,34 @@
 
 @pulumi.output_type
 class ClusterPkiNode(dict):
     """
     TODO
     """
     def __init__(__self__, *,
-                 ip: Optional[str] = None,
-                 role: Optional['NodeRole'] = None):
+                 ip: str,
+                 role: 'NodeRole'):
         """
         TODO
         :param str ip: The IP address of the node
         :param 'NodeRole' role: The role a node should be configured for
         """
-        if ip is not None:
-            pulumi.set(__self__, "ip", ip)
-        if role is not None:
-            pulumi.set(__self__, "role", role)
+        pulumi.set(__self__, "ip", ip)
+        pulumi.set(__self__, "role", role)
 
     @property
     @pulumi.getter
-    def ip(self) -> Optional[str]:
+    def ip(self) -> str:
         """
         The IP address of the node
         """
         return pulumi.get(self, "ip")
 
     @property
     @pulumi.getter
-    def role(self) -> Optional['NodeRole']:
+    def role(self) -> 'NodeRole':
         """
         The role a node should be configured for
         """
         return pulumi.get(self, "role")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     POLICY = "policy"
     ALWAYS = "always"
 
 
 class EtcdctlCommand(str, Enum):
     MEMBER = "member"
     LIST = "list"
+    VERSION = "version"
 
 
 class HostnamectlCommand(str, Enum):
     STATUS = "status"
     """
     Show system hostname and related information. If no command is specified, this is the implied default.
     """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,81 +12,61 @@
 import pulumi_command
 
 __all__ = ['EtcdctlArgs', 'Etcdctl']
 
 @pulumi.input_type
 class EtcdctlArgs:
     def __init__(__self__, *,
-                 ca_cert: pulumi.Input[str],
-                 cert: pulumi.Input[str],
                  commands: pulumi.Input['EtcdctlCommand'],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 endpoints: pulumi.Input[str],
-                 key: pulumi.Input[str],
                  binary_path: Optional[pulumi.Input[str]] = None,
+                 ca_cert: Optional[pulumi.Input[str]] = None,
+                 cert: Optional[pulumi.Input[str]] = None,
+                 endpoints: Optional[pulumi.Input[str]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
                  lifecycle: Optional['CommandLifecycle'] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
         """
         The set of arguments for constructing a Etcdctl resource.
-        :param pulumi.Input[str] ca_cert: TODO
-        :param pulumi.Input[str] cert: TODO
         :param pulumi.Input['EtcdctlCommand'] commands: TODO
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[str] endpoints: TODO
-        :param pulumi.Input[str] key: TODO
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param pulumi.Input[str] ca_cert: TODO
+        :param pulumi.Input[str] cert: TODO
+        :param pulumi.Input[str] endpoints: TODO
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
+        :param pulumi.Input[str] key: TODO
         :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
         """
-        pulumi.set(__self__, "ca_cert", ca_cert)
-        pulumi.set(__self__, "cert", cert)
         pulumi.set(__self__, "commands", commands)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "endpoints", endpoints)
-        pulumi.set(__self__, "key", key)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
+        if ca_cert is not None:
+            pulumi.set(__self__, "ca_cert", ca_cert)
+        if cert is not None:
+            pulumi.set(__self__, "cert", cert)
+        if endpoints is not None:
+            pulumi.set(__self__, "endpoints", endpoints)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
         if lifecycle is not None:
             pulumi.set(__self__, "lifecycle", lifecycle)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
 
     @property
-    @pulumi.getter(name="caCert")
-    def ca_cert(self) -> pulumi.Input[str]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "ca_cert")
-
-    @ca_cert.setter
-    def ca_cert(self, value: pulumi.Input[str]):
-        pulumi.set(self, "ca_cert", value)
-
-    @property
-    @pulumi.getter
-    def cert(self) -> pulumi.Input[str]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "cert")
-
-    @cert.setter
-    def cert(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cert", value)
-
-    @property
     @pulumi.getter
     def commands(self) -> pulumi.Input['EtcdctlCommand']:
         """
         TODO
         """
         return pulumi.get(self, "commands")
 
@@ -103,48 +83,60 @@
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def endpoints(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="binaryPath")
+    def binary_path(self) -> Optional[pulumi.Input[str]]:
+        """
+        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        """
+        return pulumi.get(self, "binary_path")
+
+    @binary_path.setter
+    def binary_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "binary_path", value)
+
+    @property
+    @pulumi.getter(name="caCert")
+    def ca_cert(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
-        return pulumi.get(self, "endpoints")
+        return pulumi.get(self, "ca_cert")
 
-    @endpoints.setter
-    def endpoints(self, value: pulumi.Input[str]):
-        pulumi.set(self, "endpoints", value)
+    @ca_cert.setter
+    def ca_cert(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ca_cert", value)
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
+    def cert(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "cert")
 
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
+    @cert.setter
+    def cert(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cert", value)
 
     @property
-    @pulumi.getter(name="binaryPath")
-    def binary_path(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def endpoints(self) -> Optional[pulumi.Input[str]]:
         """
-        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        TODO
         """
-        return pulumi.get(self, "binary_path")
+        return pulumi.get(self, "endpoints")
 
-    @binary_path.setter
-    def binary_path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "binary_path", value)
+    @endpoints.setter
+    def endpoints(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "endpoints", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
         """
@@ -152,14 +144,26 @@
 
     @environment.setter
     def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
+    def key(self) -> Optional[pulumi.Input[str]]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
     def lifecycle(self) -> Optional['CommandLifecycle']:
         """
         At what stage(s) in the resource lifecycle should the command be run
         """
         return pulumi.get(self, "lifecycle")
 
     @lifecycle.setter
@@ -268,32 +272,24 @@
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EtcdctlArgs.__new__(EtcdctlArgs)
 
             __props__.__dict__["binary_path"] = binary_path
-            if ca_cert is None and not opts.urn:
-                raise TypeError("Missing required property 'ca_cert'")
             __props__.__dict__["ca_cert"] = ca_cert
-            if cert is None and not opts.urn:
-                raise TypeError("Missing required property 'cert'")
             __props__.__dict__["cert"] = cert
             if commands is None and not opts.urn:
                 raise TypeError("Missing required property 'commands'")
             __props__.__dict__["commands"] = commands
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if endpoints is None and not opts.urn:
-                raise TypeError("Missing required property 'endpoints'")
             __props__.__dict__["endpoints"] = endpoints
             __props__.__dict__["environment"] = environment
-            if key is None and not opts.urn:
-                raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["lifecycle"] = lifecycle
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
@@ -310,23 +306,23 @@
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @property
     @pulumi.getter(name="caCert")
-    def ca_cert(self) -> pulumi.Output[str]:
+    def ca_cert(self) -> pulumi.Output[Optional[str]]:
         """
         TODO
         """
         return pulumi.get(self, "ca_cert")
 
     @property
     @pulumi.getter
-    def cert(self) -> pulumi.Output[str]:
+    def cert(self) -> pulumi.Output[Optional[str]]:
         """
         TODO
         """
         return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter
@@ -350,15 +346,15 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def endpoints(self) -> pulumi.Output[str]:
+    def endpoints(self) -> pulumi.Output[Optional[str]]:
         """
         TODO
         """
         return pulumi.get(self, "endpoints")
 
     @property
     @pulumi.getter
@@ -366,15 +362,15 @@
         """
         Environment variables
         """
         return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Output[str]:
+    def key(self) -> pulumi.Output[Optional[str]]:
         """
         TODO
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713498251
+Version: 0.0.18a1713552740
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713498251/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.18a1713552740/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.18a1713498251"
+  version = "0.0.18a1713552740"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

