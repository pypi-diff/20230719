# Comparing `tmp/kubemarine-0.18.2.tar.gz` & `tmp/kubemarine-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.18.2.tar", last modified: Fri Jun 23 09:56:57 2023, max compression
+gzip compressed data, was "kubemarine-0.19.0.tar", last modified: Mon Jul 17 12:16:54 2023, max compression
```

## Comparing `kubemarine-0.18.2.tar` & `kubemarine-0.19.0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-23 09:56:43.000000 kubemarine-0.18.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-23 09:56:43.000000 kubemarine-0.18.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-23 09:56:57.685644 kubemarine-0.18.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-23 09:56:43.000000 kubemarine-0.18.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-23 09:56:43.000000 kubemarine-0.18.2/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-23 09:56:43.000000 kubemarine-0.18.2/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    45051 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    16778 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7067 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2918 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    20072 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10967 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11269 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    65136 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5780 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    29985 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    41155 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    20211 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    19510 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    14048 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3826 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5333 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     4067 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     6255 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3177 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    25005 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4198 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2775 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26444 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11284 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    17436 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9113 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-23 09:56:43.000000 kubemarine-0.18.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 09:56:57.685644 kubemarine-0.18.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.937780 kubemarine-0.19.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-17 12:16:40.000000 kubemarine-0.19.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-17 12:16:40.000000 kubemarine-0.19.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12511 2023-07-17 12:16:54.937780 kubemarine-0.19.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9063 2023-07-17 12:16:40.000000 kubemarine-0.19.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.913779 kubemarine-0.19.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-07-17 12:16:40.000000 kubemarine-0.19.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-17 12:16:40.000000 kubemarine-0.19.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.913779 kubemarine-0.19.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7885 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    45787 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     5069 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15384 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23767 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    19237 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    36274 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    14620 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15820 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    21435 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6620 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3892 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    22272 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    11022 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3609 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    64809 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5850 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    31794 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    41882 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14948 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5769 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    20607 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20764 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2825 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50099 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    72373 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5247 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26685 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1830 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1728 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    13901 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    19949 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2476 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6032 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    13897 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    11748 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    25036 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    10664 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.909779 kubemarine-0.19.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    27551 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11474 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    17633 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12511 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5480 2023-07-17 12:16:40.000000 kubemarine-0.19.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 12:16:54.937780 kubemarine-0.19.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/setup.py
```

### Comparing `kubemarine-0.18.2/LICENSE` & `kubemarine-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/PKG-INFO` & `kubemarine-0.19.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.2
+Version: 0.19.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -20,49 +20,50 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ansible
+Provides-Extra: mypy
 License-File: LICENSE
 
 ![Kubemarine_1280х640_3_JPEG](https://user-images.githubusercontent.com/5212888/162978291-63d55f19-7dc0-4126-ad39-cd69191e7e19.jpg)
 [![GitHub stars](https://img.shields.io/github/v/release/Netcracker/Kubemarine)](https://github.com/Netcracker/KubeMarine/releases)
 [![GitHub stars](https://img.shields.io/badge/contributions-welcome-orange.svg)](https://github.com/Netcracker/KubeMarine/blob/main/CONTRIBUTING.md)
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +81,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +100,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,27 +129,28 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.2/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.19.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
+     password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
 
    nodes:
      - name: "k8s-control-plane-1"
@@ -173,42 +175,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.2/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.19.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.2/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.19.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.2/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.19.0/LICENSE)
```

### Comparing `kubemarine-0.18.2/README.md` & `kubemarine-0.19.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
 1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](documentation/Installation.md#prerequisites-for-cluster-nodes).
 1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](documentation/Installation.md#configuration) and [examples](examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
+     password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
 
    nodes:
      - name: "k8s-control-plane-1"
```

### Comparing `kubemarine-0.18.2/bin/kubemarine` & `kubemarine-0.19.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/bin/kubemarine.cmd` & `kubemarine-0.19.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/__init__.py` & `kubemarine-0.19.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/__main__.py` & `kubemarine-0.19.0/kubemarine/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import sys
 from collections import OrderedDict
+from typing import Dict, List
+
 import ruamel.yaml.resolver
 import yaml
 
 # Don't remove this line. The idna encoding
 # is used by getaddrinfo when dealing with unicode hostnames,
 # and in some cases, there appears to be a race condition
 # where threads will get a LookupError on getaddrinfo() saying
 # that the encoding doesn't exist.  Using the idna encoding before
 # running any kubemarine code (and any threads it may create) ensures that
 # the encodings.idna is imported and registered in the codecs registry,
 # which will stop the LookupErrors from happening.
 # See: https://bugs.python.org/issue29288
 u''.encode('idna')
 
-# This redirect required for fixing Fabric2 problem:
-# In Kubemarine stdout messages writes only to stdout - no stderr messaging at all,
-# but Fabric2 writes to stderr if hide=false used and remote console has stderr messages.
-sys.stderr = sys.stdout
-
-
 # Take pattern to resolve float used by ruamel instead of that is used by pyyaml.
 # https://sourceforge.net/p/ruamel-yaml/code/ci/0.17.21/tree/resolver.py#l43
 # Initially introduced for keepalived that generates random password string.
 # The generated string might be also a valid exponential float, and should be dumped with quotes.
 # See also:
 # https://stackoverflow.com/questions/30458977/yaml-loads-5e-6-as-string-and-not-a-number
 # https://github.com/yaml/pyyaml/issues/173
@@ -134,20 +130,19 @@
         elif arguments[0] == 'version':
             return version()
 
     if len(arguments) < 1 or arguments[0] not in procedures.keys():
         descriptions_print_list = []
         max_module_name_size = len(max(procedures.keys(), key=len))
 
-        items_description_by_groups = {}
+        items_description_by_groups: Dict[str, List[str]] = {}
 
         for module_name, module in procedures.items():
-            if items_description_by_groups.get(module['group']) is None:
-                items_description_by_groups[module['group']] = []
-            items_description_by_groups[module['group']].append('  %s%s  %s' % (module_name, ' ' * (max_module_name_size - len(module_name)), module['description']))
+            items_description_by_groups.setdefault(module['group'], [])\
+                .append('  %s%s  %s' % (module_name, ' ' * (max_module_name_size - len(module_name)), module['description']))
 
         previous_group = None
         for group, descriptions in items_description_by_groups.items():
             if group != previous_group:
                 descriptions_print_list.append('\n%s:' % group.upper())
                 previous_group = group
             for description in descriptions:
@@ -221,17 +216,18 @@
 
     print('\nValidating patch duplicates ...')
 
     module = import_procedure('migrate_kubemarine')
     patches = module.load_patches()
     patch_ids = [patch.identifier for patch in patches]
     unique = set()
-    duplicates = [p_id for p_id in patch_ids if p_id in unique or unique.add(p_id)]
-    if duplicates:
-        raise Exception(f'Patches identifiers {duplicates} are duplicated ')
+    for p_id in patch_ids:
+        if p_id in unique:
+            raise Exception(f'Patches identifier {p_id!r} is duplicated')
+        unique.add(p_id)
 
     print("Finished")
 
     time_end = int(round(time.time() * 1000))
     print("\nElapsed: %sms\n" % (time_end-time_start))
```

### Comparing `kubemarine-0.18.2/kubemarine/admission.py` & `kubemarine-0.19.0/kubemarine/admission.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 import uuid
 import re
+from typing import Dict, Any, List
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 
 from kubemarine import kubernetes
 from kubemarine.core import utils
@@ -48,15 +49,15 @@
 privileged_plugins = {"nginx-ingress-controller": "ingress-nginx", 
                       "local-path-provisioner": "local-path-storage"}
 
 loaded_oob_policies = {}
 
 # TODO: When KubeMarine is not support Kubernetes version lower than 1.25, the PSP implementation code should be deleted 
 
-def enrich_inventory_psp(inventory, _):
+def enrich_inventory_psp(inventory: dict, _):
     global loaded_oob_policies
     loaded_oob_policies = load_oob_policies_files()
 
     # validate custom
     custom_policies = inventory["rbac"]["psp"]["custom-policies"]
     verify_custom(custom_policies)
 
@@ -69,15 +70,15 @@
     if 'PodSecurityPolicy' not in enabled_admissions:
         enabled_admissions = "%s,PodSecurityPolicy" % enabled_admissions
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["enable-admission-plugins"] = enabled_admissions
         
     return inventory
 
 
-def enrich_inventory_pss(inventory, _):
+def enrich_inventory_pss(inventory: dict, _):
     if not is_security_enabled(inventory):
         return inventory
     # check flags, enforce and logs parameters
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if minor_version < 23:
         raise Exception("PSS is not supported properly in Kubernetes version before v1.23")
     for item in inventory["rbac"]["pss"]["defaults"]:
@@ -93,23 +94,23 @@
     else:     
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["feature-gates"] = "PodSecurity=true"
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["admission-control-config-file"] = admission_path
 
     return inventory
 
 
-def enrich_inventory(inventory, _):
+def enrich_inventory(inventory: dict, _):
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return enrich_inventory_psp(inventory, _)
     elif admission_impl == "pss":
         return enrich_inventory_pss(inventory, _)
 
 
-def manage_psp_enrichment(inventory, cluster):
+def manage_psp_enrichment(inventory: dict, cluster: KubernetesCluster):
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if minor_version >= 25:
         raise Exception("PSP is not supported in Kubernetes version higher than v1.24")
     if cluster.context.get('initial_procedure') != 'manage_psp':
         return inventory
 
     procedure_config = cluster.procedure_inventory["psp"]
@@ -160,15 +161,15 @@
         if result is None:
             raise Exception("incorrect Kubernetes version %s, valid version(for example): v1.23" % owner)
         minor_version = int(version.split('.')[1])
         if minor_version > minor_version_cfg:
             raise Exception("%s version must not be higher than Kubernetes version" % owner)
 
 
-def finalize_inventory_psp(cluster, inventory_to_finalize):
+def finalize_inventory_psp(cluster: KubernetesCluster, inventory_to_finalize: dict):
     if cluster.context.get('initial_procedure') != 'manage_psp':
         return inventory_to_finalize
     procedure_config = cluster.procedure_inventory["psp"]
 
     if "rbac" not in inventory_to_finalize:
         inventory_to_finalize["rbac"] = {}
     if "psp" not in inventory_to_finalize["rbac"]:
@@ -226,15 +227,15 @@
             continue
         # old item is nor deleted, nor updated, then we need to preserve it in resulting list
         resulting_list.append(old_item)
 
     return resulting_list
 
 
-def install_psp_task(cluster):
+def install_psp_task(cluster: KubernetesCluster):
     if not is_security_enabled(cluster.inventory):
         cluster.log.debug("Pod security disabled, skipping policies installation...")
         return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Installing OOB policies...")
@@ -244,39 +245,39 @@
 
     cluster.log.debug("Installing custom policies...")
     first_control_plane.call(manage_policies,
                       manage_type="apply",
                       manage_scope=cluster.inventory["rbac"]["psp"]["custom-policies"])
 
 
-def delete_custom_task(cluster):
+def delete_custom_task(cluster: KubernetesCluster):
     if "delete-policies" not in cluster.procedure_inventory["psp"]:
         cluster.log.debug("No 'delete-policies' specified, skipping...")
         return
 
     cluster.log.debug("Deleting custom 'delete-policies'")
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     first_control_plane.call(manage_policies,
                       manage_type="delete",
                       manage_scope=cluster.procedure_inventory["psp"]["delete-policies"])
 
 
-def add_custom_task(cluster):
+def add_custom_task(cluster: KubernetesCluster):
     if "add-policies" not in cluster.procedure_inventory["psp"]:
         cluster.log.debug("No 'add-policies' specified, skipping...")
         return
 
     cluster.log.debug("Applying custom 'add-policies'")
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     first_control_plane.call(manage_policies,
                       manage_type="apply",
                       manage_scope=cluster.procedure_inventory["psp"]["add-policies"])
 
 
-def reconfigure_oob_task(cluster):
+def reconfigure_oob_task(cluster: KubernetesCluster):
     target_security_state = cluster.procedure_inventory["psp"].get("pod-security")
     oob_policies = cluster.procedure_inventory["psp"].get("oob-policies")
 
     # reconfigure OOB only if state will be changed, or OOB configuration was changed
     if not target_security_state and not oob_policies:
         cluster.log.debug("No need to reconfigure OOB policies, skipping...")
         return
@@ -298,61 +299,60 @@
     for policy in provided_oob_policies:
         if procedure_config.get(policy, current_config[policy]) == "enabled":
             policies_to_recreate[policy] = True
     first_control_plane.call(apply_privileged_policy)
     first_control_plane.call(manage_policies, manage_type="apply", manage_scope=resolve_oob_scope(policies_to_recreate, "all"))
 
 
-def reconfigure_plugin_task(cluster):
+def reconfigure_plugin_task(cluster: KubernetesCluster):
     target_state = cluster.procedure_inventory["psp"].get("pod-security")
 
     if not target_state:
         cluster.log.debug("Security plugin will not be reconfigured")
         return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Updating kubeadm config map")
-    result = first_control_plane.call(update_kubeadm_configmap, target_state=target_state)
-    final_admission_plugins_list = list(result.values())[0]
+    final_admission_plugins_list = first_control_plane.call(update_kubeadm_configmap, target_state=target_state)
 
     # update api-server config on all control-planes
     cluster.log.debug("Updating kube-apiserver configs on control-planes")
     cluster.nodes["control-plane"].call(update_kubeapi_config, options_list=final_admission_plugins_list)
 
 
-def restart_pods_task(cluster):
+def restart_pods_task(cluster: KubernetesCluster):
     if cluster.context.get('initial_procedure') == 'manage_pss':
         # check if pods restart is enabled
         is_restart = cluster.procedure_inventory.get("restart-pods", False)
         if not is_restart:
             cluster.log.debug("'restart-pods' is disabled, pods won't be restarted")
             return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Drain-Uncordon all nodes to restart pods")
     kube_nodes = cluster.nodes["control-plane"].include_group(cluster.nodes["worker"])
-    for node in kube_nodes.get_ordered_members_list(provide_node_configs=True):
+    for node in kube_nodes.get_ordered_members_list():
         first_control_plane.sudo(
-            kubernetes.prepare_drain_command(cluster, node["name"], disable_eviction=False),
+            kubernetes.prepare_drain_command(cluster, node.get_node_name(), disable_eviction=False),
             hide=False)
-        first_control_plane.sudo("kubectl uncordon %s" % node["name"], hide=False)
+        first_control_plane.sudo("kubectl uncordon %s" % node.get_node_name(), hide=False)
 
     cluster.log.debug("Restarting daemon-sets...")
     daemon_sets = ruamel.yaml.YAML().load(list(first_control_plane.sudo("kubectl get ds -A -o yaml").values())[0].stdout)
     for ds in daemon_sets["items"]:
         first_control_plane.sudo("kubectl rollout restart ds %s -n %s" % (ds["metadata"]["name"], ds["metadata"]["namespace"]))
 
     # we do not know to wait for, only for system pods maybe
     cluster.log.debug("Waiting for system pods...")
-    first_control_plane.call(kubernetes.wait_for_any_pods, connection=None)
+    kubernetes.wait_for_any_pods(cluster, first_control_plane)
 
 
-def update_kubeadm_configmap_psp(first_control_plane, target_state):
+def update_kubeadm_configmap_psp(first_control_plane: NodeGroup, target_state: str) -> str:
     yaml = ruamel.yaml.YAML()
 
     # load kubeadm config map and retrieve cluster config
     result = first_control_plane.sudo("kubectl get cm kubeadm-config -n kube-system -o yaml")
     kubeadm_cm = yaml.load(list(result.values())[0].stdout)
     cluster_config = yaml.load(kubeadm_cm["data"]["ClusterConfiguration"])
 
@@ -372,23 +372,23 @@
     first_control_plane.put(buf, "/tmp/%s.yaml" % filename)
     first_control_plane.sudo("kubectl apply -f /tmp/%s.yaml" % filename)
     first_control_plane.sudo("rm -f /tmp/%s.yaml" % filename)
 
     return final_plugins_string
 
 
-def update_kubeadm_configmap(first_control_plane, target_state):
+def update_kubeadm_configmap(first_control_plane: NodeGroup, target_state: str) -> str:
     admission_impl = first_control_plane.cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
         return update_kubeadm_configmap_psp(first_control_plane, target_state)
-    elif admission_impl == "pss":
+    else:  # admission_impl == "pss":
         return update_kubeadm_configmap_pss(first_control_plane, target_state)
 
 
-def update_kubeapi_config_psp(control_planes, plugins_list):
+def update_kubeapi_config_psp(control_planes: NodeGroup, plugins_list: str):
     yaml = ruamel.yaml.YAML()
 
     for control_plane in control_planes.get_ordered_members_list():
         result = control_plane.sudo("cat /etc/kubernetes/manifests/kube-apiserver.yaml")
 
         # update kube-apiserver config with updated plugins list
         conf = yaml.load(list(result.values())[0].stdout)
@@ -408,61 +408,61 @@
         else:
             control_plane.call(utils.wait_command_successful,
                                                    command="docker stop $(sudo docker ps -q -f 'name=k8s_kube-apiserver'"
                                                            " | awk '{print $1}')")
         control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
 
 
-def update_kubeapi_config(control_planes, options_list):
+def update_kubeapi_config(control_planes: NodeGroup, options_list: str):
     admission_impl = control_planes.cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
         return update_kubeapi_config_psp(control_planes, options_list)
     elif admission_impl == "pss":
         return update_kubeapi_config_pss(control_planes, options_list)
 
-def is_security_enabled(inventory):
+def is_security_enabled(inventory: dict):
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return inventory["rbac"]["psp"]["pod-security"] == "enabled"
     elif admission_impl == "pss":
         return inventory["rbac"]["pss"]["pod-security"] == "enabled"
 
 
-def apply_privileged_policy(group):
+def apply_privileged_policy(group: NodeGroup):
     return manage_privileged_from_file(group, privileged_policy_filename, "apply")
 
 
-def delete_privileged_policy(group):
+def delete_privileged_policy(group: NodeGroup):
     return manage_privileged_from_file(group, privileged_policy_filename, "delete")
 
 
-def apply_admission(group):
+def apply_admission(group: NodeGroup):
     admission_impl = group.cluster.inventory['rbac']['admission']
     if is_security_enabled(group.cluster.inventory):
         if admission_impl == "psp":
             group.cluster.log.debug("Setting up privileged psp...")
             apply_privileged_policy(group)
         elif admission_impl == "pss":
             group.cluster.log.debug("Setting up default pss...")
             apply_default_pss(group.cluster)
 
 
-def apply_default_pss(cluster):
+def apply_default_pss(cluster: KubernetesCluster):
     if cluster.context.get('initial_procedure') == 'manage_pss':
         procedure_config = cluster.procedure_inventory["pss"]
         current_config = cluster.inventory["rbac"]["pss"]
         if procedure_config["pod-security"] == "enabled" and current_config["pod-security"] == "enabled":
             return manage_pss(cluster, "apply")
         elif procedure_config["pod-security"] == "enabled" and current_config["pod-security"] == "disabled":
             return manage_pss(cluster, "install")
     else:
             return manage_pss(cluster, "init")
 
 
-def delete_default_pss(cluster):
+def delete_default_pss(cluster: KubernetesCluster):
     procedure_config = cluster.procedure_inventory["pss"]
     current_config = cluster.inventory["rbac"]["pss"]
     if procedure_config["pod-security"] == "disabled" and current_config["pod-security"] == "enabled":
         return manage_pss(cluster, "delete")
 
 
 def manage_privileged_from_file(group: NodeGroup, filename, manage_type):
@@ -471,16 +471,16 @@
     privileged_policy = utils.read_internal(os.path.join(policies_file_path, filename))
     remote_path = tmp_filepath_pattern % filename
     group.put(io.StringIO(privileged_policy), remote_path, backup=True, sudo=True)
 
     return group.sudo("kubectl %s -f %s" % (manage_type, remote_path), warn=True)
 
 
-def resolve_oob_scope(oob_policies_conf, selector):
-    result = {
+def resolve_oob_scope(oob_policies_conf: Dict[str, Any], selector: str):
+    result: Dict[str, List[dict]] = {
         psp_list_option: [],
         roles_list_option: [],
         bindings_list_option: []
     }
 
     for key, value in oob_policies_conf.items():
         if value == selector or selector == "all":
@@ -501,15 +501,15 @@
         local_path = os.path.join(policies_file_path, "%s.yaml" % oob_name)
         with utils.open_internal(local_path) as stream:
             oob_policies[oob_name] = yaml.safe_load(stream)
 
     return oob_policies
 
 
-def manage_policies(group, manage_type, manage_scope):
+def manage_policies(group: NodeGroup, manage_type, manage_scope):
     psp_to_manage = manage_scope.get(psp_list_option, None)
     roles_to_manage = manage_scope.get(roles_list_option, None)
     bindings_to_manage = manage_scope.get(bindings_list_option, None)
 
     if not psp_to_manage and not roles_to_manage and not bindings_to_manage:
         group.cluster.log.verbose("No policies to %s" % manage_type)
         return
@@ -559,21 +559,21 @@
             resulting_list = current_plugins.replace("PodSecurityPolicy", "")
         else:
             resulting_list = current_plugins
 
         return resulting_list.replace(",,", ",").strip(",")
 
 
-def install(cluster):
+def install(cluster: KubernetesCluster):
     admission_impl = cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
         return install_psp_task(cluster)
 
 
-def manage_pss_enrichment(inventory, cluster):
+def manage_pss_enrichment(inventory: dict, cluster: KubernetesCluster):
     if cluster.context.get('initial_procedure') != 'manage_pss':
         return inventory
 
     procedure_config = cluster.procedure_inventory["pss"]
     minor_version = int(cluster.inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
         
     if not is_security_enabled(inventory) and procedure_config["pod-security"] == "disabled":
@@ -602,32 +602,32 @@
         for item in procedure_config["namespaces_defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["namespaces_defaults"][item], minor_version)
 
     return inventory
 
 
-def enrich_default_admission(inventory, _):
+def enrich_default_admission(inventory: dict, _):
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if not inventory["rbac"].get("admission"):
         inventory["rbac"]["admission"] = "psp" if minor_version < 25 else "pss"
     return inventory
 
 
-def manage_enrichment(inventory, cluster):
+def manage_enrichment(inventory: dict, cluster: KubernetesCluster):
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return manage_psp_enrichment(inventory, cluster)
     elif admission_impl == "pss":
         return manage_pss_enrichment(inventory, cluster)
 
     return inventory
 
 
-def manage_pss(cluster, manage_type):
+def manage_pss(cluster: KubernetesCluster, manage_type: str):
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     control_planes = cluster.nodes["control-plane"]
     # 'apply' - change options in admission.yaml, PSS is enabled
     if manage_type == "apply":
         # set labels for predifined plugins namespaces and namespaces defined in procedure config
         label_namespace_pss(cluster, manage_type)
         # copy admission config on control-planes
@@ -637,52 +637,50 @@
             if control_plane.cluster.inventory['services']['cri']['containerRuntime'] == 'containerd':
                 control_plane.call(utils.wait_command_successful, command="crictl rm -f "
                                                        "$(sudo crictl ps --name kube-apiserver -q)")
             else:
                 control_plane.call(utils.wait_command_successful, command="docker stop "
                                                        "$(sudo docker ps -f 'name=k8s_kube-apiserver'"
                                                        " | awk '{print $1}')")
-            control_planes.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
+            control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
     # 'install' - enable PSS
     elif manage_type == "install":
         # set labels for predifined plugins namespaces and namespaces defined in procedure config
         label_namespace_pss(cluster, manage_type)
         # copy admission config on control-planes
         copy_pss(cluster.nodes["control-plane"])
 
         cluster.log.debug("Updating kubeadm config map")
-        result = first_control_plane.call(update_kubeadm_configmap_pss, target_state="enabled")
-        final_features_list = list(result.values())[0]
+        final_features_list = first_control_plane.call(update_kubeadm_configmap_pss, target_state="enabled")
 
         # update api-server config on all control-planes
         cluster.log.debug("Updating kube-apiserver configs on control-planes")
         cluster.nodes["control-plane"].call(update_kubeapi_config_pss, features_list=final_features_list)
     # 'init' make changes during init Kubernetes cluster
     elif manage_type == "init":
         cluster.log.debug("Updating kubeadm config map")
-        result = first_control_plane.call(update_kubeadm_configmap_pss, target_state="enabled")
+        first_control_plane.call(update_kubeadm_configmap_pss, target_state="enabled")
     # 'delete' - disable PSS
     elif manage_type == "delete":
         # set labels for predifined plugins namespaces and namespaces defined in procedure config
         label_namespace_pss(cluster, manage_type)
 
-        result = first_control_plane.call(update_kubeadm_configmap, target_state="disabled")
-        final_features_list = list(result.values())[0]
+        final_features_list = first_control_plane.call(update_kubeadm_configmap, target_state="disabled")
 
         # update api-server config on all control-planes
         cluster.log.debug("Updating kube-apiserver configs on control-planes")
         cluster.nodes["control-plane"].call(update_kubeapi_config_pss, features_list=final_features_list)
 
         # erase PSS admission config 
         cluster.log.debug("Erase admission configuration... %s" % admission_path)
         group = cluster.nodes["control-plane"]
         group.sudo("rm -f %s" % admission_path, warn=True)
 
 
-def update_kubeapi_config_pss(control_planes, features_list):
+def update_kubeapi_config_pss(control_planes: NodeGroup, features_list: str):
     yaml = ruamel.yaml.YAML()
 
     for control_plane in control_planes.get_ordered_members_list():
         result = control_plane.sudo("cat /etc/kubernetes/manifests/kube-apiserver.yaml")
 
         # update kube-apiserver config with updated features list or delete '--feature-gates' and '--admission-control-config-file'
         conf = yaml.load(list(result.values())[0].stdout)
@@ -692,16 +690,16 @@
                 new_command.append("--admission-control-config-file=%s" % admission_path)
             else:
                 new_command.append("--admission-control-config-file=''")
             new_command.append("--feature-gates=%s" % features_list)
         else:
             for item in conf["spec"]["containers"][0]["command"]:
                 if item.startswith("--"):
-                    key = re.split('=',item)[0]
-                    value = re.search('=(.*)$', item).group(1)
+                    key = item.split('=')[0]
+                    value = item[len(key)+1:]
                     if key in ["--feature-gates", "--admission-control-config-file"]:
                         del_option = "%s=%s" % (key, value)
                         new_command.remove(del_option)
 
         conf["spec"]["containers"][0]["command"] = new_command
 
         # place updated config on control-plane
@@ -713,18 +711,18 @@
         if control_plane.cluster.inventory['services']['cri']['containerRuntime'] == 'containerd':
             control_plane.call(utils.wait_command_successful, command="crictl rm -f "
                                                        "$(sudo crictl ps --name kube-apiserver -q)")
         else:
             control_plane.call(utils.wait_command_successful, command="docker stop "
                                                        "$(sudo docker ps -f 'name=k8s_kube-apiserver'"
                                                        " | awk '{print $1}')")
-        control_planes.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
+        control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
 
 
-def update_kubeadm_configmap_pss(first_control_plane, target_state):
+def update_kubeadm_configmap_pss(first_control_plane: NodeGroup, target_state: str) -> str:
     yaml = ruamel.yaml.YAML()
 
     final_feature_list = ""
 
     # load kubeadm config map and retrieve cluster config
     result = first_control_plane.sudo("kubectl get cm kubeadm-config -n kube-system -o yaml")
     kubeadm_cm = yaml.load(list(result.values())[0].stdout)
@@ -767,15 +765,15 @@
     first_control_plane.put(buf, "/tmp/%s.yaml" % filename)
     first_control_plane.sudo("kubectl apply -f /tmp/%s.yaml" % filename)
     first_control_plane.sudo("rm -f /tmp/%s.yaml" % filename)
 
     return final_feature_list
 
 
-def finalize_inventory(cluster, inventory_to_finalize):
+def finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
     admission_impl = cluster.inventory['rbac']['admission']
 
     if admission_impl == "psp":
         return finalize_inventory_psp(cluster, inventory_to_finalize)
     elif admission_impl == "pss":
         return finalize_inventory_pss(cluster, inventory_to_finalize)
 
@@ -793,25 +791,30 @@
         default_merger.merge(current_config.setdefault("defaults", {}), procedure_config["defaults"])
     if "exemptions" in procedure_config:
         default_merger.merge(current_config.setdefault("exemptions", {}), procedure_config["exemptions"])
 
     return inventory_to_finalize
 
 # update PSP/PSS fields in the inventory dumped to cluster_finalized.yaml
-def update_finalized_inventory(cluster, inventory_to_finalize):
+def update_finalized_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
     if cluster.context.get('initial_procedure') == 'manage_pss':
         current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("pss", {})
         current_config["pod-security"] = cluster.procedure_inventory["pss"].get("pod-security", current_config.get("pod-security", "enabled"))
     elif cluster.context.get('initial_procedure') == 'manage_psp':
         current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("psp", {})
         current_config["pod-security"] = cluster.procedure_inventory["psp"].get("pod-security", current_config.get("pod-security", "enabled"))
+    # remove PSP section from cluster_finalyzed.yaml  
+    minor_version = int(inventory_to_finalize["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
+    if minor_version >= 24:
+        del inventory_to_finalize["rbac"]["psp"]
+
 
     return inventory_to_finalize
 
-def copy_pss(group):
+def copy_pss(group: NodeGroup):
     if  group.cluster.inventory['rbac']['admission'] !=  "pss":
         return
     if group.cluster.context.get('initial_procedure') == 'manage_pss':
         if not is_security_enabled(group.cluster.inventory) and \
                 group.cluster.procedure_inventory["pss"]["pod-security"] != "enabled":
             group.cluster.log.debug("Pod security disabled, skipping pod admission installation...")
             return
@@ -834,15 +837,15 @@
     group.sudo("mkdir -p %s" % admission_dir, warn=True)
     result = group.sudo("cp %s %s" % (remote_path, admission_path), warn=True)
     group.sudo("rm -f %s" % remote_path)
 
     return result
 
 
-def label_namespace_pss(cluster, manage_type):
+def label_namespace_pss(cluster: KubernetesCluster, manage_type: str):
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     # set/delete labels on predifined plugins namsespaces
     for plugin in cluster.inventory["plugins"]:
         is_install = cluster.inventory["plugins"][plugin].get("install")
         if manage_type in ["apply", "install"]:
             if is_install and plugin in privileged_plugins.keys():
                 # set label 'pod-security.kubernetes.io/enforce: privileged' for local provisioner and ingress namespaces
@@ -917,12 +920,12 @@
                 cluster.log.debug(f"Delete PSS labels on {ns_name} namespace")
                 if isinstance(namespace, dict):
                     for item in list(namespace[ns_name]):
                         first_control_plane.sudo(f"kubectl label ns {ns_name} "
                                     f"pod-security.kubernetes.io/{item}-")
 
 
-def check_inventory(cluster):
+def check_inventory(cluster: KubernetesCluster):
     # check if 'admission' option in cluster.yaml and procedure.yaml are inconsistent 
     if cluster.context.get('initial_procedure') == 'manage_pss' and cluster.inventory["rbac"]["admission"] != "pss" or \
         cluster.context.get('initial_procedure') == 'manage_psp' and cluster.inventory["rbac"]["admission"] != "psp":
         raise Exception("Procedure config and cluster config are inconsistent. Please check 'admission' option")
```

### Comparing `kubemarine-0.18.2/kubemarine/apt.py` & `kubemarine-0.19.0/kubemarine/apt.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,121 +9,134 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-
-import fabric
+from typing import Union, Optional, List, Dict
 
 from kubemarine.core import utils
-from kubemarine.core.group import NodeGroupResult, NodeGroup
+from kubemarine.core.executor import RunnersResult, Token, Callback
+from kubemarine.core.group import (
+    NodeGroup, RunnersGroupResult, AbstractGroup, RunResult, DeferredGroup, GROUP_RUN_TYPE
+)
 
 DEBIAN_HEADERS = 'DEBIAN_FRONTEND=noninteractive '
 
 
-def ls_repofiles(group, **kwargs) -> NodeGroupResult:
-    return group.sudo('ls -la /etc/apt/sources.list.d', **kwargs)
+def ls_repofiles(group: NodeGroup) -> RunnersGroupResult:
+    return group.sudo('ls -la /etc/apt/sources.list.d')
 
 
-def backup_repo(group, repo_filename="*", **kwargs) -> NodeGroupResult or None:
+def backup_repo(group: NodeGroup) -> Optional[RunnersGroupResult]:
     if not group.cluster.inventory['services']['packages']['package_manager']['replace-repositories']:
         group.cluster.log.debug("Skipped - repos replacement disabled in configuration")
-        return
+        return None
     # all files in directory will be renamed: xxx.repo -> xxx.repo.bak
     # if there already any files with ".bak" extension, they should not be renamed to ".bak.bak"!
-    return group.sudo("find %s -type f -name '%s.list' | "
-                      "sudo xargs -t -iNAME mv -bf NAME NAME.bak" % ("/etc/apt/", repo_filename), **kwargs)
+    return group.sudo("find /etc/apt/ -type f -name '*.list' | "
+                      "sudo xargs -t -iNAME mv -bf NAME NAME.bak")
 
 
-def add_repo(group, repo_data="", repo_filename="predefined", **kwargs) -> NodeGroupResult:
-    create_repo_file(group, repo_data, get_repo_file_name(repo_filename))
-    return group.sudo(DEBIAN_HEADERS + 'apt clean && sudo apt update', **kwargs)
+def add_repo(group: NodeGroup, repo_data: Union[List[str], Dict[str, dict], str]) -> RunnersGroupResult:
+    create_repo_file(group, repo_data, get_repo_file_name())
+    return group.sudo(DEBIAN_HEADERS + 'apt clean && sudo apt update')
 
 
-def get_repo_file_name(repo_filename="predefined"):
-    return '%s/%s.list' % ("/etc/apt/sources.list.d/", repo_filename)
+def get_repo_file_name() -> str:
+    return '/etc/apt/sources.list.d/predefined.list'
 
 
-def create_repo_file(group, repo_data, repo_file):
+def create_repo_file(group: AbstractGroup[RunResult],
+                     repo_data: Union[List[str], Dict[str, dict], str],
+                     repo_file: str) -> None:
     # if repo_data is list, then convert it to string using join
     if isinstance(repo_data, list):
         repo_data_str = "\n".join(repo_data) + "\n"
+    elif isinstance(repo_data, dict):
+        raise Exception("Not supported repositories format for apt package manager")
     else:
         repo_data_str = utils.read_external(repo_data)
-    group.put(io.StringIO(repo_data_str), repo_file, sudo=True)
+
+    repo_data_stream = io.StringIO(repo_data_str)
+    group.put(repo_data_stream, repo_file, sudo=True)
 
 
-def clean(group, **kwargs) -> NodeGroupResult:
-    return group.sudo(DEBIAN_HEADERS + "apt clean", **kwargs)
+def clean(group: NodeGroup) -> RunnersGroupResult:
+    return group.sudo(DEBIAN_HEADERS + "apt clean")
 
 
-def get_install_cmd(include: str or list, exclude=None) -> str:
+def get_install_cmd(include: Union[str, List[str]], exclude: Union[str, List[str]] = None) -> str:
     if isinstance(include, list):
         include = ' '.join(include)
     command = DEBIAN_HEADERS + 'apt update && ' + \
               DEBIAN_HEADERS + 'sudo apt install -y %s' % include
 
     if exclude is not None:
         if isinstance(exclude, list):
             exclude = ','.join(exclude)
         command += ' --exclude=%s' % exclude
 
+    # apt fails to install (downgrade) package if it is already present and has higher version,
+    # thus we do not need additional checks here (in contrast to yum)
     return command
 
 
-def install(group, include=None, exclude=None, **kwargs) -> NodeGroupResult:
+def install(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+            exclude: Union[str, List[str]] = None,
+            callback: Callback = None) -> GROUP_RUN_TYPE:
     if include is None:
         raise Exception('You must specify included packages to install')
 
     command = get_install_cmd(include, exclude)
 
-    return group.sudo(command, **kwargs)
-    # apt fails to install (downgrade) package if it is already present and has higher version,
-    # thus we do not need additional checks here (in contrast to yum)
+    return group.sudo(command, callback=callback)
 
 
-def remove(group, include=None, exclude=None, **kwargs) -> NodeGroupResult:
+def remove(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None, exclude: Union[str, List[str]] = None,
+           warn: bool = False, hide: bool = True) -> GROUP_RUN_TYPE:
     if include is None:
         raise Exception('You must specify included packages to remove')
 
     if isinstance(include, list):
         include = ' '.join(include)
     command = DEBIAN_HEADERS + 'apt purge -y %s' % include
 
     if exclude is not None:
         if isinstance(exclude, list):
             exclude = ','.join(exclude)
         command += ' --exclude=%s' % exclude
 
-    return group.sudo(command, **kwargs)
+    return group.sudo(command, warn=warn, hide=hide)
 
 
-def upgrade(group, include=None, exclude=None, **kwargs) -> NodeGroupResult:
+def upgrade(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+            exclude: Union[str, List[str]] = None) -> GROUP_RUN_TYPE:
     if include is None:
         raise Exception('You must specify included packages to upgrade')
 
     if isinstance(include, list):
         include = ' '.join(include)
     command = DEBIAN_HEADERS + 'apt update && ' + \
               DEBIAN_HEADERS + 'sudo apt upgrade -y %s' % include
 
     if exclude is not None:
         if isinstance(exclude, list):
             exclude = ','.join(exclude)
         command += ' --exclude=%s' % exclude
 
-    return group.sudo(command, **kwargs)
+    return group.sudo(command)
 
 
-def no_changes_found(action: callable, result: fabric.runners.Result) -> bool:
-    if action not in (install, upgrade, remove):
+def no_changes_found(action: str, result: RunnersResult) -> bool:
+    if action not in ('install', 'upgrade', 'remove'):
         raise Exception(f"Unknown action {action}")
     return "0 upgraded, 0 newly installed, 0 to remove" in result.stdout
 
 
-def search(group: NodeGroup, package: str, **kwargs) -> NodeGroupResult:
+def search(group: DeferredGroup, package: str, callback: Callback = None) -> Token:
     if package is None:
         raise Exception('You must specify package to search')
-    command = DEBIAN_HEADERS + 'apt show %s  || echo "Package is unavailable"' % package
-    return group.sudo(command, **kwargs)
+    command = DEBIAN_HEADERS + 'apt show %s' % package
+
+    return group.sudo(command, warn=True, callback=callback)
```

### Comparing `kubemarine-0.18.2/kubemarine/audit.py` & `kubemarine-0.19.0/kubemarine/audit.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 """
 This module works with audit on remote nodes.
 Using this module you can install, enable audit and configure audit rules.
 """
 
 import io
+from typing import Optional
 
 from kubemarine import system, packages
 from kubemarine.core import utils
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup, NodeGroupResult
+from kubemarine.core.group import NodeGroup, RunnersGroupResult, CollectorCallback
 
 
 def verify_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     for host in cluster.nodes['all'].get_final_nodes().get_hosts():
         package_name = cluster.get_package_association_for_node(host, 'audit', 'package_name')
         if isinstance(package_name, str):
             package_name = [package_name]
@@ -36,21 +36,21 @@
             os_family = cluster.get_os_family_for_node(host)
             raise Exception(f'Audit has multiple associated packages {package_name} for OS {os_family!r} '
                             f'that is currently not supported')
 
     return inventory
 
 
-def install(group: NodeGroup) -> str or None:
+def install(group: NodeGroup) -> Optional[RunnersGroupResult]:
     """
     Automatically installs and enables the audit service for the specified nodes
     :param group: Nodes group on which audit installation should be performed
     :return: String with installation output from nodes or None, when audit installation was skipped
     """
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     log.verbose('Searching for already installed auditd package...')
 
     # Reduce nodes amount for installation
     hosts_to_packages = packages.get_association_hosts_to_packages(group, cluster.inventory, 'audit')
 
@@ -60,51 +60,48 @@
         for detected_version, hosts in detected_audit_versions.items():
             log.verbose(f'{detected_version}: {hosts}')
             if 'not installed' in detected_version:
                 not_installed_hosts.extend(hosts)
 
     if not not_installed_hosts:
         log.debug('Auditd is already installed on all nodes')
-        return
+        return None
     else:
         log.debug(f'Auditd package is not installed on {not_installed_hosts}, installing...')
 
-    with RemoteExecutor(cluster) as exe:
-        for host in not_installed_hosts:
-            the_node = cluster.make_group([host])
+    collector = CollectorCallback(cluster)
+    with cluster.make_group(not_installed_hosts).new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            package_name = cluster.get_package_association_for_node(node.get_host(), 'audit', 'package_name')
+            packages.install(node, include=package_name, callback=collector)
 
-            package_name = cluster.get_package_association_for_node(host, 'audit', 'package_name')
-            packages.install(the_node, include=package_name)
+            service_name = cluster.get_package_association_for_node(node.get_host(), 'audit', 'service_name')
+            system.enable_service(node, name=service_name, callback=collector)
 
-            service_name = cluster.get_package_association_for_node(host, 'audit', 'service_name')
-            system.enable_service(the_node, name=service_name)
-
-    return exe.get_last_results_str()
+    return collector.result
 
 
-def apply_audit_rules(group: NodeGroup) -> NodeGroupResult:
+def apply_audit_rules(group: NodeGroup) -> RunnersGroupResult:
     """
     Generates and applies audit rules to the group
     :param group: Nodes group, where audit service should be configured
     :return: Service restart result or nothing if audit rules are non exists, or restart is not required
     """
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     log.debug('Applying audit rules...')
     rules_content = " \n".join(cluster.inventory['services']['audit']['rules'])
     utils.dump_file(cluster, rules_content, 'audit.rules')
 
-    restart_tokens = []
-    with RemoteExecutor(cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            the_node: NodeGroup = node['connection']
-            host: str = node['connect_to']
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            host = node.get_host()
 
             rules_config_location = cluster.get_package_association_for_node(host, 'audit', 'config_location')
-            the_node.put(io.StringIO(rules_content), rules_config_location,
-                         sudo=True, backup=True)
+            node.put(io.StringIO(rules_content), rules_config_location, sudo=True, backup=True)
 
             service_name = cluster.get_package_association_for_node(host, 'audit', 'service_name')
-            restart_tokens.append(the_node.sudo(f'service {service_name} restart'))
+            node.sudo(f'service {service_name} restart', callback=collector)
 
-    return exe.get_merged_nodegroup_results(restart_tokens)
+    return collector.result
```

### Comparing `kubemarine-0.18.2/kubemarine/controlplane.py` & `kubemarine-0.19.0/kubemarine/controlplane.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from kubemarine.core.cluster import KubernetesCluster
 
 
-def controlplane_node_enrichment(inventory: dict, cluster: KubernetesCluster):
+def controlplane_node_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     """
     Enriched inventory should have both the 'master' and the 'control-plane' roles for backward compatibility
     The 'control-plane' role is used instead of 'master' role since Kubernetes v1.24
     """
     for node in inventory["nodes"]:
         node_info = node.get('name', cluster.get_access_address_from_node(node))
         if "master" in node["roles"] and "control-plane" not in node["roles"]:
@@ -29,15 +29,15 @@
         if "control-plane" in node["roles"] and "master" not in node["roles"]:
             cluster.log.debug(f"The 'master' role will be added for {node_info}")
             node["roles"].append("master")
 
     return inventory
 
 
-def controlplane_finalize_inventory(cluster, inventory):
+def controlplane_finalize_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
     """
     Delete 'control-plane' and 'master' roles before inventory saving if they are not set in 'cluster.yaml'
     """
     # remove 'master' role from inventory before dump
     for node in inventory["nodes"]:
         if 'master' in node["roles"]:
             node_info = node.get('name', cluster.get_access_address_from_node(node))
```

### Comparing `kubemarine-0.18.2/kubemarine/core/__init__.py` & `kubemarine-0.19.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/core/action.py` & `kubemarine-0.19.0/kubemarine/core/action.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from kubemarine.core.resources import DynamicResources
 
 
 class Action(ABC):
     """Base class for doing some work based on provided DynamicResources"""
 
-    def __init__(self, identifier: str, recreate_inventory=False):
+    def __init__(self, identifier: str, recreate_inventory: bool = False) -> None:
         """
         Constructor of Action to be invoked from derived classes.
 
         :param identifier action identifier, which will be preserved on nodes
                           if the action is successfully performed.
         :param recreate_inventory specifies if inventory should be recreated after the action succeeds.
         """
```

### Comparing `kubemarine-0.18.2/kubemarine/core/annotations.py` & `kubemarine-0.19.0/kubemarine/core/annotations.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,37 +7,48 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Callable, TypeVar
+
+from typing_extensions import ParamSpec
 
 from kubemarine.core.group import NodeGroup
 
 
-def restrict_multi_os_group(fn: callable):
+_P = ParamSpec('_P')
+_T = TypeVar('_T')
+
+
+def restrict_multi_os_group(fn: Callable[_P, _T]) -> Callable[_P, _T]:
     """
     Method is an annotation that does not allow origin method to use different OS families in the same group.
     :param fn: Origin function to apply annotation validation to
     :return: Validation wrapper function
     """
-    def wrapper(group: NodeGroup, *args, **kwargs):
-        # TODO: walk through all nodes in *args, check isinstance NodeGroup and perform validation
+    def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+        group = next((g for g in args if isinstance(g, NodeGroup)), None)
+        if group is None:
+            raise Exception("Failed to find argument of NodeGroup type")
         if group.is_multi_os():
             raise Exception(f'Method "{str(fn)}" do not supports multi-os group')
-        return fn(group, *args, **kwargs)
+        return fn(*args, **kwargs)
     return wrapper
 
 
-def restrict_empty_group(fn: callable):
+def restrict_empty_group(fn: Callable[_P, _T]) -> Callable[_P, _T]:
     """
     Method is an annotation that prohibits passing empty groups to the function.
     :param fn: Origin function to apply annotation validation to
     :return: Validation wrapper function
     """
-    def wrapper(group: NodeGroup, *args, **kwargs):
-        # TODO: walk through all nodes in *args, check isinstance NodeGroup and perform validation
+    def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+        group = next((g for g in args if isinstance(g, NodeGroup)), None)
+        if group is None:
+            raise Exception("Failed to find argument of NodeGroup type")
         if group.is_empty():
             raise Exception(f'Method "{str(fn)}" prohibits passing empty groups to it')
-        return fn(group, *args, **kwargs)
+        return fn(*args, **kwargs)
     return wrapper
```

### Comparing `kubemarine-0.18.2/kubemarine/core/cluster.py` & `kubemarine-0.19.0/kubemarine/core/cluster.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,147 +7,144 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import re
 from copy import deepcopy
-from typing import Dict, List, Union, Iterable, Tuple, Optional
+from typing import Dict, List, Union, Iterable, Tuple, Optional, Any, Callable
 
-import fabric
 import yaml
 
-from kubemarine.core import log, utils
-from kubemarine.core.connections import ConnectionPool, Connections
+from kubemarine.core import log, utils, static
+from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.environment import Environment
-from kubemarine.core.group import NodeGroup
-
-jinja_query_regex = re.compile("{{ .* }}", re.M)
+from kubemarine.core.group import NodeGroup, NodeConfig
 
-_AnyConnectionTypes = Union[str, NodeGroup, fabric.connection.Connection]
+_AnyConnectionTypes = Union[str, NodeGroup]
 
 
 class KubernetesCluster(Environment):
 
     def __init__(self, inventory: dict, context: dict, procedure_inventory: dict = None,
-                 logger: log.EnhancedLogger = None):
-        self.roles = []
-        self.ips = {
+                 logger: log.EnhancedLogger = None) -> None:
+        self.roles: List[str] = []
+        self.ips: Dict[str, List[str]] = {
             "all": []
         }
         self.nodes: Dict[str, NodeGroup] = {}
 
         self.raw_inventory = deepcopy(inventory)
         # Should not be copied. Can be used after successful of failed execution and might store intermediate result.
         self.context = context
         self.procedure_inventory = {} if procedure_inventory is None else deepcopy(procedure_inventory)
 
+        self._connection_pool: Optional[ConnectionPool] = None
+
         self._logger = logger if logger is not None \
             else log.init_log_from_context_args(self.globals, self.context, self.raw_inventory).logger
 
-        self._inventory = {}
-        # connection pool should be created every time, because it is relied on partially enriched inventory
-        self._connection_pool = ConnectionPool(self)
+        self._inventory: dict = {}
 
-    def enrich(self, custom_enrichment_fns: List[str] = None):
+    def enrich(self, custom_enrichment_fns: List[str] = None) -> None:
         # do not make dumps for custom enrichment functions, because result is generally undefined
         make_dumps = custom_enrichment_fns is None
         from kubemarine.core import defaults
         self._inventory = defaults.enrich_inventory(
             self, self.raw_inventory, make_dumps=make_dumps, enrichment_functions=custom_enrichment_fns)
 
     @property
     def inventory(self) -> dict:
         return self._inventory
 
     @property
+    def connection_pool(self) -> ConnectionPool:
+        if self._connection_pool is None:
+            # Connection pool should be created for each cluster object,
+            # because it relies on partially enriched inventory
+            self._connection_pool = ConnectionPool(self.inventory)
+
+        return self._connection_pool
+
+    @property
     def log(self) -> log.EnhancedLogger:
         return self._logger
 
-    def make_group(self, ips: List[_AnyConnectionTypes]) -> NodeGroup:
-        connections: Connections = {}
-        for ip in ips:
-            if isinstance(ip, fabric.connection.Connection):
-                ip = ip.host
-                connections[ip] = self._connection_pool.get_connection(ip)
-            elif isinstance(ip, NodeGroup):
-                for host, connection in ip.nodes.items():
-                    ip = connection.host
-                    connections[ip] = self._connection_pool.get_connection(ip)
-            elif isinstance(ip, str):
-                connections[ip] = self._connection_pool.get_connection(ip)
-            else:
-                raise Exception('Unsupported connection object type')
-        return NodeGroup(connections, self)
+    @property
+    def globals(self) -> dict:
+        return static.GLOBALS
+
+    def make_group(self, ips: Iterable[_AnyConnectionTypes]) -> NodeGroup:
+        return NodeGroup(ips, self)
 
-    def get_access_address_from_node(self, node: dict):
+    def get_access_address_from_node(self, node: dict) -> str:
         """
         Returns address which should be used to connect to the node via Fabric.
         The address also can be used as unique identifier of the node.
         """
         address = node.get('connect_to')
         if address is None:
             address = node.get('address')
         if address is None:
-            address = node.get('internal_address')
+            address = node['internal_address']
 
         return address
 
     def get_nodes_by_names(self, node_names: List[str]) -> List[dict]:
         result = []
         for node in self.inventory["nodes"]:
             if node['name'] in node_names:
                 result.append(node)
 
         return result
 
-    def get_node_by_name(self, node_name) -> Optional[dict]:
+    def get_node_by_name(self, node_name: str) -> Optional[dict]:
         nodes = self.get_nodes_by_names([node_name])
         return next(iter(nodes), None)
 
     def get_addresses_from_node_names(self, node_names: List[str]) -> List[str]:
         return [self.get_access_address_from_node(node)
                 for node in self.get_nodes_by_names(node_names)]
 
-    def get_node(self, host: Union[str, fabric.connection.Connection]) -> dict:
-        return self.make_group([host]).get_first_member(provide_node_configs=True)
+    def get_node(self, host: _AnyConnectionTypes) -> NodeConfig:
+        return self.make_group([host]).get_config()
 
     def make_group_from_nodes(self, node_names: List[str]) -> NodeGroup:
         ips = self.get_addresses_from_node_names(node_names)
         return self.make_group(ips)
 
-    def create_group_from_groups_nodes_names(self, groups_names: List[str], nodes_names: List[str]) -> NodeGroup:
-        common_group = self.make_group([])
+    def make_group_from_roles(self, roles: Iterable[str]) -> NodeGroup:
+        group = self.make_group([])
+        for role in roles:
+            if role not in self.nodes:
+                self.log.verbose(f'Group {role!r} is requested for usage, but this group does not exist.')
+                continue
 
-        if nodes_names:
-            common_group = self.make_group_from_nodes(nodes_names)
+            group = group.include_group(self.nodes[role])
 
-        if groups_names:
-            for group in groups_names:
+        return group
 
-                if group not in self.roles:
-                    self.log.verbose('Group \'%s\' is requested for usage, but this group is not exists.' % group)
-                    continue
+    def create_group_from_groups_nodes_names(self, groups_names: List[str], nodes_names: List[str]) -> NodeGroup:
+        common_group = self.make_group_from_roles(groups_names)
 
-                common_group = common_group.include_group(self.nodes[group])
+        if nodes_names:
+            common_group = common_group.include_group(self.make_group_from_nodes(nodes_names))
 
         return common_group
 
-    def schedule_cumulative_point(self, point_method):
+    def schedule_cumulative_point(self, point_method: Callable) -> None:
         from kubemarine.core import flow
-        return flow.schedule_cumulative_point(self, point_method)
+        flow.schedule_cumulative_point(self, point_method)
 
-    def is_task_completed(self, task_path) -> bool:
+    def is_task_completed(self, task_path: str) -> bool:
         from kubemarine.core import flow
         return flow.is_task_completed(self, task_path)
 
-    def get_facts_enrichment_fns(self):
+    def get_facts_enrichment_fns(self) -> List[str]:
         return [
             "kubemarine.core.schema.verify_inventory",
             "kubemarine.core.defaults.merge_defaults",
             "kubemarine.kubernetes.verify_initial_version",
             "kubemarine.kubernetes.add_node_enrichment",
             "kubemarine.kubernetes.remove_node_enrichment",
             "kubemarine.controlplane.controlplane_node_enrichment",
@@ -174,30 +171,30 @@
         self.log.verbose('Interface check finished')
         system.detect_os_family(self)
         self.log.verbose('OS family check finished')
 
         self.log.debug('Detecting nodes context finished!')
         return deepcopy(self.context['nodes'])
 
-    def _check_online_nodes(self):
+    def _check_online_nodes(self) -> None:
         """
         Check that only subset of nodes for removal can be offline
         """
         all = self.nodes['all']
         for_removal = all.get_nodes_for_removal()
         remained = all.exclude_group(for_removal)
         offline = all.get_online_nodes(False)
         remained_offline = remained.intersection_group(offline)
         if not remained_offline.is_empty():
             raise Exception(f"{remained_offline.get_hosts()} are not reachable. "
                             "Probably they are turned off or something is incorrect with ssh daemon, "
                             "or incorrect ssh port is specified.")
 
     # todo this check can probably be moved to prepare.check tasks group of each procedure
-    def _check_accessible_nodes(self):
+    def _check_accessible_nodes(self) -> None:
         """
         Check that all online nodes are accessible.
         """
         all = self.nodes['all']
         online = all.get_online_nodes(True)
         accessible = all.get_accessible_nodes()
         not_accessible = all.exclude_group(accessible)
@@ -249,15 +246,15 @@
         os_ids = {}
         for host in nodes_check_os.get_hosts():
             os_details = self.context['nodes'][host]['os']
             os_ids[host] = (os_details['family'], os_details['version'])
 
         return os_ids
 
-    def get_associations(self):
+    def get_associations(self) -> dict:
         """
         Returns association for all packages from inventory for the cluster.
         The method can be used only if cluster has nodes with the same and supported OS family.
         """
         return self.inventory['services']['packages']['associations'][self.get_os_family()]
 
     def _get_associations_for_os(self, os_family: str, package: str) -> dict:
@@ -277,79 +274,80 @@
         :param host: The address of the node for which required to find the associations
         :param package: The package name to get the associations for
         :return: Dict with packages and their associations
         """
         node_os_family = self.get_os_family_for_node(host)
         return self._get_associations_for_os(node_os_family, package)
 
-    def _get_package_associations_for_os(self, os_family: str, package: str, association_key: str) -> str or list:
+    def _get_package_associations_for_os(self, os_family: str, package: str, association_key: str) -> Any:
         associations = self._get_associations_for_os(os_family, package)
         association_value = associations.get(association_key)
         if association_value is None:
             raise Exception(f'Failed to get association "{association_key}" for package "{package}"')
         if not isinstance(association_value, str) and not isinstance(association_value, list):
             raise Exception(f'Unsupported association "{association_key}" value type for package "{package}", '
                             f'got: {str(association_value)}')
 
         return association_value
 
-    def get_package_association(self, package: str, association_key: str) -> Union[str, List[str]]:
+    def get_package_association(self, package: str, association_key: str) -> Any:
         """
         Returns the specified association for the specified package from inventory for the cluster.
         The method can be used only if cluster has nodes with the same and supported OS family.
 
         :param package: The package name to get the association for
         :param association_key: Association key to get
         :return: Association string or list value
         """
         os_family = self.get_os_family()
         return self._get_package_associations_for_os(os_family, package, association_key)
 
-    def get_package_association_for_node(self, host: str, package: str, association_key: str) -> str or list:
+    def get_package_association_for_node(self, host: str, package: str, association_key: str) -> Any:
         """
         Returns the specified association for the specified package from inventory for specific node.
 
         :param host: The address of the node for which required to find the association
         :param package: The package name to get the association for
         :param association_key: Association key to get
         :return: Association string or list value
         """
         os_family = self.get_os_family_for_node(host)
         return self._get_package_associations_for_os(os_family, package, association_key)
 
-    def make_finalized_inventory(self):
+    def make_finalized_inventory(self) -> dict:
         from kubemarine.core import defaults
-        from kubemarine.procedures import remove_node
+        from kubemarine.procedures import add_node, remove_node
         from kubemarine import admission, controlplane, cri, packages
 
-        cluster_finalized_functions = {
+        cluster_finalized_functions: List[Callable[[KubernetesCluster, dict], dict]] = [
             packages.cache_package_versions,
             packages.remove_unused_os_family_associations,
             cri.remove_invalid_cri_config,
+            add_node.add_node_finalize_inventory,
             remove_node.remove_node_finalize_inventory,
             admission.update_finalized_inventory,
             defaults.escape_jinja_characters_for_inventory,
             controlplane.controlplane_finalize_inventory,
-        }
+        ]
 
         # copying is currently not necessary, but it is possible in general.
         prepared_inventory = self.inventory
         for finalize_fn in cluster_finalized_functions:
             prepared_inventory = finalize_fn(self, prepared_inventory)
 
         return defaults.prepare_for_dump(prepared_inventory, copy=False)
 
-    def dump_finalized_inventory(self):
+    def dump_finalized_inventory(self) -> None:
         inventory_for_dump = self.make_finalized_inventory()
         data = yaml.dump(inventory_for_dump)
         finalized_filename = "cluster_finalized.yaml"
         utils.dump_file(self, data, finalized_filename)
         utils.dump_file(self, data, finalized_filename, dump_location=False)
 
-    def preserve_inventory(self):
+    def preserve_inventory(self) -> None:
         self.log.debug("Start preserving of the information about the procedure.")
         cluster_storage = utils.ClusterStorage(self)
         cluster_storage.make_dir()
         if self.context.get('initial_procedure') == 'add_node':
             cluster_storage.upload_info_new_control_planes()
         cluster_storage.collect_procedure_info()
         cluster_storage.compress_and_upload_archive()
```

### Comparing `kubemarine-0.18.2/kubemarine/core/connections.py` & `kubemarine-0.19.0/kubemarine/core/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,79 +7,81 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import os
 from typing import Dict
 
-import fabric, os
-
-from kubemarine.core.environment import Environment
+import fabric  # type: ignore[import]
 
+from kubemarine.core import static
 
 Connections = Dict[str, fabric.connection.Connection]
 
 
 class ConnectionPool:
-    def __init__(self, env: Environment):
-        self._env = env
+    def __init__(self, inventory: dict):
+        self.inventory = inventory
         self._connections: Connections = {}
 
     def get_connection(self, ip: str) -> fabric.connection.Connection:
         conn = self._connections.get(ip)
         if conn is None:
-            for node in self._env.inventory['nodes']:
-                if node.get('address') == ip or node.get('internal_address') == ip or node.get('connect_to') == ip:
+            for node in self.inventory['nodes']:
+                if node.get('connect_to') == ip:
                     conn = self._create_connection(ip, node)
 
             if conn is None:
                 raise Exception("Failed to find suitable node to connect to by address %s" % ip)
 
             self._connections[ip] = conn
 
         return conn
 
-    def _create_connection_from_details(self, ip: str, conn_details: dict, gateway=None, inline_ssh_env=True):
-        # fabric / invoke use default encoding of deployer.
-        # We need to use encoding of remote nodes to correctly encode output of remote commands.
-        # Currently remote nodes are always Linux, so hard-code 'utf-8'.
+    def _create_connection_from_details(self, ip: str, conn_details: dict,
+                                        gateway: fabric.connection.Connection = None,
+                                        inline_ssh_env: bool = True) -> fabric.connection.Connection:
+
+        creds={}
+        if conn_details.get('keyfile'):
+            creds['key_filename'] = os.path.expanduser(conn_details['keyfile'])
+        elif conn_details.get('password'):
+            creds['password'] = conn_details.get('password')
         cfg = fabric.Config(overrides={'run': {'encoding': "utf-8"}})
         return fabric.connection.Connection(
             host=ip,
-            user=conn_details.get('username', self._env.globals['connection']['defaults']['username']),
+            user=conn_details.get('username', static.GLOBALS['connection']['defaults']['username']),
             gateway=gateway,
-            port=conn_details.get('connection_port', self._env.globals['connection']['defaults']['port']),
+            port=conn_details.get('connection_port', static.GLOBALS['connection']['defaults']['port']),
             config=cfg,
             connect_timeout=conn_details.get('connection_timeout',
-                                             self._env.globals['connection']['defaults']['timeout']),
-            connect_kwargs={
-                "key_filename": os.path.expanduser(conn_details['keyfile'])
-            },
+                                             static.GLOBALS['connection']['defaults']['timeout']),
+            connect_kwargs=creds,
             inline_ssh_env=inline_ssh_env
         )
 
     def _create_connection(self, ip: str, node: dict) -> fabric.connection.Connection:
-        if node.get('keyfile') is None:
-            raise Exception('There is no keyfile specified in configfile for node \'%s\'' % node['name'])
+        if node.get('keyfile') is None and node.get('password') is None:
+            raise Exception('There is neither keyfile not password specified in configfile for node \'%s\'' % node['name'])
 
         gateway = None
         if 'gateway' in node:
             gateway = self._get_gateway_node_connection(node['gateway'])
 
         return self._create_connection_from_details(ip, node, gateway=gateway)
 
     def _get_gateway_node_connection(self, name: str) -> fabric.connection.Connection:
         # Create new connection instance each time even if it is the same gateway node.
         # This is necessary to not share the same gateway connection instance in multiple threads
         gateway_conn = None
 
-        for gateway in self._env.inventory.get('gateway_nodes', []):
+        for gateway in self.inventory.get('gateway_nodes', []):
             if gateway.get('name') == name:
                 if gateway.get('address') is None:
                     raise Exception('There is no address specified in configfile for gateway \'%s\'' % name)
                 if gateway.get('keyfile') is None:
                     raise Exception('There is no keyfile specified in configfile for gateway \'%s\'' % name)
 
                 # todo since we have no workaround for gateway connections currently,
```

### Comparing `kubemarine-0.18.2/kubemarine/core/defaults.py` & `kubemarine-0.19.0/kubemarine/core/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
 from importlib import import_module
 from copy import deepcopy
-from typing import Optional
+from typing import Optional, Dict, Any
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.errors import KME
 from kubemarine import jinja
 from kubemarine.core import utils, static, log, os
@@ -86,17 +86,16 @@
 
 def apply_defaults(inventory, cluster: KubernetesCluster):
     recursive_apply_defaults(supported_defaults, inventory)
 
     for i, node in enumerate(inventory["nodes"]):
         address = cluster.get_access_address_from_node(node)
 
-        # we have definitely know how to connect
+        # we definitely know how to connect
         cluster.inventory["nodes"][i]["connect_to"] = address
-        cluster.inventory["nodes"][i]["connection"] = cluster.make_group([address])
 
         if not cluster.context["nodes"].get(address):
             cluster.context["nodes"][address] = {}
 
         if address not in cluster.ips["all"]:
             cluster.ips['all'].append(address)
 
@@ -106,27 +105,27 @@
                 cluster.ips[role] = []
             if address not in cluster.ips[role]:
                 cluster.ips[role].append(address)
 
     return inventory
 
 
-def apply_registry(inventory, cluster):
+def apply_registry(inventory: dict, cluster: KubernetesCluster):
 
     if not inventory.get('registry'):
         cluster.log.verbose('Unified registry is not used')
         return inventory
 
     thirdparties_address = None
     containerd_endpoints = None
     protocol = None
 
     # registry contains either 'endpoints' or 'address' that is validated by JSON schema.
     if inventory['registry'].get('endpoints'):
-        registry_mirror_address, containerd_endpoints, thirdparties_address = apply_registry_endpoints(inventory, cluster)
+        registry_mirror_address, containerd_endpoints, thirdparties_address = apply_registry_endpoints(inventory)
     else:
         if inventory['registry'].get('docker_port'):
             registry_mirror_address = "%s:%s" % (inventory['registry']['address'], inventory['registry']['docker_port'])
         else:
             registry_mirror_address = inventory['registry']['address']
 
         protocol = 'http'
@@ -214,15 +213,15 @@
             config['source'] = source
             if 'sha1' not in config:
                 config['sha1'] = sha1
 
     return inventory
 
 
-def apply_registry_endpoints(inventory, cluster):
+def apply_registry_endpoints(inventory: dict):
 
     if not inventory['registry'].get('mirror_registry'):
         inventory['registry']['mirror_registry'] = 'registry.cluster.local'
 
     registry_mirror_address = inventory['registry']['mirror_registry']
 
     # todo Currently registry.endpoints is used only for containerd registry mirrors, but it can be provided explicitly.
@@ -240,18 +239,18 @@
             cluster.log.verbose('Control plains are set manually, nothing to detect.')
         return inventory
 
     if cluster:
         cluster.log.verbose('Detecting control plains...')
 
     # calculate controlplain ips
-    internal_address = None
-    internal_address_source = None
-    external_address = None
-    external_address_source = None
+    internal_address: Optional[str] = None
+    internal_address_source: Optional[str] = None
+    external_address: Optional[str] = None
+    external_address_source: Optional[str] = None
 
     # vrrp_ip section is not enriched yet
     # todo what if ip is an ip of some node to remove?
     if inventory.get('vrrp_ips'):
         for i, item in enumerate(inventory['vrrp_ips']):
             if isinstance(item, str):
                 if internal_address is None:
@@ -284,15 +283,16 @@
                     if node.get('address') and (external_address is None or node.get('control_endpoint', False)):
                         external_address = node['address']
                         external_address_source = role
                         if node.get('name'):
                             external_address_source += ' \"%s\"' % node['name']
 
     if external_address is None:
-        cluster.log.warning('Failed to detect external control plain. Something may work incorrect!')
+        if cluster:
+            cluster.log.warning('Failed to detect external control plain. Something may work incorrect!')
         external_address = internal_address
 
     if cluster:
         cluster.log.debug('Control plains:\n   Internal: %s (%s)\n   External: %s (%s)' % (internal_address, internal_address_source, external_address, external_address_source))
 
     # apply controlplain ips
     if not inventory.get('control_plain'):
@@ -331,16 +331,16 @@
                 section_copy = deepcopy(section[value])
                 for custom_key, custom_value in section_copy.items():
                     # here section['key'] refers to default, not custom value
                     default_value = deepcopy(section[key])
                     section[value][custom_key] = default_merger.merge(default_value, custom_value)
 
 
-def calculate_node_names(inventory: dict, cluster):
-    roles_iterators = {}
+def calculate_node_names(inventory: dict, _):
+    roles_iterators: Dict[str, int] = {}
     for i, node in enumerate(inventory['nodes']):
         for role_name in ['control-plane', 'worker', 'balancer']:
             if role_name in node['roles']:
                 # The idea is this:
                 # If the name is already specified, we must skip this node,
                 # however, we must consider that we already have a node of this type
                 # and increase this type iterator
@@ -359,28 +359,28 @@
                 role_i = roles_iterators.get(role_name, 1)
                 roles_iterators[role_name] = role_i + 1
                 if node.get('name') is None:
                     inventory['nodes'][i]['name'] = '%s-%s' % (role_name, role_i)
     return inventory
 
 
-def verify_node_names(inventory, cluster):
+def verify_node_names(inventory: dict, _):
     known_names = []
     for i, node in enumerate(inventory['nodes']):
         node_name = node['name']
         if node_name in known_names:
             raise Exception('Node name %s is duplicated in configfile' % node_name)
         if re.findall(invalid_node_name_regex, node_name):
             raise Exception('Node name \"%s\" contains invalid characters. A DNS-1123 subdomain must consist of lower '
                             'case alphanumeric characters, \'-\' or \'.\'' % node_name)
         known_names.append(node_name)
     return inventory
 
 
-def calculate_nodegroups(inventory, cluster):
+def calculate_nodegroups(inventory: dict, cluster: KubernetesCluster):
     for role in cluster.ips.keys():
         cluster.nodes[role] = cluster.make_group(cluster.ips[role])
     return inventory
 
 
 def merge_defaults(inventory: dict, cluster: KubernetesCluster):
     base_inventory = deepcopy(static.DEFAULTS)
@@ -443,15 +443,15 @@
     inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, prepare_for_dump(inventory))
     merged_inventory = yaml.dump(inventory_for_dump)
     utils.dump_file(cluster, merged_inventory, "cluster_precompiled.yaml")
 
     return inventory
 
 
-def compile_object(logger: log.EnhancedLogger, struct: object, root: dict, ignore_jinja_escapes=True) -> object:
+def compile_object(logger: log.EnhancedLogger, struct: Any, root: dict, ignore_jinja_escapes=True) -> Any:
     if isinstance(struct, list):
         new_struct = []
         for i, v in enumerate(struct):
             struct[i] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
             # delete empty list entries, which can appear after jinja compilation
             if struct[i] != '':
                 new_struct.append(struct[i])
@@ -502,30 +502,26 @@
         matches = re.findall(jinja_query_regex, value)
         for match in matches:
             # TODO: rewrite to correct way of match replacement: now it can cause "{raw}{raw}xxx.." circular bug
             value = value.replace(match, '{% raw %}'+match+'{% endraw %}')
     return value
 
 
-def prepare_for_dump(inventory, copy=True):
-    # preparation for dump required to remove memory links
+def prepare_for_dump(inventory: dict, copy: bool = True) -> dict:
+    # different preparations before the inventory can be dumped
 
     if copy:
         dump_inventory = deepcopy(inventory)
     else:
         dump_inventory = inventory
 
-    for i, node in enumerate(dump_inventory['nodes']):
-        if 'connection' in dump_inventory['nodes'][i]:
-            del dump_inventory['nodes'][i]['connection']
-
     return dump_inventory
 
 
-def manage_true_false_values(inventory, cluster):
+def manage_true_false_values(inventory: dict, _):
     # Check undefined values for plugin.name.install and convert it to bool
     for plugin_name, plugin_item in inventory["plugins"].items():
         # Check install value
         if 'install' not in plugin_item:
             continue
         value = utils.true_or_false(plugin_item.get('install', False))
         if value == 'undefined':
```

### Comparing `kubemarine-0.18.2/kubemarine/core/environment.py` & `kubemarine-0.19.0/kubemarine/core/os.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-# Copyright 2021-2022 NetCracker Technology Corporation
+# Copyright 2021-2023 NetCracker Technology Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from abc import ABC, abstractmethod
+from typing import Iterator, Mapping, List
 
-from kubemarine.core import static
 
+class Environ(Mapping[str, str]):
+    """
+    Read-only view of os.environ.
+    """
 
-class Environment(ABC):
-    @property
-    @abstractmethod
-    def inventory(self) -> dict:
-        pass
+    def __getitem__(self, name: str) -> str:
+        # check presence of the variable and throw KeyError if necessary
+        return os.environ[name]
 
-    @property
-    def globals(self) -> dict:
-        return static.GLOBALS
+    def __len__(self) -> int:
+        return len(os.environ)
 
-    @staticmethod
-    def is_deploying_from_windows():
-        return os.name == 'nt'
+    def __iter__(self) -> Iterator[str]:
+        return iter(os.environ)
+
+    __slots__: List[str] = []
```

### Comparing `kubemarine-0.18.2/kubemarine/core/errors.py` & `kubemarine-0.19.0/kubemarine/core/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,144 +11,127 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import sys
 import traceback
 
-from fabric.exceptions import GroupException
 from concurrent.futures import TimeoutError
+from typing import Type
 
-KME_DICTIONARY: dict = {
-    "KME0000": {
-        "name": "Test exception"
-    },
-    "KME0003": {
-        "instance": TimeoutError,
-        "name": "Action took too long to complete and timed out"
-    },
-    "KME0004": {
-        "name": "There are no workers defined in the cluster scheme"
-    },
-    "KME0005": {
-        "name": "{hostnames} are not sudoers"
-    },
-    "KME0007": {
-        "name": "Docker CRI can not be used with endpoints registry definition."
-    },
-    "KME0008": {
-        "name": "Specified Kubernetes version '{version}' - cannot be used! Allowed versions are: {allowed_versions}."
-    },
-    "KME0009": {
-        "name": "Key {key!r} is redefined for {plugin_name!r} in cluster.yaml{previous_version_spec}, "
-                "but not present in procedure inventory{next_version_spec}. "
-                "Please, specify required plugin configuration explicitly in procedure inventory."
-    },
-    "KME0010": {
-        "name": "Associations are redefined for {package!r} in cluster.yaml{previous_version_spec}, "
-                "but not present in procedure inventory{next_version_spec}. "
-                "Please, specify required associations explicitly in procedure inventory."
-    },
-    "KME0011": {
-        "name": "Key {key!r} is redefined for third-party {thirdparty!r} in cluster.yaml{previous_version_spec}, "
-                "but not present in procedure inventory{next_version_spec}. "
-                "Please, specify required third-party configuration explicitly in procedure inventory."
-    },
-    "KME0012": {
-        "name": "Upgrade is possible only for cluster with all nodes having the same and supported OS family."
+from kubemarine.core import log as klog
+
+
+def get_kme_dictionary() -> dict:
+    from kubemarine.core.group import GroupException
+    return {
+        "KME0000": {
+            "name": "Test exception"
+        },
+        "KME0002": {
+            "instance": GroupException,
+            "name": "Remote group exception\n{reason}"
+        },
+        "KME0003": {
+            "instance": TimeoutError,
+            "name": "Action took too long to complete and timed out"
+        },
+        "KME0004": {
+            "name": "There are no workers defined in the cluster scheme"
+        },
+        "KME0005": {
+            "name": "{hostnames} are not sudoers"
+        },
+        "KME0007": {
+            "name": "Docker CRI can not be used with endpoints registry definition."
+        },
+        "KME0008": {
+            "name": "Specified Kubernetes version '{version}' - cannot be used! "
+                    "Allowed versions are: {allowed_versions}."
+        },
+        "KME0009": {
+            "name": "Key {key!r} is redefined for {plugin_name!r} in cluster.yaml{previous_version_spec}, "
+                    "but not present in procedure inventory{next_version_spec}. "
+                    "Please, specify required plugin configuration explicitly in procedure inventory."
+        },
+        "KME0010": {
+            "name": "Associations are redefined for {package!r} in cluster.yaml{previous_version_spec}, "
+                    "but not present in procedure inventory{next_version_spec}. "
+                    "Please, specify required associations explicitly in procedure inventory."
+        },
+        "KME0011": {
+            "name": "Key {key!r} is redefined for third-party {thirdparty!r} in cluster.yaml{previous_version_spec}, "
+                    "but not present in procedure inventory{next_version_spec}. "
+                    "Please, specify required third-party configuration explicitly in procedure inventory."
+        },
+        "KME0012": {
+            "name": "Upgrade is possible only for cluster with all nodes having the same and supported OS family."
+        }
     }
-}
 
 
 # TODO: support for more complex KME00XX objects with custom constructors
 class KME(RuntimeError):
-    def __init__(self, code, **kwargs):
+    def __init__(self, code: str, **kwargs: object):
         self.code = code
-        self.kme = KME_DICTIONARY.get(self.code)
+        self.kme = get_kme_dictionary().get(self.code)
         if self.kme is None:
             raise ValueError('An error was raised with an unknown error code')
-        self.message = self.kme.get('name').format(**kwargs)
+        name: str = self.kme.get('name')
+        self.message = name.format_map(kwargs)
         super().__init__(self.message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.code + ": " + self.message
 
 
 class FailException(Exception):
-    def __init__(self, message='', reason: Exception = None, hint=''):
+    def __init__(self, message: str = '', reason: Exception = None, hint: str = '') -> None:
         super().__init__(message)
         self.message = message
         self.reason = reason
         self.hint = hint
 
 
-def pretty_print_error(reason: Exception, log=None) -> None:
+def wrap_kme_exception(reason: Exception) -> Exception:
+    for dictionary_code, dictionary_kme in get_kme_dictionary().items():
+        exception_class: Type[Exception] = dictionary_kme.get('instance')
+        if exception_class is not None and isinstance(reason, exception_class):
+            return KME(dictionary_code, reason=reason)
+
+    return reason
+
+
+def pretty_print_error(message: str = '', reason: Exception = None, log: klog.EnhancedLogger = None) -> None:
     """
     Parses the passed error and nicely displays its name and structure depending on what was passed.
     The method outputs to stdout by default, but will use the logger if one is specified.
+
+    :param message: an optional message describing context of the error
     :param reason: an exception that caused the failure.
     :param log: logger object, if you need to write a log there
     :return: None
     """
-
-    if reason is None:
-        return
-
-    if isinstance(reason, KME):
+    def error_logger(msg: object) -> None:
         if log:
-            log.critical(reason)
+            log.critical(msg)
         else:
-            sys.stderr.write(str(reason))
-
-        return
-
-    for dictionary_code, dictionary_kme in KME_DICTIONARY.items():
-        if dictionary_kme.get('instance') and isinstance(reason, dictionary_kme['instance']):
-            kme = KME(dictionary_code)
-
-            if log:
-                log.critical(kme)
-            else:
-                sys.stderr.write(str(kme))
-
-            return
+            sys.stderr.write(str(msg) + "\n")
 
-    if isinstance(reason, GroupException):
-        description = "KME0002: Remote group exception"
+    error_logger('FAILURE!')
+    if message != '':
+        error_logger(message)
 
-        if log:
-            log.critical(description)
-        else:
-            sys.stderr.write(f"{description}\n")
+    if reason is None:
+        return
 
-        for connection, result in reason.result.items():
-            if log:
-                log.critical("%s:" % connection.host)
-            else:
-                sys.stderr.write("\n%s:" % connection.host)
-
-            found_dictionary_code = None
-            for dictionary_code, dictionary_kme in KME_DICTIONARY.items():
-                if dictionary_kme.get('instance') \
-                        and isinstance(result, dictionary_kme['instance']):
-                    found_dictionary_code = dictionary_code
-                    break
-
-            if found_dictionary_code:
-                kme = KME(found_dictionary_code)
-                if log:
-                    log.critical("\t" + str(kme))
-                else:
-                    sys.stderr.write("\n\t%s\n" % str(kme))
-            else:
-                if log:
-                    log.critical("\t" + str(result).replace("\n", "\n\t"))
-                else:
-                    sys.stderr.write("\n\t%s\n" % str(result).replace("\n", "\n\t"))
+    reason = wrap_kme_exception(reason)
 
+    if isinstance(reason, KME):
+        error_logger(reason)
         return
 
     if log:
         log.critical('KME0001: Unexpected exception', exc_info=reason)
     else:
         sys.stderr.write("KME0001: Unexpected exception\n")
         exc_info = (type(reason), reason, reason.__traceback__)
```

### Comparing `kubemarine-0.18.2/kubemarine/core/flow.py` & `kubemarine-0.19.0/kubemarine/core/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import argparse
 import os
 import shlex
 import sys
 import time
 from abc import abstractmethod, ABC
 from copy import deepcopy
-from typing import Type, Optional, List, Union
+from typing import Type, Optional, List, Union, Sequence
 
 from kubemarine.core import utils, cluster as c, action, resources as res, errors, summary, log
 
 DEFAULT_CLUSTER_OBJ: Optional[Type[c.KubernetesCluster]] = None
 TASK_DESCRIPTION_TEMPLATE = """
 tasks list:
     %s
@@ -38,36 +38,38 @@
         self.logger = logger
 
 
 class Flow(ABC):
     def run_flow(self, context: Union[dict, res.DynamicResources], print_summary: bool = True) -> FlowResult:
         time_start = time.time()
 
-        resources: res.DynamicResources = context
-        if isinstance(context, dict):
+        if isinstance(context, res.DynamicResources):
+            resources = context
+        else:
             resources = res.DynamicResources(context)
 
         context = resources.context
         args: dict = context['execution_arguments']
 
         try:
             if not args.get('disable_dump', True):
                 utils.prepare_dump_directory(args.get('dump_location'),
                                              reset_directory=not args.get('disable_dump_cleanup', False))
-            logger = resources.logger()
+            resources.logger()
             self._run(resources)
         except Exception as exc:
             logger = resources.logger_if_initialized()
             if isinstance(exc, errors.FailException):
                 utils.do_fail(exc.message, exc.reason, exc.hint, log=logger)
             else:
                 utils.do_fail(f"'{context['initial_procedure'] or 'undefined'}' procedure failed.", exc,
                               log=logger)
 
         time_end = time.time()
+        logger = resources.logger()
 
         if print_summary:
             summary.schedule_report(resources.working_context, summary.SummaryItem.EXECUTION_TIME,
                                     utils.get_elapsed_string(time_start, time_end))
             summary.print_summary(resources.working_context, logger)
             logger.info("SUCCESSFULLY FINISHED")
 
@@ -82,26 +84,26 @@
     def __init__(self, actions: List[action.Action]):
         self._actions = actions
 
     def _run(self, resources: res.DynamicResources):
         run_actions(resources, self._actions)
 
 
-def run_actions(resources: res.DynamicResources, actions: List[action.Action]) -> None:
+def run_actions(resources: res.DynamicResources, actions: Sequence[action.Action]) -> None:
     """
     Runs actions one by one, recreates inventory when necessary,
     managing such resources as cluster object and raw inventory.
 
     For each initialized cluster object, preserves inventory if any action is succeeded.
     """
 
     context = resources.context
     logger = resources.logger()
 
-    successfully_performed = []
+    successfully_performed: List[str] = []
     last_cluster = None
     for act in actions:
         act.prepare_context(context)
 
         if not successfully_performed:
             # first action in group
             if resources.inventory_filepath:
@@ -210,37 +212,41 @@
     result = []
     for task_name, task in tasks.items():
         __task_path = _task_path + "." + task_name if _task_path != '' else task_name
         result.extend(get_task_list(task, __task_path) if not callable(task) else [__task_path])
     return result
 
 
-def create_context(parser: argparse.ArgumentParser, cli_arguments: list, procedure: str = None):
+def create_context(parser: argparse.ArgumentParser, cli_arguments: Optional[list], procedure: str) -> dict:
+    args_list = sys.argv[1:]
+    if cli_arguments is not None:
+        args_list = cli_arguments
+
     parser.prog = procedure
-    args = vars(parse_args(parser, cli_arguments))
+    args = vars(parse_args(parser, args_list))
 
     if args.get('exclude_cumulative_points_methods', '').strip() != '':
         args['exclude_cumulative_points_methods'] = args['exclude_cumulative_points_methods'].strip().split(",")
         # print('The following cumulative points methods are marked for exclusion: [ %s ]' %
         #               ', '.join(args['exclude_cumulative_points_methods']))
     else:
         args['exclude_cumulative_points_methods'] = []
 
     context = create_empty_context(args=args, procedure=procedure)
-    context["initial_cli_arguments"] = ' '.join(map(shlex.quote, cli_arguments))
+    context["initial_cli_arguments"] = ' '.join(map(shlex.quote, args_list))
 
     return context
 
 
 def filter_flow(tasks, tasks_filter: List[str], excluded_tasks: List[str]):
     # Remove any whitespaces from filters, and split by '.'
-    tasks_filter = [tasks.split(".") for tasks in list(map(str.strip, tasks_filter))]
-    excluded_tasks = [tasks.split(".") for tasks in list(map(str.strip, excluded_tasks))]
+    tasks_path_filter = [tasks.split(".") for tasks in list(map(str.strip, tasks_filter))]
+    excluded_path_tasks = [tasks.split(".") for tasks in list(map(str.strip, excluded_tasks))]
 
-    return _filter_flow_internal(tasks, tasks_filter, excluded_tasks, [])
+    return _filter_flow_internal(tasks, tasks_path_filter, excluded_path_tasks, [])
 
 
 def _filter_flow_internal(tasks, tasks_filter: List[List[str]], excluded_tasks: List[List[str]], _task_path: List[str]):
     filtered = {}
     final_list = []
 
     for task_name, task in tasks.items():
@@ -300,15 +306,15 @@
                     "TASK FAILED %s" % __task_name, exc,
                     hint=cluster.globals['error_handling']['failure_message'] % (sys.argv[0], __task_name)
                 )
         else:
             run_tasks_recursive(task, final_task_names, cluster, cumulative_points, __task_path)
 
 
-def new_common_parser(cli_help):
+def new_common_parser(cli_help: str) -> argparse.ArgumentParser:
 
     parser = argparse.ArgumentParser(description=cli_help,
                                      formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-c', '--config',
                         default='cluster.yaml',
                         help='define main cluster configuration file')
@@ -343,15 +349,15 @@
                         action='store_true',
                         help='Do not stop the run if validation by schema fails. '
                              'The option will be removed in next release.')
 
     return parser
 
 
-def new_tasks_flow_parser(cli_help, tasks=None):
+def new_tasks_flow_parser(cli_help: str, tasks: dict = None) -> argparse.ArgumentParser:
     parser = new_common_parser(cli_help)
 
     parser.add_argument('--without-act',
                         action='store_true',
                         help='prevent tasks to be executed')
 
     parser.add_argument('--tasks',
@@ -378,39 +384,36 @@
     # Add tasks list to help section
     if tasks is not None:
         parser.epilog = TASK_DESCRIPTION_TEMPLATE % ('\n    '.join(get_task_list(tasks)))
 
     return parser
 
 
-def new_procedure_parser(cli_help, optional_config=False, tasks=None):
+def new_procedure_parser(cli_help: str, optional_config: bool = False, tasks: dict = None) -> argparse.ArgumentParser:
     parser = new_tasks_flow_parser(cli_help, tasks)
 
     help_msg = 'config file for the procedure'
     if optional_config:
         parser.add_argument('procedure_config', metavar='procedure_config', type=str, help=help_msg, nargs='?')
     else:
         parser.add_argument('procedure_config', metavar='procedure_config', type=str, help=help_msg)
 
     return parser
 
 
-def parse_args(parser, arguments: list = None):
-    if arguments is None:
-        args = parser.parse_args()
-    else:
-        args = parser.parse_args(arguments)
+def parse_args(parser: argparse.ArgumentParser, arguments: list):
+    args = parser.parse_args(arguments)
 
     if args.workdir != '':
         os.chdir(args.workdir)
 
     return args
 
 
-def schedule_cumulative_point(cluster: c.KubernetesCluster, point_method):
+def schedule_cumulative_point(cluster: c.KubernetesCluster, point_method) -> None:
     _check_within_flow(cluster)
 
     point_fullname = point_method.__module__ + '.' + point_method.__qualname__
 
     if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
         cluster.log.verbose('Method %s not scheduled - cumulative points disabled' % point_fullname)
         return
@@ -426,15 +429,15 @@
         cluster.context['scheduled_cumulative_points'] = scheduled_points
         cluster.log.verbose('Method %s scheduled' % point_fullname)
     else:
         cluster.log.verbose('Method %s already scheduled' % point_fullname)
 
 
 def proceed_cumulative_point(cluster: c.KubernetesCluster, points_list: dict,
-                             point_task_name: Union[str, type(END_OF_TASKS)], force=False):
+                             point_task_name: Union[str, object], force=False):
     _check_within_flow(cluster)
 
     if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
         return
 
     scheduled_methods = cluster.context.get('scheduled_cumulative_points', [])
 
@@ -455,26 +458,26 @@
             if point_method in scheduled_methods:
                 scheduled_methods.remove(point_method)
             results[point_method_fullname] = call_result
 
     return results
 
 
-def init_tasks_flow(cluster):
+def init_tasks_flow(cluster: c.KubernetesCluster):
     if 'proceeded_tasks' not in cluster.context:
         cluster.context['proceeded_tasks'] = []
 
 
-def add_task_to_proceeded_list(cluster, task_path):
+def add_task_to_proceeded_list(cluster: c.KubernetesCluster, task_path: str):
     if not is_task_completed(cluster, task_path):
         cluster.context['proceeded_tasks'].append(task_path)
         utils.dump_file(cluster, "\n".join(cluster.context['proceeded_tasks'])+"\n", 'finished_tasks')
 
 
-def is_task_completed(cluster, task_path):
+def is_task_completed(cluster: c.KubernetesCluster, task_path: str) -> bool:
     _check_within_flow(cluster)
     return task_path in cluster.context['proceeded_tasks']
 
 
 def _check_within_flow(cluster: c.KubernetesCluster, check=True):
     if check != ('proceeded_tasks' in cluster.context):
         raise NotImplementedError(f"The method is called {'not ' if check else ''}within tasks flow execution")
```

### Comparing `kubemarine-0.18.2/kubemarine/core/group.py` & `kubemarine-0.19.0/kubemarine/core/group.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,473 +13,396 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import io
 import os
 import random
-import re
-import time
 import uuid
-from datetime import datetime
-from typing import Callable, Dict, List, Union, IO
+from abc import ABC, abstractmethod
+from types import FunctionType
+from typing import (
+    Callable, Dict, List, Union, Any, TypeVar, Mapping, Iterator, Optional, Iterable, Generic, Set, cast
+)
 
-import fabric
-import invoke
-from invoke import UnexpectedExit
+from kubemarine.core import utils, log, errors
+from kubemarine.core.executor import (
+    RawExecutor, Token, GenericResult, RunnersResult, HostToResult, Callback, TokenizedResult,
+)
 
-from kubemarine.core import utils, log
-from kubemarine.core.connections import Connections
-from kubemarine.core.executor import RemoteExecutor
+NodeConfig = Dict[str, Any]
+GroupFilter = Union[Callable[[NodeConfig], bool], NodeConfig]
 
-_GenericResult = Union[Exception, fabric.runners.Result, fabric.transfer.Result]
-_HostToResult = Dict[str, _GenericResult]
+_RESULT = TypeVar('_RESULT', bound=GenericResult, covariant=True)
+_T = TypeVar('_T')
 
 
-# fabric.runners.Result is not equitable OOB, let it make equitable
-def _compare_fabric_results(self: fabric.runners.Result, other) -> bool:
-    if not isinstance(other, fabric.runners.Result):
-        return False
-
-    # todo should other fields be compared? Or probably custom class should be used to store result.
-    return self.exited == other.exited \
-        and self.stdout == other.stdout \
-        and self.stderr == other.stderr
-
-
-fabric.runners.Result.__eq__ = _compare_fabric_results
-fabric.runners.Result.__ne__ = lambda self, other: not _compare_fabric_results(self, other)
+class GenericGroupResult(Mapping[str, _RESULT]):
 
+    def __init__(self, cluster: object, results: Mapping[str, _RESULT]) -> None:
+        self.cluster = cluster
+        self._result: Dict[str, _RESULT] = dict(results)
 
-class NodeGroupResult(fabric.group.GroupResult, Dict[fabric.connection.Connection, _GenericResult]):
-
-    def __init__(self, cluster, results: _HostToResult or NodeGroupResult = None) -> None:
-        super().__init__()
+    def __getitem__(self, host: str) -> _RESULT:
+        return self._result[host]
 
-        self.cluster = cluster
+    def __len__(self) -> int:
+        return len(self._result)
 
-        if results is not None:
-            for host, result in results.items():
-                if isinstance(results, NodeGroupResult):
-                    host = host.host
-                connection = cluster.nodes['all'].nodes.get(host)
-                if connection is None:
-                    raise Exception(f'Host "{host}" was not found in provided cluster object')
-                self[connection] = result
+    def __iter__(self) -> Iterator[str]:
+        return iter(self._result)
 
     def get_simple_out(self) -> str:
         if len(self) != 1:
             raise NotImplementedError("Simple output can be returned only for NodeGroupResult consisted of "
                                       "exactly one node, but %s were provided." % list(self.keys()))
 
         res = list(self.values())[0]
-        if not isinstance(res, fabric.runners.Result):
+        if not isinstance(res, RunnersResult):
             raise NotImplementedError("It does not make sense to return simple output for result of type %s"
                                       % type(res))
 
         return res.stdout
 
     def __str__(self) -> str:
-        output = ""
-        for conn, result in self.items():
+        host_outputs = []
+        for host, result in self.items():
+            output = f"{host}:"
+
+            if isinstance(result, RunnersResult):
+                output += f" code={result.repr_code()}"
+                repr_out = result.repr_out()
+                if repr_out:
+                    output += '\n\t' + repr_out.replace('\n', '\n\t')
 
-            # TODO: support print other possible exceptions
-            if isinstance(result, invoke.exceptions.UnexpectedExit):
-                result = result.result
-
-            # for now we do not know how-to print transfer result
-            if not isinstance(result, fabric.runners.Result):
-                continue
-
-            if output != "":
-                output += "\n"
-            output += "\t%s: code=%i" % (conn.host, result.exited)
-            if result.stdout:
-                output += "\n\t\tSTDOUT: %s" % result.stdout.replace("\n", "\n\t\t        ")
-            if result.stderr:
-                output += "\n\t\tSTDERR: %s" % result.stderr.replace("\n", "\n\t\t        ")
-        return output
+            # The exception may be only the last in the list. We are also sure to have at least one result per node.
+            if isinstance(result, Exception):
+                exception = errors.wrap_kme_exception(result)
+                output += '\n\t' + str(exception).replace('\n', '\n\t')
 
-    def print(self) -> None:
-        """
-        Prints debug message to log with results for each node
-        :return: None
-        """
-        self.cluster.log.debug(self)
+            host_outputs.append(output)
+
+        return "\n".join(host_outputs)
+
+    def _make_group(self, hosts: Iterable[str]) -> NodeGroup:
+        return NodeGroup(hosts, self.cluster)
 
     def get_group(self) -> NodeGroup:
         """
         Forms and returns a new group from node results
         :return: NodeGroup
         """
-        hosts = []
-        for connection in list(self.keys()):
-            hosts.append(connection.host)
-        return self.cluster.make_group(hosts)
+        return self._make_group(self.keys())
 
-    def is_any_has_code(self, code: int or str) -> bool:
+    def is_any_has_code(self, code: int) -> bool:
         """
         Returns true if some group result has an exit code equal to the given one. Exceptions and other objects in
         results will be ignored.
         :param code: The code with which the result codes will be compared
         :return: Boolean
         """
-        for conn, result in self.items():
-            if isinstance(result, fabric.runners.Result) and str(result.exited) == str(code):
-                return True
-        return False
-
-    def is_any_excepted(self) -> bool:
-        """
-        Returns true if at least one result in group is an execution
-        :return: Boolean
-        """
-        for conn, result in self.items():
-            if isinstance(result, Exception):
+        for result in self.values():
+            if isinstance(result, RunnersResult) and result.exited == code:
                 return True
         return False
 
     def is_any_failed(self) -> bool:
         """
-        Returns true if at least one result in the group finished with code 1 or failed with an exception
+        Returns true if at least one result in the group finished with non-zero code
         :return: Boolean
         """
-        return self.is_any_has_code(1) or self.is_any_excepted()
-
-    def get_excepted_nodes_list(self) -> List[fabric.connection.Connection]:
-        """
-        Returns a list of nodes connections, for which the result is an exception
-        :return: List with nodes connections
-        """
-        failed_nodes: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, Exception):
-                failed_nodes.append(conn)
-        return failed_nodes
+        return len(self.get_failed_hosts_list()) > 0
 
-    def get_excepted_nodes_group(self) -> NodeGroup:
+    def get_failed_hosts_list(self) -> List[str]:
         """
-        Forms and returns new NodeGroup of nodes, for which the result is an exception
-        :return: NodeGroup:
-        """
-        nodes_list = self.get_excepted_nodes_list()
-        return self.cluster.make_group(nodes_list)
-
-    def get_exited_nodes_list(self) -> List[fabric.connection.Connection]:
+        Returns a list of hosts whose result finished with non-zero code
+        :return: List with hosts
         """
-        Returns a list of nodes connections, for which the result is the completion of the command and the formation of
-        the Fabric Result
-        :return: List with nodes connections
-        """
-        failed_nodes: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, fabric.runners.Result):
-                failed_nodes.append(conn)
-        return failed_nodes
-
-    def get_exited_nodes_group(self) -> NodeGroup:
-        """
-        Forms and returns new NodeGroup of nodes, for which the result is the completion of the command and the
-        formation of the Fabric Result
-        :return: NodeGroup:
-        """
-        nodes_list = self.get_exited_nodes_list()
-        return self.cluster.make_group(nodes_list)
-
-    def get_failed_nodes_list(self) -> List[fabric.connection.Connection]:
-        """
-        Returns a list of nodes connections that either exited with an exception, or the exit code is equals 1
-        :return: List with nodes connections
-        """
-        failed_nodes: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, Exception) or result.exited == 1:
-                failed_nodes.append(conn)
-        return failed_nodes
+        failed_hosts: List[str] = []
+        for host, result in self.items():
+            if isinstance(result, RunnersResult) and result.failed:
+                failed_hosts.append(host)
+        return failed_hosts
 
     def get_failed_nodes_group(self) -> NodeGroup:
         """
         Forms and returns new NodeGroup of nodes that either exited with an exception, or the exit code is equals 1
         :return: NodeGroup:
         """
-        nodes_list = self.get_failed_nodes_list()
-        return self.cluster.make_group(nodes_list)
-
-    def get_nonzero_nodes_list(self) -> List[fabric.connection.Connection]:
-        """
-        Returns a list of nodes connections that exited with non-zero exit code
-        :return: List with nodes connections
-        """
-        nonzero_nodes: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, Exception) or result.exited != 0:
-                nonzero_nodes.append(conn)
-        return nonzero_nodes
-
-    def get_nonzero_nodes_group(self) -> NodeGroup:
-        """
-        Forms and returns new NodeGroup of nodes that exited with non-zero exit code
-        :return: NodeGroup:
-        """
-        nodes_list = self.get_nonzero_nodes_list()
-        return self.cluster.make_group(nodes_list)
+        nodes_list = self.get_failed_hosts_list()
+        return self._make_group(nodes_list)
 
-    def get_nodes_list_where_value_in_stdout(self, value: str) -> List[fabric.connection.Connection]:
+    def get_hosts_list_where_value_in_stdout(self, value: str) -> List[str]:
         """
-        Returns a list of node connections that contains the given string value in results stderr.
-        :param value: The string value to be found in the nodes results stderr.
-        :return: List with nodes connections
+        Returns a list of hosts that contains the given string value in results stderr.
+        :param value: The string value to be found in the nodes results stdout.
+        :return: List with hosts
         """
-        nodes_with_stderr_value: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, fabric.runners.Result) and value in result.stdout:
-                nodes_with_stderr_value.append(conn)
-        return nodes_with_stderr_value
+        hosts_with_stderr_value: List[str] = []
+        for host, result in self.items():
+            if isinstance(result, RunnersResult) and value in result.stdout:
+                hosts_with_stderr_value.append(host)
+        return hosts_with_stderr_value
 
-    def get_nodes_list_where_value_in_stderr(self, value: str) -> List[fabric.connection.Connection]:
+    def get_hosts_list_where_value_in_stderr(self, value: str) -> List[str]:
         """
-        Returns a list of node connections that contains the given string value in results stderr.
+        Returns a list of hosts that contains the given string value in results stderr.
         :param value: The string value to be found in the nodes results stderr.
-        :return: List with nodes connections
+        :return: List with hosts
         """
-        nodes_with_stderr_value: List[fabric.connection.Connection] = []
-        for conn, result in self.items():
-            if isinstance(result, fabric.runners.Result) and value in result.stderr:
-                nodes_with_stderr_value.append(conn)
-        return nodes_with_stderr_value
+        hosts_with_stderr_value: List[str] = []
+        for host, result in self.items():
+            if isinstance(result, RunnersResult) and value in result.stderr:
+                hosts_with_stderr_value.append(host)
+        return hosts_with_stderr_value
 
     def get_nodes_group_where_value_in_stdout(self, value: str) -> NodeGroup:
         """
         Forms and returns new NodeGroup of nodes that contains the given string value in results stdout.
         :param value: The string value to be found in the nodes results stdout.
         :return: NodeGroup
         """
-        nodes_list = self.get_nodes_list_where_value_in_stdout(value)
-        return self.cluster.make_group(nodes_list)
+        nodes_list = self.get_hosts_list_where_value_in_stdout(value)
+        return self._make_group(nodes_list)
 
     def get_nodes_group_where_value_in_stderr(self, value: str) -> NodeGroup:
         """
         Forms and returns new NodeGroup of nodes that contains the given string value in results stderr.
         :param value: The string value to be found in the nodes results stderr.
         :return: NodeGroup
         """
-        nodes_list = self.get_nodes_list_where_value_in_stderr(value)
-        return self.cluster.make_group(nodes_list)
+        nodes_list = self.get_hosts_list_where_value_in_stderr(value)
+        return self._make_group(nodes_list)
 
     def stdout_contains(self, value: str) -> bool:
         """
         Checks for the presence of the given string in all results stdout.
         :param value: The string value to be found in the nodes results stdout.
         :return: true if string presented
         """
-        return len(self.get_nodes_list_where_value_in_stdout(value)) > 0
+        return len(self.get_hosts_list_where_value_in_stdout(value)) > 0
 
     def stderr_contains(self, value: str) -> bool:
         """
         Checks for the presence of the given string in all results stderr.
         :param value: The string value to be found in the nodes results stderr.
         :return: true if string presented
         """
-        return len(self.get_nodes_list_where_value_in_stderr(value)) > 0
+        return len(self.get_hosts_list_where_value_in_stderr(value)) > 0
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: object) -> bool:
         if self is other:
             return True
 
-        if not isinstance(other, NodeGroupResult):
+        if not isinstance(other, GenericGroupResult):
             return False
 
         if len(self) != len(other):
             return False
 
-        for conn, result in self.items():
-            compared_result = other.get(conn)
+        for host, result in self.items():
+            compared_result = other.get(host)
             if compared_result is None:
                 return False
 
-            if not isinstance(result, fabric.runners.Result) or not isinstance(compared_result, fabric.runners.Result):
-                raise NotImplementedError('Currently only instances of fabric.runners.Result can be compared')
+            if not isinstance(result, RunnersResult) or not isinstance(compared_result, RunnersResult):
+                raise NotImplementedError('Currently only instances of RunnersResult can be compared')
 
             if result != compared_result:
                 return False
 
         return True
 
-    def __ne__(self, other) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not self == other
 
 
-def _handle_internal_logging(fn: callable) -> callable:
-    """
-    Method is a decorator that handles internal streaming of output (hide=False) of fabric (invoke).
-    Note! This decorator should be the outermost.
-
-    :param fn: Origin function to apply annotation to
-    :return: Validation wrapper function
-    """
-    def do(self: 'NodeGroup', *args, logging_stream_level: int = None, **kwargs):
-        if logging_stream_level is not None and 'hide' in kwargs:
-            raise ValueError("'hide' and 'logging_stream_level' should not be combined")
-
-        logger = self.cluster.log
-        if logging_stream_level is not None:
-            # We want to stream output immediately to logging framework, thus not hide.
-            kwargs['hide'] = False
-
-            caller = log.caller_info(logger)
-            out = log.LoggerWriter(logger, logging_stream_level, caller, '[remote] ')
-            err = log.LoggerWriter(logger, logging_stream_level, caller, '[stderr] ')
-
-            return fn(self, *args, out_stream=out, err_stream=err, **kwargs)
-
-        results = None
-        try:
-            results = fn(self, *args, **kwargs)
-            return results
-        except fabric.group.GroupException as e:
-            results = e.result
-            raise
-        finally:
-            # if hide is False, we already logged only to stdout, and should log to other handlers.
-            if results is not None and not kwargs.get('hide', True):
-                logger.debug(results, extra={'ignore_stdout': True})
+class NodeGroupResult(GenericGroupResult[GenericResult]):
+    pass
+
+
+class RunnersGroupResult(GenericGroupResult[RunnersResult]):
+    pass
+
+
+class CollectorCallback(Callback):
+    def __init__(self, cluster: object) -> None:
+        self.cluster = cluster
+        self.results: Dict[str, List[RunnersResult]] = {}
+        """
+        List of collected results for each host.
+        If all commands are exited for the particular host, the number and order of results
+        correspond to the number and order of the queued commands,
+        for which the given callback was requested.
+        """
+        self._result: Optional[RunnersGroupResult] = None
+
+    def accept(self, host: str, token: Token, result: RunnersResult) -> None:
+        self.results.setdefault(host, []).append(result)
+        self._result = None
+
+    @property
+    def result(self) -> RunnersGroupResult:
+        """
+        Merges the collected `results` into the single RunnersGroupResult instance.
+        This can be useful to check merged output of the commands.
+
+        Note that if the result of more than one command is merged,
+        one SHOULD NOT use `RunnersResult.exited` and `RunnersResult.command`,
+        as the exit code and command of few commands are undefined.
+
+        :return: merged RunnersGroupResult instance.
+        """
+        if self._result is None:
+            self._result = RunnersGroupResult(
+                self.cluster,
+                {host: RunnersResult.merge(results) for host, results in self.results.items()}
+            )
+
+        return self._result
 
-    return do
 
+RunResult = Union[RunnersGroupResult, Token]
+GROUP_RUN_TYPE = TypeVar('GROUP_RUN_TYPE', bound=RunResult, covariant=True)
+GROUP_SELF = TypeVar('GROUP_SELF', bound='AbstractGroup[Union[RunnersGroupResult, Token]]')
 
-class NodeGroup:
 
-    def __init__(self, connections: Connections, cluster):
+class AbstractGroup(Generic[GROUP_RUN_TYPE], ABC):
+    def __init__(self, ips: Iterable[Union[str, GROUP_SELF]], cluster: object):
         from kubemarine.core.cluster import KubernetesCluster
 
-        self.cluster: KubernetesCluster = cluster
-        self.nodes = connections
+        self.cluster = cast(KubernetesCluster, cluster)
+        self.nodes: Set[str] = set()
+        for ip in ips:
+            if isinstance(ip, self.__class__):
+                for host in ip.nodes:
+                    self.nodes.add(host)
+            elif isinstance(ip, str):
+                self.nodes.add(ip)
+            else:
+                raise Exception('Unsupported connection object type')
+
+    @abstractmethod
+    def _make_group(self: GROUP_SELF, ips: Iterable[Union[str, GROUP_SELF]]) -> GROUP_SELF:
+        pass
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if self is other:
             return True
 
-        if not isinstance(other, NodeGroup):
-            return False
-
-        if self.cluster != other.cluster:
+        if not isinstance(other, self.__class__):
             return False
 
-        if len(self.nodes.keys()) != len(other.nodes.keys()):
-            return False
+        return self.nodes == other.nodes
 
-        for host, connection in self.nodes.items():
-            other_host_conn = other.nodes.get(host)
-            if other_host_conn is None:
-                return False
-            if other_host_conn != connection:
-                return False
-
-        return True
-
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return not self == other
 
-    def __hash__(self):
-        # TODO: include cluster object and real connections into hash value
-        nodes_addresses = tuple(self.nodes.keys())
-        return hash(nodes_addresses)
-
-    def _make_result(self, results: _HostToResult) -> NodeGroupResult:
-        group_result = NodeGroupResult(self.cluster, results)
-        return group_result
-
-    def _make_result_or_fail(self, results: _HostToResult,
-                             failure_criteria: Callable[[str, _GenericResult], bool]) -> NodeGroupResult:
-        failed_hosts = [host for host, result in results.items() if failure_criteria(host, result)]
-        group_result = self._make_result(results)
-
-        if failed_hosts:
-            raise fabric.group.GroupException(group_result)
-
-        return group_result
-
-    @_handle_internal_logging
-    def run(self, *args, **kwargs) -> Union[NodeGroupResult, int]:
-        return self.do("run", *args, **kwargs)
-
-    @_handle_internal_logging
-    def sudo(self, *args, **kwargs) -> Union[NodeGroupResult, int]:
-        return self.do("sudo", *args, **kwargs)
-
-    def put(self, local_file: Union[io.StringIO, str], remote_file: str, **kwargs):
+    def run(self, command: str,
+            warn: bool = False, hide: bool = True,
+            env: Dict[str, str] = None, timeout: int = None,
+            callback: Callback = None) -> GROUP_RUN_TYPE:
+        caller: Optional[Dict[str, object]] = None
+        if not hide:
+            # fetching of the caller info should be at the earliest point
+            caller = log.caller_info(self.cluster.log)
+        return self._run("run", command, caller,
+                         warn=warn, hide=hide, env=env, timeout=timeout, callback=callback)
+
+    def sudo(self, command: str,
+             warn: bool = False, hide: bool = True,
+             env: Dict[str, str] = None, timeout: int = None,
+             callback: Callback = None) -> GROUP_RUN_TYPE:
+        caller: Optional[Dict[str, object]] = None
+        if not hide:
+            # fetching of the caller info should be at the earliest point
+            caller = log.caller_info(self.cluster.log)
+        return self._run("sudo", command, caller,
+                         warn=warn, hide=hide, env=env, timeout=timeout, callback=callback)
+
+    @abstractmethod
+    def _run(self, do_type: str, command: str, caller: Optional[Dict[str, object]],
+             **kwargs: Any) -> GROUP_RUN_TYPE:
+        pass
+
+    @abstractmethod
+    def get(self, remote_file: str, local_file: str) -> None:
+        pass
+
+    def put(self, local_file: Union[io.StringIO, str], remote_file: str,
+            backup: bool = False, sudo: bool = False,
+            mkdir: bool = False, immutable: bool = False) -> None:
         if isinstance(local_file, io.StringIO):
-            self.cluster.log.verbose("Text is being transferred to remote file \"%s\" on nodes %s with options %s"
-                                     % (remote_file, list(self.nodes.keys()), kwargs))
+            self.cluster.log.verbose("Text is being transferred to remote file \"%s\" on nodes %s"
+                                     % (remote_file, list(self.nodes)))
             # This is a W/A to avoid https://github.com/paramiko/paramiko/issues/1133
             # if text contains non-ASCII characters.
             # Use the same encoding as paramiko uses, see paramiko/file.py/BufferedFile.write()
-            bytes_stream = io.BytesIO(local_file.getvalue().encode('utf-8'))
-            self._put(bytes_stream, remote_file, **kwargs)
-            return
 
-        self.cluster.log.verbose("Local file \"%s\" is being transferred to remote file \"%s\" on nodes %s with options %s"
-                                 % (local_file, remote_file, list(self.nodes.keys()), kwargs))
+            local_stream: Union[io.BytesIO, str] = io.BytesIO(local_file.getvalue().encode('utf-8'))
+            group_to_upload = self
+        else:
+            if not os.path.isfile(local_file):
+                raise Exception(f"File {local_file} does not exist")
 
-        self.cluster.log.verbose('File size: %s' % os.path.getsize(local_file))
-        local_file_hash = self.get_local_file_sha1(local_file)
-        self.cluster.log.verbose('Local file hash: %s' % local_file_hash)
-        remote_file_hashes = self.get_remote_file_sha1(remote_file)
-        self.cluster.log.verbose('Remote file hashes: %s' % remote_file_hashes)
-
-        hosts_to_upload = []
-        for remote_ip, remote_file_hash in remote_file_hashes.items():
-            if remote_file_hash != local_file_hash:
-                self.cluster.log.verbose('Local and remote hashes does not match on node \'%s\' %s %s'
-                                         % (remote_ip, local_file_hash, remote_file_hash))
-                hosts_to_upload.append(remote_ip)
-        if not hosts_to_upload:
-            self.cluster.log.verbose('Local and remote hashes are equal on all nodes, no transmission required')
-            return
+            self.cluster.log.verbose("Local file \"%s\" is being transferred to remote file \"%s\" on nodes %s"
+                                     % (local_file, remote_file, list(self.nodes)))
 
-        group_to_upload = self.cluster.make_group(hosts_to_upload)
+            self.cluster.log.verbose('File size: %s' % os.path.getsize(local_file))
+            eager_group = self.cluster.make_group(self.nodes)
+            local_file_hash = eager_group.get_local_file_sha1(local_file)
+            self.cluster.log.verbose('Local file hash: %s' % local_file_hash)
+            remote_file_hashes = eager_group.get_remote_file_sha1(remote_file)
+            self.cluster.log.verbose('Remote file hashes: %s' % remote_file_hashes)
+
+            hosts_to_upload = []
+            for remote_ip, remote_file_hash in remote_file_hashes.items():
+                if remote_file_hash != local_file_hash:
+                    self.cluster.log.verbose('Local and remote hashes does not match on node \'%s\' %s %s'
+                                             % (remote_ip, local_file_hash, remote_file_hash))
+                    hosts_to_upload.append(remote_ip)
+            if not hosts_to_upload:
+                self.cluster.log.verbose('Local and remote hashes are equal on all nodes, no transmission required')
+                return
 
-        with open(local_file, "rb") as local_stream:
-            group_to_upload._put(local_stream, remote_file, **kwargs)
+            local_stream = local_file
+            group_to_upload = self._make_group(hosts_to_upload)
 
-    def _put(self, local_stream: IO, remote_file: str, **kwargs):
-        hide = kwargs.pop("hide", True) is True
-        sudo = kwargs.pop("sudo", False) is True
-        backup = kwargs.pop("backup", False) is True
-        mkdir = kwargs.pop("mkdir", False) is True
-        immutable = kwargs.pop("immutable", False) is True
-
-        # for unknown reason fabric v2 can't put async
-        # Let's remember passed value, which by default is True, and make it False forcibly.
-        is_async = kwargs.pop("is_async", True) is not False
-        kwargs["is_async"] = False
+        group_to_upload._put_with_mv(local_stream, remote_file,
+                                     backup=backup, sudo=sudo, mkdir=mkdir, immutable=immutable)
+
+    def _put_with_mv(self, local_stream: Union[io.BytesIO, str], remote_file: str,
+                     backup: bool, sudo: bool, mkdir: bool, immutable: bool) -> None:
 
         if sudo:
             self.cluster.log.verbose('A sudoer upload required')
 
         if backup:
             self.cluster.log.verbose('File \"%s\" backup required' % remote_file)
 
         if mkdir:
             self.cluster.log.verbose('A parent directory will be created')
 
         if immutable:
             self.cluster.log.verbose('File \"%s\" immutable set required' % remote_file)
 
-        if not sudo and not backup and not immutable:
-            # no additional commands execution is required - directly upload file
-            self.do("put", local_stream, remote_file, **kwargs)
-            return
+        advanced_move_required = sudo or backup or immutable
+        temp_filepath = remote_file
 
-        # for unknown reason fabric v2 can't put as sudo, and we should use WA via mv
-        # also, if we need to backup the file first, then we also have to upload file to tmp first
+        if advanced_move_required:
+            # for unknown reason fabric v2 can't put as sudo, and we should use WA via mv
+            # also, if we need to backup the file first, then we also have to upload file to tmp first
 
-        temp_filepath = "/tmp/%s" % uuid.uuid4().hex
-        self.cluster.log.verbose("Uploading to temporary file '%s'..." % temp_filepath)
-        self.do("put", local_stream, temp_filepath, **kwargs)
+            temp_filepath = "/tmp/%s" % uuid.uuid4().hex
+            self.cluster.log.verbose("Uploading to temporary file '%s'..." % temp_filepath)
+
+        self._put(local_stream, temp_filepath)
+
+        if not advanced_move_required:
+            return
 
         self.cluster.log.verbose("Moving temporary file '%s' to '%s'..." % (temp_filepath, remote_file))
 
         if sudo:
             mv_command = "sudo chown root:root %s && sudo mv -f %s %s" % (temp_filepath, temp_filepath, remote_file)
         else:
             mv_command = "mv -f %s %s" % (temp_filepath, remote_file)
@@ -503,309 +426,76 @@
 
         if immutable:
             if sudo:
                 mv_command = "sudo chattr -i %s; %s; sudo chattr +i %s" % (remote_file, mv_command, remote_file)
             else:
                 mv_command = "chattr -i %s; %s; chattr +i %s" % (remote_file, mv_command, remote_file)
 
-        kwargs["hide"] = hide
-        kwargs["is_async"] = is_async
-        self.sudo(mv_command, **kwargs)
-
-    def get(self, *args, **kwargs):
-        return self.do("get", *args, **kwargs)
-
-    def do(self, do_type, *args, **kwargs) -> Union[NodeGroupResult, int]:
-        raw_results = self._do_with_wa(do_type, *args, **kwargs)
-        if isinstance(raw_results, int):
-            return raw_results
-        return self._make_result_or_fail(raw_results, lambda host, result: isinstance(result, Exception))
-
-    def _do_with_wa(self, do_type, *args, **kwargs) -> Union[_HostToResult, int]:
-        # by default all code is async, but can be set False forcibly
-        is_async = kwargs.pop("is_async", True) is not False
-
-        left_nodes = self.nodes
-        retry = 0
-        results: _HostToResult = {}
-        while True:
-            retry += 1
-
-            result = self._do(do_type, left_nodes, is_async, *args, **kwargs)
-            if isinstance(result, int):
-                return result
-
-            results.update(result)
-            left_nodes = {host: left_nodes[host] for host, result in results.items() if isinstance(result, Exception)}
-
-            if not left_nodes or retry >= self.cluster.globals['workaround']['retries'] \
-                    or not self._try_workaround(results, left_nodes):
-                break
+        self.sudo(mv_command)
 
-            self.cluster.log.verbose('Retrying #%s...' % retry)
-            time.sleep(self.cluster.globals['workaround']['delay_period'])
+    @abstractmethod
+    def _put(self, local_stream: Union[io.BytesIO, str], remote_file: str) -> None:
+        pass
+
+    def _unsafe_make_runners_result(self, host_results: HostToResult) -> RunnersGroupResult:
+        return RunnersGroupResult(self.cluster,
+                                  {host: cast(RunnersResult, result) for host, result in host_results.items()})
+
+    def call(self, action: Callable[..., _T], **kwargs: object) -> _T:
+        func = cast(FunctionType, action)
+        callable_path = "%s.%s" % (func.__module__, func.__name__)
+        self.cluster.log.debug("Running %s: " % callable_path)
+        result = action(self, **kwargs)
+        if result is not None:
+            self.cluster.log.debug(result)
 
-        return results
-
-    def _try_workaround(self, results: _HostToResult, failed_nodes: Connections) -> bool:
-        not_booted = []
-
-        for host in failed_nodes.keys():
-            exception = results[host]
-            if isinstance(exception, UnexpectedExit):
-                exception_message = str(exception.result)
-            else:
-                exception_message = str(exception)
-
-            if self.is_allowed_etcd_exception(exception_message):
-                self.cluster.log.verbose("Detected ETCD problem at %s, need retry: %s" % (host, exception_message))
-            elif self.is_allowed_kubernetes_exception(exception_message):
-                self.cluster.log.verbose("Detected kubernetes problem at %s, need retry: %s" % (host, exception_message))
-            elif self.is_allowed_connection_exception(exception_message):
-                self.cluster.log.verbose("Detected connection exception at %s, will try to reconnect to node. Exception: %s"
-                                         % (host, exception_message))
-                not_booted.append(host)
-            else:
-                self.cluster.log.verbose("Detected unavoidable exception at %s, trying to solve automatically: %s"
-                                         % (host, exception_message))
-                return False
-
-        # if there are not booted nodes, but we succeeded to wait for at least one is booted, we can continue execution
-        if not_booted and self.cluster.make_group(not_booted).wait_and_get_active_nodes().is_empty():
-            return False
-
-        return True
-
-    def _do(self, do_type: str, nodes: Connections, is_async, *args, **kwargs) -> Union[_HostToResult, int]:
-
-        if do_type in ["run", "sudo"]:
-            # by default fabric will print all output from nodes
-            # let's disable this feature if it was not forcibly defined
-            if kwargs.get("hide") is None:
-                kwargs['hide'] = True
-
-            if kwargs.get("timeout", None) is None:
-                kwargs["timeout"] = self.cluster.globals['nodes']['command_execution']['timeout']
-
-        execution_timeout = kwargs.get("timeout", None)
-
-        results = {}
-
-        if not nodes:
-            self.cluster.log.verbose('No nodes to perform %s %s with options: %s' % (do_type, args, kwargs))
-            return results
-
-        self.cluster.log.verbose('Performing %s %s on nodes %s with options: %s' % (do_type, args, list(nodes.keys()), kwargs))
-
-        executor = RemoteExecutor(self.cluster, lazy=False, parallel=is_async, timeout=execution_timeout)
-        results = executor.queue(nodes, (do_type, args, kwargs))
-
-        if not isinstance(results, int):
-            simplified_results = {}
-            for cnx, conn_results in results.items():
-                raw_results = list(conn_results.values())
-                if len(raw_results) > 1:
-                    raise Exception('Unexpected condition: not supported multiple results with non-lazy GRE')
-                simplified_results[cnx.host] = raw_results[0]
-            return simplified_results
-
-        return results
-
-    def call(self, action, **kwargs):
-        return self.call_batch([action], **{"%s.%s" % (action.__module__, action.__name__): kwargs})
-
-    def call_batch(self, actions, **kwargs):
-        results = {}
+        return result
 
+    def call_batch(self: GROUP_SELF, actions: List[Callable[[GROUP_SELF], Any]]) -> None:
         for action in actions:
+            self.call(action)
 
-            callable_path = "%s.%s" % (action.__module__, action.__name__)
-            self.cluster.log.debug("Running %s: " % callable_path)
-
-            action_kwargs = {}
-            if kwargs.get(callable_path) is not None:
-                action_kwargs = kwargs[callable_path]
-
-            results[action] = action(self, **action_kwargs)
-            if results[action] is not None:
-                self.cluster.log.debug(results[action])
-
-        return results
-
-    def get_online_nodes(self, online: bool) -> 'NodeGroup':
-        online = [host for host, node_context in self.cluster.context['nodes'].items()
-                  if node_context['access']['online'] == online]
-        return self.cluster.make_group(online).intersection_group(self)
+    def get_online_nodes(self: GROUP_SELF, online: bool) -> GROUP_SELF:
+        online_hosts = [host for host, node_context in self.cluster.context['nodes'].items()
+                        if node_context['access']['online'] == online]
+        return self._make_group(online_hosts).intersection_group(self)
 
-    def get_accessible_nodes(self) -> 'NodeGroup':
+    def get_accessible_nodes(self: GROUP_SELF) -> GROUP_SELF:
         accessible = [host for host, node_context in self.cluster.context['nodes'].items()
                       if node_context['access']['accessible']]
-        return self.cluster.make_group(accessible).intersection_group(self)
+        return self._make_group(accessible).intersection_group(self)
 
-    def get_sudo_nodes(self) -> 'NodeGroup':
+    def get_sudo_nodes(self: GROUP_SELF) -> GROUP_SELF:
         sudo = [host for host, node_context in self.cluster.context['nodes'].items()
                 if node_context['access']['sudo'] != "No"]
-        return self.cluster.make_group(sudo).intersection_group(self)
-
-    def wait_for_reboot(self, initial_boot_history: NodeGroupResult, timeout=None) -> NodeGroupResult:
-        results = self._await_rebooted_nodes(timeout, initial_boot_history=initial_boot_history)
-        return self._make_result_or_fail(
-            results,
-            lambda host, result: isinstance(result, Exception) or result == initial_boot_history.get(self.nodes[host])
-        )
-
-    def wait_and_get_boot_history(self, timeout=None) -> NodeGroupResult:
-        results = self._await_rebooted_nodes(timeout)
-        return self._make_result_or_fail(results, lambda _, r: isinstance(r, Exception))
-
-    def wait_and_get_active_nodes(self, timeout=None) -> 'NodeGroup':
-        results = self._await_rebooted_nodes(timeout)
-        not_booted = [host for host, result in results.items() if isinstance(result, Exception)]
-        return self.exclude_group(self.cluster.make_group(not_booted))
-
-    def _await_rebooted_nodes(self, timeout=None, initial_boot_history: NodeGroupResult = None) -> _HostToResult:
-
-        if timeout is None:
-            timeout = int(self.cluster.inventory['globals']['nodes']['boot']['timeout'])
-
-        delay_period = self.cluster.globals['nodes']['boot']['defaults']['delay_period']
-
-        if initial_boot_history:
-            self.cluster.log.verbose("Initial boot history:\n%s" % initial_boot_history)
-        else:
-            initial_boot_history = NodeGroupResult(self.cluster)
-
-        left_nodes = self.nodes
-        results: _HostToResult = {}
-        time_start = datetime.now()
-
-        self.cluster.log.verbose("Trying to connect to nodes, timeout is %s seconds..." % timeout)
-
-        # each connection has timeout, so the only we need is to repeat connecting attempts
-        # during specified number of seconds
-        while True:
-            attempt_time_start = datetime.now()
-            self.disconnect(list(left_nodes.keys()))
-
-            self.cluster.log.verbose("Attempting to connect to nodes...")
-            # this should be invoked without explicit timeout, and relied on fabric Connection timeout instead.
-            results.update(self._do_nopasswd(left_nodes, "last reboot"))
-            left_nodes = {host: left_nodes[host] for host, result in results.items()
-                          if (isinstance(result, Exception)
-                              # Something is wrong with sudo access. Node is active.
-                              and not NodeGroup.is_require_nopasswd_exception(result))
-                          or (not isinstance(result, Exception)
-                              and result == initial_boot_history.get(self.nodes[host]))}
-
-            waited = (datetime.now() - time_start).total_seconds()
-
-            if not left_nodes or waited >= timeout:
-                break
-
-            for host, exc in results.items():
-                if isinstance(exc, Exception) and not self.is_allowed_connection_exception(str(exc)):
-                    self.cluster.log.verbose("Unexpected exception at %s, node is considered as not booted: %s"
-                                             % (host, str(exc)))
-
-            self.cluster.log.verbose("Nodes %s are not ready yet, remaining time to wait %i"
-                                     % (list(left_nodes.keys()), timeout - waited))
-
-            attempt_time = (datetime.now() - attempt_time_start).total_seconds()
-            if attempt_time < delay_period:
-                time.sleep(delay_period - attempt_time)
-
-        if left_nodes:
-            self.cluster.log.verbose("Failed to wait for boot of nodes %s" % list(left_nodes.keys()))
-        else:
-            self.cluster.log.verbose("All nodes are online now")
-
-        return results
-
-    def _do_nopasswd(self, left_nodes: Connections, command: str):
-        prompt = '[sudo] password: '
-
-        class NoPasswdResponder(invoke.Responder):
-            def __init__(self):
-                super().__init__(re.escape(prompt), None)
-
-            def submit(self, stream):
-                if self.pattern_matches(stream, self.pattern, "index"):
-                    # If user appears to be not a NOPASSWD sudoer, "sudo" suggests to write password.
-                    # This is a W/A to handle the situation in a docker container without pseudo-TTY (no -t option)
-                    # As long as we require NOPASSWD, we can just fail immediately in such cases.
-                    raise invoke.exceptions.ResponseNotAccepted("The user should be a NOPASSWD sudoer")
-
-                # The only acceptable situation, responder does nothing.
-                return []
-
-        # Currently only NOPASSWD sudoers are supported.
-        # Thus, running of connection.sudo("something") should be equal to connection.run("sudo something")
-        return self._do("run", left_nodes, True, f"sudo -S -p '{prompt}' {command}",
-                        watchers=[NoPasswdResponder()])
-
-    @staticmethod
-    def is_require_nopasswd_exception(exc: Exception):
-        return isinstance(exc, invoke.exceptions.Failure) \
-               and isinstance(exc.reason, invoke.exceptions.ResponseNotAccepted)
-
-    def is_allowed_connection_exception(self, exception_message):
-        exception_message = exception_message.partition('\n')[0]
-        for known_exception_message in self.cluster.globals['connection']['bad_connection_exceptions']:
-            if known_exception_message in exception_message:
-                return True
+        return self._make_group(sudo).intersection_group(self)
 
-        return False
-
-    def is_allowed_etcd_exception(self, exception_message):
-        for known_exception_message in self.cluster.globals['etcd']['temporary_exceptions']:
-            if known_exception_message in exception_message:
-                return True
+    def get_ordered_members_list(self: GROUP_SELF, apply_filter: GroupFilter = None) -> List[GROUP_SELF]:
+        nodes = self.get_ordered_members_configs_list(apply_filter)
+        return [self._make_group([node['connect_to']]) for node in nodes]
 
-        return False
-
-    def is_allowed_kubernetes_exception(self, exception_message):
-        for known_exception_message in self.cluster.globals['kubernetes']['temporary_exceptions']:
-            if known_exception_message in exception_message:
-                return True
-
-        return False
-
-    def get_local_file_sha1(self, filename: str) -> str:
-        return utils.get_local_file_sha1(filename)
-
-    def get_remote_file_sha1(self, filename: str) -> Dict[str, str]:
-        results = self._do_with_wa("sudo", "openssl sha1 %s" % filename, warn=True)
-        self._make_result_or_fail(results, lambda h, r: isinstance(r, Exception))
-
-        return {host: result.stdout.split("= ")[1].strip() if result.stdout else None
-                for host, result in results.items()}
-
-    def get_ordered_members_list(self, provide_node_configs=False, apply_filter=None) \
-            -> List[Union[dict, 'NodeGroup']]:
-
-        if apply_filter is None:
-            apply_filter = {}
+    def get_ordered_members_configs_list(self, apply_filter: GroupFilter = None) -> List[NodeConfig]:
 
         result = []
         # we have to iterate strictly in order which was defined by user in config-file
         for node in self.cluster.inventory['nodes']:
             # is iterable node from inventory is part of current NodeGroup?
-            if node['connect_to'] in self.nodes.keys():
+            if node['connect_to'] in self.nodes:
 
                 # apply filters
                 suitable = True
                 if apply_filter is not None:
                     if callable(apply_filter):
                         if not apply_filter(node):
                             suitable = False
                     else:
                         # here intentionally there is no way to filter by values in lists field,
                         # for this you need to use custom functions.
                         # Current solution implemented in this way because the filtering strategy is
-                        # unclear - do I need to include when everything matches or is partial partial matching enough?
+                        # unclear - do I need to include when everything matches or is partial matching enough?
                         for key, value in apply_filter.items():
                             if node.get(key) is None:
                                 suitable = False
                                 break
                             if isinstance(value, list):
                                 if node[key] not in value:
                                     suitable = False
@@ -813,169 +503,380 @@
                             # elif should definitely be here, not if
                             elif node[key] != value:
                                 suitable = False
                                 break
 
                 # if not filtered
                 if suitable:
-                    if provide_node_configs:
-                        result.append(node)
-                    else:
-                        result.append(node['connection'])
+                    result.append(node)
 
         return result
 
-    def get_member(self, number, provide_node_configs=False, apply_filter=None):
-        results = self.get_ordered_members_list(provide_node_configs=provide_node_configs, apply_filter=apply_filter)
-
+    def get_first_member(self: GROUP_SELF, apply_filter: GroupFilter = None) -> GROUP_SELF:
+        results = self.get_ordered_members_list(apply_filter)
         if not results:
-            return None
-
-        return results[number]
+            raise Exception("Failed to find first group member by the given criteria")
+        return results[0]
 
-    def get_first_member(self, provide_node_configs=False, apply_filter=None):
-        return self.get_member(0, provide_node_configs=provide_node_configs, apply_filter=apply_filter)
-
-    def get_last_member(self, provide_node_configs=False, apply_filter=None):
-        return self.get_member(-1, provide_node_configs=provide_node_configs, apply_filter=apply_filter)
-
-    def get_any_member(self, provide_node_configs=False, apply_filter=None):
-        member = random.choice(self.get_ordered_members_list(provide_node_configs=provide_node_configs,
-                                                             apply_filter=apply_filter))
-        if isinstance(member, NodeGroup):
-            # to avoid "Selected node <kubemarine.core.group.NodeGroup object at 0x7f925625d070>" writing to log,
-            # let's get node ip from selected member and pass to it to log
-            member_str = str(list(member.nodes.keys())[0])
-        else:
-            member_str = str(member)
-        self.cluster.log.verbose(f'Selected node {member_str}')
+    def get_any_member(self: GROUP_SELF, apply_filter: GroupFilter = None) -> GROUP_SELF:
+        member: GROUP_SELF = random.choice(self.get_ordered_members_list(apply_filter))
+        self.cluster.log.verbose(f'Selected node {member.get_host()}')
         return member
 
-    def get_member_by_name(self, name, provide_node_configs=False):
-        return self.get_first_member(provide_node_configs=provide_node_configs, apply_filter={"name": name})
+    def get_member_by_name(self: GROUP_SELF, name: str) -> GROUP_SELF:
+        return self.get_first_member({"name": name})
 
-    def new_group(self, apply_filter=None):
-        return self.cluster.make_group(self.get_ordered_members_list(apply_filter=apply_filter))
+    def new_group(self: GROUP_SELF, apply_filter: GroupFilter = None) -> GROUP_SELF:
+        return self._make_group(self.get_ordered_members_list(apply_filter))
 
-    def include_group(self, group):
-        if group is None:
-            return self
-
-        ips = list(self.nodes.keys()) + list(group.nodes.keys())
-        return self.cluster.make_group(list(dict.fromkeys(ips)))
-
-    def exclude_group(self, group):
-        if group is None:
-            return self
-
-        ips = list(set(self.nodes.keys()) - set(group.nodes.keys()))
-        return self.cluster.make_group(list(dict.fromkeys(ips)))
-
-    def intersection_group(self, group):
-        if group is None:
-            return self.cluster.make_group([])
-
-        ips = list(set(self.nodes.keys()).intersection(set(group.nodes.keys())))
-        return self.cluster.make_group(list(dict.fromkeys(ips)))
-
-    def disconnect(self, hosts: List[str] = None):
-        for host, cxn in self.nodes.items():
-            if host in (hosts or self.nodes.keys()):
-                self.cluster.log.verbose('Disconnected session with %s' % host)
-                cxn.close()
-                cxn._sftp = None
+    def include_group(self: GROUP_SELF, group: GROUP_SELF) -> GROUP_SELF:
+        ips = self.nodes.union(group.nodes)
+        return self._make_group(ips)
+
+    def exclude_group(self: GROUP_SELF, group: GROUP_SELF) -> GROUP_SELF:
+        ips = self.nodes - group.nodes
+        return self._make_group(ips)
+
+    def intersection_group(self: GROUP_SELF, group: GROUP_SELF) -> GROUP_SELF:
+        ips = self.nodes.intersection(group.nodes)
+        return self._make_group(ips)
 
     def get_nodes_names(self) -> List[str]:
         result = []
-        members = self.get_ordered_members_list(provide_node_configs=True)
+        members = self.get_ordered_members_configs_list()
         for node in members:
             result.append(node['name'])
         return result
 
     def get_node_name(self) -> str:
         if len(self.nodes) != 1:
             raise Exception("Cannot get the only name from not a single node")
 
-        return self.get_first_member(provide_node_configs=True)['name']
+        return self.get_nodes_names()[0]
 
     def get_hosts(self) -> List[str]:
-        members = self.get_ordered_members_list(provide_node_configs=True)
-        return [node['connect_to'] for node in members]
+        members = self.get_ordered_members_list()
+        return [node.get_host() for node in members]
 
-    def get_host(self):
+    def get_host(self) -> str:
         if len(self.nodes) != 1:
             raise Exception("Cannot get the only host from not a single node")
 
-        return list(self.nodes.keys())[0]
+        return next(iter(self.nodes))
+
+    def get_config(self) -> NodeConfig:
+        if len(self.nodes) != 1:
+            raise Exception("Cannot get the only node config from not a single node")
+
+        return self.get_ordered_members_configs_list()[0]
 
     def is_empty(self) -> bool:
         return not self.nodes
 
-    def has_node(self, node_name):
-        return self.get_first_member(apply_filter={"name": node_name}) is not None
+    def has_node(self, node_name: str) -> bool:
+        return node_name in self.get_nodes_names()
 
-    def get_new_nodes(self) -> NodeGroup:
-        return self.intersection_group(self.cluster.nodes.get('add_node'))
+    def get_new_nodes(self: GROUP_SELF) -> GROUP_SELF:
+        return self.new_group(lambda node: 'add_node' in node['roles'])
 
-    def get_new_nodes_or_self(self) -> NodeGroup:
+    def get_new_nodes_or_self(self: GROUP_SELF) -> GROUP_SELF:
         new_nodes = self.get_new_nodes()
         if not new_nodes.is_empty():
             return new_nodes
         return self
 
-    def get_nodes_for_removal(self) -> NodeGroup:
-        return self.intersection_group(self.cluster.nodes.get('remove_node'))
+    def get_nodes_for_removal(self: GROUP_SELF) -> GROUP_SELF:
+        return self.new_group(lambda node: 'remove_node' in node['roles'])
 
-    def get_nodes_for_removal_or_self(self) -> NodeGroup:
-        nodes_for_removal = self.get_nodes_for_removal()
-        if not nodes_for_removal.is_empty():
-            return nodes_for_removal
-        return self
-
-    def get_changed_nodes(self) -> NodeGroup:
+    def get_changed_nodes(self: GROUP_SELF) -> GROUP_SELF:
         return self.get_new_nodes().include_group(self.get_nodes_for_removal())
 
-    def get_unchanged_nodes(self) -> NodeGroup:
+    def get_unchanged_nodes(self: GROUP_SELF) -> GROUP_SELF:
         return self.exclude_group(self.get_changed_nodes())
 
-    def get_final_nodes(self) -> NodeGroup:
-        return self.exclude_group(self.cluster.nodes.get('remove_node'))
+    def get_final_nodes(self: GROUP_SELF) -> GROUP_SELF:
+        return self.new_group(lambda node: 'remove_node' not in node['roles'])
 
-    def get_initial_nodes(self) -> NodeGroup:
-        return self.exclude_group(self.cluster.nodes.get('add_node'))
+    def get_initial_nodes(self: GROUP_SELF) -> GROUP_SELF:
+        return self.new_group(lambda node: 'add_node' not in node['roles'])
 
     def nodes_amount(self) -> int:
         """
         Returns the number of nodes within a group
         :return: Integer
         """
-        return len(self.nodes.keys())
+        return len(self.nodes)
 
     def get_nodes_os(self) -> str:
         """
         Returns the detected operating system family for group.
 
         :return: Detected OS family, possible values: "debian", "rhel", "rhel8", "multiple", "unknown", "unsupported".
         """
-        return self.cluster.get_os_family_for_nodes(self.nodes.keys())
+        return self.cluster.get_os_family_for_nodes(self.nodes)
 
     def is_multi_os(self) -> bool:
         """
         Returns true if same group contains nodes with multiple OS families
         :return: Boolean
         """
         return self.get_nodes_os() == 'multiple'
 
-    def get_subgroup_with_os(self, os_family: str) -> NodeGroup:
+    def get_subgroup_with_os(self: GROUP_SELF, os_family: str) -> GROUP_SELF:
         """
         Forms and returns a new group from the nodes of the original group that have a specific OS family
         :param os_family: The name of required OS family
         :return: NodeGroup
         """
         if os_family not in ['debian', 'rhel', 'rhel8']:
             raise Exception('Unsupported OS family provided')
-        node_names = []
-        for node in self.get_ordered_members_list(provide_node_configs=True):
-            node_os_family = self.cluster.get_os_family_for_node(node['connect_to'])
+        hosts = []
+        for host in self.nodes:
+            node_os_family = self.cluster.get_os_family_for_node(host)
             if node_os_family == os_family:
-                node_names.append(node['name'])
-        return self.cluster.make_group_from_nodes(node_names)
+                hosts.append(host)
+        return self._make_group(hosts)
+
+
+class NodeGroup(AbstractGroup[RunnersGroupResult]):
+    def _make_group(self: NodeGroup, ips: Iterable[Union[str, NodeGroup]]) -> NodeGroup:
+        return NodeGroup(ips, self.cluster)
+
+    def _make_defer(self, executor: RemoteExecutor) -> DeferredGroup:
+        return DeferredGroup(self.nodes, self.cluster, executor)
+
+    def new_defer(self, timeout: int = None) -> DeferredGroup:
+        return self.new_executor(timeout).group
+
+    def new_executor(self, timeout: int = None) -> RemoteExecutor:
+        return RemoteExecutor(self, timeout=timeout)
+
+    def get(self, remote_file: str, local_file: str) -> None:
+        self._do_exec("get", remote_file, local_file)
+
+    def _put(self, local_stream: Union[io.BytesIO, str], remote_file: str) -> None:
+        self._do_exec("put", local_stream, remote_file)
+
+    def _run(self, do_type: str, command: str, caller: Optional[Dict[str, object]],
+             **kwargs: Any) -> RunnersGroupResult:
+        """
+        The method should be called directly from run & sudo without any extra wrappers.
+        """
+        do_stream = not kwargs['hide']
+        if do_stream and len(self.nodes) > 1:
+            raise ValueError("Streaming of output is supported only for the single node")
+
+        if do_stream and caller is not None:
+            logger = self.cluster.log
+            kwargs['out_stream'] = log.LoggerWriter(logger, caller, '\t')
+            kwargs['err_stream'] = log.LoggerWriter(logger, caller, '\t')
+
+        results = self._do_exec(do_type, command, **kwargs)
+        return self._unsafe_make_runners_result(results)
+
+    def _do_exec(self, do_type: str, *args: object, **kwargs: Any) -> HostToResult:
+        callback: Callback = kwargs.pop('callback', None)
+
+        executor = RawExecutor(self.cluster, timeout=kwargs.get('timeout'))
+        executor.queue(self.get_hosts(), (do_type, args, kwargs), callback=callback)
+        executor.flush()
+
+        results = {host: next(iter(results.values()))
+                   for host, results in executor.get_last_results().items()}
+
+        if any(isinstance(result, Exception) for result in results.values()):
+            raise GroupResultException(NodeGroupResult(self.cluster, results))
+
+        return results
+
+    def wait_for_reboot(self, initial_boot_history: RunnersGroupResult, timeout: int = None) -> RunnersGroupResult:
+        results = self._await_rebooted_nodes(timeout, initial_boot_history=initial_boot_history)
+        if any(isinstance(result, Exception) or result == initial_boot_history.get(host)
+               for host, result in results.items()):
+            raise GroupResultException(NodeGroupResult(self.cluster, results))
+
+        return self._unsafe_make_runners_result(results)
+
+    def wait_and_get_boot_history(self, timeout: int = None) -> RunnersGroupResult:
+        return self.wait_for_reboot(RunnersGroupResult(self.cluster, {}), timeout=timeout)
+
+    def _await_rebooted_nodes(self, timeout: int = None, initial_boot_history: RunnersGroupResult = None) \
+            -> HostToResult:
+
+        executor = RawExecutor(self.cluster)
+        return executor.wait_for_boot(self.get_hosts(), timeout, initial_boot_history)
+
+    def get_local_file_sha1(self, filename: str) -> str:
+        return utils.get_local_file_sha1(filename)
+
+    def get_remote_file_sha1(self, filename: str) -> Dict[str, Optional[str]]:
+        results = self.sudo("openssl sha1 %s" % filename, warn=True)
+        return {host: result.stdout.split("= ")[1].strip() if result.stdout else None
+                for host, result in results.items()}
+
+
+class DeferredGroup(AbstractGroup[Token]):
+    def __init__(self, ips: Iterable[Union[str, DeferredGroup]], cluster: object, executor: RemoteExecutor):
+        super().__init__(ips, cluster)
+        self._executor = executor
+
+    @property
+    def executor(self) -> RemoteExecutor:
+        return self._executor
+
+    def flush(self) -> None:
+        self._executor.flush()
+
+    def _make_group(self, ips: Iterable[Union[str, DeferredGroup]]) -> DeferredGroup:
+        return DeferredGroup(ips, self.cluster, self._executor)
+
+    def get(self, remote_file: str, local_file: str) -> None:
+        self._do_queue("get", remote_file, local_file)
+
+    def _run(self, do_type: str, command: str, caller: Optional[Dict[str, object]], **kwargs: object) -> Token:
+        do_stream = not kwargs['hide']
+        if do_stream:
+            # To support streaming of output with use of RemoteExecutor in deferred mode, it is necessary to:
+            # 1) Make sure that no two commands are executed with streaming in parallel to avoid mess in output
+            # 2) Do not print output twice if error occurred.
+            raise ValueError("Streaming of output is currently not supported in deferred mode")
+        return self._do_queue(do_type, command, **kwargs)
+
+    def _put(self, local_stream: Union[io.BytesIO, str], remote_file: str) -> None:
+        self._do_queue("put", local_stream, remote_file)
+
+    def _do_queue(self, do_type: str, *args: object, **kwargs: Any) -> Token:
+        callback: Callback = kwargs.pop('callback', None)
+        return self._executor.queue(self.get_hosts(), (do_type, args, kwargs), callback=callback)
+
+    def include_group(self: DeferredGroup, group: DeferredGroup) -> DeferredGroup:
+        self._check_same_bound_executor(group)
+        return AbstractGroup.include_group(self, group)
+
+    def exclude_group(self, group: DeferredGroup) -> DeferredGroup:
+        self._check_same_bound_executor(group)
+        return AbstractGroup.exclude_group(self, group)
+
+    def intersection_group(self, group: DeferredGroup) -> DeferredGroup:
+        self._check_same_bound_executor(group)
+        return AbstractGroup.intersection_group(self, group)
+
+    def _check_same_bound_executor(self, group: DeferredGroup) -> None:
+        if self._executor is not group._executor:
+            raise ValueError("Trying to apply set operation on deferred groups bound to different executors")
+
+
+class RemoteExecutor(RawExecutor):
+    def __init__(self, group: NodeGroup, timeout: int = None) -> None:
+        super().__init__(group.cluster, timeout)
+        self.group: DeferredGroup = group._make_defer(self)
+        self.cluster = group.cluster
+
+    def flush(self) -> None:
+        """
+        Flushes the connections' queue.
+        Throws GroupException in case of any failure.
+
+        :return: grouped tokenized results per connection.
+        """
+        super().flush()
+
+        for host, results in self._last_results.items():
+            if any(isinstance(result, Exception) for _, result in results.items()):
+                raise RemoteGroupException(self.cluster, self._last_results)
+
+
+class GroupException(Exception):
+    def __init__(self, cluster: object, results: Dict[str, List[GenericResult]]):
+        self.cluster = cluster
+        self._results = results
+
+    def _make_group(self, hosts: Iterable[str]) -> NodeGroup:
+        return NodeGroup(hosts, self.cluster)
+
+    def is_any_excepted(self) -> bool:
+        """
+        Returns true if at least one result in group is an exception
+
+        :return: Boolean
+        """
+        return len(self.get_excepted_hosts_list()) > 0
+
+    def get_excepted_hosts_list(self) -> List[str]:
+        """
+        Returns a list of hosts, for which the result is an exception.
+
+        :return: List with hosts
+        """
+        excepted_hosts: List[str] = []
+        for host, results in self._results.items():
+            if any(isinstance(result, Exception) for result in results):
+                excepted_hosts.append(host)
+        return excepted_hosts
+
+    def get_excepted_nodes_group(self) -> NodeGroup:
+        """
+        Forms and returns new NodeGroup of nodes, for which the result is an exception.
+
+        :return: NodeGroup:
+        """
+        nodes_list = self.get_excepted_hosts_list()
+        return self._make_group(nodes_list)
+
+    def get_exited_hosts_list(self) -> List[str]:
+        """
+        Returns a list of hosts, for which the result is the completion of all commands.
+
+        :return: List with hosts
+        """
+        exited_hosts: List[str] = []
+        for host, results in self._results.items():
+            if all(isinstance(result, RunnersResult) for result in results):
+                exited_hosts.append(host)
+        return exited_hosts
+
+    def get_exited_nodes_group(self) -> NodeGroup:
+        """
+        Forms and returns new NodeGroup of nodes, for which the result is the completion of all commands.
+
+        :return: NodeGroup
+        """
+        nodes_list = self.get_exited_hosts_list()
+        return self._make_group(nodes_list)
+
+    def __str__(self) -> str:
+        # We always print output of all commands in the batch even if they are not failed,
+        # for the reason that the user code might want to print output of some commands in the batch,
+        # but failed to do that because of the exception.
+        host_outputs = []
+        for host, results in self._results.items():
+            output = f"{host}:"
+
+            # filter out transfer results and the last exception if present
+            runners_results = [res for res in results if isinstance(res, RunnersResult)]
+            if runners_results:
+                merged_result = RunnersResult.merge(runners_results)
+                output += f" code={merged_result.repr_code()}"
+                repr_out = merged_result.repr_out(hide_already_printed=True)
+                if repr_out:
+                    output += '\n\t' + repr_out.replace('\n', '\n\t')
+
+            # The exception may be only the last in the list. We are also sure to have at least one result per node.
+            if isinstance(results[-1], Exception):
+                exception = errors.wrap_kme_exception(results[-1])
+                output += '\n\t' + str(exception).replace('\n', '\n\t')
+
+            host_outputs.append(output)
+
+        return "\n".join(host_outputs)
+
+
+class GroupResultException(GroupException):
+    def __init__(self, result: GenericGroupResult[GenericResult]):
+        super().__init__(result.cluster, {host: [res] for host, res in result.items()})
+        self.result = result
+
+
+class RemoteGroupException(GroupException):
+    def __init__(self, cluster: object, results: Dict[str, TokenizedResult]):
+        super().__init__(cluster, {host: list(res.values()) for host, res in results.items()})
+        self.results = results
```

### Comparing `kubemarine-0.18.2/kubemarine/core/log.py` & `kubemarine-0.19.0/kubemarine/core/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 
 import logging
 import os
 import sys
 from abc import ABC, abstractmethod
 
-from pygelf import gelf, GelfTcpHandler, GelfUdpHandler, GelfTlsHandler, GelfHttpHandler
+from pygelf import gelf, GelfTcpHandler, GelfUdpHandler, GelfTlsHandler, GelfHttpHandler  # type: ignore[import]
 
 from copy import deepcopy
-from typing import List, Optional
+from typing import Any, List, Optional, cast, Dict
 
 VERBOSE = 5
 gelf.LEVELS.update({VERBOSE: 8})
 
 DEFAULT_FORMAT = '%(asctime)s %(name)s %(levelname)s %(message)s'
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
@@ -78,24 +78,24 @@
     logging.ERROR: 'error',
     logging.CRITICAL: 'critical'
 }
 
 
 class VerboseLogger(ABC):
     @abstractmethod
-    def verbose(self, msg, *args, **kwargs):
+    def verbose(self, msg: object, *args: object, **kwargs: Any) -> None:
         pass
 
 
 class EnhancedLogger(logging.Logger, VerboseLogger):
     def __init__(self, name, level=logging.NOTSET):
         super().__init__(name, level)
         logging.addLevelName(VERBOSE, 'VERBOSE')
 
-    def verbose(self, msg, *args, **kwargs):
+    def verbose(self, msg: object, *args: object, **kwargs: Any) -> None:
         if self.isEnabledFor(VERBOSE):
             self._log(VERBOSE, msg, args, **kwargs)
 
     def makeRecord(self, name: str, level: int, fn: str, lno: int, msg: object, args,
                    exc_info, func=None, extra=None,
                    sinfo=None) -> logging.LogRecord:
         record = super().makeRecord(name, level, fn, lno, msg, args, exc_info, func, extra, sinfo)
@@ -149,52 +149,41 @@
                 s += self._format(record)
             return s
         finally:
             record.msg = orig_msg
 
 
 class StdoutHandler(logging.StreamHandler):
-    def __init__(self):
+    def __init__(self, formatter: LogFormatter):
         super().__init__(sys.stdout)
+        self.formatter: LogFormatter = formatter
 
     def emit(self, record):
         if 'ignore_stdout' in record.__dict__:
             return
         super().emit(record)
         # TODO: if output stuck, then add here self.flush()
         # More about, see at https://stackoverflow.com/questions/16633911
 
 
 class FileHandlerWithHeader(logging.FileHandler):
-    def __init__(self, filename, header=None, mode='a', encoding=None, delay=0):
+    def __init__(self, formatter: LogFormatter, filename, header=None, mode='a', encoding=None):
         # Store the header information.
         self.header = header
 
-        # Determine if the file pre-exists
-        self.file_pre_exists = os.path.exists(filename)
-
         # Call the parent __init__
-        logging.FileHandler.__init__(self, filename, mode, encoding, delay)
+        logging.FileHandler.__init__(self, filename, mode, encoding)
 
-        # Write the header if delay is False and a file stream was created.
-        if not delay and header and self.stream is not None:
+        # Write the header if it was specified
+        if header:
             self.stream.write('%s\n' % header)
 
-    def emit(self, record):
-        # Create the file stream if not already created.
-        if self.stream is None:
-            self.stream = self._open()
-
-            # If the file pre_exists, it should already have a header.
-            # Else write the header to the file so that it is the first line.
-            if not self.file_pre_exists:
-                self.stream.write('')
-                if self.header:
-                    self.stream.write('%s\n' % self.header)
+        self.formatter: LogFormatter = formatter
 
+    def emit(self, record):
         # Call the parent class emit function.
         logging.FileHandler.emit(self, record)
 
 
 class LogHandler:
 
     def __init__(self,
@@ -214,17 +203,18 @@
         self._datefmt = datefmt
         self._header = header
 
         self._formatter = LogFormatter(self._format, self._datefmt,
                                        colorize=self._colorize,
                                        correct_newlines=self._correct_newlines)
 
+        self.handler: logging.Handler
         if target.lower() == 'stdout':
             self._target = 'stdout'
-            self.handler = StdoutHandler()
+            self.handler = StdoutHandler(self._formatter)
         elif target.lower() == 'graylog':
             self._target = 'graylog'
             if not kwargs.get('host'):
                 raise Exception('Graylog host is not defined')
             if not kwargs.get('port'):
                 raise Exception(f'Graylog port is not defined for "{kwargs["host"]}"')
             if not kwargs.get('type'):
@@ -251,92 +241,101 @@
             elif kwargs['type'] == 'http':
                 handler_options['compress'] = kwargs.get('compress', True)
                 handler_options['path'] = kwargs.get('path', '/gelf')
                 handler_options['timeout'] = kwargs.get('timeout', 5)
                 self.handler = GelfHttpHandler(**handler_options)
             else:
                 raise Exception(f'Unknown Graylog type "{kwargs["type"]}" for "{kwargs["host"]}:{kwargs["port"]}"')
+
+            self.handler.setFormatter(self._formatter)
         else:
             self._target = target
             # Output produced by remote commands might contain characters which cannot be encoded on Windows deployer.
             # Specify explicitly utf-8 encoding which is native to the remote machines.
-            self.handler = FileHandlerWithHeader(self._target, mode=filemode, header=self._header, encoding='utf-8')
+            self.handler = FileHandlerWithHeader(self._formatter, self._target, mode=filemode, header=self._header, encoding='utf-8')
 
-        self._level = LOGGING_LEVELS_BY_NAME.get(level)
-        if self._level is None:
+        if level not in LOGGING_LEVELS_BY_NAME:
             raise Exception(f'Failed to create logger - unknown logging level: "{level}"')
+        self._level = LOGGING_LEVELS_BY_NAME[level]
         self.handler.setLevel(self._level)
 
-        self.handler.setFormatter(self._formatter)
-
     def __str__(self):
         return f'target: {self._target}, level: {LOGGING_NAMES_BY_LEVEL[self._level]}, colorize: {self._colorize}, datefmt: {self._datefmt}, format: {self._format}'
 
     def append_to_logger(self, logger) -> None:
         logger.addHandler(self.handler)
 
     def has_stdout_target(self) -> bool:
         return self._target == 'stdout'
 
 
 class Log:
 
     def __init__(self, raw_inventory, handlers: List[LogHandler]):
-        self._logger = logging.getLogger(raw_inventory.get('cluster_name', 'cluster.local'))
+        logger = logging.getLogger(raw_inventory.get('cluster_name', 'cluster.local'))
+        self._logger = cast(EnhancedLogger, logger)
         self._logger.setLevel(VERBOSE)
 
         if self._logger.hasHandlers():
             self._logger.handlers.clear()
 
         for handler in handlers:
             handler.append_to_logger(self._logger)
 
     @property
     def logger(self) -> EnhancedLogger:
         return self._logger
 
 
 class LoggerWriter:
-    def __init__(self, logger: EnhancedLogger, level, caller: dict, prefix: str):
+    def __init__(self, logger: EnhancedLogger, caller: dict, prefix: str) -> None:
         self.logger = logger
-        self.level = level
         self.caller = caller
         self.prefix = prefix
         self.buf = ""
 
-    def write(self, message):
+    def write(self, message: str) -> None:
+        # Both remote stderr and stdout are printed to local stdout
+        sys.stdout.write(message)
+
         lines = message.split('\n')
         for line in lines[:-1]:
             self.buf = self.buf + line
             self._log()
         self.buf = self.buf + lines[-1]
 
-    def flush(self, remainder=False):
+    def flush(self, remainder: bool = False) -> None:
         if remainder and self.buf:
             self._log()
 
-    def _log(self):
-        self.logger.log(self.level, self.buf, extra={'real_caller': self.caller, 'prefix': self.prefix})
+    def _log(self) -> None:
+        self.logger.log(logging.DEBUG, self.buf, extra={
+            'real_caller': self.caller, 'prefix': self.prefix, 'ignore_stdout': True
+        })
         self.buf = ""
 
+    def __repr__(self) -> str:
+        return f"LoggerWriter{{DEBUG,stdout}} at {hex(id(self))}"
+
 
 def parse_log_argument(argument: str) -> LogHandler:
     """
     Parse raw CLI arguments and verify for required parameters
     :param argument: Raw CLI argument string. For example: test.log;level=verbose;colorize=true
     :return: Initialized LogHandler
     """
-    parameters = {}
+    parameters: Dict[str, Any] = {}
     argument_parts = argument.split(';')
     if not argument_parts:
         raise Exception('Defined logger do not contain parameters')
     parameters['target'] = argument_parts[0]
     for parameter in argument_parts[1:]:
         if parameter == '':
             continue
+        value: Any
         key, value, *rest = parameter.split('=')
         if key in ['colorize', 'correct_newlines', 'debug', 'compress', 'validate']:
             value = value.lower() in ['true', '1']
         elif key in ['chunk_size', 'timeout', 'port']:
             value = int(value)
         parameters[key] = value
     if not parameters.get('level'):
@@ -387,20 +386,24 @@
     log = Log(raw_inventory, handlers)
 
     log.logger.verbose('Using the following loggers: \n\t%s' % "\n\t".join("- " + str(x) for x in handlers))
 
     return log
 
 
-def caller_info(logger: EnhancedLogger) -> dict:
+def caller_info(logger: EnhancedLogger) -> Dict[str, object]:
     """
     Catches and returns invocation metadata of the method that calls caller_info()
+
+    :param logger: EnhancedLogger
+    :return: dictionary with the invocation metadata
     """
     fn, lno, func, sinfo = logger.findCaller()
-    record: logging.LogRecord = logger.makeRecord(None, None, fn, lno, "", (), None, func=func, extra=None, sinfo=sinfo)
+    record: logging.LogRecord = logger.makeRecord("", logging.DEBUG, fn, lno, "", (), None,
+                                                  func=func, extra=None, sinfo=sinfo)
     return dict(item for item in record.__dict__.items()
                 if item[0] in (
                     # record's fields describing invocation origin
                     'pathname', 'filename', 'module', 'lineno', 'funcName', 'stack_info',
                     # record's fields describing initial process and thread context
                     'thread', 'threadName', 'process', 'processName'
                 ))
```

### Comparing `kubemarine-0.18.2/kubemarine/core/os.py` & `kubemarine-0.19.0/kubemarine/patches/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# Copyright 2021-2023 NetCracker Technology Corporation
+# Copyright 2021-2022 NetCracker Technology Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-from typing import Iterator, Mapping
-
-
-class Environ(Mapping[str, str]):
-    """
-    Read-only view of os.environ.
-    """
-
-    def __getitem__(self, name: str) -> str:
-        # check presence of the variable and throw KeyError if necessary
-        return os.environ[name]
-
-    def __len__(self) -> int:
-        return len(os.environ)
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(os.environ)
-
-    __slots__ = []
+"""
+All files and directories inside kubemarine/patches directory should participate only in patching mechanism,
+and relate to the current Kubemarine version.
+
+The whole directory is automatically cleared and reset after new version of Kubemarine is released.
+"""
+
+from typing import List
+
+from kubemarine.core.patch import Patch
+
+patches: List[Patch] = [
+]
+"""
+List of patches that is sorted according to the Patch.priority() before execution.
+Patches that have the same priority, are executed in the declared order.
+"""
```

### Comparing `kubemarine-0.18.2/kubemarine/core/patch.py` & `kubemarine-0.19.0/kubemarine/core/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     REGULAR = 2
     """
     The patch can access and make some operations on the cluster.
     Changes in the inventory are possible, but they should not affect the software upgrade procedure.
     """
 
-    def __lt__(self, other):
+    def __lt__(self, other: '_Priority') -> bool:
         return self.value < other.value
 
 
 class Patch(ABC):
     def __init__(self, identifier: str):
         self.identifier = identifier
```

### Comparing `kubemarine-0.18.2/kubemarine/core/resources.py` & `kubemarine-0.19.0/kubemarine/core/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,84 +9,89 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import Optional
+from typing import Optional, cast, Iterator, Type
 
 import yaml
 import ruamel.yaml
 
 from kubemarine.core import utils, cluster as c, log, errors, static
 from kubemarine.core.yaml_merger import default_merger
 
 
 class DynamicResources:
-    def __init__(self, context: dict, silent=False):
+    def __init__(self, context: dict, silent: bool = False) -> None:
         self.context = context
         """
         Context holding execution arguments and other auxiliary parameters which manage the execution flow.
         The context can be mutable, but only from action to action,
         and should be copied when passing to the cluster object.
         """
         self.working_context = context
         """
         Context that is directly passed to the cluster object and that holds its intermediate result.
         """
 
         self._silent = silent
         self._logger: Optional[log.EnhancedLogger] = None
-        self._raw_inventory = None
-        self._formatted_inventory = None
-        self._procedure_inventory = None
+        self._raw_inventory: Optional[dict] = None
+        self._formatted_inventory: Optional[dict] = None
+        self._procedure_inventory: Optional[dict] = None
 
-        self._nodes_context = None
+        self._nodes_context: Optional[dict] = None
         """
         The nodes_context variable should hold node specific information that is not changed during Kubemarine run.
         The variable should be initialized on demand and only once.
         """
 
         self._cluster: Optional[c.KubernetesCluster] = None
 
         args: dict = context['execution_arguments']
-        self.inventory_filepath = args['config']
-        self.procedure_inventory_filepath = args.get('procedure_config')
+        self.inventory_filepath: Optional[str] = args['config']
+        self.procedure_inventory_filepath: Optional[str] = args.get('procedure_config')
 
-    def logger_if_initialized(self):
+    def logger_if_initialized(self) -> Optional[log.EnhancedLogger]:
         return self._logger
 
-    def logger(self):
+    def logger(self) -> log.EnhancedLogger:
         if self._logger is None:
             self._logger = self._create_logger()
 
         return self._logger
 
     def raw_inventory(self) -> dict:
         """Returns raw inventory, which does not preserve formatting and which should be read only."""
         if self._raw_inventory is None:
             self._load_inventory()
 
-        return self._raw_inventory
+        return cast(dict, self._raw_inventory)
 
     def formatted_inventory(self) -> dict:
         """Returns raw inventory with preserved comments/quotes, to be modified and later recreated."""
         if self._formatted_inventory is None:
             self._load_inventory()
 
-        return self._formatted_inventory
+        return cast(dict, self._formatted_inventory)
 
-    def procedure_inventory(self):
-        if self._procedure_inventory is None and self.procedure_inventory_filepath:
-            self._procedure_inventory = utils.load_yaml(self.procedure_inventory_filepath)
+    def procedure_inventory(self) -> dict:
+        if self._procedure_inventory is None:
+            if self.procedure_inventory_filepath:
+                self._procedure_inventory = utils.load_yaml(self.procedure_inventory_filepath)
+            else:
+                self._procedure_inventory = {}
 
         return self._procedure_inventory
 
-    def _load_inventory(self):
+    def _load_inventory(self) -> None:
+        if not self.inventory_filepath:
+            raise Exception("Path to inventory is not defined")
         logger = self._logger
         if not self._silent:
             msg = "Loading inventory file '%s'" % self.inventory_filepath
             if logger is None:
                 print(msg)
             else:
                 logger.info(msg)
@@ -94,18 +99,18 @@
             data = utils.read_external(self.inventory_filepath)
             self._raw_inventory = yaml.safe_load(data)
             # load inventory as ruamel.yaml to save original structure
             self._formatted_inventory = utils.yaml_structure_preserver().load(data)
         except (yaml.YAMLError, ruamel.yaml.YAMLError) as exc:
             utils.do_fail("Failed to load inventory file", exc, log=logger)
 
-    def make_final_inventory(self):
+    def make_final_inventory(self) -> None:
         self._formatted_inventory = utils.get_final_inventory(self.cluster(), initial_inventory=self.formatted_inventory())
 
-    def recreate_inventory(self):
+    def recreate_inventory(self) -> None:
         """
         Recreates initial inventory file using DynamicResources.formatted_inventory and resets all dynamic resources.
 
         Avoid using it directly, because cluster object and previous inventory will be lost,
         and post processing of actions may work incorrectly.
         """
         if self._formatted_inventory is None:
@@ -115,15 +120,17 @@
 
         self._raw_inventory = None
         self._formatted_inventory = None
         # no need to clear _nodes_context as it should not change after cluster is reinitialized.
         # should not clear working_context as it can be inspected after execution.
         self._cluster = None
 
-    def _store_inventory(self):
+    def _store_inventory(self) -> None:
+        if not self.inventory_filepath:
+            raise Exception("Path to inventory is not defined")
         # replace initial inventory file with changed inventory
         with utils.open_external(self.inventory_filepath, "w+") as stream:
             utils.yaml_structure_preserver().dump(self.formatted_inventory(), stream)
 
     def cluster_if_initialized(self) -> Optional[c.KubernetesCluster]:
         return self._cluster
 
@@ -131,15 +138,15 @@
         """Returns already initialized cluster object or initializes new real cluster object."""
         if self._cluster is None:
             self.working_context = deepcopy(self.context)
             self._cluster = self._create_cluster(self.working_context)
 
         return self._cluster
 
-    def create_deviated_cluster(self, deviated_context: dict):
+    def create_deviated_cluster(self, deviated_context: dict) -> c.KubernetesCluster:
         """
         Create new cluster instance with specified deviation of context params.
         The method work should minimize work with network and avoid RW work with filesystem.
         The cluster instance should be useful to develop a patch in case enrichment procedure is changed
         and it is necessary to compare the result of old and new algorithm of enrichment.
         It should not be used in tasks.
 
@@ -150,23 +157,23 @@
         sample_context['preserve_inventory'] = False
         args = sample_context['execution_arguments']
         args['disable_dump'] = True
         del args['ansible_inventory_location']
         return self._create_cluster(sample_context)
 
     @contextmanager
-    def _handle_enrichment_error(self):
+    def _handle_enrichment_error(self) -> Iterator[None]:
         try:
             yield
         except errors.FailException:
             raise
         except Exception as exc:
             raise errors.FailException("Failed to proceed inventory file", exc)
 
-    def _create_cluster(self, context):
+    def _create_cluster(self, context: dict) -> c.KubernetesCluster:
         log = self.logger()
         context['nodes'] = deepcopy(self.get_nodes_context())
         with self._handle_enrichment_error():
             cluster = self._new_cluster_instance(context)
             cluster.enrich()
 
         if not self._silent:
@@ -178,30 +185,28 @@
 
         args = context['execution_arguments']
         if 'ansible_inventory_location' in args:
             utils.make_ansible_inventory(args['ansible_inventory_location'], cluster)
 
         return cluster
 
-    def get_nodes_context(self):
+    def get_nodes_context(self) -> dict:
         if self._nodes_context is None:
             with self._handle_enrichment_error():
                 # temporary cluster instance to detect initial nodes context.
                 light_cluster = self._new_cluster_instance(deepcopy(self.context))
                 light_cluster.enrich(custom_enrichment_fns=light_cluster.get_facts_enrichment_fns())
                 self._nodes_context = light_cluster.detect_nodes_context()
 
         return self._nodes_context
 
     def _new_cluster_instance(self, context: dict) -> c.KubernetesCluster:
-        return _provide_cluster(self.raw_inventory(), context,
-                                procedure_inventory=self.procedure_inventory(),
-                                logger=self.logger())
+        from kubemarine.core import flow
+        cluster_class = c.KubernetesCluster
+        if flow.DEFAULT_CLUSTER_OBJ is not None:
+            cluster_class = flow.DEFAULT_CLUSTER_OBJ
+        return cluster_class(self.raw_inventory(), context,
+                             procedure_inventory=self.procedure_inventory(),
+                             logger=self.logger())
 
-    def _create_logger(self):
+    def _create_logger(self) -> log.EnhancedLogger:
         return log.init_log_from_context_args(static.GLOBALS, self.context, self.raw_inventory()).logger
-
-
-def _provide_cluster(*args, **kw):
-    from kubemarine.core import flow
-    return flow.DEFAULT_CLUSTER_OBJ(*args, **kw) if flow.DEFAULT_CLUSTER_OBJ is not None \
-        else c.KubernetesCluster(*args, **kw)
```

### Comparing `kubemarine-0.18.2/kubemarine/core/schema.py` & `kubemarine-0.19.0/kubemarine/core/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import pathlib
 from textwrap import dedent
-from typing import List, Dict, Callable, Iterable
+from typing import List, Dict, Callable, Union, Sequence, Hashable
 
 import jsonschema
 from ordered_set import OrderedSet
 
 from kubemarine.core import utils, log, errors
 from kubemarine.core.cluster import KubernetesCluster
 
 
-def verify_inventory(inventory: dict, cluster: KubernetesCluster):
+def verify_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     _verify_inventory_by_schema(cluster, inventory, 'cluster')
     procedure = cluster.context.get("initial_procedure")
     if procedure:
         _verify_inventory_by_schema(cluster, cluster.procedure_inventory, procedure)
     return inventory
 
 
-def _verify_inventory_by_schema(cluster: KubernetesCluster, inventory: dict, schema_name: str):
+def _verify_inventory_by_schema(cluster: KubernetesCluster, inventory: dict, schema_name: str) -> None:
     for_procedure = "" if schema_name == 'cluster' else f" for procedure '{schema_name}'"
 
     root_schema_resource = f'resources/schemas/{schema_name}.json'
-    root_schema = utils.get_internal_resource_path(root_schema_resource)
-    root_schema = pathlib.Path(root_schema)
+    root_schema_path = utils.get_internal_resource_path(root_schema_resource)
+    root_schema = pathlib.Path(root_schema_path)
     if not root_schema.exists():
         if schema_name == 'cluster' or inventory:
             raise Exception(f"Failed to find schema to validate the inventory file{for_procedure}.")
         return
 
     with utils.open_internal(root_schema_resource) as f:
         schema = json.load(f)
@@ -90,61 +90,61 @@
     else:
         hint += f"If you are sure that the file is correct, please contact support,\n" \
                 f"and use --ignore-schema-errors to proceed (option will be removed in next release).\n"
 
     raise errors.FailException(msg, hint=hint)
 
 
-def _resolve_errors(errs: List[jsonschema.ValidationError]):
+def _resolve_errors(errs: List[jsonschema.ValidationError]) -> List[jsonschema.ValidationError]:
     key = _extended_relevance()
     for error in errs:
         _unnest_errors(error)
 
     errs.sort(key=key, reverse=True)
     outer_sorted = []
     for error in errs:
         outer_sorted.extend(_descend_errors(error))
 
     return outer_sorted
 
 
-def _unnest_errors(error: jsonschema.ValidationError):
-    context: List[jsonschema.ValidationError] = error.context
-    if not context:
+def _unnest_errors(error: jsonschema.ValidationError) -> None:
+    if not error.context:
         return
 
-    errors_by_subschema: Dict[int, List[jsonschema.ValidationError]] = {}
+    context: List[jsonschema.ValidationError] = error.context
+    errors_by_subschema: Dict[Union[str, int], List[jsonschema.ValidationError]] = {}
     for child in context:
         _unnest_errors(child)
         errors_by_subschema.setdefault(child.schema_path[0], []).append(child)
 
     # jsonschema might show not very friendly messages for anyOf / oneOf.
     # In case of failed type or enum validation in each subschema, we can unnest the error to the higher level.
     # Note that possible remaining subschema errors will be discarded,
     # but it is acceptable for our current schemas implementation.
     subschemas_errors = list(errors_by_subschema.values())
     _unnest_type_subschema_errors(error, subschemas_errors)
     _unnest_enum_subschema_errors(error, subschemas_errors)
 
 
 def _descend_errors(error: jsonschema.ValidationError) -> List[jsonschema.ValidationError]:
-    context: List[jsonschema.ValidationError] = error.context
-    if not context:
+    if not error.context:
         return [error]
 
     # Here can be anyOf or oneOf with all not valid subschemas.
     # The idea is taken from jsonschema.exceptions.best_match,
     # with improved heuristic algorithm of choosing of the best subschema match.
     # 1. group errors by subschema
     # 2. find error with the max relevance in each group
     # 3. choose group with the min relevance of the error found in the previous step
     # 4. take the group instead of the parent error, sort by relevance reverse
     # 5. recurse if necessary
 
-    errors_by_subschema: Dict[int, List[jsonschema.ValidationError]] = {}
+    context: List[jsonschema.ValidationError] = error.context
+    errors_by_subschema: Dict[Union[str, int], List[jsonschema.ValidationError]] = {}
     for child in context:
         errors_by_subschema.setdefault(child.schema_path[0], []).append(child)
 
     key = _extended_relevance()
 
     for errors in errors_by_subschema.values():
         errors.sort(key=key, reverse=True)
@@ -159,195 +159,201 @@
     unnested_errors = []
     for err in smallest_subschema_errors[0]:
         unnested_errors.extend(_descend_errors(err))
 
     return unnested_errors
 
 
-def _unnest_type_subschema_errors(error: jsonschema.ValidationError, subschemas_errors: List[List[jsonschema.ValidationError]]):
+def _unnest_type_subschema_errors(error: jsonschema.ValidationError,
+                                  subschemas_errors: List[List[jsonschema.ValidationError]]) -> None:
     if not error.context:
         return
 
-    expected_types = OrderedSet()
+    expected_types = OrderedSet[str]()
     for errs in subschemas_errors:
         for child in errs:
-            if child.validator == "type" and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["type"]:
+            if _validated_by(child, "type") and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["type"]:
                 value = child.validator_value
                 expected_types.update([value] if isinstance(value, str) else value)
                 break
         else:  # not found error with "type" validation failed for root instance.
             break
     else:  # not found subschema not containing the necessary error, i. e. all subschemas has necessary error
         reprs = ", ".join(repr(type) for type in expected_types)
         for child in error.context:
             child.parent = None
         error.context = []
-        error.validator = "type"
+        error.validator = "type"  # type: ignore[assignment]
         error.validator_value = list(expected_types)
         error.schema_path[-1] = "type"
         error.message = f"{error.instance!r} is not of type {reprs}"
         subschemas_errors.clear()
 
 
-def _unnest_enum_subschema_errors(error: jsonschema.ValidationError, subschemas_errors: List[List[jsonschema.ValidationError]]):
+def _unnest_enum_subschema_errors(error: jsonschema.ValidationError,
+                                  subschemas_errors: List[List[jsonschema.ValidationError]]) -> None:
     if not error.context:
         return
 
-    expected_elems = OrderedSet()
+    expected_elems = OrderedSet[str]()
     for errs in subschemas_errors:
         for child in errs:
-            if child.validator == "enum" and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["enum"]:
+            if _validated_by(child, "enum") and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["enum"]:
                 expected_elems.update(child.validator_value)
                 break
         else:  # not found error with "enum" validation failed for root instance.
             break
     else:  # not found subschema not containing the necessary error, i. e. all subschemas has necessary error
-        expected_elems = list(expected_elems)
         for child in error.context:
             child.parent = None
         error.context = []
-        error.validator = "enum"
-        error.validator_value = expected_elems
+        error.validator = "enum"  # type: ignore[assignment]
+        error.validator_value = list(expected_elems)
         error.schema_path[-1] = "enum"
-        error.message = f"{error.instance!r} is not one of {expected_elems!r}"
+        error.message = f"{error.instance!r} is not one of {list(expected_elems)!r}"
         subschemas_errors.clear()
 
 
 def _extended_relevance() -> Callable[[jsonschema.ValidationError], tuple]:
     # The extended relevance function is intended to improve heuristic for oneOf|anyOf,
     # when it is necessary to choose the most suitable branch.
 
-    def relevance(error: jsonschema.ValidationError):
-        relevance_value = jsonschema.exceptions.relevance(error)
+    def relevance(error: jsonschema.ValidationError) -> tuple:
+        relevance_value: tuple = jsonschema.exceptions.relevance(error)  # type: ignore[assignment]
         if error.parent is None:
             return relevance_value
 
         relevance_value = _apply_property_names_heuristic(error, relevance_value)
         relevance_value = _apply_list_merging_strong_heuristic(error, relevance_value)
         relevance_value = _apply_required_and_optional_properties_heuristic(error, relevance_value)
 
         return relevance_value
 
     return relevance
 
 
-def _apply_property_names_heuristic(error: jsonschema.ValidationError, relevance_value: tuple):
+def _apply_property_names_heuristic(error: jsonschema.ValidationError, relevance_value: tuple) -> tuple:
     # jsonschema has type matching heuristic but it works bad for "propertyNames".
     # "propertyNames" does not introduce new path element and effectively verifies the object holding the property.
     # But an attempt to match the type happens for the "propertyNames" subschema.
     # The following heuristic resolves the simplest case of oneOf|anyOf(something, schema with "propertyNames" section)
 
     if len(error.relative_path) == 0 and "propertyNames" in error.schema_path:
         # "propertyNames" is validated only if the instance is "object".
         # See jsonschema._validators.propertyNames. So type is always matched.
         type_matched = True
-        relevance_value = list(relevance_value)
-        relevance_value[3] = not type_matched
-        return tuple(relevance_value)
+        mutate_relevance = list(relevance_value)
+        mutate_relevance[3] = not type_matched
+        return tuple(mutate_relevance)
 
     return relevance_value
 
 
-def _apply_list_merging_strong_heuristic(error: jsonschema.ValidationError, relevance_value: tuple):
+def _apply_list_merging_strong_heuristic(error: jsonschema.ValidationError, relevance_value: tuple) -> tuple:
     # Other conditions being equal, the error for list merging strategy has greater relevance,
     # because if the user specified '<<', we consider that he/she intends to use this advanced feature.
 
     is_list_merging = len(error.relative_path) == 0 and isinstance(error.schema, dict) \
                       and "properties" in error.schema and error.schema["properties"].keys() == {"<<"}
 
     return _append_relevance_element(relevance_value, is_list_merging)
 
 
-def _apply_required_and_optional_properties_heuristic(error: jsonschema.ValidationError, relevance_value: tuple):
+def _apply_required_and_optional_properties_heuristic(error: jsonschema.ValidationError,
+                                                      relevance_value: tuple) -> tuple:
     # Resolve oneOf|anyOf(object, object) ambiguity.
     # Currently only 'registry' section has such schema.
     # The chosen priority is:
     # 1. If all required properties are present, than the error has lower relevance.
     # 2. Otherwise, calculate proportion of matched properties.
 
     # By default, consider all required properties are present, and no properties are matched
-    coeff = [False, 0]
+    coeff: list = [False, 0]
     if len(error.relative_path) != 0 or not isinstance(error.schema, dict) or not isinstance(error.instance, dict):
         return _append_relevance_element(relevance_value, tuple(coeff))
 
     coeff[0] = not all(p in error.instance for p in error.schema.get("required", []))
 
     if len(error.schema.get("properties", {})) > 0:
         inverse_weight = len(error.schema["properties"])
         matched = set(error.instance.keys()).intersection(set(error.schema["properties"].keys()))
         # negative coefficient because more matched properties - more suitable subschema - less relevant error
         coeff[1] = - len(matched) / inverse_weight
 
     return _append_relevance_element(relevance_value, tuple(coeff))
 
 
-def _append_relevance_element(relevance_value: tuple, elem):
-    relevance_value = list(relevance_value)
-    relevance_value.append(elem)
-    return tuple(relevance_value)
+def _append_relevance_element(relevance_value: tuple, elem: Hashable) -> tuple:
+    mutate_relevance = list(relevance_value)
+    mutate_relevance.append(elem)
+    return tuple(mutate_relevance)
 
 
-def _error_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError):
+def _error_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
     return dedent(
         f"""\
         {_friendly_msg(validator, error)}
         On inventory{_convert_to_indices(error.absolute_path)}
         """.rstrip()
     )
 
 
-def _verbose_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError):
+def _verbose_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
     schema_path = _convert_to_indices(list(error.absolute_schema_path)[:-1])
     return dedent(
         f"""\
         {_friendly_msg(validator, error)}
         
         Failed validating {error.validator!r} in {schema_path}
         On inventory{_convert_to_indices(error.absolute_path)}
         """.rstrip()
     )
 
 
 def _friendly_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
-    if error.validator == 'minProperties':
+    if _validated_by(error, 'minProperties'):
         return f"Number of properties is less than the minimum of {error.validator_value!r}. " \
                f"Property names: {[prop for prop in error.instance]!r}"
 
-    if error.validator == 'maxProperties':
+    if _validated_by(error, 'maxProperties'):
         return f"Number of properties is greater than the maximum of {error.validator_value!r}. " \
                f"Property names: {[prop for prop in error.instance]!r}"
 
-    if error.validator == 'minItems':
+    if _validated_by(error, 'minItems'):
         return f"Number of items equal to {len(error.instance)} is less than the minimum of {error.validator_value!r}"
 
-    if error.validator == 'maxItems':
+    if _validated_by(error, 'maxItems'):
         return f"Number of items equal to {len(error.instance)} is greater than the maximum of {error.validator_value!r}"
 
-    if error.validator == 'type':
+    if _validated_by(error, 'type'):
         value = error.validator_value
         expected_types = [value] if isinstance(value, str) else value
         reprs = ", ".join(repr(type) for type in expected_types)
         try:
             for type in validator.TYPE_CHECKER._type_checkers:
-                if validator.is_type(error.instance, type):
+                if validator.is_type(error.instance, type):  # type: ignore[no-untyped-call]
                     return f"Actual instance type is {type!r}. Expected: {reprs}."
         except (AttributeError, TypeError, jsonschema.exceptions.UnknownType):
             # In current 3rd-party version the error should not appear, but let's still fall back to default behaviour
             pass
 
-    if error.validator == 'not' and isinstance(error.validator_value, dict) \
+    if _validated_by(error, 'not') and isinstance(error.validator_value, dict) \
             and error.validator_value.get('enum', {}) == ['<<'] and "propertyNames" in error.schema_path:
         return "Property name '<<' is unexpected"
 
-    if error.validator == 'enum':
+    if _validated_by(error, 'enum'):
         if "propertyNames" not in error.schema_path:
             return f"Value should be one of {error.validator_value!r}"
         else:
             return f"Property name {error.instance!r} is not one of {error.validator_value!r}"
 
     return error.message
 
 
-def _convert_to_indices(path: Iterable[str]):
+def _validated_by(error: jsonschema.ValidationError, expected: str) -> bool:
+    return error.validator == expected  # type: ignore[comparison-overlap]
+
+
+def _convert_to_indices(path: Sequence[Union[str, int]]) -> str:
     if not path:
         return ""
     return f"[{']['.join(repr(p) for p in path)}]"
```

### Comparing `kubemarine-0.18.2/kubemarine/core/static.py` & `kubemarine-0.19.0/kubemarine/core/static.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from kubemarine.core import utils
 
 
-def reload():
+def reload() -> None:
     global GLOBALS
     GLOBALS.clear()
     GLOBALS.update(_load_globals())
 
     global DEFAULTS
     DEFAULTS.clear()
     DEFAULTS.update(_load_defaults())
@@ -59,12 +59,14 @@
 
 
 def _load_defaults() -> dict:
     return utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/defaults.yaml'))
 
 
-GLOBALS = {}
-DEFAULTS = {}
-KUBERNETES_VERSIONS = {}
+# Cannot annotate in Python 3.7
+# https://github.com/python/cpython/issues/79120
+GLOBALS = {}  # type: ignore[var-annotated]
+DEFAULTS = {}  # type: ignore[var-annotated]
+KUBERNETES_VERSIONS = {}  # type: ignore[var-annotated]
 
 reload()
```

### Comparing `kubemarine-0.18.2/kubemarine/core/summary.py` & `kubemarine-0.19.0/kubemarine/core/summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,36 +25,36 @@
     KUBECONFIG = (0, "Kubeconfig")
     DASHBOARD_URL = (1, "Dashboard URL")
     CONTROL_PLANES = (2, "Running Control Planes")
     WORKERS = (3, "Running Workers")
     ACCOUNT_TOKENS = (4, "Account Tokens File")
     EXECUTION_TIME = (5, "Elapsed")
 
-    def __init__(self, order, text):
+    def __init__(self, order: int, text: str) -> None:
         self.order = order
         self.text = text
 
-    def __lt__(self, other):
+    def __lt__(self, other: 'SummaryItem') -> bool:
         return self.order < other.order
 
 
-def schedule_report(context: dict, property: SummaryItem, value: str):
+def schedule_report(context: dict, property: SummaryItem, value: str) -> None:
     context.setdefault('summary_report', {})[property] = value
 
 
-def schedule_delayed_report(cluster: KubernetesCluster, call: Callable[[KubernetesCluster], None]):
+def schedule_delayed_report(cluster: KubernetesCluster, call: Callable[[KubernetesCluster], None]) -> None:
     cluster.context.setdefault('delayed_summary_report', []).append(call)
     cluster.schedule_cumulative_point(exec_delayed)
 
 
-def print_summary(context: dict, logger: log.EnhancedLogger):
+def print_summary(context: dict, logger: log.EnhancedLogger) -> None:
     summary_items: Dict[SummaryItem, str] = context.get('summary_report', {})
     max_length = max(len(si.text) for si in summary_items.keys())
     logger.info('')
     for si, value in sorted(summary_items.items()):
         key = si.text + ': ' + (' ' * (max_length - len(si.text)))
         logger.info(key + value)
 
 
-def exec_delayed(cluster: KubernetesCluster):
+def exec_delayed(cluster: KubernetesCluster) -> None:
     for call in cluster.context.get('delayed_summary_report', []):
         call(cluster)
```

### Comparing `kubemarine-0.18.2/kubemarine/core/utils.py` & `kubemarine-0.19.0/kubemarine/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,50 +16,42 @@
 import json
 import os
 import shutil
 import sys
 import time
 import tarfile
 
-from typing import Tuple
+from typing import Tuple, Callable, List, IO
 
 import yaml
 import ruamel.yaml
 from copy import deepcopy
 from datetime import datetime
 from collections import OrderedDict
 
 from ruamel.yaml import CommentedMap
 
-from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.errors import pretty_print_error
 
 
 def do_fail(message='', reason: Exception = None, hint='', log=None):
 
-    if log:
-        log.critical('FAILURE!')
-        if message != "":
-            log.critical(message)
-    else:
-        sys.stderr.write("\033[91mFAILURE!")
-        if message != "":
-            sys.stderr.write(" - " + message + "\n")
-
-    pretty_print_error(reason, log)
+    if not log:
+        sys.stderr.write("\033[91m")
 
-    sys.stderr.write("\n")
+    pretty_print_error(message, reason, log)
 
     # Please do not rewrite this to logging approach:
     # hint should be visible only in stdout and without special formatting
     if hint != "":
-        sys.stderr.write(hint)
+        sys.stderr.write("\n")
+        sys.stderr.write(hint + "\n")
 
     if not log:
-        sys.stderr.write("\033[0m\n")
+        sys.stderr.write("\033[0m")
 
     sys.exit(1)
 
 
 def get_elapsed_string(start, end):
     elapsed = end - start
     hours, remainder = divmod(elapsed, 3600)
@@ -70,41 +62,44 @@
 def prepare_dump_directory(location, reset_directory=True):
     dumpdir = os.path.join(location, 'dump')
     if reset_directory and os.path.exists(dumpdir) and os.path.isdir(dumpdir):
         shutil.rmtree(dumpdir)
     os.makedirs(dumpdir, exist_ok=True)
 
 
-def make_ansible_inventory(location, cluster):
+def make_ansible_inventory(location, c):
+    from kubemarine.core.cluster import KubernetesCluster
+    cluster: KubernetesCluster = c
 
     inventory = get_final_inventory(cluster)
     roles = []
     for node in inventory['nodes']:
         for role in node['roles']:
             if role not in roles:
                 roles.append(role)
 
-    config = {
+    config: dict = {
         'all': [
             'localhost ansible_connection=local'
         ],
         'cluster:children': []
     }
 
     already_global_defined = []
 
     for role in roles:
         config[role] = []
         config['cluster:children'].append(role)
-        for node in cluster.nodes[role].get_final_nodes().get_ordered_members_list(provide_node_configs=True):
-            record = "%s ansible_host=%s ansible_ssh_user=%s ansible_ssh_private_key_file=%s ip=%s" % \
+        for node in cluster.nodes[role].get_final_nodes().get_ordered_members_configs_list():
+            record = "%s ansible_host=%s ansible_ssh_user=%s ansible_ssh_pass=%s ansible_ssh_private_key_file=%s ip=%s" % \
                      (node['name'],
                       node['connect_to'],
                       node.get('username', cluster.globals['connection']['defaults']['username']),
-                      node['keyfile'],
+                      node.get('password'),
+                      node.get('keyfile'),
                       node['internal_address'])
             if node.get('address') is not None:
                 record += ' external_ip=%s' % node['address']
 
             if node['name'] not in already_global_defined:
                 config['all'].append(record)
                 # to avoid duplicate definition in global section we have to check is that was already defined?
@@ -155,15 +150,18 @@
     dump_file({}, config_compiled, location, dump_location=False)
 
 
 def get_current_timestamp_formatted():
     return datetime.now().strftime("%Y%m%d-%H%M%S")
 
 
-def get_final_inventory(cluster, initial_inventory=None):
+def get_final_inventory(c, initial_inventory=None):
+    from kubemarine.core.cluster import KubernetesCluster
+    cluster: KubernetesCluster = c
+
     if initial_inventory is None:
         inventory = deepcopy(cluster.inventory)
     else:
         inventory = deepcopy(initial_inventory)
 
     from kubemarine import admission, kubernetes, packages, plugins, thirdparties
     from kubemarine.plugins import nginx_ingress
@@ -227,52 +225,55 @@
 def get_dump_filepath(context, filename):
     if context.get("dump_filename_prefix"):
         filename = f"{context['dump_filename_prefix']}_{filename}"
 
     return get_external_resource_path(os.path.join(context['execution_arguments']['dump_location'], 'dump', filename))
 
 
-def wait_command_successful(group, command, retries=15, timeout=5, warn=True, hide=False, is_async=True):
+def wait_command_successful(g, command, retries=15, timeout=5, warn=True, hide=False):
+    from kubemarine.core.group import NodeGroup
+    group: NodeGroup = g
+
     log = group.cluster.log
 
     while retries > 0:
         log.debug("Waiting for command to succeed, %s retries left" % retries)
-        result = group.sudo(command, warn=warn, hide=hide, is_async=is_async)
+        result = group.sudo(command, warn=warn, hide=hide)
         exit_code = list(result.values())[0].exited
         if exit_code == 0:
             log.debug("Command succeeded")
             return
         retries = retries - 1
         time.sleep(timeout)
     raise Exception("Command failed")
 
 
-def open_utf8(path: str, mode='r'):
+def open_utf8(path: str, mode='r') -> IO:
     return open(path, mode + 't', encoding='utf-8')
 
 
-def open_internal(path: str, mode='r'):
+def open_internal(path: str, mode: str = 'r') -> IO:
     return open_utf8(get_internal_resource_path(path), mode)
 
 
-def open_external(path: str, mode='r'):
+def open_external(path: str, mode: str = 'r') -> IO:
     return open_utf8(get_external_resource_path(path), mode)
 
 
 def read_internal(path: str) -> str:
     with open_internal(path) as f:
         return f.read()
 
 
 def read_external(path: str) -> str:
     with open_external(path) as f:
         return f.read()
 
 
-def get_external_resource_path(path):
+def get_external_resource_path(path: str) -> str:
     return os.path.abspath(path)
 
 
 def get_internal_resource_path(path: str) -> str:
     return os.path.abspath(
         os.path.join(os.path.dirname(__file__), '..', path)
     )
@@ -335,44 +336,46 @@
 def yaml_structure_preserver() -> ruamel.yaml.YAML:
     """YAML loader and dumper which saves original structure"""
     ruamel_yaml = ruamel.yaml.YAML()
     ruamel_yaml.preserve_quotes = True
     return ruamel_yaml
 
 
-def is_sorted(l: list, key: callable = None) -> bool:
+def is_sorted(l: list, key: Callable = None) -> bool:
     """
     Check that the specified list is sorted.
 
     :param l: list to check
     :param key: custom key function to customize the sort order
     :return: boolean flag if the list is sorted
     """
     if key is None:
         key = lambda x: x
     return all(key(l[i]) <= key(l[i + 1]) for i in range(len(l) - 1))
 
 
-def map_sorted(map_: CommentedMap, key: callable = None) -> CommentedMap:
+def map_sorted(map_: CommentedMap, key: Callable = None) -> CommentedMap:
     """
     Check that the specified CommentedMap is sorted, or create new sorted map from it otherwise.
 
     :param map_: CommentedMap instance to check
     :param key: custom key function to customize the sort order of the map keys
     :return: the same or new sorted instance of the map
     """
     if key is None:
-        key = lambda x: x
+        _key = lambda x: x
+    else:
+        _key = key
     map_keys = list(map_)
-    if not is_sorted(map_keys, key=key):
-        map_ = CommentedMap(sorted(map_.items(), key=lambda item: key(item[0])))
+    if not is_sorted(map_keys, key=_key):
+        map_ = CommentedMap(sorted(map_.items(), key=lambda item: _key(item[0])))
 
     return map_
 
-def insert_map_sorted(map_: CommentedMap, k, v, key: callable = None) -> None:
+def insert_map_sorted(map_: CommentedMap, k, v, key: Callable = None) -> None:
     """
     Insert new item to the CommentedMap or update the value for the existing key.
     The map should be already sorted.
 
     :param map_: sorted CommentedMap instance
     :param k: new key
     :param v: new value
@@ -394,17 +397,18 @@
 
 def load_yaml(filepath) -> dict:
     try:
         with open_utf8(filepath, 'r') as stream:
             return yaml.safe_load(stream)
     except yaml.YAMLError as exc:
         do_fail(f"Failed to load {filepath}", exc)
+        return {}  # unreachable
 
 
-def true_or_false(value):
+def true_or_false(value) -> str:
     """
     The method check string and boolean value
     :param value: Value that should be checked
     """
     input_string = str(value)
     if input_string in ['true', 'True', 'TRUE']:
         result = "true"
@@ -415,40 +419,42 @@
     return result
 
 
 def get_version_filepath():
     return get_internal_resource_path("version")
 
 
-def get_version():
+def get_version() -> str:
     return read_internal(get_version_filepath()).strip()
 
 
 def minor_version(version: str) -> str:
     """
     Converts vN.N.N to vN.N
     """
     return 'v' + '.'.join(map(str, _test_version(version, 3)[0:2]))
 
 
 def version_key(version: str) -> Tuple[int, int, int]:
     """
     Converts vN.N.N to (N, N, N) that can be used in comparisons.
     """
-    return tuple(_test_version(version, 3))
+    v = _test_version(version, 3)
+    return v[0], v[1], v[2]
 
 
 def minor_version_key(version: str) -> Tuple[int, int]:
     """
     Converts vN.N to (N, N) that can be used in comparisons.
     """
-    return tuple(_test_version(version, 2))
+    v = _test_version(version, 2)
+    return v[0], v[1]
 
 
-def _test_version(version: str, numbers_amount: int) -> list:
+def _test_version(version: str, numbers_amount: int) -> List[int]:
     # catch version without "v" at the first symbol
     if version.startswith('v'):
         version_list: list = version[1:].split('.')
         # catch invalid version 'v1.16'
         if len(version_list) == numbers_amount:
             # parse str to int and catch invalid symbols in version number
             try:
@@ -499,24 +505,25 @@
         This method packs files with logs and maintains a structured storage of logs on the cluster.
         """
         not_pack_file = self.cluster.inventory['procedure_history']['archive_threshold']
         delete_old = self.cluster.inventory['procedure_history']['delete_threshold']
 
         command = f'ls {self.dir_path} | grep -v latest_dump'
         node_group_results = self.cluster.nodes["control-plane"].get_final_nodes().sudo(command)
-        with RemoteExecutor(self.cluster):
-            for cxn, result in node_group_results.items():
-                control_plane = self.cluster.make_group([cxn.host])
+        with node_group_results.get_group().new_executor() as exe:
+            for control_plane in exe.group.get_ordered_members_list():
+                result = node_group_results[control_plane.get_host()]
                 files = result.stdout.split()
                 files.sort(reverse=True)
                 for i, file in enumerate(files):
                     if i >= not_pack_file and i < delete_old:
                         if 'tar.gz' not in file:
-                            control_plane.sudo(f'tar -czvf {self.dir_path + file + ".tar.gz"} {self.dir_path + file} &&'
-                                       f'sudo rm -r {self.dir_path + file}')
+                            control_plane.sudo(
+                                f'tar -czvf {self.dir_path + file + ".tar.gz"} {self.dir_path + file} &&'
+                                f'sudo rm -r {self.dir_path + file}')
                     elif i >= delete_old:
                         control_plane.sudo(f'rm -rf {self.dir_path + file}')
 
     def compress_and_upload_archive(self):
         """
         This method compose dump files and sends the collected files to the nodes.
         """
@@ -559,20 +566,18 @@
             return
 
         archive_name = 'dump_log_cluster.tar.gz'
         archive_dump_path = get_dump_filepath(self.cluster.context, archive_name)
         archive_remote_path = f"/tmp/{archive_name}"
         log = self.cluster.log
 
-        node = self.cluster.nodes['control-plane'].get_initial_nodes().get_first_member(provide_node_configs=True)
-        control_plane = self.cluster.make_group([node['connect_to']])
+        control_plane = self.cluster.nodes['control-plane'].get_initial_nodes().get_first_member()
         data_copy_res = control_plane.sudo(f'tar -czvf {archive_remote_path} {self.dir_path}')
         log.verbose("Archive with procedures history is created:\n%s" % data_copy_res)
         control_plane.get(archive_remote_path, archive_dump_path)
 
         log.debug("Archive with procedures history is downloaded")
 
-        for new_node in new_control_planes.get_ordered_members_list(provide_node_configs=True):
-            group = self.cluster.make_group([new_node['connect_to']])
+        for group in new_control_planes.get_ordered_members_list():
             group.put(archive_dump_path, archive_remote_path, sudo=True)
             group.sudo(f'tar -C / -xzvf {archive_remote_path}')
-            log.debug(f"Archive with procedures history is uploaded to {new_node['name']!r}")
+            log.debug(f"Archive with procedures history is uploaded to {group.get_node_name()!r}")
```

### Comparing `kubemarine-0.18.2/kubemarine/core/yaml_merger.py` & `kubemarine-0.19.0/kubemarine/core/yaml_merger.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from deepmerge import Merger
+from deepmerge import Merger  # type: ignore[import]
 
 
-def list_merger(config, path, base, nxt):
+def list_merger(config: Merger, path: list, base: list, nxt: list) -> list:
     strategy = None
     strategy_definition_position = 0
     for i, v in enumerate(nxt):
         if isinstance(v, dict) and '<<' in v:
             if strategy is not None:
                 raise Exception(f"Found more than one merge strategy definitions at path {path}.")
             strategy = v.get('<<')
@@ -38,15 +38,15 @@
     if strategy == 'merge':
         nxt.extend(base)
     nxt.extend(elements_after)
 
     return nxt
 
 
-default_merger = Merger(
+default_merger: Merger = Merger(
     [
         (list, [list_merger]),
         (dict, ["merge"])
     ],
     ["override"],
     ["override"]
 )
```

### Comparing `kubemarine-0.18.2/kubemarine/coredns.py` & `kubemarine-0.19.0/kubemarine/coredns.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Union, List, Optional
 
 import yaml
 
 from kubemarine import system
 from kubemarine.core import utils
 
 import io
 
+from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import RunnersGroupResult
+
+
 def proceed_section_keyvalue(data, tabsize):
     tab = " "*tabsize
     config = ''
 
     for key, value in data.items():
         if isinstance(value, bool):
             if value:
@@ -86,15 +91,15 @@
         elif type == 'hosts':
             config += '\n' + tab + type
             if data[section['name']].get('file') and isinstance(data[section['name']]['file'], str):
                 config += ' ' + data[section['name']]['file']
             config += ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2) + '\n' + tab + '}'
 
         elif type == 'template':
-            zones = [None]
+            zones: Union[str, List[Optional[str]]] = [None]
             if data[section['name']].get('zone'):
                 zones = data[section['name']]['zone']
                 if isinstance(zones, str):
                     zones = [zones]
             for zone in zones:
                 config += '\n' + tab + type
                 if data[section['name']].get('class'):
@@ -108,15 +113,15 @@
         else:
             config += '\n' + tab + type + ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2)\
                       + '\n' + tab + '}'
 
     return config
 
 
-def generate_configmap(inventory):
+def generate_configmap(inventory: dict) -> str:
     # coredns.configmap.Hosts must exist even if it's empty
     if not inventory['services']['coredns']['configmap'].get('Hosts'):
         # Hosts must exist even if it's empty
         inventory['services']['coredns']['configmap']['Hosts'] = ""
 
     config = '''apiVersion: v1
 
@@ -139,26 +144,26 @@
         if config_type == 'Hosts' and inventory['services']['coredns']['add_etc_hosts_generated']:
             config += '\n    '
             config += system.generate_etc_hosts_config(inventory,etc_hosts_part='etc_hosts_generated').replace('\n', '\n    ')
 
     return config + '\n'
 
 
-def apply_configmap(cluster, config):
+def apply_configmap(cluster: KubernetesCluster, config: str) -> RunnersGroupResult:
     utils.dump_file(cluster, config, 'coredns-configmap.yaml')
 
-    group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_final_nodes()
+    group = cluster.make_group_from_roles(['control-plane', 'worker']).get_final_nodes()
     group.put(io.StringIO(config), '/etc/kubernetes/coredns-configmap.yaml', backup=True, sudo=True)
 
     return cluster.nodes['control-plane'].get_final_nodes().get_first_member()\
         .sudo('kubectl apply -f /etc/kubernetes/coredns-configmap.yaml && '
              'sudo kubectl rollout restart -n kube-system deployment/coredns')
 
 
-def apply_patch(cluster):
+def apply_patch(cluster: KubernetesCluster) -> Union[RunnersGroupResult, str]:
     apply_command = ''
 
     for config_type in ['deployment']:
 
         if not cluster.inventory['services']['coredns'].get(config_type):
             continue
 
@@ -167,15 +172,15 @@
 
         config = yaml.dump(cluster.inventory['services']['coredns'][config_type])
         filename = 'coredns-%s-patch.yaml' % config_type
         filepath = '/etc/kubernetes/' + filename
 
         utils.dump_file(cluster, config, filename)
 
-        group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_final_nodes()
+        group = cluster.make_group_from_roles(['control-plane', 'worker']).get_final_nodes()
         group.put(io.StringIO(config), filepath, backup=True, sudo=True)
 
         apply_command = 'kubectl patch %s coredns -n kube-system --type merge -p \"$(sudo cat %s)\"' % (config_type, filepath)
 
     if apply_command == '':
         return 'Nothing to patch'
```

### Comparing `kubemarine-0.18.2/kubemarine/cri/__init__.py` & `kubemarine-0.19.0/kubemarine/cri/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
+
 from kubemarine.core import static
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import NodeGroupResult
+from kubemarine.core.group import RunnersGroupResult, NodeGroup
 from kubemarine.cri import docker, containerd
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get("initial_procedure") == "migrate_cri":
         return inventory
 
     cri_impl = inventory['services']['cri']['containerRuntime']
     if cri_impl == "docker":
         forbidden_cri_sections = {"containerd": "containerdConfig"}
     else:
@@ -30,53 +32,53 @@
         if value in cluster.raw_inventory.get('services', {}).get('cri', {}):
             raise Exception(f"{key} is not used, please remove {value} config from `services.cri` section")
 
     return inventory
 
 
 def get_initial_cri_impl(inventory: dict) -> str:
-    cri_impl = inventory.get("services", {}).get("cri", {}).get("containerRuntime")
+    cri_impl: Optional[str] = inventory.get("services", {}).get("cri", {}).get("containerRuntime")
     if cri_impl is None:
         cri_impl = static.DEFAULTS['services']['cri']['containerRuntime']
 
     return cri_impl
 
 
-def remove_invalid_cri_config(cluster: KubernetesCluster, inventory: dict):
+def remove_invalid_cri_config(cluster: KubernetesCluster, inventory: dict) -> dict:
     if inventory['services']['cri']['containerRuntime'] == 'docker':
         if inventory['services']['cri'].get('containerdConfig'):
             del inventory['services']['cri']['containerdConfig']
     elif inventory['services']['cri'].get('dockerConfig'):
         del inventory['services']['cri']['dockerConfig']
 
     return inventory
 
 
-def install(group):
+def install(group: NodeGroup) -> RunnersGroupResult:
     cri_impl = group.cluster.inventory['services']['cri']['containerRuntime']
 
     if cri_impl == "docker":
         return docker.install(group)
     else:
         return containerd.install(group)
 
 
-def configure(group):
+def configure(group: NodeGroup) -> RunnersGroupResult:
     cri_impl = group.cluster.inventory['services']['cri']['containerRuntime']
 
     if cri_impl == "docker":
         return docker.configure(group)
     else:
         return containerd.configure(group)
 
 
-def prune(group, all_implementations=False):
+def prune(group: NodeGroup, all_implementations: bool = False) -> RunnersGroupResult:
     cri_impl = group.cluster.inventory['services']['cri']['containerRuntime']
 
-    result = NodeGroupResult(group.cluster)
+    result = RunnersGroupResult(group.cluster, {})
     if cri_impl == "docker" or all_implementations:
-        result.update(docker.prune(group))
+        result = docker.prune(group)
 
     if cri_impl == "containerd" or all_implementations:
-        result.update(containerd.prune(group))
+        result = containerd.prune(group)
 
     return result
```

### Comparing `kubemarine-0.18.2/kubemarine/cri/containerd.py` & `kubemarine-0.19.0/kubemarine/cri/containerd.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,55 +9,59 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from io import StringIO
+from typing import Dict
 
 import toml
 import yaml
 import json
 
 from distutils.util import strtobool
 from kubemarine import system, packages
 from kubemarine.core import utils
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup
+from kubemarine.core.group import NodeGroup, RunnersGroupResult, CollectorCallback
 
 
-def install(group: NodeGroup):
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            os_specific_associations = group.cluster.get_associations_for_node(node['connect_to'], 'containerd')
+def install(group: NodeGroup) -> RunnersGroupResult:
+    collector = CollectorCallback(group.cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            os_specific_associations = exe.cluster.get_associations_for_node(node.get_host(), 'containerd')
 
-            group.cluster.log.debug("Installing latest containerd and podman on %s node" % node['name'])
+            exe.cluster.log.debug("Installing latest containerd and podman on %s node" % node.get_node_name())
             # always install latest available containerd and podman
-            packages.install(node['connection'], include=os_specific_associations['package_name'])
+            packages.install(node, include=os_specific_associations['package_name'], callback=collector)
 
             # remove previous config.toml to avoid problems in case when previous config was broken
-            node['connection'].sudo("rm -f %s && sudo systemctl restart %s"
-                                    % (os_specific_associations['config_location'],
-                                       os_specific_associations['service_name']))
+            node.sudo("rm -f %s && sudo systemctl restart %s"
+                      % (os_specific_associations['config_location'],
+                         os_specific_associations['service_name']),
+                      callback=collector)
+
+            system.enable_service(node, os_specific_associations['service_name'],
+                                  now=True, callback=collector)
+    return collector.result
 
-            system.enable_service(node['connection'], os_specific_associations['service_name'], now=True)
-    return exe.get_last_results_str()
 
-
-def configure(group: NodeGroup):
-    log = group.cluster.log
+def configure(group: NodeGroup) -> RunnersGroupResult:
+    cluster = group.cluster
+    log = cluster.log
 
     log.debug("Uploading crictl configuration for containerd...")
     crictl_config = yaml.dump({"runtime-endpoint": "unix:///run/containerd/containerd.sock"})
-    utils.dump_file(group.cluster, crictl_config, 'crictl.yaml')
+    utils.dump_file(cluster, crictl_config, 'crictl.yaml')
     group.put(StringIO(crictl_config), '/etc/crictl.yaml', backup=True, sudo=True)
 
     config_string = ""
     # double loop is used to make sure that no "simple" `key: value` pairs are accidentally assigned to sections
-    containerd_config = group.cluster.inventory["services"]["cri"]['containerdConfig']
+    containerd_config = cluster.inventory["services"]["cri"]['containerdConfig']
     runc_options_path = 'plugins."io.containerd.grpc.v1.cri".containerd.runtimes.runc.options'
     if not isinstance(containerd_config[runc_options_path]['SystemdCgroup'], bool):
         containerd_config[runc_options_path]['SystemdCgroup'] = \
             bool(strtobool(containerd_config[runc_options_path]['SystemdCgroup']))
     for key, value in containerd_config.items():
         # first we process all "simple" `key: value` pairs
         if not isinstance(value, dict):
@@ -77,46 +81,48 @@
             for endpoint in mirror_conf.get('endpoint', []):
                 if "http://" in endpoint:
                     is_insecure = True
                     break
             if is_insecure:
                 insecure_registries.append(mirror)
     # save 'auth.json' if there are credentials for registry
-    auth_registries = {"auths": {}}
+    auth_registries: Dict[str, dict] = {"auths": {}}
     if registry.get('configs'):
         registry_configs = registry['configs']
         for auth_registry in registry_configs:
             auth_registries['auths'][auth_registry] = {}
             if registry_configs[auth_registry].get('auth', {}).get('auth', ''):
                 auth_registries['auths'][auth_registry]['auth'] = registry_configs[auth_registry]['auth']['auth']
         auth_json = json.dumps(auth_registries)
         group.put(StringIO(auth_json), "/etc/containers/auth.json", backup=True, sudo=True)
         group.sudo("chmod 600 /etc/containers/auth.json")
     if insecure_registries:
         log.debug("Uploading podman configuration...")
         podman_registries = f"[registries.insecure]\nregistries = {insecure_registries}\n"
-        utils.dump_file(group.cluster, podman_registries, 'podman_registries.conf')
+        utils.dump_file(cluster, podman_registries, 'podman_registries.conf')
         group.sudo("mkdir -p /etc/containers/")
         group.put(StringIO(podman_registries), "/etc/containers/registries.conf", backup=True, sudo=True)
     else:
         log.debug("Removing old podman configuration...")
         group.sudo("rm -f /etc/containers/registries.conf")
 
-    utils.dump_file(group.cluster, config_string, 'containerd-config.toml')
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            os_specific_associations = group.cluster.get_associations_for_node(node['connect_to'], 'containerd')
-            log.debug("Uploading containerd configuration to %s node..." % node['name'])
-            node['connection'].put(StringIO(config_string), os_specific_associations['config_location'], backup=True,
-                                   sudo=True, mkdir=True)
-            log.debug("Restarting Containerd on %s node..." % node['name'])
-            node['connection'].sudo(f"chmod 600 {os_specific_associations['config_location']} && "
-                                    f"sudo systemctl restart {os_specific_associations['service_name']} && "
-                                    f"systemctl status {os_specific_associations['service_name']}")
-    return exe.get_last_results_str()
+    utils.dump_file(cluster, config_string, 'containerd-config.toml')
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            os_specific_associations = exe.cluster.get_associations_for_node(node.get_host(), 'containerd')
+            log.debug("Uploading containerd configuration to %s node..." % node.get_node_name())
+            node.put(StringIO(config_string), os_specific_associations['config_location'],
+                     backup=True, sudo=True, mkdir=True)
+            log.debug("Restarting Containerd on %s node..." % node.get_node_name())
+            node.sudo(
+                f"chmod 600 {os_specific_associations['config_location']} && "
+                f"sudo systemctl restart {os_specific_associations['service_name']} && "
+                f"systemctl status {os_specific_associations['service_name']}", callback=collector)
+    return collector.result
 
 
-def prune(group):
+def prune(group: NodeGroup) -> RunnersGroupResult:
     return group.sudo('crictl rm -fa; '
                       'sudo crictl rmp -fa; '
                       'sudo crictl rmi -a; '
                       'sudo ctr content ls -q | xargs -r sudo ctr content rm', warn=True)
```

### Comparing `kubemarine-0.18.2/kubemarine/cri/docker.py` & `kubemarine-0.19.0/kubemarine/cri/docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,67 +13,72 @@
 # limitations under the License.
 
 import json
 from io import StringIO
 
 from kubemarine import system, packages
 from kubemarine.core import utils
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup
+from kubemarine.core.group import NodeGroup, RunnersGroupResult, CollectorCallback
 
 
-def install(group: NodeGroup):
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            os_specific_associations = group.cluster.get_associations_for_node(node['connect_to'], 'docker')
-            packages.install(node['connection'], include=os_specific_associations['package_name'])
-            enable(node['connection'])
+def install(group: NodeGroup) -> RunnersGroupResult:
+    cluster = group.cluster
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            os_specific_associations = cluster.get_associations_for_node(node.get_host(), 'docker')
+            packages.install(node, include=os_specific_associations['package_name'], callback=collector)
+
+            system.enable_service(node, name=os_specific_associations['service_name'],
+                                  now=True, callback=collector)
 
             # remove previous daemon.json to avoid problems in case when previous config was broken
-            node['connection'].sudo("rm -f %s && sudo systemctl restart %s"
-                                % (os_specific_associations['config_location'],
-                                   os_specific_associations['service_name']))
-    return exe.get_last_results_str()
+            node.sudo("rm -f %s && sudo systemctl restart %s"
+                      % (os_specific_associations['config_location'],
+                         os_specific_associations['service_name']),
+                      callback=collector)
+    return collector.result
 
 
-def uninstall(group):
+def uninstall(group: NodeGroup) -> RunnersGroupResult:
     # delete all known docker packages
     return packages.remove(group, include=['docker', 'docker-engine', 'docker.io', 'docker-ce'])
 
 
-def enable(group: NodeGroup):
-    # currently it is invoked only for single node
-    service_name = group.cluster.get_package_association_for_node(group.get_host(), 'docker', 'service_name')
-    system.enable_service(group, name=service_name, now=True)
-
-
-def disable(group: NodeGroup):
-    service_name = group.cluster.get_package_association_for_node(group.get_host(), 'docker', 'service_name')
-    system.disable_service(group, name=service_name, now=True)
-
-
-def configure(group: NodeGroup):
-    log = group.cluster.log
-
-    settings_json = json.dumps(group.cluster.inventory["services"]['cri']['dockerConfig'], sort_keys=True, indent=4)
-    utils.dump_file(group.cluster, settings_json, 'docker-daemon.json')
-
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            os_specific_associations = group.cluster.get_associations_for_node(node['connect_to'], 'docker')
-            log.debug("Uploading docker configuration to %s node..." % node['name'])
-            node['connection'].put(StringIO(settings_json), os_specific_associations['config_location'], backup=True,
-                                   sudo=True)
-            log.debug("Restarting Docker on %s node..." % node['name'])
-            node['connection'].sudo(f"chmod 600 {os_specific_associations['config_location']} && "
-                                    f"sudo systemctl restart {os_specific_associations['service_name']} && "
-                                    f"sudo {os_specific_associations['executable_name']} info")
+def disable(group: NodeGroup) -> None:
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            service_name = exe.cluster.get_package_association_for_node(
+                node.get_host(), 'docker', 'service_name')
+            system.disable_service(node, name=service_name, now=True)
+
+
+def configure(group: NodeGroup) -> RunnersGroupResult:
+    cluster = group.cluster
+    log = cluster.log
+
+    settings_json = json.dumps(cluster.inventory["services"]['cri']['dockerConfig'], sort_keys=True, indent=4)
+    utils.dump_file(cluster, settings_json, 'docker-daemon.json')
+
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            os_specific_associations = exe.cluster.get_associations_for_node(node.get_host(), 'docker')
+            log.debug("Uploading docker configuration to %s node..." % node.get_node_name())
+            node.put(StringIO(settings_json), os_specific_associations['config_location'],
+                     backup=True, sudo=True)
+            log.debug("Restarting Docker on %s node..." % node.get_node_name())
+            node.sudo(
+                f"chmod 600 {os_specific_associations['config_location']} && "
+                f"sudo systemctl restart {os_specific_associations['service_name']} && "
+                f"sudo {os_specific_associations['executable_name']} info",
+                callback=collector)
 
-    return exe.get_last_results_str()
+    return collector.result
 
 
-def prune(group):
+def prune(group: NodeGroup) -> RunnersGroupResult:
     return group.sudo('docker container stop $(sudo docker container ls -aq); '
                       'sudo docker container rm $(sudo docker container ls -aq); '
                       'sudo docker system prune -a -f; '
                       # kill all containerd-shim processes, so that no orphan containers remain 
-                      'sudo pkill -9 -f "^containerd-shim"', warn=True, hide=True)
+                      'sudo pkill -9 -f "^containerd-shim"', warn=True)
```

### Comparing `kubemarine-0.18.2/kubemarine/demo.py` & `kubemarine-0.19.0/kubemarine/demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,71 +7,71 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from __future__ import annotations
+
 import argparse
 import io
 import re
 import threading
+import time
+from abc import ABC
 from copy import deepcopy
-from typing import List, Dict, Union, Any, IO, Optional
+from typing import List, Dict, Union, Any, Optional, Mapping, Iterable, IO
 
-import fabric
-from invoke import UnexpectedExit
+import fabric  # type: ignore[import]
+import invoke
 
 from kubemarine import system
-from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core import group, flow, connections
-from kubemarine.core.connections import Connections
-from kubemarine.core.group import NodeGroup, NodeGroupResult, _GenericResult, _HostToResult
+from kubemarine.core.cluster import KubernetesCluster, _AnyConnectionTypes
+from kubemarine.core import flow, connections, static
+from kubemarine.core.connections import ConnectionPool
+from kubemarine.core.executor import RunnersResult, GenericResult, Token, CommandTimedOut
+from kubemarine.core.group import (
+    AbstractGroup, NodeGroup, NodeGroupResult, DeferredGroup, RunnersGroupResult,
+    GROUP_RUN_TYPE, RemoteExecutor, RunResult
+)
 from kubemarine.core.resources import DynamicResources
 
-ShellResult = Dict[str, Union[NodeGroupResult, Any]]
+_ShellResult = Dict[str, Any]
+_ROLE_SPEC = Union[int, List[str]]
 
 
 class FakeShell:
     def __init__(self):
-        self.results: Dict[str, List[ShellResult]] = {}
-        self.history: Dict[str, List[ShellResult]] = {}
+        self.results: Dict[str, List[_ShellResult]] = {}
+        self.history: Dict[str, List[_ShellResult]] = {}
         self._lock = threading.Lock()
 
-    def __deepcopy__(self, memodict: dict):
-        cls = self.__class__
-        result = cls.__new__(cls)
-        memodict[id(self)] = result
-        result.results = deepcopy(self.results, memodict)
-        result.history = deepcopy(self.history, memodict)
-        result._lock = threading.Lock()
-        return result
-
     def reset(self):
         self.results = {}
         self.history = {}
 
-    def add(self, results: Union[NodeGroupResult, _HostToResult], do_type, args, usage_limit=0):
+    def add(self, results: Mapping[str, GenericResult], do_type, args, usage_limit=0):
         args.sort()
 
         for host, result in results.items():
-            host = host.host if isinstance(host, fabric.connection.Connection) else host
             result = {
                 'result': result,
                 'do_type': do_type,
                 'args': args,
                 'used_times': 0
             }
 
             if usage_limit > 0:
                 result['usage_limit'] = usage_limit
 
             self.results.setdefault(host, []).append(result)
 
-    def find(self, host: str, do_type, args, kwargs) -> _GenericResult:
+    def find(self, host: str, do_type, args, kwargs) -> GenericResult:
         # TODO: Support kwargs
         with self._lock:
             if isinstance(args, tuple):
                 args = list(args)
             results = self.results.get(host, [])
             for i, item in enumerate(results):
                 if item['do_type'] == do_type and item['args'] == args:
@@ -112,47 +112,58 @@
         found_entries = self.history_find(host, do_type, args)
         return sum(found_entry['used_times'] for found_entry in found_entries) > 0
 
 
 class FakeFS:
     def __init__(self):
         self.storage: Dict[str, Dict[str, str]] = {}
+        self.emulate_latency = False
         self._lock = threading.Lock()
 
-    def __deepcopy__(self, memodict: dict):
-        cls = self.__class__
-        result = cls.__new__(cls)
-        memodict[id(self)] = result
-        result.storage = deepcopy(self.storage, memodict)
-        result._lock = threading.Lock()
-        return result
-
     def reset(self):
         self.storage = {}
+        self.emulate_latency = False
 
     def reset_host(self, host):
         self.storage[host] = {}
 
-    # covered by test.test_demo.TestFakeFS.test_put_string
-    # covered by test.test_demo.TestFakeFS.test_put_stringio
-    # covered by test.test_demo.TestFakeFS.test_write_file_to_cluster
+    # covered by test.test_demo.TestFakeFS.test_put_file
+    # covered by test.test_demo.TestFakeFS.test_put_bytesio
+    # covered by test.test_group.TestGroupCall.test_write_stream
     def write(self, host, filename, data):
+        if isinstance(data, io.BytesIO):
+            # Emulate how fabric handles file-like objects.
+            # See fabric.transfer.Transfer.put
+            pointer = data.tell()
+            try:
+                data.seek(0)
+                text = self._transfer(data)
+            finally:
+                data.seek(pointer)
+        elif isinstance(data, str):
+            with open(data, "rb") as fl:
+                text = self._transfer(fl)
+        else:
+            raise ValueError("Unsupported data type " + str(type(data)))
+
         with self._lock:
-            if isinstance(data, io.BytesIO):
-                data = data.getvalue().decode('utf-8')
-            elif isinstance(data, str):
-                # this is for self-testing purpose
-                pass
-            elif isinstance(data, io.IOBase):
-                data = data.read().decode('utf-8')
-            else:
-                raise ValueError("Unsupported data type " + str(type(data)))
-            if self.storage.get(host) is None:
-                self.storage[host] = {}
-            self.storage[host][filename] = data
+            self.storage.setdefault(host, {})[filename] = text
+
+    def _transfer(self, fl: IO) -> str:
+        # Emulate how paramiko transfers files.
+        # See paramiko.sftp_client.SFTPClient._transfer_with_callback
+        target = io.BytesIO()
+        while True:
+            data = fl.read(32768)
+            target.write(data)
+            if self.emulate_latency:
+                time.sleep(0.1)
+            if len(data) == 0:
+                break
+        return target.getvalue().decode('utf-8')
 
     # covered by test.test_demo.TestFakeFS.test_put_string
     # covered by test.test_demo.TestFakeFS.test_get_nonexistent
     def read(self, host, filename):
         return self.storage.get(host, {}).get(filename)
 
     # covered by test.test_demo.TestFakeFS.test_write_file_to_cluster
@@ -175,19 +186,24 @@
 
 class FakeKubernetesCluster(KubernetesCluster):
 
     def __init__(self, *args, **kwargs):
         self.fake_shell = kwargs.pop("fake_shell", FakeShell())
         self.fake_fs = kwargs.pop("fake_fs", FakeFS())
         super().__init__(*args, **kwargs)
-        self._connection_pool = FakeConnectionPool(self)
 
-    def make_group(self, ips) -> NodeGroup:
-        nodegroup = super().make_group(ips)
-        return FakeNodeGroup(nodegroup.nodes, self)
+    @property
+    def connection_pool(self) -> ConnectionPool:
+        if self._connection_pool is None:
+            self._connection_pool = FakeConnectionPool(self.inventory, self.fake_shell, self.fake_fs)
+
+        return self._connection_pool
+
+    def make_group(self, ips: Iterable[_AnyConnectionTypes]) -> FakeNodeGroup:
+        return FakeNodeGroup(ips, self)
 
     def dump_finalized_inventory(self):
         return
 
     def preserve_inventory(self):
         return
 
@@ -202,43 +218,41 @@
         self.stored_inventory = raw_inventory
         self.last_cluster: Optional[FakeKubernetesCluster] = None
         self.fake_shell = fake_shell if fake_shell else FakeShell()
         self.fake_fs = fake_fs if fake_fs else FakeFS()
         self._nodes_context = nodes_context
         self._procedure_inventory = procedure_inventory
 
-    def _load_inventory(self):
+    def _load_inventory(self) -> None:
         self._raw_inventory = deepcopy(self.stored_inventory)
         self._formatted_inventory = deepcopy(self.stored_inventory)
 
-    def _store_inventory(self):
-        self.stored_inventory = deepcopy(self._formatted_inventory)
+    def _store_inventory(self) -> None:
+        self.stored_inventory = deepcopy(self.formatted_inventory())
 
     def _new_cluster_instance(self, context: dict) -> FakeKubernetesCluster:
         self.last_cluster = FakeKubernetesCluster(
             self.raw_inventory(), context,
             procedure_inventory=self.procedure_inventory(), logger=self.logger(),
             fake_shell=self.fake_shell, fake_fs=self.fake_fs
         )
         return self.last_cluster
 
 
-class FakeConnection(fabric.connection.Connection):
+class FakeConnection(fabric.connection.Connection):  # type: ignore[misc]
 
-    def __init__(self, ip, cluster: FakeKubernetesCluster, **kw):
+    def __init__(self, ip, fake_shell: FakeShell, fake_fs: FakeFS, **kw):
         super().__init__(ip, **kw)
-        self.fake_shell = cluster.fake_shell
-        self.fake_fs = cluster.fake_fs
+        self.fake_shell = fake_shell
+        self.fake_fs = fake_fs
 
         command_sep = r'[=\-_]{32}'
         sep_symbol = r'\&\&|;'
         final_sep = rf" ({sep_symbol}) " \
-                    rf"echo \"({command_sep})\" \1 " \
-                    rf"echo \$\? \1 " \
-                    rf"echo \"\2\" \1 " \
+                    rf"printf \"%s\\n\$\?\\n%s\\n\" \"({command_sep})\" \"\2\" \1 " \
                     rf"echo \"\2\" 1>\&2 \1 (sudo )?"
 
         self.separator_ptrn = re.compile(final_sep)
 
     def __setattr__(self, key, value):
         # fabric Connection has special handling of this method. Call default behaviour for custom attributes.
         if key in ('fake_shell', 'fake_fs', 'separator_ptrn'):
@@ -257,53 +271,57 @@
 
     def put(self, *args, **kwargs):
         return self._do("put", *args, **kwargs)
 
     def _do(self, do_type, *args, **kwargs) -> fabric.runners.Result:
         if do_type in ['sudo', 'run']:
             # start fake execution of commands
-            command = list(args)[0]
-            commands, sep_symbol, command_sep = self._split_command(do_type, command)
+            original_command = list(args)[0]
+            commands, sep_symbol, command_sep = self._split_command(do_type, original_command)
 
-            stdout = ""
-            stderr = ""
+            final_res = fabric.runners.Result(stdout="", stderr="", exited=None,
+                                              connection=self, command=original_command)
             prev_exited = None
             i = 0
             for command in commands:
                 found_result = self.fake_shell.find(self.host, do_type, [command], kwargs)
 
                 if found_result is None:
                     raise Exception('Fake result not found for requested action type \'%s\' and command %s' % (do_type, [command]))
 
+                timeout_exception = None
                 if isinstance(found_result, Exception):
                     if i > 0:
                         raise ValueError("Exception can be thrown only for the whole command")
+                    elif isinstance(found_result, CommandTimedOut):
+                        timeout_exception = found_result
+                        found_result = found_result.result
                     else:
                         raise found_result
 
                 if i > 0:
-                    stdout += command_sep + '\n' + str(prev_exited) + '\n' + command_sep + '\n'
-                    stderr += command_sep + '\n'
+                    final_res.stdout += command_sep + '\n' + str(prev_exited) + '\n' + command_sep + '\n'
+                    final_res.stderr += command_sep + '\n'
                 i += 1
 
-                stdout += found_result.stdout
-                stderr += found_result.stderr
-                prev_exited = found_result.exited
-                if prev_exited != 0:
-                    if sep_symbol == ';':
-                        prev_exited = 0  # todo bug of RemoteExecutor
-                    else:
-                        # stop fake execution
-                        break
+                final_res.stdout += found_result.stdout
+                final_res.stderr += found_result.stderr
+                final_res.exited = prev_exited = found_result.exited
+
+                if timeout_exception is not None:
+                    raise invoke.CommandTimedOut(final_res, timeout_exception.timeout)
+
+                if prev_exited != 0 and sep_symbol != ';':
+                    # stop fake execution
+                    break
 
-            final_res = fabric.runners.Result(stdout=stdout, stderr=stderr, exited=prev_exited, connection=self)
             if prev_exited == 0 or kwargs.get('warn', False):
                 return final_res
 
-            raise UnexpectedExit(final_res)
+            raise invoke.UnexpectedExit(final_res)
 
         elif do_type == 'put':
             # It should return fabric.transfer.Result, but currently returns None.
             # Transfer Result is currently never handled.
             return self.fake_fs.write(self.host, args[1], args[0])
 
         raise Exception('Unsupported do type')
@@ -335,46 +353,54 @@
         else:
             raise ValueError(msg)
 
     def close(self):
         pass
 
 
-class FakeNodeGroup(group.NodeGroup):
+class FakeAbstractGroup(AbstractGroup[GROUP_RUN_TYPE], ABC):
+    def _put_with_mv(self, local_stream: Union[io.BytesIO, str], remote_file: str,
+                     backup=False, sudo=False, mkdir=False, immutable=False):
+        super()._put_with_mv(local_stream, remote_file, backup=False, sudo=False, mkdir=False, immutable=False)
+
+
+class FakeNodeGroup(NodeGroup, FakeAbstractGroup[RunnersGroupResult]):
+    def _make_group(self, ips: Iterable[Union[str, NodeGroup]]) -> FakeNodeGroup:
+        return FakeNodeGroup(ips, self.cluster)
 
-    def __init__(self, connections: Connections, cluster_: FakeKubernetesCluster):
-        super().__init__(connections, cluster_)
+    def _make_defer(self, executor: RemoteExecutor) -> FakeDeferredGroup:
+        return FakeDeferredGroup(self.nodes, self.cluster, executor)
 
-    def get_local_file_sha1(self, filename):
+    def get_local_file_sha1(self, filename: str) -> str:
         return '0'
 
-    def get_remote_file_sha1(self, filename):
-        return {host: '1' for host in self.nodes.keys()}
+    def get_remote_file_sha1(self, filename: str) -> Dict[str, Optional[str]]:
+        return {host: '1' for host in self.nodes}
 
-    def _put(self, local_stream: IO, remote_file: str, **kwargs):
-        kwargs.pop("sudo", None)
-        kwargs.pop("backup", None)
-        kwargs.pop("immutable", None)
-        super()._put(local_stream, remote_file, **kwargs)
+
+class FakeDeferredGroup(DeferredGroup, FakeAbstractGroup[Token]):
+    def _make_group(self, ips: Iterable[Union[str, DeferredGroup]]) -> FakeDeferredGroup:
+        return FakeDeferredGroup(ips, self.cluster, self._executor)
 
 
 class FakeConnectionPool(connections.ConnectionPool):
-    def __init__(self, cluster: FakeKubernetesCluster):
-        super().__init__(cluster)
-        self.cluster = cluster
+    def __init__(self, inventory: dict, fake_shell: FakeShell, fake_fs: FakeFS):
+        super().__init__(inventory)
+        self.fake_shell = fake_shell
+        self.fake_fs = fake_fs
 
     def _create_connection_from_details(self, ip: str, conn_details: dict, gateway=None, inline_ssh_env=True):
         return FakeConnection(
-            ip, self.cluster,
-            user=conn_details.get('username', self._env.globals['connection']['defaults']['username']),
-            port=conn_details.get('connection_port', self._env.globals['connection']['defaults']['port'])
+            ip, self.fake_shell, self.fake_fs,
+            user=conn_details.get('username', static.GLOBALS['connection']['defaults']['username']),
+            port=conn_details.get('connection_port', static.GLOBALS['connection']['defaults']['port'])
         )
 
 
-def create_silent_context(args: list = None, parser: argparse.ArgumentParser = None, procedure: str = None):
+def create_silent_context(args: list = None, parser: argparse.ArgumentParser = None, procedure='install'):
     args = list(args) if args else []
     # todo probably increase logging level to get rid of spam in logs.
     if '--disable-dump' not in args:
         args.append('--disable-dump')
 
     if parser is None:
         parser = flow.new_common_parser("Help text")
@@ -391,14 +417,15 @@
         context = create_silent_context()
 
     nodes_context = generate_nodes_context(inventory)
     nodes_context.update(context['nodes'])
     context['nodes'] = nodes_context
 
     # It is possible to disable FakeCluster and create real cluster Object for some business case
+    cluster: KubernetesCluster
     if fake:
         cluster = FakeKubernetesCluster(inventory, context, procedure_inventory=procedure_inventory)
     else:
         cluster = KubernetesCluster(inventory, context, procedure_inventory=procedure_inventory)
 
     cluster.enrich()
     return cluster
@@ -426,28 +453,29 @@
         if node.get('address'):
             connect_to = node['address']
         context[connect_to] = node_context
 
     return context
 
 
-def generate_inventory(balancer=1, master=1, worker=1, keepalived=0, haproxy_mntc=0):
+def generate_inventory(balancer: _ROLE_SPEC = 1, master: _ROLE_SPEC = 1, worker: _ROLE_SPEC = 1,
+                       keepalived: _ROLE_SPEC = 0, haproxy_mntc: _ROLE_SPEC = 0) -> dict:
     inventory: dict = {
         'node_defaults': {
             'keyfile': '/dev/null',
             'username': 'anonymous'
         },
         'nodes': [],
         'services': {
             'cri': {}
         },
         'cluster_name': 'k8s.fake.local'
     }
 
-    id_roles_map = {}
+    id_roles_map: Dict[str, List[str]] = {}
 
     for role_name in ['balancer', 'master', 'worker']:
 
         item = locals()[role_name]
 
         if isinstance(item, int):
             ids = []
@@ -474,25 +502,25 @@
             'name': id_,
             'address': '10.101.1.%s' % ip_i,
             'internal_address': '192.168.0.%s' % ip_i,
             'roles': roles
         })
 
     ip_i = 0
-    vrrp_ips = []
+    vrrp_ips: List[Union[str, dict]] = []
 
     if isinstance(keepalived, list):
-        vrrp_ips.append(deepcopy(keepalived))
+        vrrp_ips.extend(deepcopy(keepalived))
     elif isinstance(keepalived, int) and keepalived > 0:
         for _ in range(keepalived):
             ip_i = ip_i + 1
             vrrp_ips.append('10.101.2.%s' % ip_i)
 
     if isinstance(haproxy_mntc, list):
-        vrrp_ips.append(deepcopy(haproxy_mntc))
+        vrrp_ips.extend(deepcopy(haproxy_mntc))
     elif isinstance(haproxy_mntc, int) and haproxy_mntc > 0:
         for _ in range(haproxy_mntc):
             ip_i = ip_i + 1
             vrrp_ips.append({
                 'ip': '10.101.2.%s' % ip_i,
                 'params': {
                     'maintenance-type': 'not bind'
@@ -509,34 +537,46 @@
         }
 
     inventory['vrrp_ips'] = vrrp_ips
 
     return inventory
 
 
-def create_exception_result(group_: NodeGroup, exception: Exception) -> NodeGroupResult:
-    return NodeGroupResult(group_.cluster, create_hosts_exception_result(group_.get_hosts(), exception))
+def create_nodegroup_result_by_hosts(cluster: KubernetesCluster, results: Dict[str, GenericResult]) -> NodeGroupResult:
+    return NodeGroupResult(cluster, results)
+
+
+def create_exception_result(group_: AbstractGroup[RunResult], exception: Exception) -> NodeGroupResult:
+    hosts_to_result = create_hosts_exception_result(group_.get_hosts(), exception)
+    return create_nodegroup_result_by_hosts(group_.cluster, hosts_to_result)
 
 
-def create_hosts_exception_result(hosts: List[str], exception: Exception) -> _HostToResult:
+def create_hosts_exception_result(hosts: List[str], exception: Exception) -> Dict[str, GenericResult]:
     return {host: exception for host in hosts}
 
 
-def create_nodegroup_result(group_: NodeGroup, stdout='', stderr='', code=0) -> NodeGroupResult:
-    return NodeGroupResult(group_.cluster, create_hosts_result(group_.get_hosts(), stdout, stderr, code))
+def create_nodegroup_result(group_: AbstractGroup[RunResult], stdout='', stderr='',
+                            code=0, timeout: int = None) -> NodeGroupResult:
+    hosts_to_result = create_hosts_result(group_.get_hosts(), stdout, stderr, code, timeout)
+    return create_nodegroup_result_by_hosts(group_.cluster, hosts_to_result)
 
 
-def create_hosts_result(hosts: List[str], stdout='', stderr='', code=0) -> _HostToResult:
+def create_hosts_result(hosts: List[str], stdout='', stderr='',
+                        code=0, timeout: int = None) -> Dict[str, GenericResult]:
     # each host should have its own result instance.
-    return {host: create_result(stdout, stderr, code) for host in hosts}
+    return {host: create_result(stdout, stderr, code, timeout) for host in hosts}
 
 
-def create_result(stdout='', stderr='', code=0) -> _GenericResult:
-    # connection will be later replaced to fake
-    return fabric.runners.Result(stdout=stdout, stderr=stderr, exited=code, connection=None)
+def create_result(stdout='', stderr='', code=0, timeout: int = None) -> GenericResult:
+    # command and 'hide' option will be later replaced with actual
+    result = RunnersResult(["fake command"], [code], stdout=stdout, stderr=stderr)
+    if timeout is None:
+        return result
+
+    return CommandTimedOut(result, timeout)
 
 
 def empty_action(*args, **kwargs) -> None:
     """
     A dummy method that does nothing
     :return: None
     """
@@ -545,15 +585,15 @@
 
 def new_scheme(scheme: dict, role: str, number: int):
     scheme = deepcopy(scheme)
     scheme[role] = number
     return scheme
 
 
-FULLHA = {'balancer': 1, 'master': 3, 'worker': 3}
-FULLHA_KEEPALIVED = {'balancer': 2, 'master': 3, 'worker': 3, 'keepalived': 1}
-FULLHA_NOBALANCERS = {'balancer': 0, 'master': 3, 'worker': 3}
-ALLINONE = {'master': 1, 'balancer': ['master-1'], 'worker': ['master-1'], 'keepalived': 1}
-MINIHA = {'master': 3}
-MINIHA_KEEPALIVED = {'master': 3, 'balancer': ['master-1', 'master-2', 'master-3'],
-                     'worker': ['master-1', 'master-2', 'master-3'], 'keepalived': 1}
-NON_HA_BALANCER = {'balancer': 1, 'master': 3, 'worker': ['master-1', 'master-2', 'master-3']}
+FULLHA: Dict[str, _ROLE_SPEC] = {'balancer': 1, 'master': 3, 'worker': 3}
+FULLHA_KEEPALIVED: Dict[str, _ROLE_SPEC] = {'balancer': 2, 'master': 3, 'worker': 3, 'keepalived': 1}
+FULLHA_NOBALANCERS: Dict[str, _ROLE_SPEC] = {'balancer': 0, 'master': 3, 'worker': 3}
+ALLINONE: Dict[str, _ROLE_SPEC] = {'master': 1, 'balancer': ['master-1'], 'worker': ['master-1'], 'keepalived': 1}
+MINIHA: Dict[str, _ROLE_SPEC] = {'master': 3}
+MINIHA_KEEPALIVED: Dict[str, _ROLE_SPEC] = {'master': 3, 'balancer': ['master-1', 'master-2', 'master-3'],
+                                            'worker': ['master-1', 'master-2', 'master-3'], 'keepalived': 1}
+NON_HA_BALANCER: Dict[str, _ROLE_SPEC] = {'balancer': 1, 'master': 3, 'worker': ['master-1', 'master-2', 'master-3']}
```

### Comparing `kubemarine-0.18.2/kubemarine/etcd.py` & `kubemarine-0.19.0/kubemarine/etcd.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import json
 import time
-from typing import List, Dict
-
-import fabric.connection
+from typing import List, Dict, Optional
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 
 
 # the methods requires etcdctl.sh to be installed on all active control-plane nodes during thirdparties task.
 
-def remove_members(group: NodeGroup):
-    log = group.cluster.log
+def remove_members(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    control_planes = group.cluster.nodes["control-plane"]
+    control_planes = cluster.nodes["control-plane"]
     managing_control_plane = control_planes.get_unchanged_nodes().get_any_member()
 
     log.verbose(f"etcd will be managed using {managing_control_plane.get_nodes_names()[0]}.")
     output = managing_control_plane.sudo("etcdctl member list").get_simple_out().splitlines()
 
     etcd_members = {}
     for line in output:
@@ -67,16 +66,15 @@
     timeout = cluster.globals['etcd']['health']['timeout']
     retries = cluster.globals['etcd']['health']['retries']
 
     is_healthy = False
     time.sleep(init_timeout)
     while retries > 0:
         start_time = time.time()
-        etcd_health_raw = connection.sudo('etcdctl endpoint health --cluster -w json',
-                                          is_async=False, hide=True).get_simple_out()
+        etcd_health_raw = connection.sudo('etcdctl endpoint health --cluster -w json').get_simple_out()
         end_time = time.time()
         sudo_time = int(end_time - start_time)
         log.verbose(etcd_health_raw)
         etcd_health_list = json.load(io.StringIO(etcd_health_raw.strip()))
 
         health = 0
         for etcd_health in etcd_health_list:
@@ -90,24 +88,23 @@
         else:
             log.debug('Wait for ETCD cluster is not healthy!')
             if sudo_time < timeout:
                 time.sleep(timeout - sudo_time)
             retries -= 1
 
     if is_healthy:
-        etcd_status_raw = connection.sudo('etcdctl endpoint status --cluster -w json',
-                                          is_async=False, hide=True).get_simple_out()
+        etcd_status_raw = connection.sudo('etcdctl endpoint status --cluster -w json').get_simple_out()
         log.verbose(etcd_status_raw)
-        etcd_status_list = json.load(io.StringIO(etcd_status_raw.lower().strip()))
-        elected_leader = None
+        etcd_status_list: List[dict] = json.load(io.StringIO(etcd_status_raw.lower().strip()))
+        elected_leader: Optional[int] = None
         for item in etcd_status_list:
-            leader = item.get('status', {}).get('leader')
-            if not leader:
+            leader: Optional[int] = item.get('status', {}).get('leader')
+            if leader is None:
                 raise Exception('ETCD member "%s" do not have leader' % item.get('endpoint'))
-            if not elected_leader:
+            if elected_leader is None:
                 elected_leader = leader
             elif elected_leader != leader:
                 raise Exception('ETCD leaders are not the same')
         log.debug('Leader "%s" elected' % elected_leader)
     else:
         raise Exception('ETCD cluster is still not healthy!')
```

### Comparing `kubemarine-0.18.2/kubemarine/haproxy.py` & `kubemarine-0.19.0/kubemarine/haproxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import time
+from typing import List, Optional
 
 from jinja2 import Template
 
 from kubemarine import system, packages
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroupResult, NodeGroup
+from kubemarine.core.group import (
+    NodeGroup, RunnersGroupResult, NodeConfig, DeferredGroup, RunResult, AbstractGroup, CollectorCallback
+)
 
 ERROR_VRRP_IS_NOT_CONFIGURED = \
     'Balancer is combined with other role, but there is no VRRP IP configured for node \'%s\'.'
 
 ERROR_NO_BOUND_VRRP_CONFIGURED_MNTC = \
     'No suitable bindings found for haproxy in maintenance mode for node \'%s\'. ' \
     'Balancer is combined with other role and has no configured VRRP IP ' \
@@ -33,24 +35,24 @@
 
 
 def is_maintenance_mode(cluster: KubernetesCluster) -> bool:
     return bool(cluster.raw_inventory.get('services', {}).get('loadbalancer', {})
                 .get('haproxy', {}).get('maintenance_mode', False))
 
 
-def _get_associations_for_node(node: dict) -> dict:
-    conn: NodeGroup = node['connection']
-    return conn.cluster.get_associations_for_node(node['connect_to'], 'haproxy')
+def _get_associations_for_node(node: AbstractGroup[RunResult]) -> dict:
+    return node.cluster.get_associations_for_node(node.get_host(), 'haproxy')
 
 
-def _is_vrrp_not_bind(vrrp_item: dict):
-    return vrrp_item.get('params', {}).get('maintenance-type', '') == 'not bind'
+def _is_vrrp_not_bind(vrrp_item: dict) -> bool:
+    maintenance_type: str = vrrp_item.get('params', {}).get('maintenance-type', '')
+    return maintenance_type == 'not bind'
 
 
-def _get_bindings(inventory: dict, node: dict, *, maintenance: bool):
+def _get_bindings(inventory: dict, node: NodeConfig, *, maintenance: bool) -> List[str]:
     # bindings list for common config and maintenance should be different
     if not maintenance and len(node['roles']) == 1:
         return ["0.0.0.0", '::']
 
     # If we have combination of balancer-control-plane / balancer-worker or if haproxy is in maintenance mode,
     # VRRP IP should be defined for the given balancer.
     # In maintenance mode it should also be not "not bind".
@@ -69,15 +71,15 @@
         # we can listen also own internal address of the balancer
         bindings.append(node['internal_address'])
 
     # remove duplicates
     return list(set(bindings))
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
 
     for node in inventory["nodes"]:
         if 'balancer' not in node['roles']:
             continue
 
         # todo what if balancer is removed? It will have roles=['balancer', 'remove_node'].
         #  It should probably also not participate in other vrrp_ips validation.
@@ -92,150 +94,157 @@
             raise Exception(ERROR_NO_BOUND_VRRP_CONFIGURED_MNTC % node["name"])
 
         not_bind = sum(1 for item in inventory["vrrp_ips"] if _is_vrrp_not_bind(item))
         if bool(not_bind) != is_mntc_mode:
             raise Exception("Haproxy maintenance mode should be used when and only when "
                             "there is at least one VRRP IP with 'maintenance-type: not bind'")
 
-        group: NodeGroup = node["connection"]
+        group = cluster.make_group([node['connect_to']])
         os_family = group.get_nodes_os()
         if is_mntc_mode and os_family not in ('unknown', 'unsupported'):
-            config_location = _get_associations_for_node(node)['config_location']
+            config_location = _get_associations_for_node(group)['config_location']
             mntc_config_location = inventory['services']['loadbalancer']['haproxy']['mntc_config_location']
             # if 'maintenance_mode' is True then maintenance config and default config must be stored in different files'
             if mntc_config_location == config_location:
                 raise Exception("Maintenance mode configuration file must be different with default configuration file")
 
     return inventory
 
 
-def get_config_path(group: NodeGroup) -> NodeGroupResult:
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
+def get_config_path(group: NodeGroup) -> RunnersGroupResult:
+    collector = CollectorCallback(group.cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
             package_associations = _get_associations_for_node(node)
             cmd = f"systemctl show -p MainPID {package_associations['service_name']} " \
                   f"| cut -d '=' -f2 " \
                   f"| xargs -I PID sudo cat /proc/PID/environ " \
                   f"| tr '\\0' '\\n' | grep CONFIG | cut -d \"=\" -f2 | tr -d '\\n'"
-            node['connection'].sudo(cmd)
+            node.sudo(cmd, callback=collector)
 
-    return exe.get_merged_result()
+    return collector.result
 
 
-def install(group: NodeGroup):
-    with RemoteExecutor(group.cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            package_associations = _get_associations_for_node(node)
-            node['connection'].sudo("%s -v" % package_associations['executable_name'], warn=True)
+def install(group: NodeGroup) -> RunnersGroupResult:
+    cluster = group.cluster
+    defer = group.new_defer()
+    collector = CollectorCallback(cluster)
+    for node in defer.get_ordered_members_list():
+        package_associations = _get_associations_for_node(node)
+        node.sudo("%s -v" % package_associations['executable_name'], warn=True, callback=collector)
 
-    haproxy_installed = True
-    for host, host_results in exe.get_last_results().items():
-        if list(host_results.values())[0].exited != 0:
-            haproxy_installed = False
-
-    if haproxy_installed:
-        group.cluster.log.debug("HAProxy already installed, nothing to install")
-        installation_result = exe.get_last_results_str()
+    defer.flush()
+
+    if not collector.result.is_any_failed():
+        cluster.log.debug("HAProxy already installed, nothing to install")
     else:
-        with RemoteExecutor(group.cluster) as exe:
-            for node in group.get_ordered_members_list(provide_node_configs=True):
-                package_associations = _get_associations_for_node(node)
-                packages.install(node["connection"], include=package_associations['package_name'])
+        collector = CollectorCallback(cluster)
+        for node in defer.get_ordered_members_list():
+            package_associations = _get_associations_for_node(node)
+            packages.install(node, include=package_associations['package_name'], callback=collector)
 
-        installation_result = exe.get_last_results_str()
+        defer.flush()
 
-    service_name = package_associations['service_name']
-    patch_path = "./resources/drop_ins/haproxy.conf"
-    group.call(system.patch_systemd_service, service_name=service_name, patch_source=patch_path)
-    enable(group)
-    return installation_result
+    for node in defer.get_ordered_members_list():
+        package_associations = _get_associations_for_node(node)
+        service_name = package_associations['service_name']
+        patch_path = "./resources/drop_ins/haproxy.conf"
+        node.call(system.patch_systemd_service, service_name=service_name, patch_source=patch_path)
+        enable(node)
 
+    defer.flush()
+    return collector.result
 
-def uninstall(group):
+
+def uninstall(group: NodeGroup) -> RunnersGroupResult:
     return packages.remove(group, include=['haproxy', 'rh-haproxy18'])
 
 
-def restart(group: NodeGroup):
-    cluster = group.cluster
+def restart(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
     cluster.log.debug("Restarting haproxy in all group...")
-    with RemoteExecutor(cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
             service_name = _get_associations_for_node(node)['service_name']
-            system.restart_service(node['connection'], name=service_name)
+            system.restart_service(node, name=service_name)
 
     cluster.log.debug("Sleep while haproxy comes-up...")
     time.sleep(static.GLOBALS['haproxy']['restart_wait'])
 
 
-def disable(group):
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
+def disable(group: NodeGroup) -> None:
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
             service_name = _get_associations_for_node(node)['service_name']
-            system.disable_service(node['connection'], name=service_name)
+            system.disable_service(node, name=service_name)
 
 
-def enable(group):
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            service_name = _get_associations_for_node(node)['service_name']
-            system.enable_service(node['connection'], name=service_name,
-                                  now=True)
+def enable(node: DeferredGroup) -> None:
+    # currently it is invoked only for single node
+    service_name = _get_associations_for_node(node)['service_name']
+    system.enable_service(node, name=service_name, now=True)
 
 
-def get_config(cluster: KubernetesCluster, node: dict, future_nodes, maintenance=False) -> str:
+def get_config(cluster: KubernetesCluster, node: NodeConfig, future_nodes: List[NodeConfig],
+               maintenance: bool = False) -> str:
 
     inventory = cluster.inventory
     bindings = _get_bindings(inventory, node, maintenance=maintenance)
 
-    config_options = inventory['services']['loadbalancer']['haproxy']
-    if config_options.get('config'):
-        return inventory['services']['loadbalancer']['haproxy']['config']
+    config_options: dict = inventory['services']['loadbalancer']['haproxy']
+    config_string: Optional[str] = config_options.get('config')
+    if config_string is not None:
+        return config_string
 
     # todo support custom template for maintenance mode
     if not maintenance and config_options.get('config_file'):
         config_source = utils.read_external(config_options['config_file'])
     else:
         config_source = utils.read_internal('templates/haproxy.cfg.j2')
 
     return Template(config_source).render(nodes=future_nodes,
                                           bindings=bindings,
                                           config_options=config_options)
 
 
-def configure(group: NodeGroup):
-    cluster = group.cluster
-    all_nodes_configs = cluster.nodes['all'].get_final_nodes().get_ordered_members_list(provide_node_configs=True)
-
-    for node in group.get_ordered_members_list(provide_node_configs=True):
+def configure(group: DeferredGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+    all_nodes_configs = cluster.nodes['all'].get_final_nodes().get_ordered_members_configs_list()
+
+    for node in group.get_ordered_members_list():
+        node_config = node.get_config()
+        node_name = node.get_node_name()
         package_associations = _get_associations_for_node(node)
         configs_directory = '/'.join(package_associations['config_location'].split('/')[:-1])
 
-        cluster.log.debug("\nConfiguring haproxy on \'%s\'..." % node['name'])
-        config = get_config(cluster, node, all_nodes_configs)
-        utils.dump_file(cluster, config, 'haproxy_%s.cfg' % node['name'])
-        node['connection'].sudo('mkdir -p %s' % configs_directory)
-        node['connection'].put(io.StringIO(config), package_associations['config_location'], backup=True, sudo=True)
-        node['connection'].sudo('ls -la %s' % package_associations['config_location'])
+        cluster.log.debug("\nConfiguring haproxy on \'%s\'..." % node_name)
+        config = get_config(cluster, node_config, all_nodes_configs)
+        utils.dump_file(cluster, config, 'haproxy_%s.cfg' % node_name)
+        node.sudo('mkdir -p %s' % configs_directory)
+        node.put(io.StringIO(config), package_associations['config_location'], backup=True, sudo=True)
+        node.sudo('ls -la %s' % package_associations['config_location'])
 
         # add maintenance config to balancer if 'maintenance_mode' is True
         if is_maintenance_mode(cluster):
             mntc_config_location = cluster.inventory['services']['loadbalancer']['haproxy']['mntc_config_location']
-            cluster.log.debug("\nConfiguring haproxy for maintenance on \'%s\'..." % node['name'])
-            mntc_config = get_config(cluster, node, all_nodes_configs, True)
-            utils.dump_file(cluster, mntc_config, 'haproxy_mntc_%s.cfg' % node['name'])
-            node['connection'].sudo('mkdir -p %s' % configs_directory)
-            node['connection'].put(io.StringIO(mntc_config), mntc_config_location, backup=True, sudo=True)
-            node['connection'].sudo('ls -la %s' % mntc_config_location)
+            cluster.log.debug("\nConfiguring haproxy for maintenance on \'%s\'..." % node_name)
+            mntc_config = get_config(cluster, node_config, all_nodes_configs, True)
+            utils.dump_file(cluster, mntc_config, 'haproxy_mntc_%s.cfg' % node_name)
+            node.sudo('mkdir -p %s' % configs_directory)
+            node.put(io.StringIO(mntc_config), mntc_config_location, backup=True, sudo=True)
+            node.sudo('ls -la %s' % mntc_config_location)
 
 
-def override_haproxy18(group: NodeGroup):
+def override_haproxy18(group: DeferredGroup) -> None:
     rhel_nodes = group.get_subgroup_with_os('rhel')
     if rhel_nodes.is_empty():
         group.cluster.log.debug('Haproxy18 override is not required')
         return
 
     # Any node in group has rhel OS family, so association can be fetched from any node.
     any_host = rhel_nodes.get_first_member().get_host()
     package_associations = group.cluster.get_associations_for_node(any_host, 'haproxy')
     # TODO: Do not replace the whole file, replace only parameter
-    return group.put(io.StringIO("CONFIG=%s\n" % package_associations['config_location']),
-                     '/etc/sysconfig/%s' % package_associations['service_name'], backup=True, sudo=True)
+    group.put(
+        io.StringIO("CONFIG=%s\n" % package_associations['config_location']),
+        '/etc/sysconfig/%s' % package_associations['service_name'],
+        backup=True, sudo=True)
```

### Comparing `kubemarine-0.18.2/kubemarine/jinja.py` & `kubemarine-0.19.0/kubemarine/jinja.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 
 import yaml
 import jinja2
 
 from kubemarine.core import defaults, log
 
 
-def new(logger: log.EnhancedLogger, recursive_compile=False, root: dict = None):
-    if recursive_compile and root is None:
-        raise Exception(
-            "If recursive compilation is enabled, "
-            "'root' parameter should also be specified to provide compilation context.")
-
-    def _precompile(filter_: str, struct: str):
+def new(logger: log.EnhancedLogger, recursive_compile: bool = False, root: dict = None) -> jinja2.Environment:
+    def _precompile(filter_: str, struct: str) -> str:
         if not isinstance(struct, str):
             raise ValueError(f"Filter {filter_!r} can be applied only on string")
 
         if not recursive_compile:
             return struct
+        elif root is None:
+            raise Exception(
+                "If recursive compilation is enabled, "
+                "'root' parameter should also be specified to provide compilation context.")
 
         struct = precompile(logger, struct, root)
 
         return struct
 
 
     env = jinja2.Environment()
```

### Comparing `kubemarine-0.18.2/kubemarine/k8s_certs.py` & `kubemarine-0.19.0/kubemarine/k8s_certs.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,35 +7,38 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import List
 
 from kubemarine import kubernetes
+from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import NodeGroup
 
 
-def k8s_certs_overview(control_planes):
-    for control_plane in control_planes.get_ordered_members_list(provide_node_configs=True):
-        control_planes.cluster.log.debug(f"Checking certs expiration for control_plane {control_plane['name']}")
-        control_plane['connection'].sudo("kubeadm certs check-expiration", hide=False)
+def k8s_certs_overview(control_planes: NodeGroup) -> None:
+    for control_plane in control_planes.get_ordered_members_list():
+        control_planes.cluster.log.debug(f"Checking certs expiration for control_plane {control_plane.get_node_name()}")
+        control_plane.sudo("kubeadm certs check-expiration", hide=False)
 
 
-def renew_verify(inventory, cluster):
+def renew_verify(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get('initial_procedure') != 'cert_renew' or "kubernetes" not in cluster.procedure_inventory:
         return inventory
 
     cert_list = cluster.procedure_inventory["kubernetes"].get("cert-list")
     verify_all_is_absent_or_single(cert_list)
 
     return inventory
 
 
-def renew_apply(control_planes):
+def renew_apply(control_planes: NodeGroup) -> None:
     log = control_planes.cluster.log
 
     procedure = control_planes.cluster.procedure_inventory["kubernetes"]
     cert_list = procedure["cert-list"]
 
     for cert in cert_list:
         control_planes.sudo(f"kubeadm certs renew {cert}")
@@ -45,34 +48,33 @@
         kubernetes.copy_admin_config(log, control_planes)
 
     control_planes.call(force_renew_kubelet_serving_certs)
 
     # for some reason simple pod delete do not work for certs update - we need to delete containers themselves
     control_planes.call(force_restart_control_plane)
 
-    for control_plane in control_planes.get_ordered_members_list(provide_node_configs=True):
-        kubernetes.wait_for_any_pods(control_planes.cluster, control_plane["connection"], apply_filter=control_plane["name"])
+    for control_plane in control_planes.get_ordered_members_list():
+        kubernetes.wait_for_any_pods(control_planes.cluster, control_plane, apply_filter=control_plane.get_node_name())
 
 
-def force_restart_control_plane(control_planes):
+def force_restart_control_plane(control_planes: NodeGroup) -> None:
     cri_impl = control_planes.cluster.inventory['services']['cri']['containerRuntime']
     restart_containers = ["etcd", "kube-scheduler", "kube-apiserver", "kube-controller-manager"]
     c_filter = "grep -e %s" % " -e ".join(restart_containers)
 
     if cri_impl == "docker":
         control_planes.sudo("sudo docker container rm -f $(sudo docker ps -a | %s | awk '{ print $1 }')" % c_filter, warn=True)
     else:
         control_planes.sudo("sudo crictl rm -f $(sudo crictl ps -a | %s | awk '{ print $1 }')" % c_filter, warn=True)
 
 
-def force_renew_kubelet_serving_certs(control_planes):
+def force_renew_kubelet_serving_certs(control_planes: NodeGroup) -> None:
     # Delete *serving* kubelet cert (kubelet.crt) and restart kubelet to create new up-to-date cert.
     # Client kubelet cert (kubelet.conf) is assumed to be updated automatically by kubelet.
     for control_plane in control_planes.get_ordered_members_list():
         control_plane.sudo(f"rm -f /var/lib/kubelet/pki/kubelet.crt /var/lib/kubelet/pki/kubelet.key")
     control_planes.sudo("systemctl restart kubelet")
 
 
-def verify_all_is_absent_or_single(cert_list):
+def verify_all_is_absent_or_single(cert_list: List[str]) -> None:
     if "all" in cert_list and len(cert_list) > 1:
         raise Exception(f"Found 'all' in certs list, but it is not single: {cert_list}")
-    return True
```

### Comparing `kubemarine-0.18.2/kubemarine/keepalived.py` & `kubemarine-0.19.0/kubemarine/keepalived.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,39 +12,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
 import io
 import random
 import time
+from typing import Optional, List
 
 from jinja2 import Template
 
 from kubemarine import system, packages
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup, NodeGroupResult
+from kubemarine.core.group import NodeGroup, NodeConfig, RunnersGroupResult
 
 
-def autodetect_interface(cluster: KubernetesCluster, name):
+def autodetect_interface(cluster: KubernetesCluster, name: str) -> Optional[str]:
     for node in cluster.inventory['nodes']:
         if node['name'] == name:
             address = cluster.get_access_address_from_node(node)
-            interface = cluster.context['nodes'].get(address, {}).get('active_interface')
+            interface: str = cluster.context['nodes'].get(address, {})['active_interface']
             if interface:
                 return interface
     if cluster.context['initial_procedure'] == 'remove_node':
         for node_to_remove in cluster.procedure_inventory['nodes']:
             if node_to_remove['name'] == name:
                 return None
     raise Exception('Failed to autodetect active interface for %s' % name)
 
 
-def enrich_inventory_apply_defaults(inventory, cluster):
+def enrich_inventory_apply_defaults(inventory: dict, cluster: KubernetesCluster) -> dict:
     # if vrrp_ips is empty, then nothing to do
     if not inventory['vrrp_ips']:
         return inventory
 
     default_names = get_default_node_names(inventory)
 
     cluster.log.verbose("Detected default keepalived hosts: %s" % default_names)
@@ -103,59 +103,57 @@
                 item['hosts'][j]['interface'] = item['interface']
             if item['hosts'][j].get('interface', 'auto') == 'auto':
                 item['hosts'][j]['interface'] = autodetect_interface(cluster, item['hosts'][j]['name'])
 
     return inventory
 
 
-def get_default_node_names(inventory):
+def get_default_node_names(inventory: dict) -> List[str]:
     default_names = []
 
     # well, vrrp_ips is not empty, let's find balancers defined in config-file
     for i, node in enumerate(inventory['nodes']):
         if 'balancer' in node['roles']:
             default_names.append(node['name'])
 
     # just in case, we remove duplicates
     return list(set(default_names))
 
 
-def enrich_inventory_calculate_nodegroup(inventory, cluster):
+def enrich_inventory_calculate_nodegroup(inventory: dict, cluster: KubernetesCluster) -> dict:
     # if vrrp_ips is empty, then nothing to do
     if not inventory['vrrp_ips']:
         return inventory
 
     # Calculate group, where keepalived should be installed:
     names = []
 
     for i, item in enumerate(cluster.inventory['vrrp_ips']):
         for record in item['hosts']:
             names.append(record['name'])
 
     # it is important to remove duplicates
     names = list(set(names))
 
-    filtered_members = cluster.nodes['all'].get_ordered_members_list(provide_node_configs=False, apply_filter={
+    # create new group where keepalived will be installed
+    cluster.nodes['keepalived'] = cluster.nodes['all'].new_group(apply_filter={
         'name': names
     })
 
-    # create new group where keepalived will be installed
-    cluster.nodes['keepalived'] = cluster.make_group(filtered_members)
-
     # create new role
     cluster.roles.append('keepalived')
 
     # fill in ips
-    cluster.ips['keepalived'] = list(cluster.nodes['keepalived'].nodes.keys())
+    cluster.ips['keepalived'] = cluster.nodes['keepalived'].get_hosts()
 
     return inventory
 
 
-def install(group: NodeGroup):
-    cluster = group.cluster
+def install(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     # todo why check and try to install all keepalives but finally filter out only new nodes?
     group = group.get_new_nodes_or_self()
     # todo consider probably different associations for nodes with different OS families
     any_host = group.get_first_member().get_host()
     package_associations = cluster.get_associations_for_node(any_host, 'keepalived')
@@ -178,54 +176,54 @@
     group.call(system.patch_systemd_service, service_name=service_name, patch_source=patch_path)
     group.call(install_haproxy_check_script)
     enable(group)
 
     return installation_result
 
 
-def install_haproxy_check_script(group: NodeGroup):
+def install_haproxy_check_script(group: NodeGroup) -> None:
     script = utils.read_internal("./resources/scripts/check_haproxy.sh")
     group.put(io.StringIO(script), "/usr/local/bin/check_haproxy.sh", sudo=True)
     group.sudo("chmod +x /usr/local/bin/check_haproxy.sh")
 
 
-def uninstall(group):
+def uninstall(group: NodeGroup) -> RunnersGroupResult:
     return packages.remove(group, include='keepalived')
 
 
-def restart(group: NodeGroup):
-    cluster = group.cluster
+def restart(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
     cluster.log.debug("Restarting keepalived in all group...")
-    with RemoteExecutor(cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            service_name = group.cluster.get_package_association_for_node(
-                node['connect_to'], 'keepalived', 'service_name')
-            system.restart_service(node['connection'], name=service_name)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            service_name = cluster.get_package_association_for_node(
+                node.get_host(), 'keepalived', 'service_name')
+            system.restart_service(node, name=service_name)
 
     cluster.log.debug("Sleep while keepalived comes-up...")
     time.sleep(static.GLOBALS['keepalived']['restart_wait'])
 
 
-def enable(group: NodeGroup):
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            service_name = group.cluster.get_package_association_for_node(
-                node['connect_to'], 'keepalived', 'service_name')
-            system.enable_service(node['connection'], name=service_name, now=True)
-
-
-def disable(group: NodeGroup):
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            service_name = group.cluster.get_package_association_for_node(
-                node['connect_to'], 'keepalived', 'service_name')
-            system.disable_service(node['connection'], name=service_name)
+def enable(group: NodeGroup) -> None:
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            service_name = exe.cluster.get_package_association_for_node(
+                node.get_host(), 'keepalived', 'service_name')
+            system.enable_service(node, name=service_name, now=True)
+
+
+def disable(group: NodeGroup) -> None:
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            service_name = exe.cluster.get_package_association_for_node(
+                node.get_host(), 'keepalived', 'service_name')
+            system.disable_service(node, name=service_name)
 
 
-def generate_config(inventory, node):
+def generate_config(inventory: dict, node: NodeConfig) -> str:
     config = ''
 
     for i, item in enumerate(inventory['vrrp_ips']):
 
         if i > 0:
             # this is required for double newline in config, but avoid double newline in the end of file
             config += "\n"
@@ -253,31 +251,31 @@
         config += Template(config_source).render(inventory=inventory, item=item, node=node,
                                                  interface=interface,
                                                  priority=priority, **ips) + "\n"
 
     return config
 
 
-def configure(group: NodeGroup) -> NodeGroupResult:
-    log = group.cluster.log
-    group_members = group.get_ordered_members_list(provide_node_configs=True)
-
-    with RemoteExecutor(group.cluster):
-        for node in group_members:
+def configure(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-            log.debug("Configuring keepalived on '%s'..." % node['name'])
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            node_name = node.get_node_name()
+            log.debug("Configuring keepalived on '%s'..." % node_name)
 
-            package_associations = group.cluster.get_associations_for_node(node['connect_to'], 'keepalived')
+            package_associations = cluster.get_associations_for_node(node.get_host(), 'keepalived')
             configs_directory = '/'.join(package_associations['config_location'].split('/')[:-1])
 
-            group.sudo('mkdir -p %s' % configs_directory, hide=True)
+            exe.group.sudo('mkdir -p %s' % configs_directory)
 
-            config = generate_config(group.cluster.inventory, node)
-            utils.dump_file(group.cluster, config, 'keepalived_%s.conf' % node['name'])
+            config = generate_config(cluster.inventory, node.get_config())
+            utils.dump_file(cluster, config, 'keepalived_%s.conf' % node_name)
 
-            node['connection'].put(io.StringIO(config), package_associations['config_location'], sudo=True)
+            node.put(io.StringIO(config), package_associations['config_location'], sudo=True)
 
     log.debug(group.sudo('ls -la %s' % package_associations['config_location']))
 
     restart(group)
 
     return group.sudo('systemctl status %s' % package_associations['service_name'], warn=True)
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/__init__.py` & `kubemarine-0.19.0/kubemarine/kubernetes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 import io
 import math
 import os
 import time
 import uuid
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import List, Dict, Tuple, ContextManager
+from typing import List, Dict, Tuple, Iterator
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 import ipaddress
 
 from kubemarine import system, plugins, admission, etcd, packages
 from kubemarine.core import utils, static, summary, log, errors
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup
+from kubemarine.core.executor import Token
+from kubemarine.core.group import NodeGroup, NodeConfig, RunnersGroupResult, RunResult, AbstractGroup, DeferredGroup, \
+    CollectorCallback
 from kubemarine.core.errors import KME
 
 ERROR_DOWNGRADE='Kubernetes old version \"%s\" is greater than new one \"%s\"'
 ERROR_SAME='Kubernetes old version \"%s\" is the same as new one \"%s\"'
 ERROR_MAJOR_RANGE_EXCEEDED='Major version \"%s\" rises to new \"%s\" more than one'
 ERROR_MINOR_RANGE_EXCEEDED='Minor version \"%s\" rises to new \"%s\" more than one'
 
 
-def add_node_enrichment(inventory, cluster):
+def add_node_enrichment(inventory: dict, cluster: KubernetesCluster):
     if cluster.context.get('initial_procedure') != 'add_node':
         return inventory
 
     # adding role "new_node" for all specified new nodes and putting these nodes to all "nodes" list
     for new_node in cluster.procedure_inventory.get("nodes", []):
         # deepcopy is necessary, otherwise role append will happen in procedure_inventory too
         node = deepcopy(new_node)
@@ -52,15 +53,15 @@
 
     if "vrrp_ips" in cluster.procedure_inventory:
         utils.merge_vrrp_ips(cluster.procedure_inventory, inventory)
 
     return inventory
 
 
-def remove_node_enrichment(inventory, cluster):
+def remove_node_enrichment(inventory: dict, cluster: KubernetesCluster):
     if cluster.context.get('initial_procedure') != 'remove_node':
         return inventory
 
     # adding role "remove_node" for all specified nodes
     node_names_to_remove = [node['name'] for node in cluster.procedure_inventory.get("nodes", [])]
     for i, node in enumerate(inventory['nodes']):
         if node['name'] in node_names_to_remove:
@@ -89,15 +90,15 @@
         return inventory
 
     upgrade_version = cluster.context.get("upgrade_version")
     inventory.setdefault("services", {}).setdefault("kubeadm", {})['kubernetesVersion'] = upgrade_version
     return inventory
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, _):
     repository = inventory['services']['kubeadm'].get('imageRepository', "")
     if repository:
         inventory['services']['kubeadm']['dns'] = {}
         inventory['services']['kubeadm']['dns']['imageRepository'] = ("%s/coredns" % repository)
     # if user redefined apiServer as, string, for example?
     if not isinstance(inventory["services"]["kubeadm"].get('apiServer'), dict):
         inventory["services"]["kubeadm"]['apiServer'] = {}
@@ -200,15 +201,15 @@
 
 
 def reset_installation_env(group: NodeGroup):
     log = group.cluster.log
 
     log.debug("Cleaning up previous installation...")
 
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
     grace_period = cluster.procedure_inventory.get('grace_period')
 
     # if we perform "add" or "remove" node procedure
     # then we need to additionally perform "drain" and "delete" during reset
     nodes_for_draining = cluster.make_group([])
@@ -240,247 +241,251 @@
             # this is add_node procedure
             nodes_for_draining = group
         else:
             # this is install procedure
             is_add_or_remove_procedure = False
 
     if not nodes_for_manual_etcd_remove.is_empty():
-        log.warning(f"Nodes {list(nodes_for_manual_etcd_remove.nodes.keys())} are considered as not active. "
+        log.warning(f"Nodes {nodes_for_manual_etcd_remove.get_hosts()} are considered as not active. "
                     "Full cleanup procedure cannot be performed. "
                     "Corresponding members will be removed from etcd manually.")
         etcd.remove_members(nodes_for_manual_etcd_remove)
 
     if not nodes_for_draining.is_empty():
         drain_nodes(nodes_for_draining, drain_timeout=drain_timeout, grace_period=grace_period)
 
     if is_add_or_remove_procedure and not active_nodes.is_empty():
-        log.verbose(f"Resetting kubeadm on nodes {list(active_nodes.nodes.keys())} ...")
+        log.verbose(f"Resetting kubeadm on nodes {active_nodes.get_hosts()} ...")
         result = active_nodes.sudo('sudo kubeadm reset -f')
         log.debug("Kubeadm successfully reset:\n%s" % result)
 
     if not active_nodes.is_empty():
-        log.verbose(f"Cleaning nodes {list(active_nodes.nodes.keys())} ...")
+        log.verbose(f"Cleaning nodes {active_nodes.get_hosts()} ...")
         # bash semicolon mark will avoid script from exiting and will resume the execution
         result = active_nodes.sudo(
             'sudo kubeadm reset phase cleanup-node; '  # it is required to "cleanup-node" for all procedures
             'sudo systemctl stop kubelet; '
             'sudo rm -rf /etc/kubernetes/manifests /var/lib/kubelet/pki /var/lib/etcd /etc/kubernetes/patches; '
             'sudo mkdir -p /etc/kubernetes/manifests; ', warn=True)
 
         # Disabled initial prune for images prepull feature. Need analysis for possible negative impact.
         # result.update(cri.prune(active_nodes, all_implementations=True))
 
-        log.debug(f"Nodes {list(active_nodes.nodes.keys())} cleaned up successfully:\n" + "%s" % result)
+        log.debug(f"Nodes {active_nodes.get_hosts()} cleaned up successfully:\n" + "%s" % result)
 
     if is_add_or_remove_procedure:
         return delete_nodes(group)
 
 
-def drain_nodes(group, disable_eviction=False, drain_timeout=None, grace_period=None):
-    log = group.cluster.log
+def drain_nodes(group: NodeGroup, disable_eviction=False, drain_timeout=None, grace_period=None):
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    control_plane = group.cluster.nodes['control-plane'].get_final_nodes().get_first_member()
+    control_plane = cluster.nodes['control-plane'].get_final_nodes().get_first_member()
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
     log.verbose("Detected the following nodes in cluster:\n%s" % stdout)
 
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        if node["name"] in stdout:
-            log.debug("Draining node %s..." % node["name"])
+    for node in group.get_ordered_members_list():
+        node_name = node.get_node_name()
+        if node_name in stdout:
+            log.debug("Draining node %s..." % node_name)
             drain_cmd = prepare_drain_command(
-                group.cluster, node["name"],
+                cluster, node_name,
                 disable_eviction=disable_eviction, drain_timeout=drain_timeout, grace_period=grace_period)
             control_plane.sudo(drain_cmd, hide=False)
         else:
-            log.warning("Node %s is not found in cluster and can't be drained" % node["name"])
+            log.warning("Node %s is not found in cluster and can't be drained" % node_name)
 
     return control_plane.sudo("kubectl get nodes")
 
 
-def delete_nodes(group):
-    log = group.cluster.log
+def delete_nodes(group: NodeGroup):
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    control_plane = group.cluster.nodes['control-plane'].get_final_nodes().get_first_member()
+    control_plane = cluster.nodes['control-plane'].get_final_nodes().get_first_member()
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
     log.verbose("Detected the following nodes in cluster:\n%s" % stdout)
 
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        if node["name"] in stdout:
-            log.debug("Deleting node %s from the cluster..." % node["name"])
-            control_plane.sudo("kubectl delete node %s" % node["name"], hide=False)
+    for node in group.get_ordered_members_list():
+        node_name = node.get_node_name()
+        if node_name in stdout:
+            log.debug("Deleting node %s from the cluster..." % node_name)
+            control_plane.sudo("kubectl delete node %s" % node_name, hide=False)
         else:
-            log.warning("Node %s is not found in cluster and can't be removed" % node["name"])
+            log.warning("Node %s is not found in cluster and can't be removed" % node_name)
 
     return control_plane.sudo("kubectl get nodes")
 
 
-def is_available_control_plane(control_plane):
-    return not ("new_node" in control_plane["roles"] or "remove_node" in control_plane["roles"])
-
-
-def install(group):
-    log = group.cluster.log
+def install(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    with RemoteExecutor(group.cluster):
+    with group.new_executor() as exe:
         log.debug("Making systemd unit...")
-        group.sudo('rm -rf /etc/systemd/system/kubelet*')
-        for node in group.cluster.inventory["nodes"]:
-            # perform only for current group members
-            if node["connect_to"] in group.nodes.keys():
-                template = Template(utils.read_internal('templates/kubelet.service.j2')).render(
-                    hostname=node["name"])
-                log.debug("Uploading to '%s'..." % node["connect_to"])
-                node["connection"].put(io.StringIO(template + "\n"), '/etc/systemd/system/kubelet.service', sudo=True)
-                node["connection"].sudo("chmod 644 /etc/systemd/system/kubelet.service")
+        for node in exe.group.get_ordered_members_list():
+            node.sudo('rm -rf /etc/systemd/system/kubelet*')
+            node.get_node_name()
+            template = Template(utils.read_internal('templates/kubelet.service.j2')).render(
+                hostname=node.get_node_name())
+            log.debug("Uploading to '%s'..." % node.get_host())
+            node.put(io.StringIO(template + "\n"), '/etc/systemd/system/kubelet.service', sudo=True)
+            node.sudo("chmod 600 /etc/systemd/system/kubelet.service")
 
         log.debug("\nReloading systemd daemon...")
-        system.reload_systemctl(group)
-        group.sudo('systemctl enable kubelet')
+        system.reload_systemctl(exe.group)
+        exe.group.sudo('systemctl enable kubelet')
 
     return group.sudo('systemctl status kubelet', warn=True)
 
 
-def join_other_control_planes(group):
-    other_control_planes_group = group.get_ordered_members_list(provide_node_configs=True)[1:]
+def join_other_control_planes(group: NodeGroup) -> RunnersGroupResult:
+    other_control_planes_group = group.get_ordered_members_list()[1:]
 
     join_dict = group.cluster.context["join_dict"]
     for node in other_control_planes_group:
-        join_control_plane(group, node, join_dict)
+        join_control_plane(group.cluster, node, join_dict)
 
     group.cluster.log.debug("Verifying installation...")
-    first_control_plane = group.get_first_member(provide_node_configs=True)
-    return first_control_plane['connection'].sudo("kubectl get pods --all-namespaces -o=wide")
+    first_control_plane = group.get_first_member()
+    return first_control_plane.sudo("kubectl get pods --all-namespaces -o=wide")
 
 
-def join_new_control_plane(group):
+def join_new_control_plane(group: NodeGroup):
     join_dict = get_join_dict(group)
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        join_control_plane(group, node, join_dict)
+    for node in group.get_ordered_members_list():
+        join_control_plane(group.cluster, node, join_dict)
 
 
-def join_control_plane(group, node, join_dict):
-    log = group.cluster.log
+def join_control_plane(cluster: KubernetesCluster, node: NodeGroup, join_dict: dict):
+    log = cluster.log
+    node_config = node.get_config()
+    node_name = node.get_node_name()
+    defer = node.new_defer()
 
     join_config: dict = {
-        'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
+        'apiVersion': cluster.inventory["services"]["kubeadm"]['apiVersion'],
         'kind': 'JoinConfiguration',
         'discovery': {
             'bootstrapToken': {
-                'apiServerEndpoint': group.cluster.inventory["services"]["kubeadm"]['controlPlaneEndpoint'],
+                'apiServerEndpoint': cluster.inventory["services"]["kubeadm"]['controlPlaneEndpoint'],
                 'token': join_dict['token'],
                 'caCertHashes': [
                     join_dict['discovery-token-ca-cert-hash']
                 ]
             }
         },
         'controlPlane': {
             'certificateKey': join_dict['certificate-key'],
             'localAPIEndpoint': {
-                'advertiseAddress': node['internal_address'],
+                'advertiseAddress': node_config['internal_address'],
             }
         }
     }
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, patches should be added to InitConfiguration unconditionally
-    if "v1.21" not in group.cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
+    if "v1.21" not in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         join_config['patches'] = {'directory': '/etc/kubernetes/patches'}
 
-
-    if group.cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
+    if cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
             'external-cloud-volume-plugin'):
         join_config['nodeRegistration'] = {
             'kubeletExtraArgs': {
                 'cloud-provider': 'external'
             }
         }
 
-    if 'worker' in node['roles']:
+    if 'worker' in node_config['roles']:
         join_config.setdefault('nodeRegistration', {})['taints'] = []
 
-    configure_container_runtime(group.cluster, join_config)
+    configure_container_runtime(cluster, join_config)
 
-    config = get_kubeadm_config(group.cluster.inventory) + "---\n" + yaml.dump(join_config, default_flow_style=False)
+    config = get_kubeadm_config(cluster.inventory) + "---\n" + yaml.dump(join_config, default_flow_style=False)
 
-    utils.dump_file(group.cluster, config, 'join-config_%s.yaml' % node['name'])
+    utils.dump_file(cluster, config, 'join-config_%s.yaml' % node_name)
 
-    log.debug("Uploading init config to control-plane '%s'..." % node['name'])
-    node['connection'].sudo("mkdir -p /etc/kubernetes")
-    node['connection'].put(io.StringIO(config), '/etc/kubernetes/join-config.yaml', sudo=True)
+    log.debug("Uploading init config to control-plane '%s'..." % node_name)
+    node.sudo("mkdir -p /etc/kubernetes")
+    node.put(io.StringIO(config), '/etc/kubernetes/join-config.yaml', sudo=True)
 
     # put control-plane patches
-    create_kubeadm_patches_for_node(group.cluster, node)
+    create_kubeadm_patches_for_node(cluster, node)
 
     # copy admission config to control-plane
-    admission.copy_pss(node['connection'])
+    admission.copy_pss(node)
 
     # ! ETCD on control-planes can't be initialized in async way, that is why it is necessary to disable async mode !
-    log.debug('Joining control-plane \'%s\'...' % node['name'])
+    log.debug('Joining control-plane \'%s\'...' % node_name)
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
     # and only "else" branch remains
-    if "v1.21" in group.cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
-        node['connection'].sudo("kubeadm join "
-                            " --config=/etc/kubernetes/join-config.yaml"
-                            " --ignore-preflight-errors='" + group.cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
-                            " --v=5",
-                            is_async=False, hide=False)
-
-        log.debug("Patching apiServer bind-address for control-plane %s" % node['name'])
-
-        with RemoteExecutor(group.cluster):
-            node['connection'].sudo("sed -i 's/--bind-address=.*$/--bind-address=%s/' "
-                                    "/etc/kubernetes/manifests/kube-apiserver.yaml" % node['internal_address'])
-            node['connection'].sudo("systemctl restart kubelet")
-            copy_admin_config(log, node['connection'])
+    if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
+        node.sudo(
+            "kubeadm join "
+            " --config=/etc/kubernetes/join-config.yaml"
+            " --ignore-preflight-errors='" + cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
+            " --v=5",
+            hide=False)
+
+        log.debug("Patching apiServer bind-address for control-plane %s" % node_name)
+
+        defer.sudo("sed -i 's/--bind-address=.*$/--bind-address=%s/' "
+                   "/etc/kubernetes/manifests/kube-apiserver.yaml" % node_config['internal_address'])
+        defer.sudo("systemctl restart kubelet")
+        copy_admin_config(log, defer)
+        defer.flush()
     else:
-        node['connection'].sudo("kubeadm join "
-                           " --config=/etc/kubernetes/join-config.yaml "
-                           " --ignore-preflight-errors='" + group.cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
-                            " --v=5",
-                            is_async=False, hide=False)
-        with RemoteExecutor(group.cluster):
-            node['connection'].sudo("systemctl restart kubelet")
-            copy_admin_config(log, node['connection'])
-       
+        node.sudo(
+            "kubeadm join "
+            " --config=/etc/kubernetes/join-config.yaml "
+            " --ignore-preflight-errors='" + cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
+            " --v=5",
+            hide=False)
+        defer.sudo("systemctl restart kubelet")
+        copy_admin_config(log, defer)
+        defer.flush()
 
-    wait_for_any_pods(group.cluster, node['connection'], apply_filter=node['name'])
+    wait_for_any_pods(cluster, node, apply_filter=node_name)
 
 
 @contextmanager
-def local_admin_config(node: NodeGroup) -> ContextManager[str]:
+def local_admin_config(node: NodeGroup) -> Iterator[str]:
     temp_filepath = "/tmp/%s" % uuid.uuid4().hex
 
     cluster_name = node.cluster.inventory['cluster_name']
-    internal_address = node.get_first_member(provide_node_configs=True)['internal_address']
+    internal_address = node.get_config()['internal_address']
     if type(ipaddress.ip_address(internal_address)) is ipaddress.IPv6Address:
         internal_address = f"[{internal_address}]"
 
     try:
         node.sudo(f"cp /root/.kube/config {temp_filepath} "
                   f"&& sudo sed -i 's/{cluster_name}/{internal_address}/' {temp_filepath}")
         yield temp_filepath
     finally:
         node.sudo(f'rm -f {temp_filepath}')
 
 
-def copy_admin_config(log, nodes):
-    log.debug("Setting up admin-config...")
-    nodes.sudo("mkdir -p /root/.kube && sudo cp -f /etc/kubernetes/admin.conf /root/.kube/config")
+def copy_admin_config(logger: log.EnhancedLogger, nodes: AbstractGroup[RunResult]) -> None:
+    logger.debug("Setting up admin-config...")
+    command = "mkdir -p /root/.kube && sudo cp -f /etc/kubernetes/admin.conf /root/.kube/config"
+    nodes.sudo(command)
 
 
 def fetch_admin_config(cluster: KubernetesCluster) -> str:
     log = cluster.log
 
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
-    log.debug(f"Downloading kubeconfig from node {first_control_plane['name']!r}...")
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
+    log.debug(f"Downloading kubeconfig from node {first_control_plane.get_node_name()!r}...")
 
-    kubeconfig = list(first_control_plane['connection'].sudo('cat /root/.kube/config').values())[0].stdout
+    kubeconfig = list(first_control_plane.sudo('cat /root/.kube/config').values())[0].stdout
 
     # Replace cluster FQDN with ip
     public_cluster_ip = cluster.inventory.get('public_cluster_ip')
     if public_cluster_ip:
         if type(ipaddress.ip_address(public_cluster_ip)) is ipaddress.IPv6Address:
             public_cluster_ip = f"[{public_cluster_ip}]"
         cluster_name = cluster.inventory['cluster_name']
@@ -489,92 +494,96 @@
     kubeconfig_filename = os.path.abspath("kubeconfig")
     utils.dump_file(cluster.context, kubeconfig, kubeconfig_filename, dump_location=False)
     cluster.log.debug(f"Kubeconfig saved to {kubeconfig_filename}")
 
     return kubeconfig_filename
 
 
-def get_join_dict(group):
-    first_control_plane = group.cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
-    token_result = first_control_plane['connection'].sudo("kubeadm token create --print-join-command", hide=False)
+def get_join_dict(group: NodeGroup) -> dict:
+    cluster: KubernetesCluster = group.cluster
+    first_control_plane = cluster.nodes["control-plane"].get_first_member()
+    token_result = first_control_plane.sudo("kubeadm token create --print-join-command", hide=False)
     join_strings = list(token_result.values())[0].stdout.rstrip("\n")
 
     join_dict = {"worker_join_command": join_strings}
     join_array = join_strings[join_strings.find("--"):].split()
     for idx, _ in enumerate(join_array):
         current_string = join_array[idx]
         if "--" in current_string:
             join_dict[current_string.lstrip("--")] = join_array[idx + 1]
 
-    cert_key_result = first_control_plane['connection'].sudo("kubeadm init phase upload-certs --upload-certs")
+    cert_key_result = first_control_plane.sudo("kubeadm init phase upload-certs --upload-certs")
     cert_key = list(cert_key_result.values())[0].stdout.split("Using certificate key:\n")[1].rstrip("\n")
     join_dict["certificate-key"] = cert_key
     return join_dict
 
 
-def init_first_control_plane(group):
-    log = group.cluster.log
+def init_first_control_plane(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    first_control_plane = group.get_first_member(provide_node_configs=True)
-    first_control_plane_group = first_control_plane["connection"]
+    first_control_plane = group.get_first_member()
+    node_config = first_control_plane.get_config()
+    node_name = first_control_plane.get_node_name()
 
     init_config: dict = {
-        'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
+        'apiVersion': cluster.inventory["services"]["kubeadm"]['apiVersion'],
         'kind': 'InitConfiguration',
         'localAPIEndpoint': {
-            'advertiseAddress': first_control_plane['internal_address']
+            'advertiseAddress': node_config['internal_address']
         }
     }
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, patches should be added to InitConfiguration unconditionally
-    if "v1.21" not in group.cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
+    if "v1.21" not in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         init_config['patches'] = {'directory': '/etc/kubernetes/patches'}
 
-    if group.cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
+    if cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
             'external-cloud-volume-plugin'):
         init_config['nodeRegistration'] = {
             'kubeletExtraArgs': {
                 'cloud-provider': 'external'
             }
         }
 
-    if 'worker' in first_control_plane['roles']:
+    if 'worker' in node_config['roles']:
         init_config.setdefault('nodeRegistration', {})['taints'] = []
 
-    configure_container_runtime(group.cluster, init_config)
+    configure_container_runtime(cluster, init_config)
 
-    config = get_kubeadm_config(group.cluster.inventory) + "---\n" + yaml.dump(init_config, default_flow_style=False)
+    config = get_kubeadm_config(cluster.inventory) + "---\n" + yaml.dump(init_config, default_flow_style=False)
 
-    utils.dump_file(group.cluster, config, 'init-config_%s.yaml' % first_control_plane['name'])
+    utils.dump_file(cluster, config, 'init-config_%s.yaml' % node_name)
 
     log.debug("Uploading init config to initial control_plane...")
-    first_control_plane_group.sudo("mkdir -p /etc/kubernetes")
-    first_control_plane_group.put(io.StringIO(config), '/etc/kubernetes/init-config.yaml', sudo=True)
+    first_control_plane.sudo("mkdir -p /etc/kubernetes")
+    first_control_plane.put(io.StringIO(config), '/etc/kubernetes/init-config.yaml', sudo=True)
 
     # put control-plane patches
-    create_kubeadm_patches_for_node(group.cluster, first_control_plane)
+    create_kubeadm_patches_for_node(cluster, first_control_plane)
 
     # copy admission config to first control-plane
-    first_control_plane_group.call(admission.copy_pss)
+    first_control_plane.call(admission.copy_pss)
 
     log.debug("Initializing first control_plane...")
-    result = first_control_plane_group.sudo("kubeadm init"
-                                     " --upload-certs"
-                                     " --config=/etc/kubernetes/init-config.yaml"
-                                     " --ignore-preflight-errors='" + group.cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
-                                     " --v=5",
-                                     hide=False)
+    result = first_control_plane.sudo(
+        "kubeadm init"
+        " --upload-certs"
+        " --config=/etc/kubernetes/init-config.yaml"
+        " --ignore-preflight-errors='" + cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
+        " --v=5",
+        hide=False)
 
-    copy_admin_config(log, first_control_plane_group)
+    copy_admin_config(log, first_control_plane)
 
-    kubeconfig_filepath = fetch_admin_config(group.cluster)
-    summary.schedule_report(group.cluster.context, summary.SummaryItem.KUBECONFIG, kubeconfig_filepath)
+    kubeconfig_filepath = fetch_admin_config(cluster)
+    summary.schedule_report(cluster.context, summary.SummaryItem.KUBECONFIG, kubeconfig_filepath)
 
     # Invoke method from admission module for applying default PSS or privileged PSP if they are enabled
-    first_control_plane_group.call(admission.apply_admission)
+    first_control_plane.call(admission.apply_admission)
 
     # Preparing join_dict to init other nodes
     control_plane_lines = list(result.values())[0].stdout. \
                        split("You can now join any number of the control-plane")[1].splitlines()[2:5]
     worker_lines = list(result.values())[0].stdout. \
                        split("Then you can join any number of worker")[1].splitlines()[2:4]
     control_plane_join_command = " ".join([x.replace("\\", "").strip() for x in control_plane_lines])
@@ -584,27 +593,22 @@
     args = control_plane_join_command.split("--")
     join_dict = {}
     for arg in args:
         key_val = arg.split(" ")
         if len(key_val) > 1:
             join_dict[key_val[0].strip()] = key_val[1].strip()
     join_dict["worker_join_command"] = worker_join_command
-    group.cluster.context["join_dict"] = join_dict
+    cluster.context["join_dict"] = join_dict
 
-    wait_for_any_pods(group.cluster, first_control_plane_group, apply_filter=first_control_plane['name'])
+    wait_for_any_pods(cluster, first_control_plane, apply_filter=node_name)
     # refresh cluster installation status in cluster context
-    is_cluster_installed(group.cluster)
+    is_cluster_installed(cluster)
 
 
-
-def wait_for_any_pods(cluster, connection, apply_filter=None):
-    if isinstance(cluster, NodeGroup):
-        # cluster is a group, not a cluster
-        cluster = cluster.cluster
-
+def wait_for_any_pods(cluster: KubernetesCluster, connection: NodeGroup, apply_filter: str = None) :
     plugins.expect_pods(cluster, [
         'kube-apiserver',
         'kube-controller-manager',
         'kube-proxy',
         'kube-scheduler',
         'etcd'
     ], node=connection, apply_filter=apply_filter,
@@ -614,36 +618,37 @@
 
 def wait_uncordon(node: NodeGroup):
     cluster = node.cluster
     timeout_config = cluster.inventory['globals']['expect']['pods']['kubernetes']
     # This forces to use local API server and waits till it is up.
     with local_admin_config(node) as kubeconfig:
         utils.wait_command_successful(node, f"kubectl --kubeconfig {kubeconfig} uncordon {node.get_node_name()}",
-                                      is_async=False, hide=False,
+                                      hide=False,
                                       timeout=timeout_config['timeout'],
                                       retries=timeout_config['retries'])
 
 
 def wait_for_nodes(group: NodeGroup):
-    log = group.cluster.log
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
-    first_control_plane = group.cluster.nodes["control-plane"].get_first_member()
+    first_control_plane = cluster.nodes["control-plane"].get_first_member()
     node_names = group.get_nodes_names()
 
     wait_conditions = {
         "Ready": "True",
         "NetworkUnavailable": "False"
     }
     if len(node_names) > 1:
         status_cmd = "kubectl get nodes %s -o jsonpath='{.items[*].status.conditions[?(@.type==\"%s\")].status}'"
     else:
         status_cmd = "kubectl get nodes %s -o jsonpath='{.status.conditions[?(@.type==\"%s\")].status}'"
 
-    timeout = int(group.cluster.inventory['globals']['nodes']['ready']['timeout'])
-    retries = int(group.cluster.inventory['globals']['nodes']['ready']['retries'])
+    timeout = int(cluster.inventory['globals']['nodes']['ready']['timeout'])
+    retries = int(cluster.inventory['globals']['nodes']['ready']['retries'])
     log.debug("Waiting for new kubernetes nodes to become ready, %s retries every %s seconds" % (retries, timeout))
     while retries > 0:
         correct_conditions = 0
         for condition, cond_value in wait_conditions.items():
             result = first_control_plane.sudo(status_cmd % (" ".join(node_names), condition), warn=True)
             node_result = list(result.values())[0]
             if node_result.failed:
@@ -665,226 +670,236 @@
         else:
             retries = retries - 1
             time.sleep(timeout)
 
     raise Exception("Nodes did not become ready in the expected time, %s retries every %s seconds. Try to increase node.ready.retries parameter in globals: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#globals" % (retries, timeout))
 
 
-def init_workers(group):
-    join_dict = group.cluster.context.get("join_dict", get_join_dict(group))
+def init_workers(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+    join_dict = cluster.context.get("join_dict", get_join_dict(group))
 
     join_config = {
         'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
         'kind': 'JoinConfiguration',
         'discovery': {
             'bootstrapToken': {
-                'apiServerEndpoint': group.cluster.inventory["services"]["kubeadm"]['controlPlaneEndpoint'],
+                'apiServerEndpoint': cluster.inventory["services"]["kubeadm"]['controlPlaneEndpoint'],
                 'token': join_dict['token'],
                 'caCertHashes': [
                     join_dict['discovery-token-ca-cert-hash']
                 ]
             }
         }
     }
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, patches should be added to InitConfiguration unconditionally
-    if "v1.21" not in group.cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
+    if "v1.21" not in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         join_config['patches'] = {'directory': '/etc/kubernetes/patches'}
 
-
-    if group.cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
+    if cluster.inventory['services']['kubeadm']['controllerManager']['extraArgs'].get(
             'external-cloud-volume-plugin'):
         join_config['nodeRegistration'] = {
             'kubeletExtraArgs': {
                 'cloud-provider': 'external'
             }
         }
 
-    configure_container_runtime(group.cluster, join_config)
+    configure_container_runtime(cluster, join_config)
 
     config = yaml.dump(join_config, default_flow_style=False)
 
-    utils.dump_file(group.cluster, config, 'join-config-workers.yaml')
+    utils.dump_file(cluster, config, 'join-config-workers.yaml')
 
     group.sudo("mkdir -p /etc/kubernetes")
     group.put(io.StringIO(config), '/etc/kubernetes/join-config.yaml', sudo=True)
 
     # put control-plane patches
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        create_kubeadm_patches_for_node(group.cluster, node)
+    for node in group.get_ordered_members_list():
+        create_kubeadm_patches_for_node(cluster, node)
 
-    group.cluster.log.debug('Joining workers...')
+    cluster.log.debug('Joining workers...')
 
-    return group.sudo(
+    for node in group.get_ordered_members_list():
+        node.sudo(
             "kubeadm join --config=/etc/kubernetes/join-config.yaml"
-            " --ignore-preflight-errors='" + group.cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
+            " --ignore-preflight-errors='" + cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors'] + "'"
             " --v=5",
-            is_async=False, hide=False)
+            hide=False)
 
-def apply_labels(group):
-    log = group.cluster.log
+
+def apply_labels(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
     log.debug("Applying additional labels for nodes")
     # TODO: Add "--overwrite-labels" switch
     # TODO: Add labels validation after applying
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
+    control_plane = cluster.nodes["control-plane"].get_first_member()
+    with control_plane.new_executor() as exe:
+        for node in group.get_ordered_members_configs_list():
             if "labels" not in node:
                 log.verbose("No additional labels found for %s" % node['name'])
                 continue
             log.verbose("Found additional labels for %s: %s" % (node['name'], node['labels']))
             for key, value in node["labels"].items():
-                group.cluster.nodes["control-plane"].get_first_member() \
-                    .sudo("kubectl label node %s %s=%s" % (node["name"], key, value))
+                exe.group.sudo("kubectl label node %s %s=%s" % (node["name"], key, value))
 
     log.debug("Successfully applied additional labels")
 
-    return group.cluster.nodes["control-plane"].get_first_member() \
-        .sudo("kubectl get nodes --show-labels")
+    return control_plane.sudo("kubectl get nodes --show-labels")
     # TODO: Add wait for pods on worker nodes
 
 
-def apply_taints(group):
-    log = group.cluster.log
+def apply_taints(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
     log.debug("Applying additional taints for nodes")
-    with RemoteExecutor(group.cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
+    control_plane = cluster.nodes["control-plane"].get_first_member()
+    with control_plane.new_executor() as exe:
+        for node in group.get_ordered_members_configs_list():
             if "taints" not in node:
                 log.verbose("No additional taints found for %s" % node['name'])
                 continue
             log.verbose("Found additional taints for %s: %s" % (node['name'], node['taints']))
             for taint in node["taints"]:
-                group.cluster.nodes["control-plane"].get_first_member() \
-                    .sudo("kubectl taint node %s %s" % (node["name"], taint))
+                exe.group.sudo("kubectl taint node %s %s" % (node["name"], taint))
 
     log.debug("Successfully applied additional taints")
 
-    return group.cluster.nodes["control-plane"].get_first_member() \
-        .sudo("kubectl get nodes -o=jsonpath="
-              "'{range .items[*]}{\"node: \"}{.metadata.name}{\"\\ntaints: \"}{.spec.taints}{\"\\n\"}'", hide=True)
+    return control_plane.sudo(
+        "kubectl get nodes -o=jsonpath="
+        "'{range .items[*]}{\"node: \"}{.metadata.name}{\"\\ntaints: \"}{.spec.taints}{\"\\n\"}'")
 
 
-def is_cluster_installed(cluster):
+def is_cluster_installed(cluster: KubernetesCluster):
     cluster.log.verbose('Searching for already installed cluster...')
     try:
-        result = cluster.nodes['control-plane'].sudo('kubectl cluster-info', warn=True, timeout=15)
-        for conn, result in result.items():
+        results = cluster.nodes['control-plane'].sudo('kubectl cluster-info', warn=True, timeout=15)
+        for host, result in results.items():
             if 'is running at' in result.stdout:
-                cluster.log.verbose('Detected running Kubernetes cluster on %s' % conn.host)
+                cluster.log.verbose('Detected running Kubernetes cluster on %s' % host)
                 for line in result.stdout.split("\n"):
                     if 'Kubernetes control plane' in line:
                         cluster.context['controlplain_uri'] = line.split('at ')[1]
                 return True
     except Exception as e:
         cluster.log.verbose(e)
     cluster.context['controlplain_uri'] = None
     cluster.log.verbose('Failed to detect any Kubernetes cluster')
     return False
 
 
-def get_kubeadm_config(inventory):
+def get_kubeadm_config(inventory: dict):
     kubeadm_kubelet = yaml.dump(inventory["services"]["kubeadm_kubelet"], default_flow_style=False)
     kubeadm = yaml.dump(inventory["services"]["kubeadm"], default_flow_style=False)
     return f'{kubeadm_kubelet}---\n{kubeadm}'
 
 
 def upgrade_first_control_plane(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
+    node_name = first_control_plane.get_node_name()
 
-    if not upgrade_group.has_node(first_control_plane['name']):
-        cluster.log.debug("First control-plane \"%s\" upgrade is not required" % first_control_plane['name'])
+    if not upgrade_group.has_node(node_name):
+        cluster.log.debug("First control-plane \"%s\" upgrade is not required" % node_name)
         return
 
-    cluster.log.debug("Upgrading first control-plane \"%s\"" % first_control_plane)
+    cluster.log.debug("Upgrading first control-plane \"%s\"" % node_name)
 
     # put control-plane patches
     create_kubeadm_patches_for_node(cluster, first_control_plane)
     
     # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
     # and only "else" branch remains
     if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s'" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
     else:
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s' --patches=/etc/kubernetes/patches" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
 
     if patch_kubeadm_configmap(first_control_plane, cluster):
         flags += " --config /tmp/kubeadm_config.yaml"
 
-    drain_cmd = prepare_drain_command(cluster, first_control_plane['name'], **drain_kwargs)
-    first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
+    drain_cmd = prepare_drain_command(cluster, node_name, **drain_kwargs)
+    first_control_plane.sudo(drain_cmd, hide=False)
 
-    upgrade_cri_if_required(first_control_plane['connection'])
+    upgrade_cri_if_required(first_control_plane)
 
     # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
     fix_flag_kubelet(cluster, first_control_plane)
 
-    first_control_plane['connection'].sudo(f"sudo kubeadm upgrade apply {version} {flags} && "
-                                    f"sudo kubectl uncordon {first_control_plane['name']} && "
-                                    f"sudo systemctl restart kubelet", is_async=False, hide=False)
-
-    copy_admin_config(cluster.log, first_control_plane['connection'])
-
-    expect_kubernetes_version(cluster, version, apply_filter=first_control_plane['name'])
-    wait_for_any_pods(cluster, first_control_plane['connection'], apply_filter=first_control_plane['name'])
-    exclude_node_from_upgrade_list(first_control_plane['connection'], first_control_plane['name'])
+    first_control_plane.sudo(
+        f"sudo kubeadm upgrade apply {version} {flags} && "
+        f"sudo kubectl uncordon {node_name} && "
+        f"sudo systemctl restart kubelet", hide=False)
+
+    copy_admin_config(cluster.log, first_control_plane)
+
+    expect_kubernetes_version(cluster, version, apply_filter=node_name)
+    wait_for_any_pods(cluster, first_control_plane, apply_filter=node_name)
+    exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
 def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
-    for node in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
-        if node['name'] != first_control_plane['name']:
+    for node in cluster.nodes['control-plane'].get_ordered_members_list():
+        node_name = node.get_node_name()
+        if node_name != first_control_plane.get_node_name():
 
-            if not upgrade_group.has_node(node['name']):
-                cluster.log.debug("Control-plane \"%s\" upgrade is not required" % node['name'])
+            if not upgrade_group.has_node(node_name):
+                cluster.log.debug("Control-plane \"%s\" upgrade is not required" % node_name)
                 continue
 
-            cluster.log.debug("Upgrading control-plane \"%s\"" % node['name'])
+            cluster.log.debug("Upgrading control-plane \"%s\"" % node_name)
 
             # put control-plane patches
             create_kubeadm_patches_for_node(cluster, node)
 
-            drain_cmd = prepare_drain_command(cluster, node['name'], **drain_kwargs)
-            node['connection'].sudo(drain_cmd, is_async=False, hide=False)
+            drain_cmd = prepare_drain_command(cluster, node_name, **drain_kwargs)
+            node.sudo(drain_cmd, hide=False)
 
-            upgrade_cri_if_required(node['connection'])
+            upgrade_cri_if_required(node)
 
             # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
             fix_flag_kubelet(cluster, node)
 
             # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
             # and only "else" branch remains
             if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
-                node['connection'].sudo(f"sudo kubeadm upgrade node --certificate-renewal=true && "
-                                    f"sudo sed -i 's/--bind-address=.*$/--bind-address={node['internal_address']}/' "
-                                    f"/etc/kubernetes/manifests/kube-apiserver.yaml && "
-                                    f"sudo kubectl uncordon {node['name']} && "
-                                    f"sudo systemctl restart kubelet", is_async=False, hide=False)
+                node.sudo(
+                    f"sudo kubeadm upgrade node --certificate-renewal=true && "
+                    f"sudo sed -i 's/--bind-address=.*$/--bind-address={node.get_config()['internal_address']}/' "
+                    f"/etc/kubernetes/manifests/kube-apiserver.yaml && "
+                    f"sudo kubectl uncordon {node_name} && "
+                    f"sudo systemctl restart kubelet",
+                    hide=False)
             else:
-                node['connection'].sudo(f"sudo kubeadm upgrade node --certificate-renewal=true --patches=/etc/kubernetes/patches && "
-                                    f"sudo kubectl uncordon {node['name']} && "
-                                    f"sudo systemctl restart kubelet", is_async=False, hide=False)
-
-            expect_kubernetes_version(cluster, version, apply_filter=node['name'])
-            copy_admin_config(cluster.log, node['connection'])
-            wait_for_any_pods(cluster, node['connection'], apply_filter=node['name'])
-            exclude_node_from_upgrade_list(first_control_plane, node['name'])
+                node.sudo(
+                    f"sudo kubeadm upgrade node --certificate-renewal=true --patches=/etc/kubernetes/patches && "
+                    f"sudo kubectl uncordon {node_name} && "
+                    f"sudo systemctl restart kubelet",
+                    hide=False)
+
+            expect_kubernetes_version(cluster, version, apply_filter=node_name)
+            copy_admin_config(cluster.log, node)
+            wait_for_any_pods(cluster, node, apply_filter=node_name)
+            exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
-def patch_kubeadm_configmap(first_control_plane, cluster):
+def patch_kubeadm_configmap(first_control_plane: NodeGroup, cluster: KubernetesCluster):
     '''
     Checks and patches the Kubeadm configuration for compliance with the current imageRepository, audit log path
     and the corresponding version of the CoreDNS path to the image.
     '''
     # TODO: get rid of this method after k8s 1.21 support stop
     current_kubernetes_version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
-    kubeadm_config_map = first_control_plane["connection"].sudo("kubectl get cm -o yaml -n kube-system kubeadm-config") \
+    kubeadm_config_map = first_control_plane.sudo("kubectl get cm -o yaml -n kube-system kubeadm-config") \
         .get_simple_out()
     ryaml = ruamel.yaml.YAML()
     config_map = ryaml.load(kubeadm_config_map)
     cluster_configuration_yaml = config_map["data"]["ClusterConfiguration"]
     cluster_config = ryaml.load(cluster_configuration_yaml)
 
     if not cluster_config.get("dns"):
@@ -903,83 +918,86 @@
     if new_image_repo_port and old_image_repo_port:
         cluster_config["imageRepository"] = cluster_config["imageRepository"].replace('/k8s.gcr.io', '')
         cluster_config["imageRepository"] = cluster_config["imageRepository"].replace(old_image_repo_port,
                                                                                       new_image_repo_port)
 
     cluster_config['dns']['imageRepository'] = "%s/coredns" % cluster_config["imageRepository"]
 
-    kubelet_config = first_control_plane["connection"].sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
+    kubelet_config = first_control_plane.sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
     ryaml.dump(cluster_config, updated_config)
     result_config = kubelet_config + "---\n" + updated_config.getvalue()
-    first_control_plane["connection"].put(io.StringIO(result_config), "/tmp/kubeadm_config.yaml", sudo=True)
+    first_control_plane.put(io.StringIO(result_config), "/tmp/kubeadm_config.yaml", sudo=True)
 
     return True
 
 
 def upgrade_workers(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
-    for node in cluster.nodes.get('worker').exclude_group(cluster.nodes['control-plane']).get_ordered_members_list(
-            provide_node_configs=True):
+    for node in cluster.nodes['worker'].exclude_group(cluster.nodes['control-plane'])\
+            .get_ordered_members_list():
+        node_name = node.get_node_name()
 
-        if not upgrade_group.has_node(node['name']):
-            cluster.log.debug("Worker \"%s\" upgrade is not required" % node['name'])
+        if not upgrade_group.has_node(node_name):
+            cluster.log.debug("Worker \"%s\" upgrade is not required" % node_name)
             continue
 
-        cluster.log.debug("Upgrading worker \"%s\"" % node['name'])
+        cluster.log.debug("Upgrading worker \"%s\"" % node_name)
 
         # put control-plane patches
         create_kubeadm_patches_for_node(cluster, node)
 
-        drain_cmd = prepare_drain_command(cluster, node['name'], **drain_kwargs)
-        first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
+        drain_cmd = prepare_drain_command(cluster, node_name, **drain_kwargs)
+        first_control_plane.sudo(drain_cmd, hide=False)
 
-        upgrade_cri_if_required(node['connection'])
+        upgrade_cri_if_required(node)
 
         # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
         fix_flag_kubelet(cluster, node)
 
         # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
         # and only "else" branch remains
         if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
-            node['connection'].sudo("kubeadm upgrade node --certificate-renewal=true && "
-                                "sudo systemctl restart kubelet")
+            node.sudo(
+                "kubeadm upgrade node --certificate-renewal=true && "
+                "sudo systemctl restart kubelet")
         else:
-           node['connection'].sudo("kubeadm upgrade node --certificate-renewal=true --patches=/etc/kubernetes/patches && "
-                                "sudo systemctl restart kubelet")
+            node.sudo(
+                "kubeadm upgrade node --certificate-renewal=true --patches=/etc/kubernetes/patches && "
+                "sudo systemctl restart kubelet")
 
-        first_control_plane['connection'].sudo("kubectl uncordon %s" % node['name'], is_async=False, hide=False)
+        first_control_plane.sudo("kubectl uncordon %s" % node_name, hide=False)
 
-        expect_kubernetes_version(cluster, version, apply_filter=node['name'])
+        expect_kubernetes_version(cluster, version, apply_filter=node_name)
         # workers do not have system pods to wait for their start
-        exclude_node_from_upgrade_list(first_control_plane, node['name'])
+        exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
 def prepare_drain_command(cluster: KubernetesCluster, node_name: str,
                           *,
                           disable_eviction=False,
                           drain_timeout: int = None, grace_period: int = None):
     drain_globals = static.GLOBALS['nodes']['drain']
     if drain_timeout is None:
-        drain_timeout = recalculate_proper_timeout(cluster.nodes, drain_globals['timeout'])
+        drain_timeout = recalculate_proper_timeout(cluster, drain_globals['timeout'])
 
     if grace_period is None:
         grace_period = drain_globals['grace_period']
 
     drain_cmd = f"kubectl drain {node_name} --force --ignore-daemonsets --delete-emptydir-data " \
                 f"--timeout={drain_timeout}s --grace-period={grace_period}"
     if disable_eviction:
         drain_cmd += " --disable-eviction=true"
     return drain_cmd
 
 
 def upgrade_cri_if_required(group: NodeGroup):
     # currently it is invoked only for single node
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
 
     if cri_impl in cluster.context["packages"]["upgrade_required"]:
         cri_packages = cluster.get_package_association_for_node(group.get_host(), cri_impl, 'package_name')
 
         log.debug(f"Installing {cri_packages} on node: {group.get_node_name()}")
@@ -989,25 +1007,25 @@
             group.sudo("docker container rm -f $(sudo docker container ls -q)", warn=True)
         else:
             group.sudo("crictl rm -fa", warn=True)
     else:
         log.debug(f"{cri_impl} upgrade is not required")
 
 
-def verify_upgrade_versions(cluster):
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+def verify_upgrade_versions(cluster: KubernetesCluster):
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
     upgrade_version = cluster.context["upgrade_version"]
 
     k8s_nodes_group = cluster.nodes["worker"].include_group(cluster.nodes['control-plane'])
-    for node in k8s_nodes_group.get_ordered_members_list(provide_node_configs=True):
-        cluster.log.debug(f"Verifying current k8s version for node {node['name']}")
-        result = first_control_plane['connection'].sudo("kubectl get nodes "
-                                                 f"{node['name']}"
-                                                 " -o custom-columns='VERSION:.status.nodeInfo.kubeletVersion' "
-                                                 "| grep -vw ^VERSION ")
+    for node in k8s_nodes_group.get_ordered_members_list():
+        cluster.log.debug(f"Verifying current k8s version for node {node.get_node_name()}")
+        result = first_control_plane.sudo("kubectl get nodes "
+                                          f"{node.get_node_name()}"
+                                          " -o custom-columns='VERSION:.status.nodeInfo.kubeletVersion' "
+                                          "| grep -vw ^VERSION ")
         curr_version = list(result.values())[0].stdout
         test_version_upgrade_possible(curr_version, upgrade_version, skip_equal=True)
 
 
 def get_initial_kubernetes_version(inventory: dict) -> str:
     kubernetes_version = inventory.get("services", {}).get("kubeadm", {}).get("kubernetesVersion")
     if kubernetes_version is None:
@@ -1034,15 +1052,16 @@
     verify_allowed_version(target_version)
     minor_version = utils.minor_version(target_version)
     supported_versions = static.KUBERNETES_VERSIONS['kubernetes_versions']
     if not supported_versions.get(minor_version, {}).get("supported", False):
         logger.warning(f"Specified target Kubernetes version {target_version!r} - is not supported!")
 
 
-def expect_kubernetes_version(cluster, version, timeout=None, retries=None, node=None, apply_filter=None):
+def expect_kubernetes_version(cluster: KubernetesCluster, version: str,
+                              timeout=None, retries=None, node: NodeGroup = None, apply_filter: str = None):
     if timeout is None:
         timeout = cluster.globals['nodes']['expect']['kubernetes_version']['timeout']
     if retries is None:
         retries = cluster.globals['nodes']['expect']['kubernetes_version']['retries']
 
     cluster.log.debug("Expecting Kubernetes version %s" % version)
     cluster.log.debug("Max expectation time: %ss" % (timeout * retries))
@@ -1101,23 +1120,23 @@
         raise Exception(ERROR_MAJOR_RANGE_EXCEEDED % (versions_unchanged['old'], versions_unchanged['new']))
 
     # test minor step is not greater than 1
     if versions['new'][1] - versions['old'][1] > 1:
         raise Exception(ERROR_MINOR_RANGE_EXCEEDED % (versions_unchanged['old'], versions_unchanged['new']))
 
 
-def recalculate_proper_timeout(nodes, timeout):
+def recalculate_proper_timeout(cluster: KubernetesCluster, timeout: int):
     try:
-        amount_str = nodes['control-plane'].get_first_member().sudo('kubectl get pods -A | wc -l').get_simple_out()
+        amount_str = cluster.nodes['control-plane'].get_first_member().sudo('kubectl get pods -A | wc -l').get_simple_out()
         return timeout * int(amount_str)
     except Exception:
-        return timeout * 10 * nodes['all'].nodes_amount()
+        return timeout * 10 * cluster.nodes['all'].nodes_amount()
 
 
-def configure_container_runtime(cluster, kubeadm_config):
+def configure_container_runtime(cluster: KubernetesCluster, kubeadm_config: dict):
     if cluster.inventory['services']['cri']['containerRuntime'] == "containerd":
         if 'nodeRegistration' not in kubeadm_config:
             kubeadm_config['nodeRegistration'] = {}
         if 'kubeletExtraArgs' not in kubeadm_config['nodeRegistration']:
             kubeadm_config['nodeRegistration']['kubeletExtraArgs'] = {}
 
         kubeadm_config['nodeRegistration']['criSocket'] = '/var/run/containerd/containerd.sock'
@@ -1126,21 +1145,19 @@
         if minor_version < 27:
             kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime'] = 'remote'
 
         kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime-endpoint'] = \
             'unix:///run/containerd/containerd.sock'
 
 
-def exclude_node_from_upgrade_list(first_control_plane, node_name):
-    if isinstance(first_control_plane, dict):
-        first_control_plane = first_control_plane['connection']
+def exclude_node_from_upgrade_list(first_control_plane: NodeGroup, node_name: str):
     return first_control_plane.sudo('sed -i \'/%s/d\' /etc/kubernetes/nodes-k8s-versions.txt' % node_name, warn=True)
 
 
-def autodetect_non_upgraded_nodes(cluster, future_version) -> List[str]:
+def autodetect_non_upgraded_nodes(cluster: KubernetesCluster, future_version: str) -> List[str]:
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     try:
         nodes_list_result = first_control_plane.sudo('[ ! -f /etc/kubernetes/nodes-k8s-versions.txt ] && '
                                               'sudo kubectl get nodes -o custom-columns=\''
                                               'VERSION:.status.nodeInfo.kubeletVersion,'
                                               'NAME:.metadata.name,'
                                               'STATUS:.status.conditions[-1].type\' '
@@ -1150,15 +1167,15 @@
                                               'If all the nodes are completely updated or you manually fixed the '
                                               'problem that occurred during the upgrade, you can delete it.\' '
                                               '| sudo tee /etc/kubernetes/nodes-k8s-versions.txt; '
                                               'sudo cat /etc/kubernetes/nodes-k8s-versions.txt') \
             .get_simple_out()
         cluster.log.verbose("Remote response with nodes description:\n%s" % nodes_list_result)
     except Exception as e:
-        cluster.log.warn("Failed to detect cluster status before upgrade. All nodes will be scheduled for upgrade.")
+        cluster.log.warning("Failed to detect cluster status before upgrade. All nodes will be scheduled for upgrade.")
         cluster.log.verbose(e)
         return cluster.nodes['all'].get_nodes_names()
 
     detected_nodes_lines = nodes_list_result.splitlines()
 
     if not detected_nodes_lines:
         raise Exception('Remote result did not returned any lines containing node info')
@@ -1179,15 +1196,15 @@
             upgrade_list.append(node_name)
         else:
             cluster.log.verbose("Node \"%s\" already upgraded." % node_name)
 
     return upgrade_list
 
 
-def get_group_for_upgrade(cluster, ignore_cache=False):
+def get_group_for_upgrade(cluster: KubernetesCluster, ignore_cache=False) -> NodeGroup:
 
     if cluster.context.get('upgrade_group') and not ignore_cache:
         return cluster.context['upgrade_group']
 
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     if cluster.procedure_inventory.get('upgrade_nodes'):
         nodes_for_upgrade = []
@@ -1213,45 +1230,47 @@
     Prepull kubeadm images on group, separated on sub-groups with certain group size. Separation required to avoid high
     load on images repository server, when using large clusters.
     :param group: NodeGroup where prepull should be performed.
     :param group_size: integer number of nodes per group. Will be automatically used from procedure_yaml or globals, if not set.
     :return: String results from all nodes in presented group.
     """
 
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
-    if not group_size:
+    if group_size is None:
         group_size = cluster.procedure_inventory.get('prepull_group_size')
 
-    if not group_size:
+    if group_size is None:
         log.verbose("Group size is not set in procedure inventory, a default one will be used")
-        group_size = cluster.globals.get('prepull_group_size')
+        group_size = cluster.globals['prepull_group_size']
 
-    nodes = group.get_ordered_members_list()
+    nodes_amount = group.nodes_amount()
 
     # group_size should be greater than 0
-    if len(nodes) != 0 and len(nodes) < group_size:
-        group_size = len(nodes)
+    if nodes_amount != 0 and nodes_amount < group_size:
+        group_size = nodes_amount
 
-    groups_amount = math.ceil(len(nodes) / group_size)
+    groups_amount = math.ceil(nodes_amount / group_size)
 
-    log.verbose("Nodes amount: %s\nGroup size: %s\nGroups amount: %s" % (len(nodes), group_size, groups_amount))
-    with RemoteExecutor(cluster) as exe:
+    log.verbose("Nodes amount: %s\nGroup size: %s\nGroups amount: %s" % (nodes_amount, group_size, groups_amount))
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        nodes = exe.group.get_ordered_members_list()
         for group_i in range(groups_amount):
             log.verbose('Prepulling images for group #%s...' % group_i)
             # RemoteExecutor used for future cases, when some nodes will require another/additional actions for prepull
             for node_i in range(group_i*group_size, (group_i*group_size)+group_size):
-                if node_i < len(nodes):
-                    images_prepull(nodes[node_i])
+                if node_i < nodes_amount:
+                    images_prepull(nodes[node_i], collector=collector)
 
-    return exe.get_last_results_str()
+    return collector.result
 
 
-def images_prepull(group: NodeGroup):
+def images_prepull(group: DeferredGroup, collector: CollectorCallback) -> Token:
     """
     Prepull kubeadm images on group.
     :param group: NodeGroup where prepull should be performed.
     :return: NodeGroupResult from all nodes in presented group.
     """
 
     config = get_kubeadm_config(group.cluster.inventory)
@@ -1261,15 +1280,16 @@
     }
 
     configure_container_runtime(group.cluster, kubeadm_init)
     config = f'{config}---\n{yaml.dump(kubeadm_init, default_flow_style=False)}'
 
     group.put(io.StringIO(config), '/etc/kubernetes/prepull-config.yaml', sudo=True)
 
-    return group.sudo("kubeadm config images pull --config=/etc/kubernetes/prepull-config.yaml")
+    return group.sudo("kubeadm config images pull --config=/etc/kubernetes/prepull-config.yaml",
+                      callback=collector)
 
 
 def schedule_running_nodes_report(cluster: KubernetesCluster):
     summary.schedule_delayed_report(cluster, exec_running_nodes_report)
 
 
 def exec_running_nodes_report(cluster: KubernetesCluster):
@@ -1301,15 +1321,15 @@
     cmd = get_nodes_description_cmd()
     result = cluster.nodes['control-plane'].get_final_nodes().get_any_member().sudo(cmd)
     cluster.log.verbose(result)
     return yaml.safe_load(list(result.values())[0].stdout)
 
 
 def get_actual_roles(nodes_description: dict) -> Dict[str, List[str]]:
-    result = {}
+    result: Dict[str, List[str]] = {}
     for node_description in nodes_description['items']:
         node_name = node_description['metadata']['name']
         labels = node_description['metadata']['labels']
         result[node_name] = []
         # TODO check label accordingly to Kubernetes version
         if 'node-role.kubernetes.io/master' in labels or 'node-role.kubernetes.io/control-plane' in labels:
             result[node_name].append('control-plane')
@@ -1319,23 +1339,23 @@
     return result
 
 
 def get_nodes_conditions(nodes_description: dict) -> Dict[str, Dict[str, dict]]:
     result = {}
     for node_description in nodes_description['items']:
         node_name = node_description['metadata']['name']
-        conditions_by_type = {}
+        conditions_by_type: Dict[str, dict] = {}
         result[node_name] = conditions_by_type
         for condition in node_description['status']['conditions']:
             conditions_by_type[condition['type']] = condition
 
     return result
 
 # function to get dictionary of flags to be patched for a given control plane item and a given node
-def get_patched_flags_for_control_plane_item(inventory, control_plane_item, node):
+def get_patched_flags_for_control_plane_item(inventory: dict, control_plane_item: str, node: NodeConfig):
     flags = {}
 
     for n in inventory['services']['kubeadm_patches'][control_plane_item]:
         if n.get('groups') is not None and list(set(node['roles']) & set(n['groups'])):
             if n.get('patch') is not None:
                 for arg, value in n['patch'].items():
                     flags[arg] = value
@@ -1346,18 +1366,19 @@
 
     # we always set binding-address to the node's internal address for apiServer
     if control_plane_item == 'apiServer' and 'control-plane' in node['roles']:
         flags['bind-address'] = node['internal_address']
 
     return flags
 
+
 # function to create kubeadm patches and put them to a node
-def create_kubeadm_patches_for_node(cluster, node):
-    cluster.log.verbose(f"Create and upload kubeadm patches to %s..." % node['name'])
-    node['connection'].sudo('sudo rm -rf /etc/kubernetes/patches ; sudo mkdir -p /etc/kubernetes/patches', warn=True)
+def create_kubeadm_patches_for_node(cluster: KubernetesCluster, node: NodeGroup):
+    cluster.log.verbose(f"Create and upload kubeadm patches to %s..." % node.get_node_name())
+    node.sudo('sudo rm -rf /etc/kubernetes/patches ; sudo mkdir -p /etc/kubernetes/patches', warn=True)
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
     if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         # do nothing, patches are supported since v1.22
         return
 
     control_plane_patch_files = {
@@ -1365,36 +1386,51 @@
         'etcd' : 'etcd+json.json',
         'controllerManager' : 'kube-controller-manager+json.json',
         'scheduler' : 'kube-scheduler_json.json',
         'kubelet' : 'kubeletconfiguration.yaml'
     }
 
     # read patches content from inventory and upload patch files to a node
+    node_config = node.get_config()
     for control_plane_item in cluster.inventory['services']['kubeadm_patches']:
-        patched_flags = get_patched_flags_for_control_plane_item(cluster.inventory, control_plane_item, node)
+        patched_flags = get_patched_flags_for_control_plane_item(cluster.inventory, control_plane_item, node_config)
         if patched_flags:
             if control_plane_item == 'kubelet':
                 template_filename = 'templates/patches/kubelet.yaml.j2'
             else:
                 template_filename = 'templates/patches/control-plane-pod.json.j2'
 
             control_plane_patch = Template(utils.read_internal(template_filename)).render(flags=patched_flags)
-            node['connection'].put(io.StringIO(control_plane_patch + "\n"), '/etc/kubernetes/patches/' +
-                                 control_plane_patch_files[control_plane_item], sudo=True)
-            node['connection'].sudo('chmod 644 /etc/kubernetes/patches/' +
-                                 control_plane_patch_files[control_plane_item])
+            patch_file = '/etc/kubernetes/patches/' + control_plane_patch_files[control_plane_item]
+            node.put(io.StringIO(control_plane_patch + "\n"), patch_file, sudo=True)
+            node.sudo(f'chmod 644 {patch_file}')
 
     return
 
-def fix_flag_kubelet(cluster: KubernetesCluster, node: dict):
+
+def fix_flag_kubelet(cluster: KubernetesCluster, node: NodeGroup):
     #Deprecated flag removal function for kubelet
     kubeadm_file = "/var/lib/kubelet/kubeadm-flags.env"
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
 
     if utils.version_key(version) < utils.version_key("v1.27.0"):
         # Target version is lower than v1.27.0. Flag is actual and should not be removed.
         return
 
-    kubeadm_flags = node['connection'].sudo(f"cat {kubeadm_file}", is_async=False).get_simple_out()
+    kubeadm_flags = node.sudo(f"cat {kubeadm_file}").get_simple_out()
     if kubeadm_flags.find('--container-runtime=remote') != -1:
         kubeadm_flags = kubeadm_flags.replace('--container-runtime=remote', '')
-        node['connection'].put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
+        node.put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
+ 
+
+def _config_changer(config: str, word: str):
+    equal_pos = word.find("=") + 1
+    param_begin_pos = config.find(word[:equal_pos])
+    if param_begin_pos != -1:
+        param_end_pos = config[param_begin_pos:].find(" ")
+        if param_end_pos == -1:
+            return config[:param_begin_pos] + word + "\""
+        return config[:param_begin_pos] + word + config[param_end_pos + param_begin_pos:]
+    else:
+        param_end_pos = config.rfind("\"")
+        return config[:param_end_pos] + " " + word[:] + "\""
+
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.19.0/kubemarine/kubernetes/daemonset.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.kubernetes.object import KubernetesObject
 
 
 class DaemonSet(KubernetesObject):
 
-    def __init__(self, cluster: KubernetesCluster, name=None, namespace=None, obj=None):
+    def __init__(self, cluster: KubernetesCluster, name: str = None, namespace: str = None, obj: dict = None) -> None:
         super().__init__(cluster, kind='DaemonSet', name=name, namespace=namespace, obj=obj)
 
     def is_actual_and_ready(self) -> bool:
         return self.is_ready() and self.is_up_to_date()
 
     def is_up_to_date(self) -> bool:
         desired_number_scheduled = self._obj.get('status', {}).get('desiredNumberScheduled')
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/deployment.py` & `kubemarine-0.19.0/kubemarine/kubernetes/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.kubernetes.object import KubernetesObject
 
 
 class Deployment(KubernetesObject):
 
-    def __init__(self, cluster: KubernetesCluster, name=None, namespace=None, obj=None):
+    def __init__(self, cluster: KubernetesCluster, name: str = None, namespace: str = None, obj: dict = None) -> None:
         super().__init__(cluster, kind='Deployment', name=name, namespace=namespace, obj=obj)
 
     def is_actual_and_ready(self) -> bool:
         return self.is_ready() and self.is_up_to_date()
 
     def is_up_to_date(self) -> bool:
         desired_number_scheduled = self._obj.get('spec', {}).get('replicas')
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/object.py` & `kubemarine-0.19.0/kubemarine/kubernetes/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 
 from __future__ import annotations
 
 import io
 import json
 import uuid
 import time
+from typing import TypeVar
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import NodeGroup
+
+_T = TypeVar('_T', bound='KubernetesObject')
 
 
 class KubernetesObject:
-    def __init__(self, cluster: KubernetesCluster, kind=None, name=None, namespace=None, obj=None):
+    def __init__(self, cluster: KubernetesCluster, kind: str = None, name: str = None,
+                 namespace: str = None, obj: dict = None) -> None:
 
         self._cluster = cluster
-        self._reload_t = -1
+        self._reload_t: float = -1
 
         if not kind and not name and not namespace and not obj:
             raise RuntimeError('Not enough parameter values to construct the object')
         if obj:
             self._obj = obj
         else:
             if not kind or not name or not namespace:
@@ -42,58 +47,58 @@
                 "kind": kind,
                 "metadata": {
                     "name": name,
                     "namespace": namespace,
                 }
             }
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.to_yaml()
 
     @property
-    def uid(self):
-        uid = self._obj.get('metadata', {}).get('uid')
+    def uid(self) -> str:
+        uid = self._obj['metadata'].get('uid')
         if uid:
             return uid
 
         return str(uuid.uuid4())
 
     @property
-    def kind(self):
-        return self._obj.get('kind').lower()
+    def kind(self) -> str:
+        return self._obj['kind'].lower()
 
     @property
-    def namespace(self):
-        return self._obj.get('metadata', {}).get('namespace').lower()
+    def namespace(self) -> str:
+        return self._obj['metadata']['namespace'].lower()
 
     @property
-    def name(self):
-        return self._obj.get('metadata', {}).get('name').lower()
+    def name(self) -> str:
+        return self._obj['metadata']['name'].lower()
 
-    def to_json(self):
+    def to_json(self) -> str:
         return json.dumps(self._obj)
 
-    def to_yaml(self):
+    def to_yaml(self) -> str:
         return yaml.dump(self._obj)
 
-    def is_reloaded(self):
+    def is_reloaded(self) -> bool:
         return self._reload_t > -1
 
-    def reload(self, control_plane=None, suppress_exceptions=False) -> KubernetesObject:
+    def reload(self: _T, control_plane: NodeGroup = None, suppress_exceptions: bool = False) -> _T:
         if not control_plane:
             control_plane = self._cluster.nodes['control-plane'].get_any_member()
         cmd = f'kubectl get {self.kind} -n {self.namespace} {self.name} -o json'
         result = control_plane.sudo(cmd, warn=suppress_exceptions)
         self._cluster.log.verbose(result)
-        if not result.is_any_failed():
+        if not result.is_any_has_code(1):
             self._obj = json.loads(result.get_simple_out())
             self._reload_t = time.time()
         return self
 
-    def apply(self, control_plane=None):
+    def apply(self, control_plane: NodeGroup = None) -> None:
         if not control_plane:
             control_plane = self._cluster.nodes['control-plane'].get_any_member()
 
         json_str = self.to_json()
         obj_filename = "_".join([self.kind, self.namespace, self.name, self.uid]) + '.json'
         obj_path = f'/tmp/{obj_filename}'
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.19.0/kubemarine/kubernetes/replicaset.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.kubernetes.object import KubernetesObject
 
 
 class ReplicaSet(KubernetesObject):
 
-    def __init__(self, cluster: KubernetesCluster, name=None, namespace=None, obj=None):
+    def __init__(self, cluster: KubernetesCluster, name: str = None, namespace: str = None, obj: dict = None) -> None:
         super().__init__(cluster, kind='ReplicaSet', name=name, namespace=namespace, obj=obj)
 
     def is_actual_and_ready(self) -> bool:
         return self.is_available() and self.is_fully_labeled() and self.is_ready()
 
     def is_ready(self) -> bool:
         desired_number_scheduled = self._obj.get('spec', {}).get('replicas')
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.19.0/kubemarine/kubernetes/statefulset.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.kubernetes.object import KubernetesObject
 
 
 class StatefulSet(KubernetesObject):
 
-    def __init__(self, cluster: KubernetesCluster, name=None, namespace=None, obj=None):
+    def __init__(self, cluster: KubernetesCluster, name: str = None, namespace: str = None, obj: dict = None) -> None:
         super().__init__(cluster, kind='StatefulSet', name=name, namespace=namespace, obj=obj)
 
     def is_actual_and_ready(self) -> bool:
         return self.is_updated() and self.is_ready()
 
     def is_ready(self) -> bool:
         desired_number = self._obj.get('spec', {}).get('replicas')
```

### Comparing `kubemarine-0.18.2/kubemarine/kubernetes_accounts.py` & `kubemarine-0.19.0/kubemarine/kubernetes_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-import os
+from typing import Optional
 
 import yaml
 
 from kubemarine.core import utils, summary
 from kubemarine.core.cluster import KubernetesCluster
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, _: KubernetesCluster) -> dict:
     rbac = inventory['rbac']
     if not rbac.get("accounts"):
         return inventory
 
     for i, account in enumerate(rbac["accounts"]):
         if account['configs'][0]['metadata'].get('name') is None:
             rbac["accounts"][i]['configs'][0]['metadata']['name'] = account['name']
@@ -60,15 +60,15 @@
                 rbac["accounts"][i]['configs'][0]['secrets'][0]['name'] = f"{account['name']}-token"
             if account['configs'][2]['metadata'].get('namespace') is None:
                 rbac["accounts"][i]['configs'][2]['metadata']['namespace'] = account['namespace']
 
     return inventory
 
 
-def install(cluster: KubernetesCluster):
+def install(cluster: KubernetesCluster) -> None:
     rbac = cluster.inventory['rbac']
     if not rbac.get("accounts"):
         cluster.log.debug("No accounts specified to install, skipping...")
         return
 
     tokens = []
     for account in rbac["accounts"]:
@@ -92,15 +92,15 @@
         cluster.nodes['control-plane'].get_first_member().sudo('kubectl apply -f %s' % destination_path, hide=False)
 
         cluster.log.debug('Loading token...')
         load_tokens_cmd = 'kubectl -n %s get secret ' \
                           '$(sudo kubectl -n %s get sa %s -o \'jsonpath={.secrets[0].name}\') -o \'jsonpath={.data.token}\'' \
                           '| sudo base64 -d' % (account['namespace'], account['namespace'], account['name'])
 
-        token = []
+        token: Optional[str] = None
         retries = cluster.globals['accounts']['retries']
         # Token creation in Kubernetes 1.24 is not syncronus, therefore retries are necessary
         while retries > 0:
             result = cluster.nodes['control-plane'].get_first_member().sudo(load_tokens_cmd)
             token = list(result.values())[0].stdout
             if not token:
                 retries -= 1
```

### Comparing `kubemarine-0.18.2/kubemarine/packages.py` & `kubemarine-0.19.0/kubemarine/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from copy import deepcopy
-from typing import List, Dict, Tuple
+from typing import List, Dict, Tuple, Optional, Union, Mapping, Set
 
-import fabric
+from typing_extensions import Protocol
 
 from kubemarine import yum, apt
 from kubemarine.core import errors, utils, static
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup, NodeGroupResult
+from kubemarine.core.executor import RunnersResult, Token, Callback
+from kubemarine.core.group import (
+    NodeGroup, DeferredGroup, AbstractGroup, RunResult, GROUP_RUN_TYPE,
+    CollectorCallback, RunnersGroupResult
+)
 from kubemarine.core.yaml_merger import default_merger
 
 
 ERROR_GLOBAL_ASSOCIATIONS_REDEFINED_MULTIPLE_OS = \
     "It is not supported to customize services.packages.associations section " \
     "if nodes have different OS families. " \
     "Please move the section to corresponding services.packages.associations.<os_family> section."
@@ -40,15 +43,15 @@
 def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     enrich_inventory_associations(inventory, cluster)
     enrich_inventory_packages(inventory, cluster)
 
     return inventory
 
 
-def enrich_inventory_associations(inventory, cluster: KubernetesCluster):
+def enrich_inventory_associations(inventory: dict, cluster: KubernetesCluster) -> None:
     associations: dict = inventory['services']['packages']['associations']
     enriched_associations = {}
 
     # Move associations for OS families and merge with globals
     for association_name in get_associations_os_family_keys():
         os_associations: dict = deepcopy(cluster.globals['packages']['common_associations'])
         if association_name == 'debian':
@@ -69,24 +72,24 @@
 
     if 'semanage' in enriched_associations['debian']:
         raise Exception(ERROR_SEMANAGE_NOT_MANAGED_DEBIAN)
 
     inventory['services']['packages']['associations'] = enriched_associations
 
 
-def enrich_inventory_packages(inventory: dict, _):
+def enrich_inventory_packages(inventory: dict, _: KubernetesCluster) -> None:
     for _type in ['install', 'upgrade', 'remove']:
         packages_list = inventory['services']['packages'].get(_type)
         if isinstance(packages_list, list):
             inventory['services']['packages'][_type] = {
                 'include': packages_list
             }
 
 
-def enrich_inventory_apply_defaults(inventory: dict, _) -> dict:
+def enrich_inventory_apply_defaults(inventory: dict, _: KubernetesCluster) -> dict:
     kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
 
     for os_family in get_associations_os_family_keys():
         cluster_associations = inventory["services"]["packages"]["associations"][os_family]
         for package in static.GLOBALS['packages'][os_family]:
             if cluster_associations[package].get('package_name') is None:
                 cluster_associations[package]['package_name'] = \
@@ -96,15 +99,15 @@
 
 
 def _get_associations_upgrade_plan(cluster: KubernetesCluster, inventory: dict) -> List[Tuple[str, dict]]:
     context = cluster.context
     if context.get("initial_procedure") == "upgrade":
         upgrade_version = context["upgrade_version"]
         upgrade_plan = []
-        for version in cluster.procedure_inventory.get('upgrade_plan'):
+        for version in cluster.procedure_inventory['upgrade_plan']:
             if utils.version_key(version) < utils.version_key(upgrade_version):
                 continue
 
             upgrade_associations = cluster.procedure_inventory.get(version, {}).get("packages", {}).get("associations", {})
             upgrade_associations = dict(item for item in upgrade_associations.items()
                                         if item[0] in _get_system_packages_support_upgrade(inventory))
             upgrade_plan.append((version, upgrade_associations))
@@ -147,30 +150,30 @@
     upgrade_inventory_associations(cluster, inventory, enrich_global=False)
     upgrade_inventory_packages(cluster, inventory)
 
     return inventory
 
 
 def upgrade_inventory_associations(cluster: KubernetesCluster, inventory: dict,
-                                   *, enrich_global: bool):
+                                   *, enrich_global: bool) -> None:
     # pass enriched 'cluster.inventory' instead of 'inventory' that is being finalized
     upgrade_plan = _get_associations_upgrade_plan(cluster, cluster.inventory)
     if not upgrade_plan:
         return
 
     _, upgrade_associations = upgrade_plan[0]
     if upgrade_associations:
         cluster_associations = inventory.setdefault("services", {}).setdefault("packages", {}) \
             .setdefault("associations", {})
         if not enrich_global:
             cluster_associations = cluster_associations.setdefault(cluster.get_os_family(), {})
         default_merger.merge(cluster_associations, upgrade_associations)
 
 
-def upgrade_inventory_packages(cluster: KubernetesCluster, inventory: dict):
+def upgrade_inventory_packages(cluster: KubernetesCluster, inventory: dict) -> None:
     if cluster.context.get("initial_procedure") != "upgrade":
         return
 
     upgrade_version = cluster.context["upgrade_version"]
     for _type in ['install', 'upgrade', 'remove']:
         packages_section = cluster.procedure_inventory.get(upgrade_version, {}).get("packages", {})
         upgrade_packages = packages_section.get(_type)
@@ -186,15 +189,15 @@
                 'include': inventory_packages
             }
 
         default_merger.merge(inventory_packages, upgrade_packages)
 
 
 def _verify_upgrade_plan(cluster_associations: dict, previous_version: str,
-                         packages_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+                         packages_verify: List[str], upgrade_plan: List[Tuple[str, dict]]) -> None:
     cluster_associations = deepcopy(cluster_associations)
 
     # validate all packages sections in procedure inventory
     for version, upgrade_associations in upgrade_plan:
         for package in packages_verify:
             upgrade_package_name = upgrade_associations.get(package, {}).get('package_name')
             # Here default package names are not yet enriched and thus hold the custom supplied package names.
@@ -206,19 +209,19 @@
                 cluster_associations[package]['package_name'] = upgrade_package_name
         previous_version = version
 
 
 def get_default_package_names(os_family: str, package: str, kubernetes_version: str) -> List[str]:
     version_key = get_compatibility_version_key(os_family)
     compatibility = static.GLOBALS['compatibility_map']['software']
-    packages_names = static.GLOBALS['packages'][os_family][package]['package_name']
+    packages_names: List[Dict[str, str]] = static.GLOBALS['packages'][os_family][package]['package_name']
 
     package_versions = []
     for kv in packages_names:
-        package_name, software_name = list(kv.items())[0]
+        package_name, software_name = next((k, v) for k, v in kv.items())
         if software_name in ('haproxy', 'keepalived'):
             version = compatibility[software_name][version_key]
         else:
             version = compatibility[software_name][kubernetes_version][version_key]
 
         package_versions.append(f"{package_name}{get_package_version_separator(os_family)}{version}")
 
@@ -263,19 +266,19 @@
 
         if old_package_name is undefined_package_name or old_package_name != new_package_name:
             upgrade_required.append(package)
 
     return upgrade_required
 
 
-def _get_system_packages_support_upgrade(inventory: dict):
+def _get_system_packages_support_upgrade(inventory: dict) -> List[str]:
     return [inventory['services']['cri']['containerRuntime'], 'haproxy', 'keepalived']
 
 
-def enrich_inventory_include_all(inventory: dict, _):
+def enrich_inventory_include_all(inventory: dict, _: KubernetesCluster) -> dict:
     for _type in ['upgrade', 'remove']:
         packages: dict = inventory['services']['packages'].get(_type)
         if packages is not None:
             packages.setdefault('include', ['*'])
 
     return inventory
 
@@ -285,15 +288,15 @@
     # we still merge global associations section because it has priority during enrichment.
     upgrade_inventory_associations(cluster, inventory, enrich_global=True)
     upgrade_inventory_packages(cluster, inventory)
 
     return inventory
 
 
-def cache_package_versions(cluster: KubernetesCluster, inventory: dict, by_initial_nodes=False) -> dict:
+def cache_package_versions(cluster: KubernetesCluster, inventory: dict, by_initial_nodes: bool = False) -> dict:
     os_ids = cluster.get_os_identifiers()
     different_os = list(set(os_ids.values()))
     if len(different_os) > 1:
         cluster.log.debug(f"Final nodes have different OS families or versions, packages will not be cached. "
                           f"List of (OS family, version): {different_os}")
         return inventory
 
@@ -335,61 +338,61 @@
     :param inventory: Inventory of the cluster. May be different from the inventory of the cluster instance,
                       if used during finalization.
     :param ensured_association_only: Specify whether to take 'cache_versions' property into account for associations.
                                      Additionally, if true, will skip custom packages.
     :return: List of packages for each relevant host.
     """
     packages_section = inventory['services']['packages']
-    hosts_to_packages = {}
+    hosts_to_packages: Dict[str, List[str]] = {}
     for node in group.get_ordered_members_list():
         os_family = node.get_nodes_os()
         node_associations = packages_section['associations'].get(os_family, {})
         for association_name in node_associations.keys():
-            packages = get_association_hosts_to_packages(
+            host_packages = get_association_hosts_to_packages(
                 node, inventory, association_name, ensured_association_only)
 
-            packages = next(iter(packages.values()), [])
+            packages: List[str] = next(iter(host_packages.values()), [])
             hosts_to_packages.setdefault(node.get_host(), []).extend(packages)
 
     custom_install_packages = inventory['services']['packages'].get('install', {}).get('include', [])
     if not ensured_association_only and custom_install_packages:
         for host in group.get_hosts():
             hosts_to_packages.setdefault(host, []).extend(custom_install_packages)
 
     return hosts_to_packages
 
 
-def get_association_hosts_to_packages(group: NodeGroup, inventory: dict, association_name: str,
+def get_association_hosts_to_packages(group: AbstractGroup[RunResult], inventory: dict, association_name: str,
                                       ensured_association_only: bool = False) \
         -> Dict[str, List[str]]:
     """
     Returns hosts with associated packages list for the specified association name.
     Only subset of hosts is returned on which the association is managed by KubeMarine.
 
     :param group: Group of nodes to check the applicability of the association.
     :param inventory: Inventory of the cluster. May be different from the inventory of the cluster instance,
                       if used during finalization.
     :param association_name: target association name
     :param ensured_association_only: Specify whether to take 'cache_versions' property into account.
     :return: List of packages for each relevant host.
     """
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
 
     packages_section = inventory['services']['packages']
     if not packages_section['mandatory'].get(association_name, True):
         return {}
 
     hosts_to_packages = {}
 
     if association_name == 'unzip':
         from kubemarine import thirdparties
-        relevant_group = thirdparties.get_group_require_unzip(cluster, inventory)
+        relevant_group: AbstractGroup[RunResult] = thirdparties.get_group_require_unzip(cluster, inventory)
     else:
         groups = cluster.globals['packages']['common_associations'].get(association_name, {}).get('groups', [])
-        relevant_group = cluster.create_group_from_groups_nodes_names(groups, [])
+        relevant_group = cluster.make_group_from_roles(groups)
 
     if association_name in ('docker', 'containerd') \
             and association_name != inventory['services']['cri']['containerRuntime']:
         relevant_group = cluster.make_group([])
 
     relevant_group = relevant_group.intersection_group(group)
 
@@ -408,16 +411,16 @@
         if packages:
             hosts_to_packages[node.get_host()] = packages
 
     return hosts_to_packages
 
 
 def _cache_package_associations(group: NodeGroup, inventory: dict,
-                                detected_packages: Dict[str, Dict[str, List]], ensured_association_only: bool):
-    cluster = group.cluster
+                                detected_packages: Dict[str, Dict[str, List]], ensured_association_only: bool) -> None:
+    cluster: KubernetesCluster = group.cluster
     associations = inventory['services']['packages']['associations'][cluster.get_os_family()]
     for association_name, associated_params in associations.items():
         hosts_to_packages = get_association_hosts_to_packages(
             group, inventory, association_name, ensured_association_only)
         if not hosts_to_packages:
             continue
 
@@ -430,21 +433,21 @@
             final_package = _detect_final_package(cluster, detected_packages, package, ensured_association_only)
             final_packages_list.append(final_package)
 
         # if non-multiple value, then convert to simple string
         # packages can contain multiple package values, like docker package
         # (it has docker-ce, docker-cli and containerd.io packages for installation)
         if len(final_packages_list) == 1:
-            final_packages_list = final_packages_list[0]
-
-        associated_params['package_name'] = final_packages_list
+            associated_params['package_name'] = final_packages_list[0]
+        else:
+            associated_params['package_name'] = final_packages_list
 
 
 def _cache_custom_packages(cluster: KubernetesCluster, inventory: dict,
-                           detected_packages: Dict[str, Dict[str, List]], ensured_association_only: bool):
+                           detected_packages: Dict[str, Dict[str, List]], ensured_association_only: bool) -> None:
     if ensured_association_only:
         return
     # packages from direct installation section
     custom_install_packages = inventory['services']['packages'].get('install', {})
     if custom_install_packages.get('include', []):
         final_packages_list = []
         for package in custom_install_packages['include']:
@@ -471,25 +474,25 @@
                 f"Use default package '{package}' from inventory.")
             # return default package from inventory if multiple versions detected
             return package
     else:
         return detected_package_versions[0]
 
 
-def remove_unused_os_family_associations(cluster: KubernetesCluster, inventory: dict):
+def remove_unused_os_family_associations(cluster: KubernetesCluster, inventory: dict) -> dict:
     final_nodes = cluster.nodes['all'].get_final_nodes()
     for os_family in get_associations_os_family_keys():
         # Do not remove OS family associations section in finalized inventory if any node has this OS family.
         if final_nodes.get_subgroup_with_os(os_family).is_empty():
             del inventory['services']['packages']['associations'][os_family]
 
     return inventory
 
 
-def get_associations_os_family_keys():
+def get_associations_os_family_keys() -> Set[str]:
     return {'debian', 'rhel', 'rhel8'}
 
 
 def get_compatibility_version_key(os_family: str) -> str:
     """
     Get os-specific version key to be used in software compatibility map.
     :param os_family: one of supported OS families
@@ -497,77 +500,115 @@
     """
     if os_family in get_associations_os_family_keys():
         return f"version_{os_family}"
     else:
         raise ValueError(f"Unsupported {os_family!r} OS family")
 
 
-def get_package_manager(group: NodeGroup) -> apt or yum:
+class PackageManager(Protocol):
+    def ls_repofiles(self, group: NodeGroup) -> RunnersGroupResult: ...
+
+    def backup_repo(self, group: NodeGroup) -> Optional[RunnersGroupResult]: ...
+
+    def add_repo(self, group: NodeGroup, repo_data: Union[List[str], Dict[str, dict], str]) -> RunnersGroupResult: ...
+
+    def get_repo_file_name(self) -> str: ...
+
+    def create_repo_file(self, group: AbstractGroup[RunResult],
+                         repo_data: Union[List[str], Dict[str, dict], str],
+                         repo_file: str) -> None: ...
+
+    def clean(self, group: NodeGroup) -> RunnersGroupResult: ...
+
+    def install(self, group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+                exclude: Union[str, List[str]] = None,
+                callback: Callback = None) -> GROUP_RUN_TYPE: ...
+
+    def remove(self, group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+               exclude: Union[str, List[str]] = None,
+               warn: bool = False, hide: bool = True) -> GROUP_RUN_TYPE: ...
+
+    def upgrade(self, group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+                exclude: Union[str, List[str]] = None) -> GROUP_RUN_TYPE: ...
+
+    def no_changes_found(self, action: str, result: RunnersResult) -> bool: ...
+
+    def search(self, group: DeferredGroup, package: str, callback: Callback = None) -> Token: ...
+
+
+def get_package_manager(group: AbstractGroup[GROUP_RUN_TYPE]) -> PackageManager:
     os_family = group.get_nodes_os()
 
     if os_family in ['rhel', 'rhel8']:
         return yum
     elif os_family == 'debian':
         return apt
 
     raise Exception('Failed to return package manager for unknown or multiple OS')
 
 
-def ls_repofiles(group: NodeGroup, **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).ls_repofiles(group, **kwargs)
+def ls_repofiles(group: NodeGroup) -> RunnersGroupResult:
+    return get_package_manager(group).ls_repofiles(group)
 
 
-def backup_repo(group: NodeGroup, repo_filename="*", **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).backup_repo(group, repo_filename, **kwargs)
+def backup_repo(group: NodeGroup) -> Optional[RunnersGroupResult]:
+    return get_package_manager(group).backup_repo(group)
 
 
-def add_repo(group: NodeGroup, repo_data="", repo_filename="predefined", **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).add_repo(group, repo_data, repo_filename, **kwargs)
+def add_repo(group: NodeGroup, repo_data: Union[List[str], dict, str]) -> RunnersGroupResult:
+    return get_package_manager(group).add_repo(group, repo_data)
 
 
-def clean(group: NodeGroup, mode="all", **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).clean(group, mode, **kwargs)
+def get_repo_filename(group: AbstractGroup[RunResult]) -> str:
+    return get_package_manager(group).get_repo_file_name()
 
 
-def install(group: NodeGroup, include=None, exclude=None, **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).install(group, include, exclude, **kwargs)
+def create_repo_file(group: AbstractGroup[RunResult], repo_data: Union[List[str], dict, str], repo_file: str) -> None:
+    get_package_manager(group).create_repo_file(group, repo_data, repo_file)
 
 
-def remove(group: NodeGroup, include=None, exclude=None, **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).remove(group, include, exclude, **kwargs)
+def clean(group: NodeGroup) -> RunnersGroupResult:
+    return get_package_manager(group).clean(group)
 
 
-def upgrade(group: NodeGroup, include=None, exclude=None, **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).upgrade(group, include, exclude, **kwargs)
+def install(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+            exclude: Union[str, List[str]] = None,
+            callback: Callback = None) -> GROUP_RUN_TYPE:
+    return get_package_manager(group).install(group, include, exclude, callback)
 
 
-def no_changes_found(group: NodeGroup, action: callable, result: fabric.runners.Result) -> bool:
+def remove(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None, exclude: Union[str, List[str]] = None,
+           warn: bool = False, hide: bool = True) -> GROUP_RUN_TYPE:
+    return get_package_manager(group).remove(group, include, exclude, warn=warn, hide=hide)
+
+
+def upgrade(group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
+            exclude: Union[str, List[str]] = None) -> GROUP_RUN_TYPE:
+    return get_package_manager(group).upgrade(group, include, exclude)
+
+
+def no_changes_found(group: NodeGroup, action: str, result: RunnersResult) -> bool:
     pkg_mgr = get_package_manager(group)
-    if action is install:
-        action = pkg_mgr.install
-    elif action is upgrade:
-        action = pkg_mgr.upgrade
-    elif action is remove:
-        action = pkg_mgr.remove
     return pkg_mgr.no_changes_found(action, result)
 
 
+def search_package(group: DeferredGroup, package: str, callback: Callback = None) -> Token:
+    return get_package_manager(group).search(group, package, callback)
+
+
 def get_detect_package_version_cmd(os_family: str, package_name: str) -> str:
     if os_family in ["rhel", "rhel8"]:
         cmd = r"rpm -q %s" % package_name
     else:
         cmd = r"dpkg-query -f '${Package}=${Version}\n' -W %s" % package_name
 
-    # This is WA for RemoteExecutor, since any package failed others are not checked
-    # TODO: get rid of this WA and use warn=True in sudo
-    cmd += ' || true'
     return cmd
 
 
-def _detect_installed_package_version(group: NodeGroup, package: str) -> NodeGroupResult:
+def _detect_installed_package_version(group: DeferredGroup, package: str, collector: CollectorCallback) -> Token:
     """
     Detect package versions for each host on remote group
     :param group: Group of nodes, where package should be found
     :param package: package name, which version should be detected (eg. 'podman' and 'containerd')
     :return: NodeGroupResults with package version on each host
 
     Method generates different package query for different OS.
@@ -576,62 +617,58 @@
     (for example docker-ce* returns docker-ce and docker-ce-cli).
     """
 
     os_family = group.get_nodes_os()
     package_name = get_package_name(os_family, package)
 
     cmd = get_detect_package_version_cmd(os_family, package_name)
-    return group.sudo(cmd)
+    return group.sudo(cmd, warn=True, callback=collector)
 
 
-def _parse_node_detected_package(result: fabric.runners.Result, package: str) -> str:
+def _parse_node_detected_package(result: RunnersResult, package: str) -> str:
     node_detected_package = result.stdout.strip() + result.stderr.strip()
     # consider version, which ended with special symbol = or - as not installed
     # (it is possible in some cases to receive "containerd=" version)
     if "not installed" in node_detected_package or "no packages found" in node_detected_package \
             or node_detected_package[-1] == '=' or node_detected_package[-1] == '-':
         node_detected_package = f"not installed {package}"
 
     return node_detected_package
 
 
-def detect_installed_packages_version_hosts(cluster: KubernetesCluster, hosts_to_packages: Dict[str, List[str]]) \
-        -> Dict[str, Dict[str, List]]:
+def detect_installed_packages_version_hosts(
+        cluster: KubernetesCluster, hosts_to_packages: Mapping[str, Union[str, List[str]]]
+) -> Dict[str, Dict[str, List[str]]]:
     """
     Detect grouped packages versions for specified list of packages for each remote host.
 
     :param cluster: KubernetesCluster instance
     :param hosts_to_packages: Remote hosts with list of packages to detect versions.
     :return: Dictionary with grouped versions for each queried package, pointing to list of hosts,
         e.g. {"foo" -> {"foo-1": [host1, host2]}, "bar" -> {"bar-1": [host1], "bar-2": [host2]}}
     """
+    hosts_to_packages_dedup = {}
     for host, packages_list in hosts_to_packages.items():
         if isinstance(packages_list, str):
             packages_list = [packages_list]
         # deduplicate
-        hosts_to_packages[host] = list(set(packages_list))
+        hosts_to_packages_dedup[host] = list(set(packages_list))
 
-    with RemoteExecutor(cluster) as exe:
-        for host, packages_list in hosts_to_packages.items():
-            node = cluster.make_group([host])
-            for package in packages_list:
-                _detect_installed_package_version(node, package)
-
-    raw_result = exe.get_last_results()
-    if not raw_result:
-        return {}
+    collector = CollectorCallback(cluster)
+    with cluster.make_group(hosts_to_packages).new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            for package in hosts_to_packages_dedup[node.get_host()]:
+                _detect_installed_package_version(node, package, collector)
 
     results: Dict[str, Dict[str, List]] = {}
 
-    for conn, multiple_results in raw_result.items():
-        multiple_results = list(multiple_results.values())
-        host = conn.host
-        packages_list = hosts_to_packages[host]
-        for i, package in enumerate(packages_list):
-            node_detected_package = _parse_node_detected_package(multiple_results[i], package)
+    for host, multiple_results in collector.results.items():
+        for i, result in enumerate(multiple_results):
+            package = hosts_to_packages_dedup[host][i]
+            node_detected_package = _parse_node_detected_package(result, package)
             results.setdefault(package, {}).setdefault(node_detected_package, []).append(host)
 
     return results
 
 
 def get_package_version_separator(os_family: str) -> str:
     return '=' if os_family == 'debian' else '-'
@@ -651,19 +688,7 @@
             # regexp is needed to split package and its version, the pattern start with '-' then should be number or '*'
             package_name = re.split(r'-[\d,\*]', package)[0]
         else:
             # in ubuntu it is much easier to parse package name
             package_name = package.split("=")[0]
 
     return package_name
-
-
-def search_package(group: NodeGroup, package: str, **kwargs) -> NodeGroupResult:
-    return get_package_manager(group).search(group, package, **kwargs)
-
-
-def create_repo_file(group: NodeGroup, repo_data, repo_file):
-    get_package_manager(group).create_repo_file(group, repo_data, repo_file)
-
-
-def get_repo_filename(group: NodeGroup, repo_filename="predefined"):
-    return get_package_manager(group).get_repo_file_name(repo_filename)
```

### Comparing `kubemarine-0.18.2/kubemarine/patches/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.19.0/kubemarine/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/__init__.py` & `kubemarine-0.19.0/kubemarine/plugins/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import glob
 import importlib.util
 import io
-import logging
 import os
 import re
 import shutil
 import ssl
 import subprocess
 import sys
 import tarfile
@@ -28,58 +27,60 @@
 import urllib.request
 import zipfile
 from copy import deepcopy
 from distutils.dir_util import copy_tree
 from distutils.dir_util import remove_tree
 from distutils.dir_util import mkpath
 from itertools import chain
-from typing import Dict, List, Tuple
+from types import ModuleType
+from typing import Dict, List, Tuple, Callable, Union, no_type_check, Set
+
 import yaml
 import inspect
-from inspect import signature
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine import jinja, thirdparties
 from kubemarine.core import utils, static, errors, os as kos
 from kubemarine.core.yaml_merger import default_merger
-from kubemarine.core.group import NodeGroup, NodeGroupResult
+from kubemarine.core.group import NodeGroup
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.kubernetes.replicaset import ReplicaSet
 from kubemarine.kubernetes.statefulset import StatefulSet
 
 # list of plugins owned and managed by kubemarine
 oob_plugins = list(static.DEFAULTS["plugins"].keys())
-LOADED_MODULES = {}
+LOADED_MODULES: Dict[str, ModuleType] = {}
+
 
-def verify_inventory(inventory, cluster):
+def verify_inventory(inventory: dict, cluster: KubernetesCluster):
     for plugin_name, plugin_item in inventory["plugins"].items():
         for step in plugin_item.get('installation', {}).get('procedures', []):
             for procedure_type, configs in step.items():
-                if procedure_types[procedure_type].get('verify') is not None:
-                    procedure_types[procedure_type]['verify'](cluster, configs)
+                if procedure_types()[procedure_type].get('verify') is not None:
+                    procedure_types()[procedure_type]['verify'](cluster, configs)
 
     return inventory
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster):
     for plugin_name, plugin_item in inventory["plugins"].items():
         for i, step in enumerate(plugin_item.get('installation', {}).get('procedures', [])):
             for procedure_type, configs in step.items():
-                if procedure_types[procedure_type].get('convert') is not None:
-                    step[procedure_type] = procedure_types[procedure_type]['convert'](cluster, configs)
+                if procedure_types()[procedure_type].get('convert') is not None:
+                    step[procedure_type] = procedure_types()[procedure_type]['convert'](cluster, configs)
     return inventory
 
 
 def _get_upgrade_plan(cluster: KubernetesCluster) -> List[Tuple[str, dict]]:
     context = cluster.context
     if context.get("initial_procedure") == "upgrade":
         upgrade_version = context["upgrade_version"]
         upgrade_plan = []
-        for version in cluster.procedure_inventory.get('upgrade_plan'):
+        for version in cluster.procedure_inventory['upgrade_plan']:
             if utils.version_key(version) < utils.version_key(upgrade_version):
                 continue
 
             upgrade_plan.append((version, cluster.procedure_inventory.get(version, {}).get("plugins", {})))
 
     elif context.get("initial_procedure") == "migrate_kubemarine" and 'upgrading_plugin' in context:
         upgrade_plugins = cluster.procedure_inventory.get('upgrade', {}).get("plugins", {})
@@ -162,17 +163,19 @@
     _, upgrade_plugins = upgrade_plan[0]
     if upgrade_plugins:
         default_merger.merge(inventory.setdefault("plugins", {}), upgrade_plugins)
 
     return inventory
 
 
-def install(cluster, plugins=None):
-    if not plugins:
+def install(cluster: KubernetesCluster, plugins_: Dict[str, dict] = None):
+    if plugins_ is None:
         plugins = cluster.inventory["plugins"]
+    else:
+        plugins = plugins_
     plugins_queue: List[str] = []
     max_priority = 0
     for plugin_name, plugin_item in plugins.items():
         if plugin_item.get("install", False) and plugin_item.get("installation", {}).get('procedures') is not None:
             plugins_queue.append(plugin_name)
             if plugin_item.get("installation", {}).get('priority') is not None \
                     and plugin_item['installation']['priority'] > max_priority:
@@ -189,24 +192,24 @@
 
     cluster.log.debug('Starting plugins installation:')
 
     for plugin_name in plugins_queue:
         install_plugin(cluster, plugin_name, plugins[plugin_name]["installation"]['procedures'])
 
 
-def install_plugin(cluster, plugin_name, installation_procedure):
+def install_plugin(cluster: KubernetesCluster, plugin_name: str, installation_procedure: List[dict]):
     cluster.log.debug("**** INSTALLING PLUGIN %s ****" % plugin_name)
 
     for current_step_i, step in enumerate(installation_procedure):
         for apply_type, configs in step.items():
-            procedure_types[apply_type]['apply'](cluster, configs, plugin_name)
+            procedure_types()[apply_type]['apply'](cluster, configs, plugin_name)
 
 
 def expect_daemonset(cluster: KubernetesCluster,
-                     daemonsets_names: List[str] or List[Dict[str, str]],
+                     daemonsets_names: List[Union[str, Dict[str, str]]],
                      timeout: int = None,
                      retries: int = None,
                      node: NodeGroup = None) -> None:
     """
     The method waits for the configuration parameters of the given DaemonSets to be applied.
     :param cluster: KubernetesCluster object where method should be performed
     :param daemonsets_names: List of DaemonSet names (or dicts with name and namespace) to be
@@ -250,15 +253,15 @@
             cluster.log.debug(f"DaemonSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
     raise Exception('In the expected time, the DaemonSets did not become ready. Try to increase number of retries in expect.daemonsets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_replicaset(cluster: KubernetesCluster,
-                      replicasets_names: List[str] or List[Dict[str, str]],
+                      replicasets_names: List[Union[str, Dict[str, str]]],
                       timeout: int = None,
                       retries: int = None,
                       node: NodeGroup = None) -> None:
     """
     The method waits for the configuration parameters of the given ReplicaSets to be applied.
     :param cluster: KubernetesCluster object where method should be performed
     :param replicasets_names: List of ReplicaSets names (or dicts with name and namespace) to be
@@ -302,15 +305,15 @@
             cluster.log.debug(f"ReplicaSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
     raise Exception('In the expected time, the ReplicaSets did not become ready. Try to increase number of retries in expect.replicasets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_statefulset(cluster: KubernetesCluster,
-                       statefulsets_names: List[str] or List[Dict[str, str]],
+                       statefulsets_names: List[Union[str, Dict[str, str]]],
                        timeout: int = None,
                        retries: int = None,
                        node: NodeGroup = None) -> None:
     """
     The method waits for the configuration parameters of the given StatefulSets to be applied.
     :param cluster: KubernetesCluster object where method should be performed
     :param statefulsets_names: List of StatefulSets names (or dicts with name and namespace) to be
@@ -354,15 +357,15 @@
             cluster.log.debug(f"StatefulSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
     raise Exception('In the expected time, the StatefulSets did not become ready. Try to increase number of retries in expect.statefulsets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_deployment(cluster: KubernetesCluster,
-                      deployments_names: List[str] or List[Dict[str, str]],
+                      deployments_names: List[Union[str, Dict[str, str]]],
                       timeout: int = None,
                       retries: int = None,
                       node: NodeGroup = None):
     """
     The method waits for the configuration parameters of the given Deployments to be applied.
     :param cluster: KubernetesCluster object where method should be performed
     :param deployments_names: List of Deployments names (or dicts with name and namespace) to be
@@ -405,20 +408,16 @@
             retries -= 1
             cluster.log.debug(f"Deployments are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
     raise Exception('In the expected time, the Deployments did not become ready. Try to increase number of retries in expect.deployments: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
-def expect_pods(cluster, pods, namespace=None, timeout=None, retries=None,
-                node=None, apply_filter=None):
-
-    if isinstance(cluster, NodeGroup):
-        # when instead of cluster there was received a group
-        cluster = cluster.cluster
+def expect_pods(cluster: KubernetesCluster, pods: List[str], namespace=None, timeout=None, retries=None,
+                node: NodeGroup = None, apply_filter: str = None):
 
     if timeout is None:
         timeout = cluster.inventory['globals']['expect']['pods']['plugins']['timeout']
     if retries is None:
         retries = cluster.inventory['globals']['expect']['pods']['plugins']['retries']
 
     cluster.log.debug("Expecting the following pods to be ready: %s" % pods)
@@ -491,38 +490,38 @@
             cluster.log.debug("Pods are not ready yet... (%ss left)" % (retries * timeout))
             cluster.log.debug(running_pods_stdout)
             time.sleep(timeout)
 
     raise Exception('In the expected time, the pods did not become ready')
 
 
-def is_critical_state_in_stdout(cluster, stdout):
+def is_critical_state_in_stdout(cluster: KubernetesCluster, stdout: str):
     for state in cluster.globals['pods']['critical_states']:
         if state in stdout:
             return True
     return False
 
 
 # **** TEMPLATES ****
 
-def convert_template(cluster, config):
+def convert_template(_, config):
     return _convert_file(config)
 
 
-def verify_template(cluster, config):
+def verify_template(_, config: dict):
     return _verify_file(config, "Template")
 
 
-def apply_template(cluster, config, plugin_name=None):
+def apply_template(cluster: KubernetesCluster, config: dict, plugin_name=None):
     return _apply_file(cluster, config, "Template")
 
 
 # **** EXPECT ****
 
-def convert_expect(cluster, config):
+def convert_expect(_, config: dict):
     if config.get('daemonsets') is not None and isinstance(config['daemonsets'], list):
         config['daemonsets'] = {
             'list': config['daemonsets']
         }
     if config.get('replicasets') is not None and isinstance(config['replicasets'], list):
         config['replicasets'] = {
             'list': config['replicasets']
@@ -538,15 +537,15 @@
     if config.get('pods') is not None and isinstance(config['pods'], list):
         config['pods'] = {
             'list': config['pods']
         }
     return config
 
 
-def apply_expect(cluster, config, plugin_name=None):
+def apply_expect(cluster: KubernetesCluster, config: dict, plugin_name=None):
     # TODO: Add support for expect services and expect nodes
 
     for expect_type, expect_conf in config.items():
         if expect_type == 'daemonsets':
             expect_daemonset(cluster, config['daemonsets']['list'],
                              timeout=config['daemonsets'].get('timeout'),
                              retries=config['daemonsets'].get('retries'))
@@ -569,29 +568,31 @@
         elif expect_type == 'pods':
             expect_pods(cluster, config['pods']['list'], namespace=config['pods'].get('namespace'),
                         timeout=config['pods'].get('timeout'),
                         retries=config['pods'].get('retries'))
 
 # **** PYTHON ****
 
-def get_python_module(module_path):
+
+@no_type_check
+def get_python_module(module_path: str):
     if module_path in LOADED_MODULES:
         return LOADED_MODULES[module_path]
 
     spec = importlib.util.spec_from_file_location('module', module_path)
     try:
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         LOADED_MODULES[module_path] = module
     except Exception as e:
         raise ValueError(f"Could not import module {module_path}: {e}")
     return module 
 
 
-def get_python_method_args(cluster, step):
+def get_python_method_args(cluster: KubernetesCluster, step: dict):
     module_path, _ = utils.determine_resource_absolute_file(step['module'])
     method_name = step['method']
     method_arguments = step.get('arguments', {})
 
     module = get_python_module(module_path)
 
     # Check if the method exists
@@ -609,50 +610,50 @@
         signature.bind(cluster=cluster, **method_arguments)
     except TypeError as e:
         raise ValueError(f"Invalid arguments for method {method_name}: {e}")
 
     return method, method_arguments
 
 
-def verify_python(cluster, step):
+def verify_python(cluster: KubernetesCluster, step: dict):
     method, method_arguments = get_python_method_args(cluster, step)
     # Additional verification logic can be added here
 
 
-def apply_python(cluster, step, plugin_name=None):
+def apply_python(cluster: KubernetesCluster, step: dict, plugin_name=None):
     method, method_arguments = get_python_method_args(cluster, step)
 
     cluster.log.debug("Running method %s from %s module..." % (method.__name__, method.__module__))
     method(cluster, **method_arguments)
 
 
 # **** THIRDPARTIES ****
 
-def verify_thirdparty(cluster, thirdparty):
+def verify_thirdparty(cluster: KubernetesCluster, thirdparty: str):
     defined_thirdparties = list(cluster.inventory['services'].get('thirdparties', {}).keys())
     if thirdparty not in defined_thirdparties:
         raise Exception('Specified thirdparty %s not found in thirdpartirs definition. Expected any of %s.'
                         % (thirdparty, defined_thirdparties))
 
 
 def apply_thirdparty(cluster: KubernetesCluster, thirdparty: str, plugin_name=None):
     return thirdparties.install_thirdparty(cluster.nodes['all'], thirdparty)
 
 
 # **** SHELL ****
 
-def convert_shell(cluster, config):
+def convert_shell(_, config):
     if isinstance(config, str):
         config = {
             'command': config
         }
     return config
 
 
-def verify_shell(cluster, config):
+def verify_shell(cluster: KubernetesCluster, config: dict):
     out_vars = config.get('out_vars', [])
     groups = config.get('groups', [])
     nodes = config.get('nodes', [])
     explicit_group = cluster.create_group_from_groups_nodes_names(groups, nodes)
     if out_vars and (groups or nodes) and explicit_group.nodes_amount() != 1:
         raise Exception('Shell output variables could be used for single-node groups, but multi-node group was found')
 
@@ -662,15 +663,15 @@
         var_name = var['name']
         if len(words_splitter.split(var_name)) > 1:
             raise Exception(f"'{var_name}' is not a valid shell variable name")
 
     # TODO: verify fields types and contents
 
 
-def apply_shell(cluster, step, plugin_name=None):
+def apply_shell(cluster: KubernetesCluster, step: dict, plugin_name=None):
     commands = step['command']
     sudo = step.get('sudo', False)
     groups = step.get('groups', [])
     nodes = step.get('nodes', [])
     in_vars = step.get('in_vars', [])
     out_vars = step.get('out_vars', [])
     vars_separator = "~~~~EXPORTED_VARIABLE~~~~"
@@ -679,15 +680,15 @@
         common_group = cluster.nodes['control-plane'].get_any_member()
     else:
         common_group = cluster.create_group_from_groups_nodes_names(groups, nodes)
 
     if isinstance(commands, list):
         commands = ' && '.join(commands)
 
-    out_vars_aliases = {}
+    out_vars_aliases: Dict[str, Set[str]] = {}
     for var in out_vars:
         var_name = var['name']
         if var_name in out_vars_aliases:
             # var is already exported, need to only add alternative alias
             out_vars_aliases[var_name].add(var.get('save_as', var_name))
             continue
 
@@ -696,30 +697,29 @@
         # quotes usage is important for following code to work correctly in different cases
         echo_var_cmd = f"echo {vars_separator} && " \
             f"echo name: {var_name} && " \
             f"echo 'value: |2-' && " \
             f"echo \"${var_name}\" | sed 's/^/  /'"
         commands = f"{commands} && {echo_var_cmd}"
 
-    in_vars_dict = {}
+    in_vars_dict: Dict[str, str] = {}
     for var in in_vars:
         var_name = var['name']
         # get defined value or saved value, defaulting to empty value
         var_value = var.get('value', cluster.context['runtime_vars'].get(var_name, ''))
         # replace single-quotes with '"'"' to isolate all single quotes during ssh env inlining
         var_value = var_value.replace("'", "'\"'\"'")
         # wrap variable value with single-quotes for `inline_ssh_env` feature to work correctly with different content
         in_vars_dict[var_name] = f"'{var_value}'"
 
-    method = common_group.run
-    if sudo:
-        method = common_group.sudo
-
     cluster.log.debug('Running shell command...')
-    result = method(commands, env=in_vars_dict)
+    if sudo:
+        result = common_group.sudo(commands, env=in_vars_dict)
+    else:
+        result = common_group.run(commands, env=in_vars_dict)
 
     if out_vars:
         stdout = list(result.values())[0].stdout
         stdout_parts = stdout.split(vars_separator)
         cluster.log.debug(stdout_parts[0])  # printing original user output
         for part in stdout_parts[1:]:
             var = yaml.safe_load(part)
@@ -730,34 +730,34 @@
         cluster.log.debug(result)
 
     return result
 
 
 # **** ANSIBLE ****
 
-def convert_ansible(cluster, config):
+def convert_ansible(_, config):
     if isinstance(config, str):
         config = {
             'playbook': config
         }
     return config
 
 
-def _get_absolute_playbook(config) -> str:
+def _get_absolute_playbook(config: dict) -> str:
     return utils.determine_resource_absolute_file(config['playbook'])[0]
 
 
-def verify_ansible(cluster: KubernetesCluster, config):
+def verify_ansible(cluster: KubernetesCluster, config: dict):
     _get_absolute_playbook(config)
     if cluster.is_deploying_from_windows():
         raise Exception("Executing of playbooks on Windows deployer is currently not supported")
     # TODO: verify fields types and contents
 
 
-def apply_ansible(cluster, step, plugin_name=None):
+def apply_ansible(cluster: KubernetesCluster, step: dict, plugin_name=None):
     playbook_path = _get_absolute_playbook(step)
     external_vars = step.get('vars', {})
     become = step.get('become', False)
     groups = step.get('groups', [])
     nodes = step.get('nodes', [])
 
     command = 'ansible-playbook -i ansible-inventory.ini %s' % playbook_path
@@ -780,15 +780,15 @@
     result = subprocess.run(command, stdout=sys.stdout, stderr=sys.stderr, shell=True)
     if result.returncode != 0:
         raise Exception("Failed to apply ansible plugin, see error above")
 
     return result
 
 
-def apply_helm(cluster: KubernetesCluster, config, plugin_name=None):
+def apply_helm(cluster: KubernetesCluster, config: dict, plugin_name=None):
     chart_path = get_local_chart_path(cluster.log, config)
     process_chart_values(config, chart_path)
 
     from kubemarine import kubernetes
     local_config_path = kubernetes.fetch_admin_config(cluster)
 
     with utils.open_external(os.path.join(chart_path, 'Chart.yaml'), 'r') as stream:
@@ -815,22 +815,22 @@
     if release in helm_existed_releases.splitlines():
         cluster.log.debug("Deployed release %s is found. Upgrading it..." % release)
         deployment_mode = "upgrade"
     else:
         cluster.log.debug("Deployed release %s is not found. Installing it..." % release)
         deployment_mode = "install"
 
-    command = prepare_for_helm_command + f'{deployment_mode} {release} {chart_path} --debug'
+    command = prepare_for_helm_command + f'{deployment_mode} {release} {chart_path} --create-namespace --debug'
     output = subprocess.check_output(command, shell=True)
     cluster.log.debug(output.decode('utf-8'))
 
     return output
 
 
-def process_chart_values(config, local_chart_path):
+def process_chart_values(config: dict, local_chart_path: str):
     config_values = config.get("values")
     file_values = None
     config_values_file = config.get("values_file")
     if config_values_file is not None:
         with utils.open_external(config_values_file) as stream:
             file_values = yaml.safe_load(stream)
 
@@ -846,16 +846,16 @@
     # Values from 'values' section have priority over values in 'values_file' section
     if config_values is not None:
         merged_values = default_merger.merge(merged_values, config_values)
 
     utils.dump_file({}, yaml.dump(merged_values), chart_values, dump_location=False)
 
 
-def get_local_chart_path(log, config):
-    chart_path = config.get('chart_path')
+def get_local_chart_path(log, config: dict):
+    chart_path = config['chart_path']
 
     is_curl = chart_path[:4] == 'http' and '://' in chart_path[4:8]
 
     local_chart_folder = "local_chart_folder"
     if os.path.isdir(local_chart_folder):
         remove_tree(local_chart_folder)
     mkpath(local_chart_folder)
@@ -900,41 +900,41 @@
         if not os.path.commonpath([chart_metadata[i], local_chart_folder]) == local_chart_folder:
             raise Exception(
                 f"Incorrect format of helm chart: inner {chart_metadata[i]} is not inside {local_chart_folder} directory.")
 
     return local_chart_folder
 
 
-def convert_config(cluster, config):
+def convert_config(_, config):
     return _convert_file(config)
 
 
-def verify_config(cluster, config):
+def verify_config(_, config: dict):
     return _verify_file(config, "Config")
 
 
-def apply_config(cluster, config, plugin_name=None):
+def apply_config(cluster: KubernetesCluster, config: dict, plugin_name=None):
     return _apply_file(cluster, config, "Config")
 
 
 def _convert_file(config):
     if isinstance(config, str):
         config = {
             'source': config
         }
     return config
 
 
-def get_source_absolute_pattern(config) -> Tuple[str, bool]:
+def get_source_absolute_pattern(config: dict) -> Tuple[str, bool]:
     abs_dir, is_external = utils.determine_resource_absolute_dir(config['source'])
     basename = os.path.basename(config['source'])
     return os.path.join(abs_dir, basename), is_external
 
 
-def _verify_file(config, file_type):
+def _verify_file(config: dict, file_type: str):
     """
         Verifies if the path matching the config 'source' key exists and points to
         existing files.
     """
 
     # Determite absolute path to templates
     source, _ = get_source_absolute_pattern(config)
@@ -954,14 +954,15 @@
     """
         Apply yamls as is or
         renders and applies templates that match the config 'source' key.
     """
     log = cluster.log
     do_render = config.get('do_render', True)
 
+    source: Union[str, io.StringIO]
     source, is_external = get_source_absolute_pattern(config)
     files = glob.glob(source)
 
     for file in files:
         cfg_copy = dict(config)
         source_filename = os.path.basename(file)
         source = file
@@ -1017,53 +1018,54 @@
         apply_common_group = cluster.nodes['control-plane'].get_any_member()
     else:
         apply_common_group = cluster.create_group_from_groups_nodes_names(apply_groups, apply_nodes)
 
     destination_common_group.put(source, destination_path, backup=True, sudo=use_sudo)
 
     if apply_required:
-        method = apply_common_group.run
-        if use_sudo:
-            method = apply_common_group.sudo
         cluster.log.debug("Applying yaml...")
-        method(apply_command, logging_stream_level=logging.DEBUG)
+        if use_sudo:
+            apply_common_group.sudo(apply_command, hide=False)
+        else:
+            apply_common_group.run(apply_command, hide=False)
     else:
         cluster.log.debug('Apply is not required')
 
 
-procedure_types = {
-    'template': {
-        'convert': convert_template,
-        'verify': verify_template,
-        'apply': apply_template
-    },
-    'expect': {
-        'convert': convert_expect,
-        'apply': apply_expect
-    },
-    'python': {
-        'verify': verify_python,
-        'apply': apply_python
-    },
-    'thirdparty': {
-        'verify': verify_thirdparty,
-        'apply': apply_thirdparty
-    },
-    'shell': {
-        'convert': convert_shell,
-        'verify': verify_shell,
-        'apply': apply_shell
-    },
-    'ansible': {
-        'convert': convert_ansible,
-        'verify': verify_ansible,
-        'apply': apply_ansible
-    },
-    'helm': {
-        'apply': apply_helm
-    },
-    'config': {
-        'convert': convert_config,
-        'verify': verify_config,
-        'apply': apply_config
-    },
-}
+def procedure_types() -> Dict[str, Dict[str, Callable]]:
+    return {
+        'template': {
+            'convert': convert_template,
+            'verify': verify_template,
+            'apply': apply_template
+        },
+        'expect': {
+            'convert': convert_expect,
+            'apply': apply_expect
+        },
+        'python': {
+            'verify': verify_python,
+            'apply': apply_python
+        },
+        'thirdparty': {
+            'verify': verify_thirdparty,
+            'apply': apply_thirdparty
+        },
+        'shell': {
+            'convert': convert_shell,
+            'verify': verify_shell,
+            'apply': apply_shell
+        },
+        'ansible': {
+            'convert': convert_ansible,
+            'verify': verify_ansible,
+            'apply': apply_ansible
+        },
+        'helm': {
+            'apply': apply_helm
+        },
+        'config': {
+            'convert': convert_config,
+            'verify': verify_config,
+            'apply': apply_config
+        },
+    }
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/builtin.py` & `kubemarine-0.19.0/kubemarine/plugins/builtin.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "calico": CalicoManifestProcessor,
     "nginx-ingress-controller": get_ingress_nginx_manifest_processor,
     "kubernetes-dashboard": get_dashboard_manifest_processor,
     "local-path-provisioner": LocalPathProvisionerManifestProcessor,
 }
 
 
-def verify_inventory(inventory: dict, cluster: KubernetesCluster):
+def verify_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     for plugin_name, processor_provider in MANIFEST_PROCESSOR_PROVIDERS.items():
         if not inventory["plugins"][plugin_name]["install"]:
             continue
 
         items = inventory['plugins'][plugin_name]['installation']['procedures']
         for i, item in enumerate(items):
             if 'python' not in item:
@@ -52,32 +52,36 @@
 
             expected_args = {'plugin_name', 'original_yaml_path', 'destination_name'}
             declared_args = set(arguments.keys())
             if not declared_args.issubset(expected_args):
                 raise Exception(f"Unexpected python method arguments {list(declared_args.difference(expected_args))} "
                                 f"in {plugin_name!r} installation step {i}.")
 
-            processor_provider(cluster.log, inventory, **arguments).validate_inventory()
+            processor = processor_provider(
+                cluster.log, inventory, arguments.get('original_yaml_path'), arguments.get('destination_name')
+            )
+            processor.validate_inventory()
             break
         else:
             cluster.log.warning(f"Invocation of plugins.builtin.apply_yaml is not found for {plugin_name!r} plugin. "
                                 f"Such configuration is obsolete, and support for it may be stopped in future releases.")
 
     return inventory
 
 
-def get_manifest_processor(logger: log.VerboseLogger, inventory: dict, plugin_name: str, **arguments):
+def get_manifest_processor(logger: log.VerboseLogger, inventory: dict, plugin_name: str,
+                           **arguments: str) -> manifest.Processor:
     if plugin_name not in MANIFEST_PROCESSOR_PROVIDERS:
         raise Exception(f"Manifest processor is not registered for {plugin_name!r} plugin.")
 
     processor_provider = MANIFEST_PROCESSOR_PROVIDERS[plugin_name]
-    return processor_provider(logger, inventory, **arguments)
+    return processor_provider(logger, inventory, arguments.get('original_yaml_path'), arguments.get('destination_name'))
 
 
-def apply_yaml(cluster: KubernetesCluster, **arguments):
+def apply_yaml(cluster: KubernetesCluster, **arguments: str) -> None:
     arguments = dict(arguments)
     plugin_name = arguments.pop('plugin_name')
 
     processor = get_manifest_processor(cluster.log, cluster.inventory, plugin_name, **arguments)
 
     manifest = processor.enrich()
     processor.apply(cluster, manifest)
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/calico.py` & `kubemarine-0.19.0/kubemarine/plugins/calico.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import ipaddress
-from typing import Optional, List
+from typing import Optional, List, Dict
 
 import os
 
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
 # DEPRECATED
-def apply_calico_yaml(cluster: KubernetesCluster, calico_original_yaml: str, calico_yaml: str):
+def apply_calico_yaml(cluster: KubernetesCluster, calico_original_yaml: str, calico_yaml: str) -> None:
     """
     The method implements full processing for Calico plugin
     :param calico_original_yaml: path to original Calico manifest
     :param calico_yaml: file name of the resulting Calico manifest
     :param cluster: Cluster object
     """
 
@@ -125,33 +125,33 @@
         The method implements the enrichment procedure for 'calico-node' container in Calico node DaemonSet.
         The method attempts to preserve initial formatting.
 
         :param container_pos: container position in spec
         :param container: object describing a container
         """
         key = "DaemonSet_calico-node"
-        env_delete = []
+        env_delete: List[str] = []
         ip = self.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
         if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
             env_delete.extend([
                 'CALICO_IPV6POOL_CIDR', 'IP6', 'IP6_AUTODETECTION_METHOD',
                 'CALICO_IPV6POOL_IPIP', 'CALICO_IPV6POOL_VXLAN'
             ])
         if utils.true_or_false(self.inventory['plugins']['calico']['typha']['enabled']) == "false":
             env_delete.append('FELIX_TYPHAK8SSERVICENAME')
 
-        for env in env_delete:
+        for name in env_delete:
             for i, e in enumerate(container['env']):
-                if e['name'] == env:
+                if e['name'] == name:
                     del container['env'][i]
-                    self.log.verbose(f"The {env!r} env variable has been removed from "
+                    self.log.verbose(f"The {name!r} env variable has been removed from "
                                     f"'spec.template.spec.containers.[{container_pos}].env' in the {key}")
                     break
 
-        env_update = {}
+        env_update: Dict[str, dict] = {}
         for name, value in self.inventory['plugins']['calico']['env'].items():
             if name in env_delete:
                 continue
             if type(value) is str:
                 env_update[name] = {'value': value}
             elif type(value) is dict:
                 env_update[name] = {'valueFrom': value}
@@ -179,17 +179,17 @@
     def enrich_deployment_calico_typha(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Typha Deployment
         :param manifest: Container to operate with manifest objects
         """
 
         key = "Deployment_calico-typha"
-        source_yaml = manifest.get_obj(key, patch=True, allow_absent=True)
-        if source_yaml is None:
-            return
+        if not manifest.has_obj(key):
+            return None
+        source_yaml = manifest.get_obj(key, patch=True)
 
         default_tolerations = [{'key': 'node.kubernetes.io/network-unavailable', 'effect': 'NoSchedule'},
                                {'key': 'node.kubernetes.io/network-unavailable', 'effect': 'NoExecute'}]
 
         val = self.inventory['plugins']['calico']['typha']['replicas']
         source_yaml['spec']['replicas'] = int(val)
         self.log.verbose(f"The {key} has been patched in 'spec.replicas' with '{val}'")
@@ -226,16 +226,15 @@
             api_list = source_yaml['rules']
             api_list.append(psp_calico_node)
             self.log.verbose(f"The {key} has been patched in 'rules' with '{psp_calico_node}'")
 
     def enrich_crd_felix_configuration(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico CRD Felixconfigurations
-        :param cluster: Cluster object
-        :param obj_list: list of objects for enrichment
+        :param manifest: Container to operate with manifest objects
         """
 
         key = "CustomResourceDefinition_felixconfigurations.crd.projectcalico.org"
         source_yaml = manifest.get_obj(key, patch=True)
 
         api_list = \
         source_yaml['spec']['versions'][0]['schema']['openAPIV3Schema']['properties']['spec']['properties'][
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.19.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from typing import List, Optional
 
 from kubemarine.core import summary, utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
-def schedule_summary_report(cluster: KubernetesCluster):
+def schedule_summary_report(cluster: KubernetesCluster) -> None:
     plugin_item = cluster.inventory['plugins']['kubernetes-dashboard']
     hostname = plugin_item['hostname']
     # Currently we declare that Dashboard UI is available only via HTTPS
     summary.schedule_report(cluster.context, summary.SummaryItem.DASHBOARD_URL, f'https://{hostname}')
 
 
 class DashboardManifestProcessor(Processor):
     def __init__(self, logger: log.VerboseLogger, inventory: dict,
-                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
+                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None) -> None:
         super().__init__(logger, inventory, 'kubernetes-dashboard', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_kubernetes-dashboard",
             "ServiceAccount_kubernetes-dashboard",
             "Service_kubernetes-dashboard",
@@ -51,50 +51,49 @@
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
         return [
             self.enrich_namespace_kubernetes_dashboard,
             self.enrich_deployment_kubernetes_dashboard,
             self.enrich_deployment_dashboard_metrics_scraper,
         ]
 
-    def enrich_namespace_kubernetes_dashboard(self, manifest: Manifest):
+    def enrich_namespace_kubernetes_dashboard(self, manifest: Manifest) -> None:
         key = "Namespace_kubernetes-dashboard"
         rbac = self.inventory['rbac']
         if rbac['admission'] == 'pss' and rbac['pss']['pod-security'] == 'enabled' \
                 and rbac['pss']['defaults']['enforce'] == 'restricted':
             self.assign_default_pss_labels(manifest, key, 'baseline')
 
-    def enrich_deployment_kubernetes_dashboard(self, manifest: Manifest):
+    def enrich_deployment_kubernetes_dashboard(self, manifest: Manifest) -> None:
         key = "Deployment_kubernetes-dashboard"
         self.enrich_image_for_container(manifest, key,
             plugin_service='dashboard', container_name='kubernetes-dashboard', is_init_container=False)
 
         self.enrich_node_selector(manifest, key, plugin_service='dashboard')
         self.enrich_tolerations(manifest, key, plugin_service='dashboard', override=True)
 
-    def enrich_deployment_dashboard_metrics_scraper(self, manifest: Manifest):
+    def enrich_deployment_dashboard_metrics_scraper(self, manifest: Manifest) -> None:
         key = "Deployment_dashboard-metrics-scraper"
         self.enrich_image_for_container(manifest, key,
             plugin_service='metrics-scraper', container_name='dashboard-metrics-scraper', is_init_container=False)
 
         self.enrich_node_selector(manifest, key, plugin_service='metrics-scraper')
         self.enrich_tolerations(manifest, key, plugin_service='metrics-scraper', override=True)
 
 
 class V2_5_X_DashboardManifestProcessor(DashboardManifestProcessor):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def enrich_deployment_dashboard_metrics_scraper(self, manifest: Manifest):
+    def enrich_deployment_dashboard_metrics_scraper(self, manifest: Manifest) -> None:
         key = "Deployment_dashboard-metrics-scraper"
         source_yaml = manifest.get_obj(key, patch=True)
         template_spec: dict = source_yaml['spec']['template']['spec']
         del template_spec['securityContext']
         self.log.verbose(f"The 'securityContext' property has been removed from 'spec.template.spec' in the {key}")
         super().enrich_deployment_dashboard_metrics_scraper(manifest)
 
 
-def get_dashboard_manifest_processor(logger: log.VerboseLogger, inventory: dict, **kwargs):
+def get_dashboard_manifest_processor(logger: log.VerboseLogger, inventory: dict,
+                                     yaml_path: Optional[str] = None, destination: Optional[str] = None) -> Processor:
     version: str = inventory['plugins']['kubernetes-dashboard']['version']
+    kwargs = {'original_yaml_path': yaml_path, 'destination_name': destination}
     if utils.minor_version(version) == 'v2.5':
         return V2_5_X_DashboardManifestProcessor(logger, inventory, **kwargs)
 
     return DashboardManifestProcessor(logger, inventory, **kwargs)
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.19.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import yaml
 
 from kubemarine.core import log
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 class LocalPathProvisionerManifestProcessor(Processor):
     def __init__(self, logger: log.VerboseLogger, inventory: dict,
-                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
+                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None) -> None:
         super().__init__(logger, inventory, 'local-path-provisioner', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_local-path-storage",
             "ServiceAccount_local-path-provisioner-service-account",
             "ClusterRole_local-path-provisioner-role",
@@ -41,51 +41,51 @@
             self.enrich_namespace_local_path_storage,
             self.add_clusterrolebinding_local_path_provisioner_privileged_psp,
             self.enrich_deployment_local_path_provisioner,
             self.enrich_storageclass_local_path,
             self.enrich_configmap_local_path_config,
         ]
 
-    def enrich_namespace_local_path_storage(self, manifest: Manifest):
+    def enrich_namespace_local_path_storage(self, manifest: Manifest) -> None:
         key = "Namespace_local-path-storage"
         rbac = self.inventory['rbac']
         if rbac['admission'] == 'pss' and rbac['pss']['pod-security'] == 'enabled' \
                 and rbac['pss']['defaults']['enforce'] != 'privileged':
             self.assign_default_pss_labels(manifest, key, 'privileged')
 
-    def add_clusterrolebinding_local_path_provisioner_privileged_psp(self, manifest: Manifest):
+    def add_clusterrolebinding_local_path_provisioner_privileged_psp(self, manifest: Manifest) -> None:
         # TODO add only if psp is enabled?
         new_yaml = yaml.safe_load(clusterrolebinding_local_path_provisioner_privileged_psp)
         # Insert new ClusterRoleBinding after all existing resources of this kind
         max_crb_idx = max(i for i, key in enumerate(manifest.all_obj_keys())
                           if key.startswith("ClusterRoleBinding_"))
         self.include(manifest, max_crb_idx + 1, new_yaml)
 
-    def enrich_deployment_local_path_provisioner(self, manifest: Manifest):
+    def enrich_deployment_local_path_provisioner(self, manifest: Manifest) -> None:
         key = "Deployment_local-path-provisioner"
         self.enrich_image_for_container(manifest, key,
             container_name='local-path-provisioner', is_init_container=False)
 
         self.enrich_tolerations(manifest, key)
 
-    def enrich_storageclass_local_path(self, manifest: Manifest):
+    def enrich_storageclass_local_path(self, manifest: Manifest) -> None:
         key = "StorageClass_local-path"
         source_yaml = manifest.get_obj(key, patch=True)
         metadata = source_yaml['metadata']
 
         is_default = str(self.inventory['plugins']['local-path-provisioner']['storage-class']['is-default'])
         metadata.setdefault('annotations', {})['storageclass.kubernetes.io/is-default-class'] = is_default
         self.log.verbose(f"The {key} has been patched in 'metadata.annotations' "
                          f"with 'storageclass.kubernetes.io/is-default-class: {is_default}'")
 
         name = self.inventory['plugins']['local-path-provisioner']['storage-class']['name']
         metadata['name'] = self.inventory['plugins']['local-path-provisioner']['storage-class']['name']
         self.log.verbose(f"The {key} has been patched in 'metadata.name' with {name!r}")
 
-    def enrich_configmap_local_path_config(self, manifest: Manifest):
+    def enrich_configmap_local_path_config(self, manifest: Manifest) -> None:
         key = "ConfigMap_local-path-config"
         source_yaml = manifest.get_obj(key, patch=True)
         data = source_yaml['data']
 
         config_json = data['config.json']
         config_json = config_json.replace('/opt/local-path-provisioner',
                                           self.inventory['plugins']['local-path-provisioner']['volume-dir'])
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/manifest.py` & `kubemarine-0.19.0/kubemarine/plugins/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,39 +9,39 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-from typing import Callable, Optional, List, IO
+from typing import Callable, Optional, List, IO, Tuple, cast
 
 import ruamel.yaml
 import os
 from abc import ABC, abstractmethod
 
 from ordered_set import OrderedSet
 
 from kubemarine import plugins
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 
 ERROR_MANIFEST_NOT_FOUND = "Cannot find original manifest %s for '%s' plugin"
 
 
-def get_default_manifest_path(plugin_name: str, version: str):
+def get_default_manifest_path(plugin_name: str, version: str) -> str:
     resource = f"plugins/yaml/{plugin_name}-{version}-original.yaml"
     return utils.get_internal_resource_path(resource)
 
 
 class Manifest:
-    def __init__(self, stream: IO):
-        self._patched = OrderedSet()
-        self._excluded = OrderedSet()
-        self._included = OrderedSet()
+    def __init__(self, stream: IO) -> None:
+        self._patched = OrderedSet[str]()
+        self._excluded = OrderedSet[str]()
+        self._included = OrderedSet[str]()
         self._obj_list = self._load(stream)
 
     def obj_key(self, obj: dict) -> str:
         return f"{obj['kind']}_{obj['metadata']['name']}"
 
     def all_obj_keys(self) -> List[str]:
         return [self.obj_key(obj) for obj in self._obj_list]
@@ -49,42 +49,42 @@
     def key_index(self, key: str) -> int:
         for i, obj in enumerate(self._obj_list):
             if self.obj_key(obj) == key:
                 return i
 
         raise ValueError(f"{key} not found")
 
-    def get_obj(self, key: str, *, patch: bool, allow_absent=False) -> Optional[dict]:
+    def has_obj(self, key: str) -> bool:
+        return any(self.obj_key(obj) == key for obj in self._obj_list)
+
+    def get_obj(self, key: str, *, patch: bool) -> dict:
         """
         Get manifest object in YAML format for the specified key.
         By default, ensure presence of the object.
         If the object is absent, it may be a sign that we no longer able to fulfill the previous contract.
         Caller methods must explicitly allow absent object when necessary.
 
         :param key: 'kind' and 'name' of object
         :param patch: boolean value that tells the manifest that the searched object is going to be patched.
-        :param allow_absent: if true, do not throw exception if the object by key is absent.
         :return: manifest object
         """
         for obj in self._obj_list:
             if self.obj_key(obj) == key:
                 if patch:
                     self._patched.add(key)
                 return obj
 
-        if not allow_absent:
-            raise ValueError(f"{key} not found")
-        return None
+        raise ValueError(f"{key} not found")
 
-    def include(self, index: int, obj: dict):
+    def include(self, index: int, obj: dict) -> None:
         self._obj_list.insert(index, obj)
         key = self.obj_key(obj)
         self._included.add(key)
 
-    def exclude(self, key: str):
+    def exclude(self, key: str) -> None:
         del self._obj_list[self.key_index(key)]
         self._excluded.add(key)
 
     @property
     def patched(self) -> List[str]:
         return list(self._patched)
 
@@ -147,15 +147,15 @@
 
 
 EnrichmentFunction = Callable[[Manifest], None]
 
 
 class Processor(ABC):
     def __init__(self, logger: log.VerboseLogger, inventory: dict, plugin_name: str,
-                 original_yaml_path: Optional[str], destination_name: Optional[str]):
+                 original_yaml_path: Optional[str], destination_name: Optional[str]) -> None:
         """
         :param logger: VerboseLogger instance
         :param inventory: inventory of the cluster
         :param plugin_name: name of plugin-owner
         :param original_yaml_path: path to custom manifest
         :param destination_name: custom destination manifest file name
         """
@@ -175,22 +175,23 @@
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
         """
         :return: list of enrichment methods
         """
         pass
 
     def get_version(self) -> str:
-        return self.inventory['plugins'][self.plugin_name]['version']
+        version: str = self.inventory['plugins'][self.plugin_name]['version']
+        return version
 
-    def include(self, manifest: Manifest, index: int, obj: dict):
+    def include(self, manifest: Manifest, index: int, obj: dict) -> None:
         key = manifest.obj_key(obj)
         manifest.include(index, obj)
         self.log.verbose(f"The {key} has been added")
 
-    def exclude(self, manifest: Manifest, key: str):
+    def exclude(self, manifest: Manifest, key: str) -> None:
         manifest.exclude(key)
         self.log.verbose(f"The {key} has been excluded from result")
 
     def validate_inventory(self) -> None:
         """
         # Check if original YAML exists
         """
@@ -208,15 +209,15 @@
         # check if there are new objects
         for key in manifest.all_obj_keys():
             if key not in known_objects:
                 self.log.verbose(f"The current version of original yaml has a new object: {key}")
 
         # check if known objects were excluded
         for key in known_objects:
-            if manifest.get_obj(key, patch=False, allow_absent=True) is None:
+            if not manifest.has_obj(key):
                 self.log.verbose(f"The current version of original yaml does not include "
                                  f"the following object: {key}")
 
     def enrich(self) -> Manifest:
         """
         The method implements full processing for the plugin main manifest.
         """
@@ -240,15 +241,15 @@
         self.log.verbose(f"The total number of added objects is {len(manifest.included)} "
                          f"the objects are the following: {manifest.included}")
         self.log.verbose(f"The total number of excluded objects is {len(manifest.excluded)} "
                          f"the objects are the following: {manifest.excluded}")
 
         return manifest
 
-    def apply(self, cluster: KubernetesCluster, manifest: Manifest):
+    def apply(self, cluster: KubernetesCluster, manifest: Manifest) -> None:
         logger = cluster.log
         enriched_manifest = manifest.dump()
         utils.dump_file(cluster, enriched_manifest, self.destination_name)
 
         destination = '/etc/kubernetes/%s' % self.destination_name
 
         # create config for plugin module
@@ -268,118 +269,126 @@
             config = {"source": custom_manifest_path}
             manifest_path, _ = plugins.get_source_absolute_pattern(config)
         else:
             manifest_path = get_default_manifest_path(self.plugin_name, self.get_version())
 
         return manifest_path
 
-    def _get_destination(self, custom_destination_name) -> str:
+    def _get_destination(self, custom_destination_name: Optional[str]) -> str:
         if custom_destination_name is not None:
             return custom_destination_name
 
         return f'{self.plugin_name}-{self.get_version()}.yaml'
 
-    def assign_default_pss_labels(self, manifest: Manifest, key: str, profile: str):
+    def assign_default_pss_labels(self, manifest: Manifest, key: str, profile: str) -> None:
         source_yaml = manifest.get_obj(key, patch=True)
         labels: dict = source_yaml['metadata'].setdefault('labels', {})
         labels.update({
             'pod-security.kubernetes.io/enforce': profile,
             'pod-security.kubernetes.io/enforce-version': 'latest',
             'pod-security.kubernetes.io/audit': profile,
             'pod-security.kubernetes.io/audit-version': 'latest',
             'pod-security.kubernetes.io/warn': profile,
             'pod-security.kubernetes.io/warn-version': 'latest',
         })
         self.log.verbose(f"The {key} has been patched in 'metadata.labels' with pss labels for {profile!r} profile")
 
     def find_container_for_patch(self, manifest: Manifest, key: str,
                                  *,
-                                 container_name: str, is_init_container: bool, allow_absent=False) -> (int, dict):
+                                 container_name: str, is_init_container: bool) -> Tuple[int, dict]:
         """
         Find container according to the search criteria.
 
         :param manifest: container to operate with manifest objects
         :param key: 'kind' and 'name' of object
         :param container_name: name of container to assign the image in the spec
         :param is_init_container: whether to search container in 'initContainers' or in 'containers' spec.
-        :param allow_absent: if True, and if container is not found, return -1, None
         :return: tuple of container index within the spec and the container data.
         """
+        pos, container = self._find_optional_container(
+            manifest, key,
+            container_name=container_name, is_init_container=is_init_container, allow_absent=False)
+
+        return pos, cast(dict, container)
+
+    def _find_optional_container(self, manifest: Manifest, key: str,
+                                 container_name: str, is_init_container: bool, allow_absent: bool = False) \
+            -> Tuple[int, Optional[dict]]:
         source_yaml = manifest.get_obj(key, patch=True)
         template_spec = source_yaml['spec']['template']['spec']
         spec_containers_section = 'initContainers' if is_init_container else 'containers'
         container_pos, container = next(((i, c) for i, c in enumerate(template_spec[spec_containers_section])
                                          if c['name'] == container_name),
                                         (-1, None))
 
         if container_pos == -1 and not allow_absent:
             raise ValueError(f"Container {container_name!r} is not found in {spec_containers_section!r} spec of {key}")
 
         return container_pos, container
 
-    def get_target_image(self, plugin_service: Optional[str] = None, image_key: Optional[str] = 'image'):
+    def get_target_image(self, plugin_service: Optional[str] = None, image_key: Optional[str] = 'image') -> str:
         """
         Calculates full image path from the plugin configuration in inventory.
 
         :param plugin_service: section of plugin that contains the desirable image_key
         :param image_key: property name by which the inventory holds the desirable image
         :return: target image to be used in a container
         """
         plugin_section = self.inventory['plugins'][self.plugin_name]
         registry = plugin_section['installation'].get('registry')
         plugin_service_section = plugin_section
         if plugin_service:
             plugin_service_section = plugin_service_section[plugin_service]
-        image = plugin_service_section[image_key]
+        image: str = plugin_service_section[image_key]
         if registry:
             image = f"{registry}/{image}"
 
         return image
 
     def enrich_image_for_container(self, manifest: Manifest, key: str,
                                    *,
                                    plugin_service: Optional[str] = None,
                                    container_name: str, is_init_container: bool,
-                                   allow_absent=False) -> None:
+                                   allow_absent: bool = False) -> None:
         """
         The method patches the image of the specified container.
 
         :param manifest: container to operate with manifest objects
         :param key: 'kind' and 'name' of object
         :param plugin_service: section of plugin that contains the desirable 'image'
         :param container_name: name of container to assign the image in the spec
         :param is_init_container: whether to search container in 'initContainers' or in 'containers' spec.
         :param allow_absent: if True, and if container is not found, silently do nothing.
         """
         image = self.get_target_image(plugin_service=plugin_service, image_key='image')
 
         spec_containers_section = 'initContainers' if is_init_container else 'containers'
 
-        container_pos, container = self.find_container_for_patch(manifest, key,
+        container_pos, container = self._find_optional_container(manifest, key,
             container_name=container_name, is_init_container=is_init_container, allow_absent=allow_absent)
-        if container_pos == -1:
+        if container is None:
             return
 
         container['image'] = image
         self.log.verbose(f"The {key} has been patched in "
                          f"'spec.template.spec.{spec_containers_section}.[{container_pos}].image' with {image!r}")
 
     def enrich_node_selector(self, manifest: Manifest, key: str,
                              *,
-                             plugin_service: str):
+                             plugin_service: str) -> None:
         source_yaml = manifest.get_obj(key, patch=True)
         node_selector = self.inventory['plugins'][self.plugin_name][plugin_service]['nodeSelector']
         source_yaml['spec']['template']['spec']['nodeSelector'] = node_selector
         self.log.verbose(f"The {key} has been patched in 'spec.template.spec.nodeSelector' with {node_selector!r}")
 
     def enrich_tolerations(self, manifest: Manifest, key: str,
                            *,
                            plugin_service: Optional[str] = None,
                            extra_tolerations: List[dict] = None,
-                           override=False):
+                           override: bool = False) -> None:
         source_yaml = manifest.get_obj(key, patch=True)
         template_spec: dict = source_yaml['spec']['template']['spec']
         if override and template_spec.get('tolerations', []):
             del template_spec['tolerations']
             self.log.verbose(f"The 'tolerations' property has been removed from 'spec.template.spec' in the {key}")
 
         tolerations: List[dict] = []
@@ -391,8 +400,8 @@
         tolerations.extend(plugin_service_section.get('tolerations', []))
 
         for val in tolerations:
             template_spec.setdefault('tolerations', []).append(val)
             self.log.verbose(f"The {key} has been patched in 'spec.template.spec.tolerations' with '{val}'")
 
 
-PROCESSOR_PROVIDER = Callable[[log.VerboseLogger, dict, str, str], Processor]
+PROCESSOR_PROVIDER = Callable[[log.VerboseLogger, dict, Optional[str], Optional[str]], Processor]
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.19.0/kubemarine/plugins/nginx_ingress.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,42 +18,43 @@
 
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
-def check_job_for_nginx(cluster: KubernetesCluster):
-    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+def check_job_for_nginx(cluster: KubernetesCluster) -> None:
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
     version = cluster.inventory['plugins']['nginx-ingress-controller']['version'].replace('v', '.').split('.')
 
     major_version = int(version[1])
     minor_version = int(version[2])
 
-    check_jobs = first_control_plane['connection'].sudo(f"kubectl get jobs -n ingress-nginx")
+    check_jobs = first_control_plane.sudo(f"kubectl get jobs -n ingress-nginx")
     if list(check_jobs.values())[0].stderr == "" and major_version >= 1 and minor_version >= 4:
         cluster.log.debug('Delete old jobs for nginx')
-        first_control_plane['connection'].sudo(f"sudo kubectl delete job --all -n ingress-nginx", is_async=False)
+        first_control_plane.sudo(f"sudo kubectl delete job --all -n ingress-nginx")
     else:
         cluster.log.debug('There are no jobs to delete')
 
-def enrich_inventory(inventory, _):
+
+def enrich_inventory(inventory: dict, _: KubernetesCluster) -> dict:
     if not inventory["plugins"]["nginx-ingress-controller"]["install"]:
         return inventory
 
     if inventory["plugins"]["nginx-ingress-controller"].get('custom_headers'):
         if not inventory["plugins"]["nginx-ingress-controller"].get('config_map'):
             inventory["plugins"]["nginx-ingress-controller"]['config_map'] = {}
         if not inventory["plugins"]["nginx-ingress-controller"]['config_map'].get('proxy-set-headers'):
             inventory["plugins"]["nginx-ingress-controller"]['config_map']['proxy-set-headers'] = 'ingress-nginx/custom-headers'
 
     return inventory
 
 
-def cert_renew_enrichment(inventory, cluster):
+def cert_renew_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     # check that renewal is required for nginx
     if cluster.context.get('initial_procedure') != 'cert_renew' \
             or not cluster.procedure_inventory.get("nginx-ingress-controller"):
         return inventory
 
     nginx_plugin = inventory["plugins"]["nginx-ingress-controller"]
 
@@ -63,15 +64,15 @@
 
     # update certificates in inventory
     nginx_plugin["controller"]["ssl"]["default-certificate"] = cluster.procedure_inventory["nginx-ingress-controller"]
 
     return inventory
 
 
-def finalize_inventory(cluster, inventory_to_finalize):
+def finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     # check that renewal is required for nginx
     if cluster.context.get('initial_procedure') != 'cert_renew' \
             or not cluster.procedure_inventory.get("nginx-ingress-controller"):
         return inventory_to_finalize
 
     if not inventory_to_finalize["plugins"].get("nginx-ingress-controller"):
         inventory_to_finalize["plugins"]["nginx-ingress-controller"] = {}
@@ -84,15 +85,15 @@
 
     nginx_plugin = inventory_to_finalize["plugins"]["nginx-ingress-controller"]
     nginx_plugin["controller"]["ssl"]["default-certificate"] = cluster.procedure_inventory["nginx-ingress-controller"]
 
     return inventory_to_finalize
 
 
-def manage_custom_certificate(cluster):
+def manage_custom_certificate(cluster: KubernetesCluster) -> None:
     if not cluster.inventory["plugins"]["nginx-ingress-controller"]["controller"]["ssl"].get("default-certificate"):
         cluster.log.debug("No custom default ingress certificate specified, skipping...")
         return
 
     base_path = "/etc/kubernetes/custom-certs"
     certificate_path = base_path + "/cert"
     private_key_path = base_path + "/key"
@@ -121,41 +122,41 @@
                           name=secret_name,
                           namespace=secret_namespace)
     finally:
         # fourth, we need to remove base path dir
         first_control_plane.sudo(f"rm -rf {base_path}")
 
 
-def put_custom_certificate(first_control_plane: NodeGroup, default_cert, crt_path, key_path):
+def put_custom_certificate(first_control_plane: NodeGroup, default_cert: dict, crt_path: str, key_path: str) -> None:
     if default_cert.get("data"):
         cert = io.StringIO(default_cert["data"]["cert"])
         key = io.StringIO(default_cert["data"]["key"])
     else:
         cert = io.StringIO(utils.read_external(default_cert["paths"]["cert"]))
         key = io.StringIO(utils.read_external(default_cert["paths"]["key"]))
 
     first_control_plane.put(cert, crt_path, sudo=True)
     first_control_plane.put(key, key_path, sudo=True)
 
 
-def verify_certificate_and_key(first_control_plane: NodeGroup, crt_path, key_path):
+def verify_certificate_and_key(first_control_plane: NodeGroup, crt_path: str, key_path: str) -> None:
     crt_md5 = first_control_plane.sudo(f"openssl x509 -noout -modulus -in {crt_path} | openssl md5").get_simple_out()
     key_md5 = first_control_plane.sudo(f"openssl rsa -noout -modulus -in {key_path} | openssl md5").get_simple_out()
     if crt_md5 != key_md5:
         raise Exception("Custom default ingress certificate and key are not compatible!")
 
 
-def create_tls_secret(first_control_plane, crt_path, key_path, name, namespace):
+def create_tls_secret(first_control_plane: NodeGroup, crt_path: str, key_path: str, name: str, namespace: str) -> None:
     first_control_plane.sudo(f"kubectl create secret tls {name} --key {key_path} --cert {crt_path} -n {namespace} "
                       f"--dry-run -o yaml | sudo kubectl apply -f -", timeout=300)
 
 
 class IngressNginxManifestProcessor(Processor):
     def __init__(self, logger: log.VerboseLogger, inventory: dict,
-                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
+                 original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None) -> None:
         super().__init__(logger, inventory, 'nginx-ingress-controller', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_ingress-nginx",
             "ServiceAccount_ingress-nginx",
             "ServiceAccount_ingress-nginx-admission",
@@ -185,43 +186,43 @@
             self.enrich_deployment_ingress_nginx_controller,
             self.enrich_ingressclass_nginx,
             self.enrich_job_ingress_nginx_admission_create,
             self.enrich_job_ingress_nginx_admission_patch,
             self.enrich_service_ingress_nginx_controller,
         ]
 
-    def enrich_namespace_ingress_nginx(self, manifest: Manifest):
+    def enrich_namespace_ingress_nginx(self, manifest: Manifest) -> None:
         key = "Namespace_ingress-nginx"
         rbac = self.inventory['rbac']
         if rbac['admission'] == 'pss' and rbac['pss']['pod-security'] == 'enabled' \
                 and rbac['pss']['defaults']['enforce'] != 'privileged':
             self.assign_default_pss_labels(manifest, key, 'privileged')
 
-    def enrich_configmap_ingress_nginx_controller(self, manifest: Manifest):
+    def enrich_configmap_ingress_nginx_controller(self, manifest: Manifest) -> None:
         key = "ConfigMap_ingress-nginx-controller"
         config_map = self.inventory['plugins']['nginx-ingress-controller'].get('config_map')
         if config_map:
             source_yaml = manifest.get_obj(key, patch=True)
             data: dict = source_yaml['data']
             data.update(config_map)
             self.log.verbose(f"The {key} has been patched in 'data' "
                              f"with the data from 'plugins.nginx-ingress-controller.config_map'")
 
-    def add_configmap_ingress_nginx_controller(self, manifest: Manifest):
+    def add_configmap_ingress_nginx_controller(self, manifest: Manifest) -> None:
         custom_headers = self.inventory['plugins']['nginx-ingress-controller'].get('custom_headers')
         if custom_headers:
             custom_headers_cm = dict(CUSTOM_HEADERS_CM)
             custom_headers_cm['data'] = custom_headers
             # Insert custom-headers ConfigMap before ingress-nginx-controller ConfigMap
             ingres_nginx_cm = manifest.key_index("ConfigMap_ingress-nginx-controller")
             self.include(manifest, ingres_nginx_cm, custom_headers_cm)
             self.log.verbose(f"The {manifest.obj_key(custom_headers_cm)} has been patched in 'data' "
                              f"with the data from 'plugins.nginx-ingress-controller.custom_headers'")
 
-    def enrich_deployment_ingress_nginx_controller(self, manifest: Manifest):
+    def enrich_deployment_ingress_nginx_controller(self, manifest: Manifest) -> None:
         key = "Deployment_ingress-nginx-controller"
         source_yaml = manifest.get_obj(key, patch=True)
 
         container_pos, container = self.find_container_for_patch(
             manifest, key, container_name='controller', is_init_container=False)
         self.enrich_deamonset_ingress_nginx_controller_container(container_pos, container)
 
@@ -231,27 +232,27 @@
         self.enrich_node_selector(manifest, key, plugin_service='controller')
         self.enrich_tolerations(manifest, key, plugin_service='controller')
 
         # Patch kind in the last step to avoid sudden key change in log messages
         source_yaml['kind'] = 'DaemonSet'
         self.log.verbose(f"The {key} has been patched in 'kind' with 'DaemonSet'")
 
-    def enrich_deamonset_ingress_nginx_controller_container(self, container_pos: int, container: dict):
+    def enrich_deamonset_ingress_nginx_controller_container(self, container_pos: int, container: dict) -> None:
         key = "Deployment_ingress-nginx-controller"
         container_args = container['args']
         for i, arg in enumerate(container_args):
             if arg.startswith('--publish-service='):
                 del container_args[i]
                 self.log.verbose(f"The {arg!r} argument has been removed from "
                                  f"'spec.template.spec.containers.[{container_pos}].args' in the {key}")
                 break
         else:
             raise Exception("Failed to find '--publish-service' argument in ingress-nginx-controller container specification.")
 
-        extra_args = [
+        extra_args: List[tuple] = [
             ('--watch-ingress-without-class=', 'true')
         ]
         ssl_options = self.inventory['plugins']['nginx-ingress-controller']['controller']['ssl']
         additional_args = self.inventory['plugins']['nginx-ingress-controller']['controller'].get('args')
 
         if additional_args:
             for arg in additional_args:
@@ -283,66 +284,63 @@
                 self.log.verbose(f"The {arg!r} argument has been added to "
                                  f"'spec.template.spec.containers.[{container_pos}].args' in the {key}")
 
         container['ports'] = self.inventory['plugins']['nginx-ingress-controller']['ports']
         self.log.verbose(f"The {key} has been patched in 'spec.template.spec.containers.[{container_pos}].ports' "
                          f"with the data from 'plugins.nginx-ingress-controller.ports'")
 
-    def enrich_ingressclass_nginx(self, manifest: Manifest):
+    def enrich_ingressclass_nginx(self, manifest: Manifest) -> None:
         key = "IngressClass_nginx"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['metadata'].setdefault('annotations', {})['ingressclass.kubernetes.io/is-default-class'] = 'true'
         self.log.verbose(f"The {key} has been patched in 'metadata.annotations' "
                          f"with 'ingressclass.kubernetes.io/is-default-class: true'")
 
-    def enrich_job_ingress_nginx_admission_create(self, manifest: Manifest):
+    def enrich_job_ingress_nginx_admission_create(self, manifest: Manifest) -> None:
         key = "Job_ingress-nginx-admission-create"
         self.enrich_image_for_container(manifest, key,
             plugin_service='webhook', container_name='create', is_init_container=False)
 
-    def enrich_job_ingress_nginx_admission_patch(self, manifest: Manifest):
+    def enrich_job_ingress_nginx_admission_patch(self, manifest: Manifest) -> None:
         key = "Job_ingress-nginx-admission-patch"
         self.enrich_image_for_container(manifest, key,
             plugin_service='webhook', container_name='patch', is_init_container=False)
 
-    def enrich_service_ingress_nginx_controller(self, manifest: Manifest):
+    def enrich_service_ingress_nginx_controller(self, manifest: Manifest) -> None:
         # The method needs some rework in case of dual stack support
         key = "Service_ingress-nginx-controller"
         ip = self.inventory['services']['kubeadm']['networking']['serviceSubnet'].split('/')[0]
         if type(ipaddress.ip_address(ip)) is ipaddress.IPv6Address:
             source_yaml = manifest.get_obj(key, patch=True)
             source_yaml['spec']['ipFamilies'] = ['IPv6']
             self.log.verbose(f"The {key} has been patched in 'spec.ipFamilies' with 'IPv6'")
 
 
 class V1_2_X_IngressNginxManifestProcessor(IngressNginxManifestProcessor):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
         enrichment_functions = super().get_enrichment_functions()
         enrichment_functions.extend([
             self.exclude_webhook_resources,
             self.enrich_role_ingress_nginx,
         ])
         return enrichment_functions
 
-    def enrich_configmap_ingress_nginx_controller(self, manifest: Manifest):
+    def enrich_configmap_ingress_nginx_controller(self, manifest: Manifest) -> None:
         key = "ConfigMap_ingress-nginx-controller"
         source_yaml = manifest.get_obj(key, patch=True)
         # For some reason, we took manifest for Digital Ocean, removed use-proxy-protocol: "true" property,
         # but left service.beta.kubernetes.io/do-loadbalancer-enable-proxy-protocol: "true" annotation
         # in ingress-nginx-controller Service.
         # The behaviour is left as-is for compatibility.
         # For v.1.4.0 we took the default manifest which lacks of the mentioned properties.
         del source_yaml['data']['use-proxy-protocol']
         self.log.verbose(f"The 'use-proxy-protocol' property has been removed from 'data' in the {key}")
         super().enrich_configmap_ingress_nginx_controller(manifest)
 
-    def enrich_deamonset_ingress_nginx_controller_container(self, container_pos: int, container: dict):
+    def enrich_deamonset_ingress_nginx_controller_container(self, container_pos: int, container: dict) -> None:
         key = "Deployment_ingress-nginx-controller"
         container_args = container['args']
         webhook_args_remove = [
             '--validating-webhook=',
             '--validating-webhook-certificate=',
             '--validating-webhook-key='
         ]
@@ -356,46 +354,48 @@
 
         del container['volumeMounts']
         self.log.verbose(f"The 'volumeMounts' property has been removed "
                          f"from 'spec.template.spec.containers.[{container_pos}]' in the {key}")
 
         super().enrich_deamonset_ingress_nginx_controller_container(container_pos, container)
 
-    def enrich_job_ingress_nginx_admission_create(self, manifest: Manifest):
+    def enrich_job_ingress_nginx_admission_create(self, manifest: Manifest) -> None:
         return
 
-    def enrich_job_ingress_nginx_admission_patch(self, manifest: Manifest):
+    def enrich_job_ingress_nginx_admission_patch(self, manifest: Manifest) -> None:
         return
 
-    def exclude_webhook_resources(self, manifest: Manifest):
+    def exclude_webhook_resources(self, manifest: Manifest) -> None:
         webhook_resources = [
             "ServiceAccount_ingress-nginx-admission",
             "Role_ingress-nginx-admission",
             "ClusterRole_ingress-nginx-admission",
             "RoleBinding_ingress-nginx-admission",
             "ClusterRoleBinding_ingress-nginx-admission",
             "Service_ingress-nginx-controller-admission",
             "Job_ingress-nginx-admission-create",
             "Job_ingress-nginx-admission-patch",
             "ValidatingWebhookConfiguration_ingress-nginx-admission",
         ]
         for key in webhook_resources:
             self.exclude(manifest, key)
 
-    def enrich_role_ingress_nginx(self, manifest: Manifest):
+    def enrich_role_ingress_nginx(self, manifest: Manifest) -> None:
         key = "Role_ingress-nginx"
         source_yaml = manifest.get_obj(key, patch=True)
         # TODO patch only if psp is enabled?
         api_list = source_yaml['rules']
         api_list.append(psp_ingress_nginx)
         self.log.verbose(f"The {key} has been patched in 'rules' with {psp_ingress_nginx}")
 
 
-def get_ingress_nginx_manifest_processor(logger: log.VerboseLogger, inventory: dict, **kwargs):
+def get_ingress_nginx_manifest_processor(logger: log.VerboseLogger, inventory: dict,
+                                         yaml_path: Optional[str] = None, destination: Optional[str] = None) -> Processor:
     version: str = inventory['plugins']['nginx-ingress-controller']['version']
+    kwargs = {'original_yaml_path': yaml_path, 'destination_name': destination}
     if utils.minor_version(version) == 'v1.2':
         return V1_2_X_IngressNginxManifestProcessor(logger, inventory, **kwargs)
 
     return IngressNginxManifestProcessor(logger, inventory, **kwargs)
 
 
 CUSTOM_HEADERS_CM = {
```

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/procedures/__init__.py` & `kubemarine-0.19.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/procedures/add_node.py` & `kubemarine-0.19.0/kubemarine/procedures/add_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,74 +11,77 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import copy
+import typing
 
 from collections import OrderedDict
+from typing import Any
+
 from kubemarine import kubernetes, packages
 from kubemarine.core import flow, utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 
 
-def deploy_kubernetes_join(cluster):
+def deploy_kubernetes_join(cluster: KubernetesCluster):
 
-    group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_new_nodes()
+    group = cluster.make_group_from_roles(['control-plane', 'worker']).get_new_nodes()
 
     if group.is_empty():
         cluster.log.debug("No kubernetes nodes to perform")
         return
 
     cluster.nodes['control-plane'].get_new_nodes().call(kubernetes.join_new_control_plane)
 
     if "worker" in cluster.nodes:
-        cluster.nodes["worker"].get_new_nodes().new_group(apply_filter=lambda node: 'control-plane' not in node['roles']) \
+        cluster.nodes['worker'].get_new_nodes().exclude_group(cluster.nodes['control-plane']) \
             .call(kubernetes.init_workers)
 
     group.call_batch([
         kubernetes.apply_labels,
         kubernetes.apply_taints
     ])
 
     cluster.log.debug("Waiting for new kubernetes nodes...")
     kubernetes.wait_for_nodes(group)
     kubernetes.schedule_running_nodes_report(cluster)
 
 
-def add_node_finalize_inventory(cluster, inventory_to_finalize):
+def add_node_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
     if cluster.context.get('initial_procedure') != 'add_node':
         return inventory_to_finalize
 
     new_nodes = cluster.nodes['all'].get_new_nodes()
 
     # add nodes to inventory if they in new nodes
-    for new_node in new_nodes.get_ordered_members_list(provide_node_configs=True):
+    for new_node in new_nodes.get_ordered_members_list():
+        new_node_name = new_node.get_node_name()
         new_node_found = False
         for i, node in enumerate(inventory_to_finalize['nodes']):
-            if node['name'] == new_node['name']:
+            if node['name'] == new_node_name:
                 # new node already presented in final inventory - ok, just remove label
                 if 'add_node' in inventory_to_finalize['nodes'][i]['roles']:
                     inventory_to_finalize['nodes'][i]['roles'].remove('add_node')
-                    cluster.inventory['nodes'][i]['roles'].remove('add_node')
                 new_node_found = True
                 break
 
         # new node is not presented in final inventory - let's add it original config
         if not new_node_found:
             node_config = None
 
             # search for new node config in procedure inventory
             if cluster.procedure_inventory.get('nodes', {}):
                 for node_from_procedure in cluster.procedure_inventory['nodes']:
-                    if node_from_procedure['name'] == new_node['name']:
+                    if node_from_procedure['name'] == new_node_name:
                         node_config = node_from_procedure
                         break
             # maybe new nodes from other places?
 
             if node_config is None:
                 raise Exception('Not possible to find new node config for final inventory')
             inventory_to_finalize["nodes"].append(node_config)
@@ -95,15 +98,15 @@
     Task which is used to collect already installed packages versions on already existing nodes.
     It is called first during "add_node" procedure,
     so that new nodes install exactly the same packages as on other already existing nodes.
     """
     packages.cache_package_versions(cluster, cluster.inventory, by_initial_nodes=True)
 
 
-tasks = OrderedDict(copy.deepcopy(install.tasks))
+tasks: typing.OrderedDict[str, Any] = OrderedDict(copy.deepcopy(install.tasks))
 del tasks["deploy"]["plugins"]
 del tasks["deploy"]["accounts"]
 tasks["deploy"]["kubernetes"]["init"] = deploy_kubernetes_join
 tasks["cache_packages"] = cache_installed_packages
 tasks.move_to_end("cache_packages", last=False)
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/backup.py` & `kubemarine-0.19.0/kubemarine/procedures/backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import json
 import os
 import random
 import shutil
 import tarfile
 import time
 from collections import OrderedDict
+from typing import List
+
 import yaml
 
 from kubemarine.core import utils, flow
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
@@ -61,67 +63,67 @@
     elif cri_impl == "containerd":
         backup_files_list.append("/etc/containerd/config.toml")
         backup_files_list.append("/etc/crictl.yaml")
 
     return backup_files_list
 
 
-def prepare_backup_tmpdir(cluster):
+def prepare_backup_tmpdir(cluster: KubernetesCluster):
     backup_directory = cluster.context.get('backup_tmpdir')
     if not backup_directory:
         cluster.log.verbose('Backup directory is not ready yet, preparing..')
         backup_directory = cluster.context['backup_tmpdir'] = utils.get_dump_filepath(cluster.context, 'backup')
         shutil.rmtree(backup_directory, ignore_errors=True)
         os.mkdir(backup_directory)
         cluster.log.verbose('Backup directory prepared')
     return backup_directory
 
 
-def verify_backup_location(cluster):
+def verify_backup_location(cluster: KubernetesCluster):
     target = utils.get_external_resource_path(cluster.procedure_inventory.get('backup_location', 'backup.tar.gz'))
     if not os.path.isdir(target) and not os.path.isdir(os.path.abspath(os.path.join(target, os.pardir))):
         raise FileNotFoundError('Backup location directory not exists')
 
 
-def export_ansible_inventory(cluster):
+def export_ansible_inventory(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
     shutil.copyfile(cluster.context['execution_arguments']['ansible_inventory_location'],
                     os.path.join(backup_directory, 'ansible-inventory.ini'))
     cluster.log.verbose('ansible-inventory.ini exported to backup')
 
 
 def export_packages_list(cluster: KubernetesCluster):
     cluster.context['backup_descriptor']['nodes']['packages'] = {}
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         cmd = r"rpm -qa"
     else:
         cmd = r"dpkg-query -f '${Package}=${Version}\n' -W"
     results = cluster.nodes['all'].sudo(cmd)
-    for conn, result in results.items():
-        cluster.context['backup_descriptor']['nodes']['packages'][conn.host] = result.stdout.strip().split('\n')
+    for host, result in results.items():
+        cluster.context['backup_descriptor']['nodes']['packages'][host] = result.stdout.strip().split('\n')
 
 
-def export_hostname(cluster):
+def export_hostname(cluster: KubernetesCluster):
     cluster.context['backup_descriptor']['nodes']['hostnames'] = {}
     results = cluster.nodes['all'].sudo('hostnamectl status | head -n 1 | sed -e \'s/[a-zA-Z ]*://g\'')
     cluster.log.verbose(results)
-    for conn, result in results.items():
-        cluster.context['backup_descriptor']['nodes']['hostnames'][conn.host] = result.stdout.strip()
+    for host, result in results.items():
+        cluster.context['backup_descriptor']['nodes']['hostnames'][host] = result.stdout.strip()
 
 
-def export_cluster_yaml(cluster):
+def export_cluster_yaml(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
     shutil.copyfile(utils.get_dump_filepath(cluster.context, 'cluster.yaml'),
                     os.path.join(backup_directory, 'cluster.yaml'))
     shutil.copyfile(utils.get_external_resource_path(cluster.context['execution_arguments']['config']),
                     os.path.join(backup_directory, 'original_cluster.yaml'))
     cluster.log.verbose('cluster.yaml exported to backup')
 
 
-def export_nodes(cluster):
+def export_nodes(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
     backup_nodes_data_dir = os.path.join(backup_directory, 'nodes_data')
     os.mkdir(backup_nodes_data_dir)
 
     backup_list = get_default_backup_files_list(cluster)
     for filepath, enabled in cluster.procedure_inventory.get('backup_plan', {}).get('nodes', {}).items():
         if not enabled and filepath in backup_list:
@@ -137,18 +139,18 @@
                      'sudo du -hs /tmp/kubemarine-backup.tar.gz' % (' '.join(backup_list))
 
     data_copy_res = cluster.nodes['all'].run(backup_command)
 
     cluster.log.debug('Backup created:\n%s' % data_copy_res)
 
     cluster.log.debug('Downloading nodes backups:')
-    for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
-        node['connection'].get('/tmp/kubemarine-backup.tar.gz',
-                               os.path.join(backup_nodes_data_dir, '%s.tar.gz' % node['name']))
-        cluster.log.debug('Backup \'%s\' downloaded' % node['name'])
+    for node in cluster.nodes['all'].get_ordered_members_list():
+        node.get('/tmp/kubemarine-backup.tar.gz',
+                 os.path.join(backup_nodes_data_dir, '%s.tar.gz' % node.get_node_name()))
+        cluster.log.debug('Backup \'%s\' downloaded' % node.get_node_name())
 
     cluster.log.verbose('Deleting backup file from nodes...')
     cluster.nodes['all'].sudo('rm -f /tmp/kubemarine-backup.tar.gz')
 
 
 def export_etcd(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
@@ -162,22 +164,22 @@
         cluster.log.verbose(result)
 
         etcd_status = json.load(io.StringIO(result.lower()))
         parsed_etcd_status = {}
         for item in etcd_status:
             # get rid of https:// and :2379
             address = item['endpoint'].split('//')[1].split(':')[0]
-            node_name = cluster.nodes['all'].get_first_member(apply_filter={"internal_address": address}, provide_node_configs=True)['name']
+            node_name = cluster.nodes['all'].get_first_member(apply_filter={"internal_address": address}).get_node_name()
             parsed_etcd_status[node_name] = item
         cluster.context['backup_descriptor']['etcd']['status'] = parsed_etcd_status
     except Exception:
         cluster.log.verbose('Failed to load and parse ETCD status')
 
     if is_custom_etcd_node:
-        cluster.context['backup_descriptor']['etcd']['source'] = etcd_node.get_nodes_names()[0]
+        cluster.context['backup_descriptor']['etcd']['source'] = etcd_node.get_node_name()
     else:
         # if user did not provide node, then we have to select leader by ourselves
         if not etcd_status:
             raise Exception('Failed to load ETCD status and impossible to detect ETCD leader for making snapshot from it')
         etcd_leader_id = etcd_status[0]['status']['leader']
         etcd_leader_name = None
         for name, item in parsed_etcd_status.items():
@@ -187,42 +189,42 @@
             cluster.log.verbose('Detected ETCD leader: %s' % etcd_leader_name)
             cluster.context['backup_descriptor']['etcd']['source'] = etcd_leader_name
             etcd_node = cluster.nodes['control-plane'].get_member_by_name(etcd_leader_name)
         else:
             raise Exception('Failed to detect ETCD leader - not possible to create backup from actual DB')
 
     snap_name = 'snapshot%s.db' % int(round(time.time() * 1000))
-    endpoint_ip = etcd_node.get_ordered_members_list(provide_node_configs=True)[0]["internal_address"]
+    endpoint_ip = etcd_node.get_config()["internal_address"]
     cluster.log.debug('Creating ETCD backup "%s"...' % snap_name)
     result = etcd_node.sudo(f'etcdctl snapshot save /var/lib/etcd/{snap_name} --endpoints=https://{endpoint_ip}:2379 '
                             f'&& sudo mv /var/lib/etcd/{snap_name} /tmp/{snap_name} '
                             f'&& sudo ls -la /tmp/{snap_name} '
                             f'&& sudo du -hs /tmp/{snap_name} '
                             f'&& sudo chmod 666 /tmp/{snap_name}', timeout=600)
     cluster.log.debug(result)
     etcd_node.get('/tmp/' + snap_name, backup_directory + '/etcd.db')
     cluster.log.verbose('Deleting ETCD snapshot file from "%s"...')
     etcd_node.sudo('rm -f /tmp/%s' % snap_name)
 
 
-def select_etcd_node(cluster):
+def select_etcd_node(cluster: KubernetesCluster):
     custom_etcd_node = cluster.procedure_inventory.get('backup_plan', {}).get('etcd', {}).get('source_node')
 
     if custom_etcd_node:
-        etcd_node = cluster.nodes['all'].get_member_by_name(custom_etcd_node)
-        if etcd_node is None:
+        if not cluster.nodes['all'].has_node(custom_etcd_node):
             raise Exception('Unknown ETCD node selected as source')
+        etcd_node = cluster.nodes['all'].get_member_by_name(custom_etcd_node)
         return etcd_node, True
     else:
         return cluster.nodes['control-plane'].get_any_member(), False
 
 
-def retrieve_etcd_image(cluster, etcd_node):
+def retrieve_etcd_image(cluster: KubernetesCluster, etcd_node: NodeGroup):
     # TODO: Detect ETCD version via /etc/kubernetes/manifests/etcd.yaml config if presented, otherwise use containers
-    node_name = etcd_node.get_nodes_names()[0]
+    node_name = etcd_node.get_node_name()
     if "docker" == cluster.inventory['services']['cri']['containerRuntime']:
         cont_inspect = "docker inspect $(sudo docker ps -a | grep etcd-%s | awk '{print $1; exit}')" % node_name
         etcd_container_json = json.loads(list(etcd_node.sudo(cont_inspect).values())[0].stdout)[0]
         etcd_image_sha = etcd_container_json['Image'][7:]  # remove "sha256:" prefix
 
         images_result = etcd_node.sudo("docker image ls --format '{{json .}}'")
         formatted_images_result = "[" + ",".join(list(images_result.values())[0].stdout.strip().split('\n')) + "]"
@@ -248,20 +250,20 @@
     control_plane = cluster.nodes['control-plane'].get_any_member()
     version = control_plane.sudo('kubectl get nodes --no-headers | head -n 1 | awk \'{print $5; exit}\'').get_simple_out()
     cluster.context['backup_descriptor']['kubernetes']['version'] = version.strip()
 
 
 # There is no way to parallel resources connection via Queue or Pool:
 # the ssh connection is not possible to parallelize due to thread lock
-def download_resources(log, resources, location, control_plane: NodeGroup, namespace=None):
+def download_resources(log, resources: List[str], location, control_plane: NodeGroup, namespace=None):
 
     if namespace:
         log.debug('Downloading resources from namespace "%s"...' % namespace)
 
-    actual_resources = []
+    actual_resources: List[str] = []
 
     if not resources:
         log.debug('No resources found to download')
         return actual_resources
 
     cmd = ''
     resource_separator = ''.join(random.choice('=-_') for _ in range(32))
@@ -285,15 +287,15 @@
         if result and result != '':
             actual_resources.append(resource)
             utils.dump_file({}, result, resource_file_path, dump_location=False)
 
     return actual_resources
 
 
-def export_kubernetes(cluster):
+def export_kubernetes(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
     control_plane = cluster.nodes['control-plane'].get_any_member()
 
     cluster.log.debug('Loading namespaces:')
     namespaces_result = control_plane.sudo('kubectl get ns -o yaml')
     cluster.log.verbose(namespaces_result)
     namespaces_string = list(namespaces_result.values())[0].stdout.strip()
@@ -377,25 +379,25 @@
     if namespaced_resources_map:
         cluster.context['backup_descriptor']['kubernetes']['resources']['namespaced'] = namespaced_resources_map
 
     if nonnamespaced_resources_list:
         cluster.context['backup_descriptor']['kubernetes']['resources']['nonnamespaced'] = nonnamespaced_resources_list
 
 
-def make_descriptor(cluster):
+def make_descriptor(cluster: KubernetesCluster):
     backup_directory = prepare_backup_tmpdir(cluster)
 
     cluster.context['backup_descriptor']['kubernetes']['thirdparties'] = cluster.inventory['services']['thirdparties']
     cluster.context['backup_descriptor']['meta']['time']['finished'] = datetime.datetime.now()
 
     with utils.open_external(os.path.join(backup_directory, 'descriptor.yaml'), 'w') as output:
         output.write(yaml.dump(cluster.context['backup_descriptor']))
 
 
-def pack_data(cluster):
+def pack_data(cluster: KubernetesCluster):
     cluster_name = cluster.inventory['cluster_name']
     backup_directory = prepare_backup_tmpdir(cluster)
 
     backup_filename = 'backup-%s-%s.tar.gz' % (cluster_name, utils.get_current_timestamp_formatted())
 
     target = utils.get_external_resource_path(cluster.procedure_inventory.get('backup_location', backup_filename))
     if os.path.isdir(target):
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/cert_renew.py` & `kubemarine-0.19.0/kubemarine/procedures/cert_renew.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,62 +11,64 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
+from typing import List
 
 from kubemarine import plugins, k8s_certs
 from kubemarine.core import flow
 from kubemarine.core.action import Action
+from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 
 
-def renew_nginx_ingress_certs_task(cluster):
+def renew_nginx_ingress_certs_task(cluster: KubernetesCluster) -> None:
     # check that renewal is required for nginx
     if not cluster.procedure_inventory.get("nginx-ingress-controller"):
         cluster.log.debug("Skipped: nginx ingress controller certs renewal is not required")
         return
 
     cluster.log.debug("Starting certificate renewal for nginx ingress controller, plugin will be reinstalled")
     plugin = cluster.inventory["plugins"]["nginx-ingress-controller"]
     plugins.install_plugin(cluster, "nginx-ingress-controller", plugin["installation"]['procedures'])
 
 
-def k8s_certs_renew_task(cluster):
+def k8s_certs_renew_task(cluster: KubernetesCluster) -> None:
     if not cluster.procedure_inventory.get("kubernetes"):
         cluster.log.debug("Skipped: kubernetes certs renewal is not required")
         return
 
     cluster.log.debug("Starting certificate renewal for kubernetes")
     cluster.nodes['control-plane'].call(k8s_certs.renew_apply)
 
 
-def k8s_certs_overview_task(cluster):
+def k8s_certs_overview_task(cluster: KubernetesCluster) -> None:
     cluster.nodes['control-plane'].call(k8s_certs.k8s_certs_overview)
 
 
 tasks = OrderedDict({
     "kubernetes": k8s_certs_renew_task,
     "nginx_ingress_controller": renew_nginx_ingress_certs_task,
     "certs_overview": k8s_certs_overview_task
 })
 
 
 class CertRenewAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('cert renew', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     cli_help = '''
     Script for certificates renewal on existing Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/check_iaas.py` & `kubemarine-0.19.0/kubemarine/procedures/check_iaas.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,74 +18,74 @@
 import os
 import re
 import sys
 import uuid
 from collections import OrderedDict
 import time
 from contextlib import contextmanager
+from typing import List, Dict, Any, cast, Match, Iterator, Optional
 
-import fabric
 import yaml
 
 from kubemarine.core import flow, utils
 from kubemarine import system, packages
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.resources import DynamicResources
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
-from kubemarine.core.group import NodeGroupResult
+from kubemarine.core.group import NodeConfig, GroupException, GroupResultException, CollectorCallback
 
-def connection_ssh_connectivity(cluster):
+
+def connection_ssh_connectivity(cluster: KubernetesCluster):
     with TestCase(cluster, '001', 'SSH', 'Connectivity', default_results='Connected'):
         failed_nodes = []
-        for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
+        for node in cluster.nodes['all'].get_ordered_members_list():
             try:
-                cluster.log.verbose(node['connection'].run("echo 1"))
-            except fabric.group.GroupException as e:
-                failed_nodes.append(node['name'])
-                cluster.log.error("Connection test failed for node \"%s\"" % node['name'])
+                cluster.log.verbose(node.run("echo 1"))
+            except GroupException as e:
+                failed_nodes.append(node.get_node_name())
+                cluster.log.error("Connection test failed for node \"%s\"" % node.get_node_name())
                 cluster.log.error("Exception details:")
                 cluster.log.error(e)
         if failed_nodes:
             raise TestFailure("Failed to connect to %s nodes" % len(failed_nodes),
                               hint="Failed to connect from the deploy node to the remote node of the cluster. Check that "
                                    "the inventory details (key, username, and nodes addresses) are entered correctly, and verify "
                                    "the access to remote nodes.")
 
 
-def connection_ssh_latency_single(cluster):
+def connection_ssh_latency_single(cluster: KubernetesCluster):
     with TestCase(cluster, '002',  'SSH', 'Latency - Single Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 5:
             i += 1
-            for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
+            for node in cluster.nodes['all'].get_ordered_members_list():
                 time_start = time.time()
-                node['connection'].run("echo 1")
+                node.run("echo 1")
                 time_end = time.time()
                 diff = (time_end - time_start) * 1000
-                cluster.log.debug('Connection to %s - %sms' % (node['name'], diff))
+                cluster.log.debug('Connection to %s - %sms' % (node.get_node_name(), diff))
                 measurements.append(diff)
         average_latency = math.floor(sum(measurements) / cluster.nodes['all'].nodes_amount() / 5)
         if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical']:
             raise TestFailure("Very high latency: %sms" % average_latency,
                               hint="A very high latency was detected between the deploy node and cluster nodes. "
                                    "Check your network settings and status. It is necessary to reduce the latency to %sms."
                                    % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'])
         if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
-def connection_ssh_latency_multiple(cluster):
+def connection_ssh_latency_multiple(cluster: KubernetesCluster):
     with TestCase(cluster, '003',  'SSH', 'Latency - Multi Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 10:
             i += 1
@@ -104,30 +104,30 @@
         if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
-def connection_sudoer_access(cluster):
+def connection_sudoer_access(cluster: KubernetesCluster):
     with TestCase(cluster, '004', 'SSH', 'Sudoer Access', default_results='Access provided'):
         non_root = []
         for host, node_context in cluster.context['nodes'].items():
             access_info = node_context['access']
             if access_info['online'] and access_info['sudo'] == 'Root':
                 cluster.log.debug("%s online and has root" % host)
             else:
                 non_root.append(host)
         if non_root:
             raise TestFailure("Non-sudoer access found at: %s" % ", ".join(non_root),
                               hint="Certain nodes do not have the appropriate sudoer access. At these nodes, add "
                                    "a connection user to the sudoers group.")
 
 
-def hardware_members_amount(cluster, group_name):
+def hardware_members_amount(cluster: KubernetesCluster, group_name: str):
     beauty_name = group_name.capitalize()
     if group_name == 'vip':
         beauty_name = 'VIP'
     if group_name == 'all':
         beauty_name = 'Total Node'
 
     with TestCase(cluster, '005',  'Hardware', '%ss Amount' % beauty_name,
@@ -160,38 +160,38 @@
             raise TestWarn("Less than recommended. Detected %s item%s" % (amount, s),
                            hint="Increase the number of resources, so that the number of %ss in the cluster should not "
                                 "be less than %s." % (beauty_name, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount']))
 
         tc.success("%s item%s" % (amount, s))
 
 
-def hardware_cpu(cluster, group_name):
+def hardware_cpu(cluster: KubernetesCluster, group_name: str):
     minimal_cpu = cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'] \
-        if group_name == 'balancer' or cluster.nodes.get('all').nodes_amount() > 1 \
+        if group_name == 'balancer' or cluster.nodes['all'].nodes_amount() > 1 \
         else cluster.globals['compatibility_map']['hardware']['minimal']['control-plane']['vcpu']
     with TestCase(cluster, '006',  'Hardware', 'VCPUs Amount - %ss' % group_name.capitalize(),
                   minimal=minimal_cpu,
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
             return tc.success(results='Skipped')
         results = cluster.nodes[group_name].sudo("nproc --all")
         cluster.log.verbose(results)
-        minimal_amount = None
-        for connection, result in results.items():
+        minimal_amount: Optional[int] = None
+        for host, result in results.items():
             amount = int(result.stdout)
             if minimal_amount is None or minimal_amount > amount:
                 minimal_amount = amount
             if amount < minimal_cpu:
                 cluster.log.error('%s node %s has insufficient VCPUs: expected %s, but %s found.'
-                                  % (group_name.capitalize(), connection.host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'], amount))
+                                  % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'], amount))
             elif amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']:
                 cluster.log.warning('%s node %s has less VCPUs than recommended: recommended %s, but %s found.'
-                                    % (group_name.capitalize(), connection.host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'], amount))
+                                    % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'], amount))
             else:
-                cluster.log.debug('%s node %s has enough VCPUs: %s' % (group_name.capitalize(), connection.host, amount))
+                cluster.log.debug('%s node %s has enough VCPUs: %s' % (group_name.capitalize(), host, amount))
 
         s = ''
         if minimal_amount != 1:
             s = 's'
 
         if minimal_amount < minimal_cpu:
             raise TestFailure("Less than minimal. Detected %s VCPU%s" % (minimal_amount, s),
@@ -200,47 +200,47 @@
         if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']:
             raise TestWarn("Less than recommended. Detected %s VCPU%s" % (minimal_amount, s),
                            hint="Increase the number of VCPUs in the node configuration up to %s VCPUs."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'])
         tc.success(results='%s VCPU%s' % (minimal_amount, s))
 
 
-def hardware_ram(cluster, group_name):
+def hardware_ram(cluster: KubernetesCluster, group_name: str):
     with TestCase(cluster, '007',  'Hardware', 'RAM Amount - %ss' % group_name.capitalize(),
                   minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'],
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
             return tc.success(results='Skipped')
         results = cluster.nodes[group_name].sudo("cat /proc/meminfo | awk '/DirectMap/ { print $2 }'")
         cluster.log.verbose(results)
-        minimal_amount = None
-        for connection, result in results.items():
+        minimal_amount: Optional[int] = None
+        for host, result in results.items():
             amount = math.floor(sum(map(lambda x: int(x), result.stdout.strip().split("\n"))) / 1000000)
             if minimal_amount is None or minimal_amount > amount:
                 minimal_amount = amount
             if amount < cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram']:
                 cluster.log.error('%s node %s has insufficient RAM: expected %sGB, but %sGB found.'
-                                  % (group_name.capitalize(), connection.host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'], amount))
+                                  % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'], amount))
             elif amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']:
                 cluster.log.warning('%s node %s has less RAM than recommended: recommended %sGB, but %sGB found.'
-                                    % (group_name.capitalize(), connection.host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'], amount))
+                                    % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'], amount))
             else:
-                cluster.log.debug('%s node %s has enough RAM: %sGB' % (group_name.capitalize(), connection.host, amount))
+                cluster.log.debug('%s node %s has enough RAM: %sGB' % (group_name.capitalize(), host, amount))
         if minimal_amount < cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram']:
             raise TestFailure("Less than minimal. Detected %sGB" % minimal_amount,
                               hint="Increase the number of RAM in the node configuration to at least the minimum "
                                    "value: %sGB." % cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'])
         if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']:
             raise TestWarn("Less than recommended. Detected %sGB" % minimal_amount,
                            hint="Increase the number of RAM in the node configuration up to %s GB."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'])
         tc.success(results='%sGB' % minimal_amount)
 
 
-def system_distributive(cluster):
+def system_distributive(cluster: KubernetesCluster):
     with TestCase(cluster, '008', 'System', 'Distibutive') as tc:
         supported_distributives = cluster.globals['compatibility_map']['distributives'].keys()
 
         cluster.log.debug(system.fetch_os_versions(cluster))
 
         detected_unsupported_os = []
         detected_supported_os = []
@@ -284,33 +284,33 @@
                 f"Nodes have different OS families or versions. "
                 f"List of (OS family, version): {list(different_os)}")
             raise TestWarn(f"Nodes have different OS families or versions")
         
         tc.success(results=", ".join(detected_supported_os))
 
 
-def check_kernel_version(cluster):
+def check_kernel_version(cluster: KubernetesCluster):
     """
     This method compares the linux kernel version with the bad version
     """
     with TestCase(cluster, '015', "Software", "Kernel version") as tc:
         bad_results = {}
-        unstable_kernel_ubuntu = cluster.globals['compatibility_map']['distributives']['ubuntu'][0].get('unstable_kernel')
-        unstable_kernel_centos = []
+        unstable_kernel_ubuntu: List[str] = cluster.globals['compatibility_map']['distributives']['ubuntu'][0].get('unstable_kernel')
+        unstable_kernel_centos: List[str] = []
         group = cluster.nodes['all']
         result_group = group.run('uname -r')
-        for connection, results in result_group.items():
-            os_name = cluster.context['nodes'][connection.host]['os']['name']
+        for host, results in result_group.items():
+            os_name = cluster.context['nodes'][host]['os']['name']
             result = results.stdout.rstrip()
             if os_name == 'ubuntu':
                 if result in unstable_kernel_ubuntu:
-                    bad_results[connection.host] = result
+                    bad_results[host] = result
             elif os_name == 'centos':
                 if result in unstable_kernel_centos:
-                    bad_results[connection.host] = result
+                    bad_results[host] = result
 
         if len(bad_results) > 0:
             for host, kernel_version in bad_results.items():
                 cluster.log.debug(f"Unstable kernel %s on: %s" % (kernel_version, host))
             cluster.log.debug(f"Update the linux kernel version to 5.4.0-135-generic")
             raise TestWarn("Kernel version unstable")
         else:
@@ -331,24 +331,24 @@
 
         for destination, config in cluster.inventory['services'].get('thirdparties', {}).items():
             # Check if curl
             if config['source'][:4] != 'http' or '://' not in config['source'][4:8]:
                 continue
             # Check with script
             common_group = cluster.create_group_from_groups_nodes_names(config.get('groups', []), config.get('nodes', []))
-            for node in common_group.get_ordered_members_list(provide_node_configs=True):
-                if cluster.context['nodes'][node['connect_to']]['python'] == "Not installed":
-                    nodes_without_python.add(node["connect_to"])
+            for node in common_group.get_ordered_members_list():
+                host = node.get_host()
+                if cluster.context['nodes'][host]['python'] == "Not installed":
+                    nodes_without_python.add(host)
                     continue
-                python_executable = cluster.context['nodes'][node['connect_to']]['python']['executable']
-                res = node['connection'].run("%s %s %s %s" % (python_executable, random_temp_path, config['source'],
-                                                           cluster.inventory['globals']['timeout_download']), warn=True)
-                _, result = list(res.items())[0]
-                if result.failed:
-                    broken.append(f"{node['connect_to']}, {destination}: {result.stderr}")
+                python_executable = cluster.context['nodes'][host]['python']['executable']
+                res = node.run("%s %s %s %s" % (python_executable, random_temp_path, config['source'],
+                                                cluster.inventory['globals']['timeout_download']), warn=True)
+                if res.is_any_failed():
+                    broken.append(f"{host}, {destination}: {res[host].stderr}")
 
         # Remove file
         rm_command = "rm %s" % random_temp_path
         all_group.run(rm_command)
 
         if broken:
             raise TestFailure('Required thirdparties are unavailable', hint=yaml.safe_dump(broken))
@@ -369,21 +369,21 @@
     else:
         # Create temp resolv.conf file
         resolv_conf_buffer = system.get_resolv_conf_buffer(cluster.inventory["services"].get("resolv.conf"))
         random_resolv_conf_path = "/tmp/%s.conf" % uuid.uuid4().hex
         group.put(resolv_conf_buffer, random_resolv_conf_path)
 
         # Compare with existed resolv.conf
-        with RemoteExecutor(cluster) as exe:
-            group.run('[ -f /etc/resolv.conf ] && '
-                      'cmp --silent /etc/resolv.conf %s' % random_resolv_conf_path,
-                      warn=True)
+        results = group.run(
+            '[ -f /etc/resolv.conf ] && '
+            'cmp --silent /etc/resolv.conf %s' % random_resolv_conf_path,
+            warn=True)
 
-        for conn, res in exe.get_last_results().items():
-            nodes_context[conn.host]["resolv_conf_is_actual"] = not res[0].failed
+        for host, res in results.items():
+            nodes_context[host]["resolv_conf_is_actual"] = not res.failed
         # Remove temp resolv.conf file
         group.run("rm %s" % random_resolv_conf_path)
 
 
 def check_package_repositories(cluster: KubernetesCluster):
     nodes_context = cluster.context['nodes']
     hosts = [host for host, node_context in nodes_context.items() if 'package_repos_are_actual' not in node_context]
@@ -391,113 +391,115 @@
     repositories = cluster.inventory['services']['packages']['package_manager'].get("repositories")
     if repositories is None:
         for host in hosts:
             nodes_context[host]["package_repos_are_actual"] = True
     else:
         group = cluster.make_group(hosts)
         random_repos_conf_path = "/tmp/%s.repo" % uuid.uuid4().hex
-        with RemoteExecutor(cluster) as exe:
-            for node in group.get_ordered_members_list(provide_node_configs=True):
+        collector = CollectorCallback(cluster)
+        with group.new_executor() as exe:
+            for node in exe.group.get_ordered_members_list():
                 # Create temp repos file
-                packages.create_repo_file(node['connection'], repositories, random_repos_conf_path)
+                packages.create_repo_file(node, repositories, random_repos_conf_path)
 
                 # Compare with existed resolv.conf
-                predefined_repos_file = packages.get_repo_filename(node['connection'])
-                node['connection'].sudo('[ -f %s ] && cmp --silent %s %s' %
-                                        (predefined_repos_file, predefined_repos_file, random_repos_conf_path),
-                                        warn=True, hide=False)
+                predefined_repos_file = packages.get_repo_filename(node)
+                node.sudo(
+                    '[ -f %s ] && cmp --silent %s %s' %
+                    (predefined_repos_file, predefined_repos_file, random_repos_conf_path),
+                    warn=True, callback=collector)
 
-        for conn, results in exe.get_last_results().items():
-            nodes_context[conn.host]["package_repos_are_actual"] = not list(results.values())[-1].failed
+        for host, result in collector.result.items():
+            nodes_context[host]["package_repos_are_actual"] = not result.failed
 
         # Remove temp .repo file
         group.sudo("rm %s" % random_repos_conf_path)
 
 
 def check_access_to_package_repositories(cluster: KubernetesCluster):
     with TestCase(cluster, '013', 'Software', 'Package Repositories') as tc:
         detect_preinstalled_python(cluster)
         check_resolv_conf(cluster)
         broken = []
         warnings = []
 
         # Collect repository urls
         # TODO: think about better parsing
-        repository_urls = set()
+        repository_urls: List[str] = []
         repositories = cluster.inventory['services']['packages']['package_manager'].get("repositories")
         if cluster.get_os_family() not in ['debian', 'rhel', 'rhel8']:
             # Skip check in case of multiply or unknown OS
             raise TestWarn("Can't check package repositories on multiply OS")
         if isinstance(repositories, list):
             # For debian
             for repo in repositories:
-                repository_url = next(filter(lambda x: x[:4] == 'http' and '://' in x[4:8], repo.split(' ')), None)
-                if repository_url is not None:
-                    repository_urls.add(repository_url)
+                repository_url = list(filter(lambda x: x[:4] == 'http' and '://' in x[4:8], repo.split(' ')))
+                if repository_url:
+                    repository_urls.append(repository_url[0])
                 else:
                     broken.append(f"Found broken repository: '{repo}'")
         elif isinstance(repositories, dict):
             # For rhel
             for repo_name, repo_conf in repositories.items():
                 if repo_conf.get('baseurl') is not None:
-                    repository_urls.add(repo_conf.get('baseurl'))
+                    repository_urls.append(repo_conf.get('baseurl'))
                 else:
                     broken.append(f"Found broken repository: '{repo_name}'")
         elif isinstance(repositories, str):
             path = utils.get_external_resource_path(repositories)
             if not os.path.isfile(path):
                 broken.append(f"File {path} with the repositories content does not exist")
             else:
                 repositories = utils.read_external(path)
                 for repo in repositories.split('\n'):
-                    repository_url = next(filter(lambda x: x[:4] == 'http' and '://' in x[4:8], repo.split(' ')), None)
-                    if repository_url is not None:
-                        repository_urls.add(repository_url)
+                    repository_url = list(filter(lambda x: x[:4] == 'http' and '://' in x[4:8], repo.split(' ')))
+                    if repository_url:
+                        repository_urls.append(repository_url[0])
                 if not repository_urls:
                     broken.append(f"Failed to detect repository URLs in file {path}")
 
-        repository_urls = list(repository_urls)
+        repository_urls = list(set(repository_urls))
         cluster.log.debug(f"Repositories to check: {repository_urls}")
 
         # Load script for checking sources
         all_group = cluster.nodes['all']
         check_script = utils.read_internal("resources/scripts/check_url_availability.py")
         random_temp_path = "/tmp/%s.py" % uuid.uuid4().hex
         all_group.put(io.StringIO(check_script), random_temp_path)
 
         if repository_urls:
-            with RemoteExecutor(cluster) as exe:
-                for node in all_group.get_ordered_members_list(provide_node_configs=True):
+            collector = CollectorCallback(cluster)
+            with all_group.new_executor() as exe:
+                for node in exe.group.get_ordered_members_list():
+                    host = node.get_host()
                     # Check with script
-                    if cluster.context['nodes'][node['connect_to']]['python'] == 'Not installed':
-                        warnings.append(f"Can't detect python version for node {node['connect_to']}, "
+                    if cluster.context['nodes'][host]['python'] == 'Not installed':
+                        warnings.append(f"Can't detect python version for node {host}, "
                                         f"operation can't be performed for it")
                         continue
-                    python_executable = cluster.context['nodes'][node['connect_to']]['python']['executable']
-                    for repository_url in repository_urls:
-                        node['connection'].run('%s %s %s %s || echo "Package repository is unavailable"'
-                                               % (python_executable, random_temp_path, repository_url,
-                                                  cluster.inventory['globals']['timeout_download']))
-
-            results = exe.get_last_results()
-            if results is None:
-                results = NodeGroupResult(cluster)
-            for conn, url_results in results.items():
+                    python_executable = cluster.context['nodes'][host]['python']['executable']
+                    for repo_url in repository_urls:
+                        node.run('%s %s %s %s'
+                                 % (python_executable, random_temp_path, repo_url,
+                                    cluster.inventory['globals']['timeout_download']),
+                                 warn=True, callback=collector)
+
+            for host, url_results in collector.results.items():
                 # Check if resolv.conf is actual
-                resolv_conf_actual = cluster.context['nodes'][conn.host]['resolv_conf_is_actual']
+                resolv_conf_actual = cluster.context['nodes'][host]['resolv_conf_is_actual']
                 if not resolv_conf_actual:
-                    warnings.append(f"resolv.conf is not installed for node {conn.host}: "
+                    warnings.append(f"resolv.conf is not installed for node {host}: "
                                     f"Package repositories can be unavailable. You can install resolv.conf using task "
                                     f"`install --tasks prepare.dns.resolv_conf`")
                     problem_handler = warnings
                 else:
                     problem_handler = broken
-                for i, result in enumerate(url_results.values()):
-                    if "Package repository is unavailable" in result.stdout:
-                        problem_handler.append(f"{conn.host}, {repository_urls[i]}: {result.stderr}")
+                for i, result in enumerate(url_results):
+                    if result.failed:
+                        problem_handler.append(f"{host}, {repository_urls[i]}: {result.stderr}")
 
         # Remove file
         rm_command = "rm %s" % random_temp_path
         all_group.run(rm_command)
 
         if broken:
             raise TestFailure('Found problems for package repositories', hint=yaml.safe_dump(broken))
@@ -505,42 +507,43 @@
             raise TestWarn('Found potential problems for package repositories or nodes', hint=yaml.safe_dump(warnings))
         tc.success('All package repositories are correct and available')
 
 
 def check_access_to_packages(cluster: KubernetesCluster):
     with TestCase(cluster, '014', 'Software', 'Package Availability') as tc:
         check_package_repositories(cluster)
-        broken = []
-        warnings = []
+        broken: List[str] = []
+        warnings: List[str] = []
         group = cluster.nodes['all']
         hosts_to_packages = packages.get_all_managed_packages_for_group(group, cluster.inventory)
-        with RemoteExecutor(cluster) as exe:
-            for host, packages_to_check in hosts_to_packages.items():
-                packages_to_check = list(set(packages_to_check))
+        collector = CollectorCallback(cluster)
+        with group.new_executor() as exe:
+            for node in exe.group.get_ordered_members_list():
+                host = node.get_host()
+                packages_to_check = list(set(hosts_to_packages[host]))
                 hosts_to_packages[host] = packages_to_check
                 cluster.log.debug(f"Packages to check for node {host}: {packages_to_check}")
 
-                node = cluster.make_group([host])
                 for package in packages_to_check:
-                    packages.search_package(node, package)
+                    packages.search_package(node, package, callback=collector)
 
         # Check packages from install section
-        for conn, results in exe.get_last_results().items():
-            package_repos_are_actual = cluster.context['nodes'][conn.host]["package_repos_are_actual"]
+        for host, results in collector.results.items():
+            package_repos_are_actual = cluster.context['nodes'][host]["package_repos_are_actual"]
             if not package_repos_are_actual:
-                warnings.append(f"Package repositories are not installed for {conn.host}: "
+                warnings.append(f"Package repositories are not installed for {host}: "
                                 f"Packages can be unavailable. You can install it using tasks "
                                 f"`install --tasks prepare.dns.resolv_conf,prepare.package_manager.configure`")
                 problem_handler = warnings
             else:
                 problem_handler = broken
-            packages_to_check = hosts_to_packages[conn.host]
-            for i, result in enumerate(results.values()):
-                if "Package is unavailable" in result.stdout:
-                    problem_handler.append(f"Package {packages_to_check[i]} is unavailable for node {conn.host}")
+            packages_to_check = hosts_to_packages[host]
+            for i, result in enumerate(results):
+                if result.failed:
+                    problem_handler.append(f"Package {packages_to_check[i]} is unavailable for node {host}")
 
         if broken:
             raise TestFailure('Required packages are unavailable', hint=yaml.safe_dump(broken))
         elif warnings:
             raise TestWarn('Found potential problems for packages', hint=yaml.safe_dump(warnings))
         tc.success('All packages are available')
 
@@ -554,129 +557,130 @@
     group_unknown_python = cluster.make_group(hosts_unknown_python)
     detected_python = group_unknown_python.run(
         rf'for i in $(whereis -b python && whereis -b python3 ); do '
         rf'if [[ -f "$i" ]] && [[ $($i --version 2>&1 | head -n 1) =~ {bash_version_pattern} ]]; then '
         rf'echo "$i"; $i --version 2>&1; break; '
         rf'fi; done')
 
-    for conn, result in detected_python.items():
-        result = result.stdout.strip()
-        if not result:
-            nodes_context[conn.host]["python"] = "Not installed"
+    for host, result in detected_python.items():
+        identity = result.stdout.strip()
+        if not identity:
+            nodes_context[host]["python"] = "Not installed"
         else:
-            executable, version = tuple(result.splitlines())
-            version = re.match(python_version_pattern, version).group(1)
-            nodes_context[conn.host]["python"] = {
+            executable, version = tuple(identity.splitlines())
+            version = cast(Match[str], re.match(python_version_pattern, version)).group(1)
+            nodes_context[host]["python"] = {
                 "executable": executable,
                 "major_version": version
             }
 
 
 @contextmanager
 def suspend_firewalld(cluster: KubernetesCluster):
     firewalld_statuses = system.fetch_firewalld_status(cluster.nodes["all"])
     stop_firewalld_group = firewalld_statuses.get_nodes_group_where_value_in_stdout("active (running)")
 
     nodes_to_rollback = cluster.make_group([])
     try:
         try:
             nodes_to_rollback = system.stop_service(stop_firewalld_group, "firewalld").get_group()
-        except fabric.group.GroupException as e:
-            nodes_to_rollback = e.result.get_exited_nodes_group()
+        except GroupException as e:
+            nodes_to_rollback = e.get_exited_nodes_group()
             raise
 
         yield
     finally:
         system.start_service(nodes_to_rollback, "firewalld")
 
 
-def _get_not_balancers(cluster: KubernetesCluster) -> dict:
+def _get_not_balancers(cluster: KubernetesCluster) -> Dict[str, NodeConfig]:
     nodes = {}
-    for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
+    for node in cluster.inventory['nodes']:
         # exclude nodes which are only balancers.
         if node["roles"] == ["balancer"]:
             cluster.log.debug(f"Exclude balancer '{node['name']}' from subnet connectivity check.")
             continue
         nodes[node["connect_to"]] = node
 
     return nodes
 
 
 @contextmanager
-def assign_random_ips(cluster: KubernetesCluster, nodes: dict, subnet):
+def assign_random_ips(cluster: KubernetesCluster, nodes: Dict[str, NodeConfig], subnet) -> Iterator[Dict[str, Any]]:
     inet = ipaddress.ip_network(subnet)
     net_mask = str(inet.netmask)
     prefix = str(inet.prefixlen)
     subnet_hosts = []
-    ip_numbers=0
-    for i in inet.hosts():
-        subnet_hosts.append(i)
-        ip_numbers +=1
+    ip_numbers = 0
+    for addr in inet.hosts():
+        subnet_hosts.append(addr)
+        ip_numbers += 1
         if ip_numbers == 1000000:
            break
     subnet_hosts_len = len(subnet_hosts)
 
     host_to_inf = {}
     host_to_ip = {}
     skipped_nodes = []
     nodes_to_rollback = cluster.make_group([])
 
     try:
         # Assign random IP for the subnet on every node
         i = 30
-        for host, node in nodes.items():
+        for host, node_config in nodes.items():
             inf = cluster.context['nodes'][host]['active_interface']
             if not inf:
-                raise TestFailure(f"Failed to detect active interface on {node['name']}")
+                raise TestFailure(f"Failed to detect active interface on {node_config['name']}")
             host_to_inf[host] = inf
             random_host = subnet_hosts[subnet_hosts_len - i]
             host_to_ip[host] = random_host
             i = i + 1
 
-        with RemoteExecutor(cluster) as exe:
-            for host, node in nodes.items():
+        collector = CollectorCallback(cluster)
+        with cluster.make_group(nodes).new_executor() as exe:
+            for node in exe.group.get_ordered_members_list():
+                host = node.get_host()
                 existing_alias = f"ip -o a | grep {host_to_inf[host]} | grep {host_to_ip[host]}"
-                node['connection'].sudo(existing_alias, warn=True)
+                node.sudo(existing_alias, warn=True, callback=collector)
 
-            exe.flush()
-            for cxn, result in exe.get_merged_result().items():
-                host = cxn.host
-                if not result.stdout and not result.stderr and result.exited == 1:
-                    # grep returned nothing, subnet is not used.
-                    pass
-                else:
-                    skipped_nodes.append(nodes[host]["name"])
-                    del nodes[host]
-
-            # Create alias from the node network interface for the subnet on every node
-            for host, node in nodes.items():
-                node['connection'].sudo(f"ip a add {host_to_ip[host]}/{prefix} dev {host_to_inf[host]}")
+        for host, result in collector.result.items():
+            if not result.stdout and not result.stderr and result.exited == 1:
+                # grep returned nothing, subnet is not used.
+                pass
+            else:
+                skipped_nodes.append(nodes[host]["name"])
+                del nodes[host]
 
-            exe.flush()
-            try:
-                nodes_to_rollback = exe.get_merged_result().get_group()
-            except fabric.group.GroupException as e:
-                nodes_to_rollback = e.result.get_exited_nodes_group()
-                raise
+        try:
+            with cluster.make_group(nodes).new_executor() as exe:
+                # Create alias from the node network interface for the subnet on every node
+                for node in exe.group.get_ordered_members_list():
+                    host = node.get_host()
+                    node.sudo(f"ip a add {host_to_ip[host]}/{prefix} dev {host_to_inf[host]}")
+
+            nodes_to_rollback = cluster.make_group(nodes.keys())
+        except GroupException as e:
+            nodes_to_rollback = e.get_exited_nodes_group()
+            raise
 
         yield host_to_ip
     finally:
         # Remove the created aliases from network interfaces
-        with RemoteExecutor(cluster):
-            for node in nodes_to_rollback.get_ordered_members_list(provide_node_configs=True):
-                host = node["connect_to"]
-                node['connection'].sudo(f"ip a del {host_to_ip[host]}/{prefix} dev {host_to_inf[host]}",
-                                        warn=True)
+        with nodes_to_rollback.new_executor() as exe:
+            for node in exe.group.get_ordered_members_list():
+                host = node.get_host()
+                node.sudo(f"ip a del {host_to_ip[host]}/{prefix} dev {host_to_inf[host]}",
+                          warn=True)
 
     if skipped_nodes:
         raise TestWarn(f"Cannot perform check on {skipped_nodes}: subnet is already in use. "
                        f"Use check_paas procedure if you already have installed cluster.")
 
 
-def pod_subnet_connectivity(cluster):
+def pod_subnet_connectivity(cluster: KubernetesCluster):
     with TestCase(cluster, '009', 'Network', 'PodSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         pod_subnet = cluster.inventory['services']['kubeadm']['networking']['podSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, pod_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
@@ -684,15 +688,15 @@
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Traffic is not allowed for the pod subnet({pod_subnet}) "
                                        f"on nodes: {failed_nodes}.")
 
 
-def service_subnet_connectivity(cluster):
+def service_subnet_connectivity(cluster: KubernetesCluster):
     with TestCase(cluster, '010', 'Network', 'ServiceSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         service_subnet = cluster.inventory['services']['kubeadm']['networking']['serviceSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, service_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
@@ -707,20 +711,22 @@
 def cmd_for_ports(ports, query):
     result = ""
     for port in ports:
         result += f" && echo 'port: {port}' && ( {query % port} ) "
     return result[3:]
 
 
-def tcp_connect(cluster, node_from, node_to, tcp_ports, host_to_ip, mtu):
+def tcp_connect(cluster: KubernetesCluster, node_from: NodeConfig, node_to: NodeConfig,
+                tcp_ports: List[str], host_to_ip: Dict[str, Any], mtu):
     # 40 bites for headers
     mtu -= 40
     cluster.log.verbose(f"Trying connection from '{node_from['name']}' to '{node_to['name']}")
     cmd = cmd_for_ports(tcp_ports, f"echo $(dd if=/dev/urandom bs={mtu}  count=1) >/dev/tcp/{host_to_ip[node_to['connect_to']]}/%s")
-    node_from['connection'].sudo(cmd, timeout=cluster.globals['connection']['defaults']['timeout'])
+    group = cluster.make_group([node_from['connect_to']])
+    group.sudo(cmd, timeout=cluster.globals['connection']['defaults']['timeout'])
 
 
 def get_start_tcp_listener_cmd(python_executable, tcp_listener, ip_version):
     # 1. Create anonymous pipe
     # 2. Create python tcp listener process in background and redirect output to pipe
     # 3. Wait till the listener successfully binds the port, or till it fails and exits.
     #    Read one line from pipe to check that.
@@ -745,15 +751,16 @@
 
 def get_stop_tcp_listener_cmd(tcp_listener):
     identify_pid = "ps aux | grep \" %s ${port} \" | grep -v grep | grep -v nohup | awk '{print $2}'" % tcp_listener
     return f"port=%s;pid=$({identify_pid}) " \
            "&& if [ ! -z $pid ]; then sudo kill -9 $pid; echo \"killed pid $pid for port $port\"; fi"
 
 
-def check_tcp_connect_between_all_nodes(cluster, node_list, tcp_ports, host_to_ip):
+def check_tcp_connect_between_all_nodes(cluster: KubernetesCluster, node_list: List[NodeConfig],
+                                        tcp_ports: List[str], host_to_ip: Dict[str, Any]):
     if len(node_list) <= 1:
         return []
 
     mtu = cluster.inventory['plugins']['calico']['mtu']
 
     cluster.log.verbose("Searching for success node...")
     success_node = None
@@ -791,86 +798,82 @@
                 cluster.log.error(f"Subnet connectivity test failed from '{success_node['name']}' to '{node['name']}'")
                 cluster.log.verbose(f"Exception details: {e}")
 
     return failed_nodes
 
 
 @contextmanager
-def install_tcp_listener(cluster: KubernetesCluster, nodes: dict, tcp_ports):
+def install_tcp_listener(cluster: KubernetesCluster, nodes: Dict[str, NodeConfig], tcp_ports):
     detect_preinstalled_python(cluster)
-    nodes_without_python = {node['name']: node for host, node in nodes.items()
+    nodes_without_python = {node_config['name']: node_config for host, node_config in nodes.items()
                             if cluster.context['nodes'][host]['python'] == "Not installed"}
-    for node in nodes_without_python.values():
-        del nodes[node['connect_to']]
+    for node_nonfig in nodes_without_python.values():
+        del nodes[node_nonfig['connect_to']]
 
     # currently tcp listener can be run on both python 2 and 3
     check_script = utils.read_internal('resources/scripts/simple_tcp_listener.py')
     tcp_listener = "/tmp/%s.py" % uuid.uuid4().hex
-    cluster.make_group(list(nodes.keys())).put(io.StringIO(check_script), tcp_listener)
+    cluster.make_group(nodes.keys()).put(io.StringIO(check_script), tcp_listener)
 
     skipped_nodes = {}
     nodes_to_rollback = cluster.make_group([])
     try:
-        with RemoteExecutor(cluster) as exe:
-            # Run process that LISTEN TCP port
-            for host, node in nodes.items():
-                internal_ip = node.get('internal_address')
-                ip_version = ipaddress.ip_address(internal_ip).version 
-                python_executable = cluster.context['nodes'][host]['python']['executable']
-                tcp_listener_cmd = cmd_for_ports(tcp_ports, get_start_tcp_listener_cmd(python_executable, tcp_listener, ip_version))
-                node['connection'].sudo(tcp_listener_cmd, warn=True)
+        collector = CollectorCallback(cluster)
+        try:
+            nodes_to_rollback = group = cluster.make_group(nodes)
+            with group.new_executor() as exe:
+                # Run process that LISTEN TCP port
+                for node in exe.group.get_ordered_members_list():
+                    host = node.get_host()
+                    internal_ip: str = nodes[host]['internal_address']
+                    ip_version = ipaddress.ip_address(internal_ip).version
+                    python_executable = cluster.context['nodes'][host]['python']['executable']
+                    tcp_listener_cmd = cmd_for_ports(tcp_ports, get_start_tcp_listener_cmd(python_executable, tcp_listener, ip_version))
+                    node.sudo(tcp_listener_cmd, warn=True, callback=collector)
+        except GroupException as e:
+            nodes_to_rollback = e.get_exited_nodes_group()
+            raise
 
-            exe.flush()
-            try:
-                results = exe.get_merged_result()
-                if results is None:
-                    results = NodeGroupResult(cluster)
-                nodes_to_rollback = results.get_group()
-            except fabric.group.GroupException as e:
-                nodes_to_rollback = e.result.get_exited_nodes_group()
-                raise
-
-            port_in_use = re.compile(r'^(\d+) in use$')
-            for cxn, result in results.items():
-                host = cxn.host
-                matcher = port_in_use.match(result.stderr.strip())
-                if matcher is not None:
-                    skipped_nodes[nodes[host]["name"]] = matcher.group(1)
-                    del nodes[host]
-                elif result.exited != 0:
-                    raise fabric.group.GroupException(results)
-                else:
-                    cluster.log.verbose(result)
+        port_in_use = re.compile(r'^(\d+) in use$')
+        for host, result in collector.result.items():
+            matcher = port_in_use.match(result.stderr.strip())
+            if matcher is not None:
+                skipped_nodes[nodes[host]["name"]] = matcher.group(1)
+                del nodes[host]
+            elif result.exited != 0:
+                raise GroupResultException(collector.result)
+            else:
+                cluster.log.verbose(result)
 
         yield
 
     finally:
-        with RemoteExecutor(cluster):
+        with nodes_to_rollback.new_executor() as exe:
             # Kill the created during the test processes
-            for node in nodes_to_rollback.get_ordered_members_list(provide_node_configs=True):
+            for node in exe.group.get_ordered_members_list():
                 tcp_listener_cmd = cmd_for_ports(tcp_ports, get_stop_tcp_listener_cmd(tcp_listener))
-                node['connection'].sudo(tcp_listener_cmd, warn=True)
+                node.sudo(tcp_listener_cmd, warn=True)
 
     if skipped_nodes:
         cluster.log.warning(f"Ports in use: {skipped_nodes}")
         raise TestWarn(f"Cannot perform check on {list(skipped_nodes.keys())}: some ports are already in use. "
                        f"Use check_paas procedure if you already have installed cluster.")
 
     if nodes_without_python:
         cluster.log.warning(f"Nodes without python: {nodes_without_python.keys()}")
         raise TestWarn(f"Cannot perform check on {list(nodes_without_python.keys())}: python doesn't exist.")
 
 
-def check_tcp_ports(cluster):
+def check_tcp_ports(cluster: KubernetesCluster):
     with TestCase(cluster, '011', 'Network', 'TCPPorts', default_results='Connected'),\
             suspend_firewalld(cluster):
         tcp_ports = ["80", "443", "179", "5473", "6443", "8443", "2379", "2380", "9091", "9094", "10250", "10254",
                      "10257", "10259", "30001", "30002"]
         nodes = {node["connect_to"]: node
-                 for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True)}
+                 for node in cluster.inventory['nodes']}
         host_to_ip = {host: node['internal_address'] for host, node in nodes.items()}
         with install_tcp_listener(cluster, nodes, tcp_ports):
             failed_nodes = check_tcp_connect_between_all_nodes(cluster, list(nodes.values()), tcp_ports, host_to_ip)
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Not all needed tcp ports are opened on nodes: {failed_nodes}. "
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/check_paas.py` & `kubemarine-0.19.0/kubemarine/procedures/check_paas.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,82 +13,83 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import sys
 import time
 from collections import OrderedDict
 import re
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 import yaml
 import ruamel.yaml
 import ipaddress
 import uuid
 
 from kubemarine import packages as pckgs, system, selinux, etcd, thirdparties, apparmor, kubernetes
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import NodeConfig, NodeGroup
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import check_iaas
 from kubemarine.core import flow, static
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.coredns import generate_configmap
-from deepdiff import DeepDiff
+from deepdiff import DeepDiff  # type: ignore[import]
 
 
 def services_status(cluster: KubernetesCluster, service_type: str):
     with TestCase(cluster, '201', "Services", "%s Status" % service_type.capitalize(),
                   default_results='active (running)'):
         service_name = service_type
 
         if cluster.get_os_family() != 'multiple' and service_type != 'kubelet':
             service_name = cluster.get_package_association(service_type, 'service_name')
 
         group = cluster.nodes['all']
         if service_type == 'haproxy':
-            group = cluster.nodes.get('balancer', {})
+            group = cluster.make_group_from_roles(['balancer'])
         elif service_type == 'keepalived':
-            group = cluster.nodes.get('keepalived', {})
+            group = cluster.make_group_from_roles(['keepalived'])
         elif service_type == 'docker' or service_type == "containerd" or service_type == 'kubelet':
-            group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker'))
+            group = cluster.make_group_from_roles(['control-plane', 'worker'])
 
-        if not group or group.is_empty():
+        if group.is_empty():
             raise TestWarn("No nodes to check service status",
                            hint="The node group to check the service is empty. Check skipped.")
 
         result = group.sudo('systemctl status %s' % service_name, warn=True)
         cluster.log.verbose(result)
 
         status_regexp = re.compile("Active:\s([a-z\s()]*)(\ssince|$)", re.M)
 
         statuses = []
         failed = False
-        for connection, node_result in result.items():
+        for host, node_result in result.items():
             if node_result.return_code == 4:
                 statuses.append('service is missing')
                 failed = True
                 cluster.log.debug('%s is not presented on host %s, skipped'
-                                  % (service_type.capitalize(), connection.host))
+                                  % (service_type.capitalize(), host))
                 continue
             matches = re.findall(status_regexp, node_result.stdout)
             if matches:
                 status = matches[0][0].strip()
                 cluster.log.debug(
-                    '%s status is \"%s\" at host %s' % (service_type.capitalize(), status, connection.host))
+                    '%s status is \"%s\" at host %s' % (service_type.capitalize(), status, host))
                 if status != 'active (running)':
                     statuses.append(status)
                     failed = True
             elif node_result.return_code != 0:
                 failed = True
                 cluster.log.error('%s status has bad exit code \"%s\" at host %s'
-                                  % (service_type.capitalize(), node_result.return_code, connection.host))
+                                  % (service_type.capitalize(), node_result.return_code, host))
             else:
-                raise Exception('Failed to detect status for \"%s\"' % connection.host)
+                raise Exception('Failed to detect status for \"%s\"' % host)
 
         statuses = list(set(statuses))
 
         if failed:
             raise TestFailure("Bad status detected: %s" % ', '.join(statuses),
                               hint="Fix the service to be enabled and has running status.")
 
@@ -169,15 +170,15 @@
     """
     Verifies that mandatory packages are installed on required nodes and have equal versions.
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     """
     with TestCase(cluster, '205', "Services", "Mandatory package versions") as tc:
         _check_same_os(cluster)
-        hosts_to_packages = {}
+        hosts_to_packages: Dict[str, List[str]] = {}
         group = cluster.nodes['all']
         for package in cluster.inventory["services"]["packages"]['mandatory'].keys():
             packages = pckgs.get_association_hosts_to_packages(group, cluster.inventory, package)
 
             for host, packages_list in packages.items():
                 hosts_to_packages.setdefault(host, []).extend(packages_list)
 
@@ -195,15 +196,15 @@
     with TestCase(cluster, '206', "Services", f"Generic packages version") as tc:
         _check_same_os(cluster)
         packages = cluster.inventory['services']['packages'].get('install', {}).get('include', [])
         hosts_to_packages = {host: packages for host in cluster.nodes['all'].get_hosts()}
         return check_packages_versions(cluster, tc, hosts_to_packages, warn_on_bad_result=True)
 
 
-def check_packages_versions(cluster, tc, hosts_to_packages: Dict[str, List[str]],
+def check_packages_versions(cluster: KubernetesCluster, tc: TestCase, hosts_to_packages: Dict[str, List[str]],
                             warn_on_bad_result=False, raise_successful=True):
     """
     Verifies that all packages are installed on required nodes and have equal versions
     :param cluster: main cluster object
     :param tc: current test case object
     :param hosts_to_packages: hosts where to check packages
     :param warn_on_bad_result: if true then uses Warning instead of Failure. Default False.
@@ -237,19 +238,19 @@
             raise TestWarn("detected incorrect packages versions", hint=hint_message)
         raise TestFailure("detected incorrect packages versions", hint=hint_message)
     cluster.log.debug(f"installed packages: {good_results}")
     if raise_successful:
         tc.success("all packages have correct versions")
 
 
-def get_nodes_description(cluster):
+def get_nodes_description(cluster: KubernetesCluster):
     return kubernetes.get_nodes_description(cluster)
 
 
-def kubelet_version(cluster):
+def kubelet_version(cluster: KubernetesCluster):
     with TestCase(cluster, '203', "Services", "Kubelet Version",
                   default_results=cluster.inventory['services']['kubeadm']['kubernetesVersion']):
         nodes_description = get_nodes_description(cluster)
         bad_versions = []
         for node_description in nodes_description['items']:
             node_name = node_description['metadata']['name']
             kubelet_version = node_description['status']['nodeInfo']['kubeletVersion']
@@ -260,28 +261,29 @@
         if bad_versions:
             raise TestFailure("Invalid version detected: %s" % ', '.join(bad_versions),
                               hint="All nodes must have the same correct Kubelet version \"%s\". Remove nodes with the "
                                    "incorrect version from the cluster and reinstall them to the corresponding "
                                    "versions." % cluster.inventory['services']['kubeadm']['kubernetesVersion'])
 
 
-def thirdparties_hashes(cluster):
+def thirdparties_hashes(cluster: KubernetesCluster):
     """
     Task which is used to verify configured thirdparties hashes agains actual hashes on nodes.
     If thirdparty is an archive, then archive files hashes are also verified.
     If hash is not specified, then thirdparty is skipped.
     If there is no thirdparties with hashes, then warning is shown.
     """
     with TestCase(cluster, '212', "Thirdparties", "Hashes") as tc:
         successful = []
         warnings = []
         broken = []
 
         #Create tmp dir for loading thirdparty without default sha
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
+        first_control_plane_host = first_control_plane.get_host()
 
         for path, config in cluster.inventory['services']['thirdparties'].items():
             group = cluster.create_group_from_groups_nodes_names(config.get('groups', []), config.get('nodes', []))
             hosts_missing = find_hosts_missing_thirdparty(group, path)
             if hosts_missing:
                 broken.append(f"thirdparty {path} is missing on {hosts_missing}")
                 # if thirdparty is missing somewhere, do not check anything further for it
@@ -297,33 +299,35 @@
                 random_dir = "/tmp/%s" % uuid.uuid4().hex
                 final_commands = "rm -r -f %s" % random_dir
                 random_path = "%s%s" % (random_dir, path)
                 cluster.log.verbose('Temporary path: %s' % random_path)
                 remote_commands = "mkdir -p %s" % ('/'.join(random_path.split('/')[:-1]))
                 # Load thirdparty to temporary dir
                 remote_commands += "&& sudo curl -f -g -s --show-error -L %s -o %s" % (config['source'], random_path)
-                results = first_control_plane.sudo(remote_commands, hide=True, warn=True)
-                host, result = list(results.items())[0]
-                if result.failed:
-                    broken.append(f"Can`t download thirdparty {path} on {host.host} for getting sha: {result.stderr}")
-                    cluster.log.verbose(f"Can`t download thirdparty {path} on {host.host} for getting sha: {result.stderr}")
+                results = first_control_plane.sudo(remote_commands, warn=True)
+                if results.is_any_failed():
+                    host = first_control_plane_host
+                    msg = f"Can`t download thirdparty {path} on {host} for getting sha: {results[host].stderr}"
+                    broken.append(msg)
+                    cluster.log.verbose(msg)
                 else:
                     # Get temporary thirdparty sha
                     cluster.log.verbose(f"Get temporary thirdparty sha for {path}...")
                     results = first_control_plane.sudo(f'openssl sha1 {random_path} | sed "s/^.* //"', warn=True)
-                    host, result = list(results.items())[0]
-                    if result.failed:
-                        broken.append(f'failed to get sha for temporary file {random_path} on {host.host}: {result.stderr}')
-                        cluster.log.verbose(f'failed to get sha for temporary file {random_path} on {host.host}: {result.stderr}')
+                    if results.is_any_failed():
+                        host = first_control_plane_host
+                        msg = f'failed to get sha for temporary file {random_path} on {host}: {results[host].stderr}'
+                        broken.append(msg)
+                        cluster.log.verbose(msg)
                     else:
-                        expected_sha = result.stdout.strip()
+                        expected_sha = results.get_simple_out().strip()
                         cluster.log.verbose(f"Expected sha was got for {path}: {expected_sha}")
                 # Remove temporary dir in any case
                 cluster.log.verbose(f"Remove temporary dir {random_dir}...")
-                first_control_plane.sudo(final_commands, hide=True, warn=True)
+                first_control_plane.sudo(final_commands, warn=True)
 
             recommended_sha = thirdparties.get_thirdparty_recommended_sha(path, cluster)
             if recommended_sha is not None and recommended_sha != expected_sha:
                 warnings.append(f"{path} source contains not recommended thirdparty version for used kubernetes version")
 
             if config.get("sha1", expected_sha) != expected_sha and expected_sha is not None:
                 broken .append("Given sha is not equal with actual sha from source for %s" % path)
@@ -332,28 +336,28 @@
 
             if expected_sha is None:
                 cluster.log.verbose(f"Can`t get expected sha for {path}, skip it")
                 # Skip checking sha if something went wrong or this sha can't be loaded
                 continue
 
             results = group.sudo(f'openssl sha1 {path} | sed "s/^.* //"', warn=True)
-            actual_sha = None
-            first_host = None
+            actual_sha: Optional[str] = None
+            first_host: Optional[str] = None
             # Searching actual SHA, if possible
             for host, result in results.items():
                 if result.failed:
-                    broken.append(f'failed to get {path} sha {host.host}: {result.stderr}')
+                    broken.append(f'failed to get {path} sha {host}: {result.stderr}')
                     continue
 
                 found_sha = result.stdout.strip()
                 if actual_sha is None:
                     actual_sha = found_sha
-                    first_host = host.host
+                    first_host = host
                 elif actual_sha != found_sha:
-                    broken.append(f'got inconsistent sha for {path}: {found_sha} on host {host.host}, '
+                    broken.append(f'got inconsistent sha for {path}: {found_sha} on host {host}, '
                                   f'different from first host {first_host} sha {actual_sha}')
                     actual_sha = None
                     break
 
             if actual_sha is None:
                 # was not able to find single actual SHA, errors already collected, nothing to do
                 continue
@@ -379,51 +383,51 @@
                                  '    $(sudo openssl sha1 %s/${file_name} | cut -d\\  -f2); '  # 3) sha unpacked
                                  'done' % (path, path, unpack_dir))
                 
                 # for each file on each host, verify that SHA in archive is equal to SHA for unpacked
                 for host, result in res.items():
                     if result.failed:
                         broken.append(f'can not verify files SHA for archive {path} '
-                                      f'on host {host.host}, unpacked to {unpack_dir}')
+                                      f'on host {host}, unpacked to {unpack_dir}')
                         continue
                     files_results = result.stdout.strip().split('\n')
                     for file_result in files_results:
                         result_parts = file_result.split()
                         if len(result_parts) != 3:
                             broken.append(f'can not verify files SHA for archive {path} '
-                                          f'on host {host.host}, unpacked to {unpack_dir}')
+                                          f'on host {host}, unpacked to {unpack_dir}')
                             continue
                         filename, archive_hash, fs_hash = result_parts[0], result_parts[1], result_parts[2]
                         if archive_hash != fs_hash:
                             broken.append(f'hash for file {filename} from archive {path} '
-                                          f'on host {host.host} is not equal to hash for file unpacked to {unpack_dir}')
+                                          f'on host {host} is not equal to hash for file unpacked to {unpack_dir}')
 
         if broken:
             raise TestFailure('Found inconsistent hashes', hint=yaml.safe_dump(broken))
         if warnings:
             raise TestWarn('Found warnings', hint=yaml.safe_dump(warnings))
         tc.success('All found hashes are correct')
 
 
-def find_hosts_missing_thirdparty(group, path) -> List[str]:
+def find_hosts_missing_thirdparty(group: NodeGroup, path: str) -> List[str]:
     """
     Search group for a list of hosts where thirdparty is missing
     :param group: group of hosts where to search thirdparty
     :param path: path to thirdparty to search
     :return: list of hosts where thirdparty is missing
     """
     results = group.sudo(f'ls {path}', warn=True)
     missing = []
     for host, result in results.items():
         if result.failed:
-            missing.append(host.host)
+            missing.append(host)
     return missing
 
 
-def kubernetes_nodes_existence(cluster):
+def kubernetes_nodes_existence(cluster: KubernetesCluster):
     with TestCase(cluster, '209', "Kubernetes", "Nodes Existence",
                   default_results="All nodes presented"):
         nodes_description = get_nodes_description(cluster)
         nodes_names = kubernetes.get_actual_roles(nodes_description).keys()
         not_found = []
         for node in cluster.inventory['nodes']:
             if 'control-plane' in node['roles'] or 'worker' in node['roles']:
@@ -462,15 +466,15 @@
         nodes_with_bad_roles = list(set(nodes_with_bad_roles))
         if nodes_with_bad_roles:
             raise TestFailure("Incorrect role detected at: %s" % ', '.join(nodes_with_bad_roles),
                               hint="Some nodes whose role differs from that specified in the "
                                    "inventory were detected. The configuration of these nodes should be fixed.")
 
 
-def kubernetes_nodes_condition(cluster, condition_type):
+def kubernetes_nodes_condition(cluster: KubernetesCluster, condition_type: str):
     with TestCase(cluster, '211', "Kubernetes", "Nodes Condition - %s" % condition_type) as tc:
         nodes_description = get_nodes_description(cluster)
         expected_status = 'False'
         if condition_type == 'Ready':
             expected_status = 'True'
         positive_conditions = []
         negative_conditions = []
@@ -494,23 +498,23 @@
             raise TestFailure("%s" % ', '.join(negative_conditions),
                               hint="A condition in negative status means that there are problems with the health of "
                                    "the node.")
 
         tc.success(results="%s" % ', '.join(positive_conditions))
 
 
-def get_not_running_pods(cluster):
+def get_not_running_pods(cluster: KubernetesCluster):
     # Completed pods should be excluded from the list as well
     get_pods_cmd = 'kubectl get pods -A --field-selector status.phase!=Running | awk \'{ print $1" "$2" "$4 }\' | grep -vw Completed || true'
     result = cluster.nodes['control-plane'].get_any_member().sudo(get_pods_cmd)
     cluster.log.verbose(result)
     return list(result.values())[0].stdout.strip()
 
 
-def kubernetes_pods_condition(cluster):
+def kubernetes_pods_condition(cluster: KubernetesCluster):
     system_namespaces = ["kube-system", "ingress-nginx", "kube-public", "kubernetes-dashboard", "default"]
     critical_states = cluster.globals['pods']['critical_states']
     with TestCase(cluster, '207', "Kubernetes", "Pods Condition") as tc:
         pods_description = get_not_running_pods(cluster)
         total_failed_amount = len(pods_description.split('\n')[1:])
         critical_system_failed_amount = 0
 
@@ -534,15 +538,15 @@
                            hint="Try to determine the reason the pods are not operational, "
                                 "try to wait, redeploy, reapply, or restart them. "
                                 "If this is not fixed, some deployed applications may not work or may work incorrectly.")
         else:
             tc.success(results="All pods are running")
 
 
-def kubernetes_dashboard_status(cluster):
+def kubernetes_dashboard_status(cluster: KubernetesCluster):
     with TestCase(cluster, '208', "Plugins", "Dashboard Availability") as tc:
         retries = 10
         test_succeeded = False
         i = 0
         while not test_succeeded and i < retries:
             i += 1
             if cluster.inventory['plugins']['kubernetes-dashboard']['install']:
@@ -568,49 +572,51 @@
                 test_succeeded = True
                 tc.success(results="skipped")
         if not test_succeeded:
             raise TestFailure("not available",
                               hint=f"Please verify the following Kubernetes Dashboard status and fix this issue:\n{status}")
 
 
-def nodes_pid_max(cluster):
+def nodes_pid_max(cluster: KubernetesCluster):
     with TestCase(cluster, '202', "Nodes", "Nodes pid_max correctly installed") as tc:
         control_plane = cluster.nodes['control-plane'].get_any_member()
         yaml = ruamel.yaml.YAML()
         nodes_failed_pid_max_check = {}
-        for node in cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_ordered_members_list(provide_node_configs=True):
+        for node in cluster.make_group_from_roles(['control-plane', 'worker']).get_ordered_members_list():
+            node_name = node.get_node_name()
 
-            node_info = control_plane.sudo("kubectl get node %s -o yaml" % node["name"]).get_simple_out()
+            node_info = control_plane.sudo("kubectl get node %s -o yaml" % node_name).get_simple_out()
             config = yaml.load(node_info)
             max_pods = int(config['status']['capacity']['pods'])
 
-            kubelet_config = node["connection"].sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
+            kubelet_config = node.sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
             config = yaml.load(kubelet_config)
             pod_pids_limit = int(config['podPidsLimit'])
 
-            pid_max = int(node["connection"].sudo("cat /proc/sys/kernel/pid_max").get_simple_out())
+            pid_max = int(node.sudo("cat /proc/sys/kernel/pid_max").get_simple_out())
             required_pid_max = max_pods * pod_pids_limit + 2048
             cluster.log.debug("Current values:\n maxPods = %s \n podPidsLimit = %s \n pid_max = %s"
                               % (max_pods, pod_pids_limit, pid_max))
             cluster.log.debug("Required pid_max for current kubelet configuration is %s for node '%s'"
-                              % (required_pid_max, node["name"]))
+                              % (required_pid_max, node_name))
             if cluster.inventory['services']['sysctl'].get("kernel.pid_max"):
                 inventory_pid_max = cluster.inventory['services']['sysctl'].get("kernel.pid_max")
                 if pid_max != inventory_pid_max:
                     raise TestWarn("The 'kernel.pid_max' value defined in system = %s, "
                                    "but 'kernel.pid_max', which defined in cluster.yaml = %s"
                                    % (pid_max, inventory_pid_max))
             if pid_max < required_pid_max:
-                nodes_failed_pid_max_check[node["name"]] = [pid_max, required_pid_max]
+                nodes_failed_pid_max_check[node_name] = [pid_max, required_pid_max]
 
         if nodes_failed_pid_max_check:
             output = "The requirement for the 'pid_max' value is not met for nodes:\n"
-            for node in nodes_failed_pid_max_check:
+            for node_name in nodes_failed_pid_max_check:
                 output += ("For node %s pid_max value = '%s', but it should be >= then '%s'\n"
-                           % (node, nodes_failed_pid_max_check[node][0], nodes_failed_pid_max_check[node][1]))
+                           % (node_name, nodes_failed_pid_max_check[node_name][0],
+                              nodes_failed_pid_max_check[node_name][1]))
             raise TestFailure(output)
         tc.success(results="pid_max correctly installed on all nodes")
 
 
 def verify_selinux_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which checks the status of Selinux. It must be `enforcing`. It may be `permissive`, but must
@@ -629,25 +635,25 @@
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         cluster.log.debug(selinux_result)
         enforcing_ips = []
         permissive_ips = []
         bad_ips = []
-        for conn, results in selinux_parsed_result.items():
+        for host, results in selinux_parsed_result.items():
             if results.get('status', '') != 'disabled':
                 if results['mode'] == 'enforcing':
-                    enforcing_ips.append(conn.host)
+                    enforcing_ips.append(host)
                 elif results['mode'] == 'permissive' and cluster.inventory.get('services', {})\
                         .get('kernel_security', {}).get('selinux', {}).get('state') == 'permissive':
-                    permissive_ips.append(conn.host)
+                    permissive_ips.append(host)
                 else:
-                    bad_ips.append([conn.host, results['mode']])
+                    bad_ips.append([host, results['mode']])
             else:
-                bad_ips.append([conn.host, 'disabled'])
+                bad_ips.append([host, 'disabled'])
 
         if group.nodes_amount() == len(enforcing_ips):
             tc.success(results='enforcing')
         elif len(bad_ips) == 0:
             pretty_list = '\n - ' + ('\n - '.join(permissive_ips))
             raise TestWarn('permissive',
                            hint=f"It is not recommended to use the permissive state, but this is possible if you "
@@ -726,15 +732,15 @@
     with TestCase(cluster, '218', "System", "Time difference") as tc:
         group = cluster.nodes['all']
         current_node_time, nodes_timestamp, time_diff = system.get_nodes_time(group)
         cluster.log.verbose('Current node time: %s' % current_node_time)
         cluster.log.verbose('Time difference: %s' % time_diff)
         cluster.log.verbose('Nodes time details:')
         for host, timestamp in nodes_timestamp.items():
-            cluster.log.verbose(' - %s: %s' % (host.host, timestamp))
+            cluster.log.verbose(' - %s: %s' % (host, timestamp))
 
         if time_diff > cluster.globals['nodes']['max_time_difference']:
             raise TestWarn("%sms" % time_diff,
                            hint=f"The time difference between nodes is too large, this can lead to incorrect "
                                 f"behavior of Kubernetes and services. To fix this problem, run the NTP configuring "
                                 f"task on all nodes with the correct parameters. It is also worth paying attention to "
                                 f"the delay between the deployed node and all the others - too much delay can lead to "
@@ -778,15 +784,15 @@
             tc.success(results='valid')
         else:
             raise TestFailure('invalid',
                               hint=f"Modprobe rules do not match those loaded in modprobe on cluster nodes. Check "
                                    f"manually what the differences are and make changes on the appropriate nodes.")
 
 
-def etcd_health_status(cluster):
+def etcd_health_status(cluster: KubernetesCluster):
     """
     This method is a test, check ETCD health
     :param cluster: KubernetesCluster object
     :return: None
     """
     with TestCase(cluster, '219', "ETCD", "Health status ETCD") as tc:
         try:
@@ -796,51 +802,50 @@
             raise TestFailure('invalid',
                               hint=f"ETCD not ready, please check"
                                    f" because of {e} ")
         cluster.log.debug(etcd_health_status)
         tc.success(results='healthy')
 
 
-def control_plane_configuration_status(cluster):
+def control_plane_configuration_status(cluster: KubernetesCluster):
     '''
     This test verifies the consistency of the configuration (image version, `extra_args`, `extra_volumes`) of static pods of Control Plain like `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '220', "Control plane", "configuration status") as tc:
-        results = []
+        results: List[dict] = []
         static_pod_names = {'kube-apiserver': 'apiServer',
                             'kube-controller-manager': 'controllerManager',
                             'kube-scheduler': 'scheduler'}
         static_pods_content = []
         not_presented_static_pods = []
-        for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
+        for control_plane in cluster.nodes['control-plane'].get_ordered_members_list():
             for static_pod_name, value in static_pod_names.items():
-                result = control_plane['connection'].sudo(f'cat /etc/kubernetes/manifests/{static_pod_name}.yaml', warn=True)
-                exit_code = list(result.values())[0].exited
-                result = result.get_simple_out()
+                static_pod_result = control_plane.sudo(f'cat /etc/kubernetes/manifests/{static_pod_name}.yaml', warn=True)
+                exit_code = list(static_pod_result.values())[0].exited
                 if exit_code == 0:
-                    result = yaml.safe_load(result)
-                    result[static_pod_name] = value
-                    static_pods_content.append(result)
+                    static_pod = yaml.safe_load(static_pod_result.get_simple_out())
+                    static_pod[static_pod_name] = value
+                    static_pods_content.append(static_pod)
                 else:
                     not_presented_static_pods.append(static_pod_name)
             for not_presented_static_pod in not_presented_static_pods:
                 del static_pod_names[not_presented_static_pod]
 
-            result = dict()
-            result['name'] = control_plane['name']
+            result: dict = {'name': control_plane.get_node_name()}
             version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
 
+            node_config = control_plane.get_config()
             for static_pod in static_pods_content:
-                result[static_pod['metadata']['name']] = dict()
+                result[static_pod['metadata']['name']] = {}
                 result[static_pod['metadata']['name']]['correct_version'] = \
                     version in static_pod["spec"]["containers"][0].get("image", "")
                 result[static_pod['metadata']['name']]['correct_properties'] = \
-                    check_extra_args(cluster, static_pod, control_plane)
+                    check_extra_args(cluster, static_pod, node_config)
                 result[static_pod['metadata']['name']]['correct_volumes'] = check_extra_volumes(cluster, static_pod)
             results.append(result)
 
         message = ""
         for result in results:
             for static_pod_name in static_pod_names:
                 if result[static_pod_name]['correct_version'] and \
@@ -854,15 +859,15 @@
 
         if not message:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=message)
 
 
-def check_extra_args(cluster, static_pod, node):
+def check_extra_args(cluster: KubernetesCluster, static_pod: dict, node: NodeConfig):
     static_pod_name = static_pod[static_pod['metadata']['name']]
     for arg, value in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraArgs", {}).items():
         if arg == "bind-address":
             # for "bind-address" we do not take default value into account, because its patched to node internal-address
             value = node["internal_address"]
         correct_property = False
         original_property = arg + "=" + value
@@ -872,15 +877,15 @@
                 correct_property = True
                 break
         if not correct_property:
             return False
     return True
 
 
-def check_extra_volumes(cluster, static_pod):
+def check_extra_volumes(cluster: KubernetesCluster, static_pod: dict):
     static_pod_name = static_pod[static_pod['metadata']['name']]
     #for original_volume in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraVolumes", {}).items():
     for original_volume in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraVolumes", {}):
         correct_volume = False
         volume_mounts = static_pod["spec"]["containers"][0].get("volumeMounts", {})
         for volumeMount in volume_mounts:
             if volumeMount['mountPath'] == original_volume['mountPath'] and \
@@ -901,58 +906,56 @@
                 correct_volume = True
                 break
         if not correct_volume:
             return False
     return True
 
 
-def control_plane_health_status(cluster):
+def control_plane_health_status(cluster: KubernetesCluster):
     '''
     This test verifies the health of static pods `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '221', "Control plane", "health status") as tc:
         static_pods = ['kube-apiserver', 'kube-controller-manager', 'kube-scheduler']
         static_pod_names = []
 
-        for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
+        for control_plane in cluster.nodes['control-plane'].get_ordered_members_list():
             for static_pod in static_pods:
-                static_pod_names.append(static_pod + '-' + control_plane['name'])
+                static_pod_names.append(static_pod + '-' + control_plane.get_node_name())
 
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         not_found_pod = []
         for static_pod_name in static_pod_names:
-            result = first_control_plane.sudo(f"kubectl get pod -n kube-system -oyaml {static_pod_name}", warn=True)
-            exit_code = list(result.values())[0].exited
+            results = first_control_plane.sudo(f"kubectl get pod -n kube-system -oyaml {static_pod_name}", warn=True)
+            exit_code = list(results.values())[0].exited
             if exit_code == 0:
-                result = result.get_simple_out()
-                result = yaml.safe_load(result)
+                result = yaml.safe_load(results.get_simple_out())
                 if result['status']['containerStatuses'][0]['state'].get('running'):
                     break
             not_found_pod.append(static_pod_name)
 
         if len(not_found_pod) == 0:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=f"{not_found_pod} pods doesn't running")
 
 
-def default_services_configuration_status(cluster):
+def default_services_configuration_status(cluster: KubernetesCluster):
     '''
     In this test, the versions of the images of the default services, such as `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`, are checked, and the `coredns` configmap is also checked.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '222', "Default services", "configuration status") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
-        original_coredns_cm = generate_configmap(cluster.inventory)
-        original_coredns_cm = yaml.safe_load(original_coredns_cm)
-        coredns_cm = first_control_plane.sudo('kubectl get cm coredns -n kube-system -oyaml').get_simple_out()
-        coredns_cm = yaml.safe_load(coredns_cm)
+        original_coredns_cm = yaml.safe_load(generate_configmap(cluster.inventory))
+        result = first_control_plane.sudo('kubectl get cm coredns -n kube-system -oyaml')
+        coredns_cm = yaml.safe_load(result.get_simple_out())
         ddiff = DeepDiff(coredns_cm['data'], original_coredns_cm['data'], ignore_order=True)
         coredns_result = ddiff.to_dict().get('values_changed', {}).get("root['Corefile']", {}).get('diff')
 
         message = ""
         if coredns_result:
             message += f"CoreDNS config is outdated: \n {coredns_result} \n"
 
@@ -969,31 +972,31 @@
             for type_dict in types_dict:
                 for type, services in type_dict.items():
                     for service in services:
                         for service_name, properties in service.items():
                             if service_name == "ingress-nginx-controller":
                                 if not cluster.inventory['plugins']['nginx-ingress-controller']['install']:
                                     break
-                            content = first_control_plane.sudo(f"kubectl get {type} {service_name} -n {namespace} -oyaml").get_simple_out()
-                            content = yaml.safe_load(content)
+                            result = first_control_plane.sudo(f"kubectl get {type} {service_name} -n {namespace} -oyaml")
+                            content = yaml.safe_load(result.get_simple_out())
                             if properties["version"] in content["spec"]["template"]["spec"]["containers"][0].get("image", ""):
                                 results[service_name] = True
                             else:
                                 results[service_name] = False
         for item, condition in results.items():
             if not condition:
                 message += f"{item} has outdated image version\n"
 
         if message:
             raise TestFailure('invalid', hint=f"{message}")
         else:
             tc.success(results='valid')
 
 
-def default_services_health_status(cluster):
+def default_services_health_status(cluster: KubernetesCluster):
     '''
     This test verifies the health of pods `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '223', "Default services", "health status") as tc:
         entities_to_check = {"kube-system": [{"DaemonSet": ["calico-node", "kube-proxy"]},
@@ -1022,59 +1025,58 @@
                                 not_ready_entities.append(service)
         if len(not_ready_entities) == 0:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=f"{not_ready_entities} pods doesn't ready")
 
 
-def calico_config_check(cluster):
+def calico_config_check(cluster: KubernetesCluster):
     '''
     This test checks the configuration of the `calico-node` envs, Calico's ConfigMap in case of `ipam`, and also performed `calicoctl ipam check`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '224', "Calico", "configuration check") as tc:
         message = ""
         correct_config = True
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         result = first_control_plane.sudo(f"kubectl get DaemonSet calico-node -n kube-system -oyaml")
-        result = result.get_simple_out()
-        result = yaml.safe_load(result)
-        for env in result["spec"]["template"]["spec"]["containers"][0]["env"]:
+        calico_daemonset = yaml.safe_load(result.get_simple_out())
+        for env in calico_daemonset["spec"]["template"]["spec"]["containers"][0]["env"]:
             if cluster.inventory["plugins"]["calico"]["env"].get(env["name"]):
                 if "value" in env.keys() and not str(cluster.inventory["plugins"]["calico"]["env"].get(env["name"])) == env["value"]:
                     correct_config = False
                 if "valueFrom" in env.keys() and len(DeepDiff(cluster.inventory["plugins"]["calico"]["env"].get(env["name"]), env["valueFrom"], ignore_order=True)) != 0:
                     correct_config = False
         if not correct_config:
             message += "calico-node env configuration is outdated\n"
 
-        result = first_control_plane.sudo(f"kubectl get cm calico-config -n kube-system -oyaml").get_simple_out()
-        result = yaml.safe_load(result)
-        result = yaml.safe_load(result["data"]["cni_network_config"])
+        result = first_control_plane.sudo(f"kubectl get cm calico-config -n kube-system -oyaml")
+        calico_config = yaml.safe_load(result.get_simple_out())
+        cni_network_config = yaml.safe_load(calico_config["data"]["cni_network_config"])
         ip = cluster.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
         if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
             ipam_config = cluster.inventory["plugins"]["calico"]["cni"]["ipam"]["ipv4"]
         else:
             ipam_config = cluster.inventory["plugins"]["calico"]["cni"]["ipam"]["ipv6"]
-        ddiff = DeepDiff(ipam_config, result["plugins"][0]["ipam"], ignore_order=True)
+        ddiff = DeepDiff(ipam_config, cni_network_config["plugins"][0]["ipam"], ignore_order=True)
         if ddiff:
             message += f"calico cm is outdated: {ddiff.to_dict()}\n"
 
-        result = first_control_plane.sudo("calicoctl ipam check | grep 'found .* problems' |  tr -dc '0-9'").get_simple_out()
-        if int(result) > 0:
+        result = first_control_plane.sudo("calicoctl ipam check | grep 'found .* problems' |  tr -dc '0-9'")
+        if int(result.get_simple_out()) > 0:
             message += "ipam check indicates some problems," \
                        " for more info you can use `calicoctl ipam check --show-problem-ips`"
         if message:
             raise TestFailure('invalid', hint=message)
         else:
             tc.success(results='valid')
 
 
-def kubernetes_admission_status(cluster):
+def kubernetes_admission_status(cluster: KubernetesCluster):
     """
     The method checks status of Pod Security Admissions, default Pod Security Profile,
     and 'kube-apiserver.yaml' and 'kubeadm-config' consistancy
     """
     with TestCase(cluster, '225', "Kubernetes", "Pod Security Admissions") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         profile_inv = ""
@@ -1087,16 +1089,16 @@
         cluster_config = yaml.safe_load(kubeadm_cm["data"]["ClusterConfiguration"])
         api_result = first_control_plane.sudo("cat /etc/kubernetes/manifests/kube-apiserver.yaml")
         api_conf = yaml.safe_load(list(api_result.values())[0].stdout)
         ext_args = [cmd for cmd in api_conf["spec"]["containers"][0]["command"]]
         admission_path = ""
         for item in ext_args:
             if item.startswith("--"):
-                key = re.split('=',item)[0]
-                value = re.search('=(.*)$', item).group(1)
+                key = item.split('=')[0]
+                value = item[len(key) + 1:]
                 if key == "--admission-control-config-file":
                     admission_path = value
                     adm_result = first_control_plane.sudo("cat %s" % admission_path)
                     adm_conf = yaml.safe_load(list(adm_result.values())[0].stdout)
                     profile = adm_conf["plugins"][0]["configuration"]["defaults"]["enforce"]
                 if key == "--feature-gates":
                     features = value
@@ -1124,29 +1126,27 @@
                          f"that is applied on cluster in 'kube-apiserver.yaml' and 'admission.yaml'")
         if not profile:
             kube_admission_status = 'PSS is "disabled"'
             cluster.log.debug(kube_admission_status)
             tc.success(results='disabled')
 
 
-def geo_check(cluster):
+def geo_check(cluster: KubernetesCluster):
     """
     This test checks connectivity between clusters in geo schemas using paas-geo-monitor service.
     This test only work if "procedure.yaml" has "geo-monitor" section filled.
     """
     if not cluster.procedure_inventory or not cluster.procedure_inventory.get("geo-monitor"):
         cluster.log.debug("Geo connectivity check is skipped, no configuration provided")
         return
 
-    collected_results = {
-        "statusCollected": False,
-        "dnsStatus": {"failed": []},
-        "svcStatus": {"failed": [], "skipped": []},
-        "podStatus": {"failed": [], "skipped": []}
-    }
+    status_collected = False
+    dns_status: Dict[str, List[str]] = {"failed": []}
+    svc_status: Dict[str, List[str]] = {"failed": [], "skipped": []}
+    pod_status: Dict[str, List[str]] = {"failed": [], "skipped": []}
 
     # Here we actually collect information about all statuses, but report information about DNS only.
     # Other statuses are reported in other TestCases below. This is done for better UX.
     with TestCase(cluster, '226', "Geo Monitor", "Geo check - DNS resolving") as tc_dns:
         geo_monitor_inventory = cluster.procedure_inventory["geo-monitor"]
         namespace = geo_monitor_inventory["namespace"]
         service = geo_monitor_inventory["service"]
@@ -1169,55 +1169,55 @@
             raise TestFailure("configuration error", hint="geo-monitor instance has no peers")
 
         for peer in peers:
             status = peer["clusterIpStatus"]
             if not status["dnsStatus"]["resolved"]:
                 error = f'FAILED DNS resolving for peer ({peer["name"]}) service ' \
                         f'name: {status["name"]}, error: {status["dnsStatus"]["error"]}'
-                collected_results["dnsStatus"]["failed"].append(error)
-                collected_results["svcStatus"]["skipped"].append(error)
-                collected_results["podStatus"]["skipped"].append(error)
+                dns_status["failed"].append(error)
+                svc_status["skipped"].append(error)
+                pod_status["skipped"].append(error)
                 continue
             if not status["svcStatus"]["available"]:
                 error = f'FAILED ping service for peer ({peer["name"]}), ' \
                         f'address: {status["svcStatus"]["address"]}, error: {status["svcStatus"]["error"]}'
-                collected_results["svcStatus"]["failed"].append(error)
-                collected_results["podStatus"]["skipped"].append(error)
+                svc_status["failed"].append(error)
+                pod_status["skipped"].append(error)
                 continue
             if not status["podStatus"]["available"]:
                 error = f'FAILED ping pod for peer ({peer["name"]}), ' \
                         f'address: {status["podStatus"]["address"]}, error: {status["podStatus"]["error"]}'
-                collected_results["podStatus"]["failed"].append(error)
+                pod_status["failed"].append(error)
                 continue
 
-        collected_results["statusCollected"] = True
-        if collected_results["dnsStatus"]["failed"]:
-            raise TestFailure("found failed DNS statuses", hint=yaml.safe_dump(collected_results["dnsStatus"]["failed"]))
+        status_collected = True
+        if dns_status["failed"]:
+            raise TestFailure("found failed DNS statuses", hint=yaml.safe_dump(dns_status["failed"]))
         tc_dns.success("all peer names resolved")
 
     with TestCase(cluster, '226', "Geo Monitor", "Geo check - Pod-to-service") as tc_svc:
-        if not collected_results["statusCollected"]:
+        if not status_collected:
             raise TestFailure("configuration error", hint="DNS check failed with error, statuses not collected")
 
-        if collected_results["svcStatus"]["failed"]:
+        if svc_status["failed"]:
             raise TestFailure("found unavailable peer services",
-                              hint=yaml.safe_dump(collected_results["svcStatus"]["failed"]+collected_results["svcStatus"]["skipped"]))
-        if collected_results["svcStatus"]["skipped"]:
-            raise TestWarn("found skipped peer services", hint=yaml.safe_dump(collected_results["svcStatus"]["skipped"]))
+                              hint=yaml.safe_dump(svc_status["failed"] + svc_status["skipped"]))
+        if svc_status["skipped"]:
+            raise TestWarn("found skipped peer services", hint=yaml.safe_dump(svc_status["skipped"]))
         tc_svc.success("all peer services available")
 
     with TestCase(cluster, '226', "Geo Monitor", "Geo check - Pod-to-pod") as tc_pod:
-        if not collected_results["statusCollected"]:
+        if not status_collected:
             raise TestFailure("configuration error", hint="DNS check failed with error, statuses not collected")
 
-        if collected_results["podStatus"]["failed"]:
+        if pod_status["failed"]:
             raise TestFailure("found unavailable peer pod",
-                              hint=yaml.safe_dump(collected_results["podStatus"]["failed"]+collected_results["podStatus"]["skipped"]))
-        if collected_results["podStatus"]["skipped"]:
-            raise TestWarn("found skipped peer pods", hint=yaml.safe_dump(collected_results["podStatus"]["skipped"]))
+                              hint=yaml.safe_dump(pod_status["failed"] + pod_status["skipped"]))
+        if pod_status["skipped"]:
+            raise TestWarn("found skipped peer pods", hint=yaml.safe_dump(pod_status["skipped"]))
         tc_pod.success("all peer pods available")
 
 
 def verify_apparmor_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which checks the status of Apparmor.
     This test is applicable only for systems of the Debian family.
@@ -1226,23 +1226,23 @@
     """
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         return
 
     with TestCase(cluster, '227', "Security", "Apparmor security policy") as tc:
         group = cluster.nodes['all'].get_accessible_nodes()
         results = group.sudo("aa-enabled")
-        enabled_nodes = []
-        invalid_nodes = []
-        for connection, item in results.items():
+        enabled_nodes: List[str] = []
+        invalid_nodes: List[str] = []
+        for host, item in results.items():
             apparmor_status = item.stdout
-            cluster.log.warning(f"Apparmor on node: {connection.host} enabled: {apparmor_status}")
+            cluster.log.warning(f"Apparmor on node: {host} enabled: {apparmor_status}")
             if apparmor_status ==  "Yes":
-                enabled_nodes.append(connection.host)
+                enabled_nodes.append(host)
             else:
-                enabled_nodes.append(connection.host)
+                enabled_nodes.append(host)
         if group.nodes_amount() == len(enabled_nodes):
             tc.success(results='enabled')
         else:
             raise TestFailure(f"Apparmor does not properly configured on the following nodes: {invalid_nodes}")
 
 
 def verify_apparmor_config(cluster: KubernetesCluster) -> None:
@@ -1255,15 +1255,15 @@
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         return
 
     with TestCase(cluster, '228', "Security", "Apparmor security policy") as tc:
         expected_profiles = cluster.inventory['services']['kernel_security'].get('apparmor', {})
         group = cluster.nodes['all'].get_accessible_nodes()
         if expected_profiles:
-            apparmor_configured, result = apparmor.is_state_valid(group, expected_profiles)
+            apparmor_configured = apparmor.is_state_valid(group, expected_profiles)
             if apparmor_configured:
                 cluster.log.verbose(f"Apparmor is configured properly on cluster")
                 tc.success(results='valid')
             else:
                 raise TestFailure('invalid',
                         hint=f"Some nodes do not have properly configured Apparmor service")
         else:
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/do.py` & `kubemarine-0.19.0/kubemarine/procedures/do.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import argparse
 import sys
-from typing import Callable
+from typing import Callable, List, Dict
 
 from kubemarine.core import flow, resources
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 
@@ -28,37 +28,39 @@
 Script for executing shell command
     
 additional arguments:
     shell_command       command to execute on nodes
 """
 
 class CLIAction(Action):
-    def __init__(self, node_group_provider: Callable[[KubernetesCluster], NodeGroup], remote_args, no_stream):
+    def __init__(self, node_group_provider: Callable[[KubernetesCluster], NodeGroup],
+                 remote_args: List[str], no_stream: bool) -> None:
         super().__init__('do')
         self.node_group_provider = node_group_provider
         self.remote_args = remote_args
         self.no_stream = no_stream
 
-    def run(self, res: DynamicResources):
-        executors_group = self.node_group_provider(res.cluster())
+    def run(self, res: DynamicResources) -> None:
+        cluster = res.cluster()
+        executors_group = self.node_group_provider(cluster)
         if executors_group.is_empty():
             print('Failed to find any of specified nodes or groups')
             sys.exit(1)
 
-        res = executors_group.sudo(" ".join(self.remote_args), hide=self.no_stream, warn=True)
+        result = executors_group.sudo(" ".join(self.remote_args), hide=self.no_stream, warn=True)
         if self.no_stream:
-            res.print()
+            cluster.log.debug(result)
 
-        if res.is_any_failed():
+        if result.is_any_failed():
             sys.exit(1)
 
         sys.exit(0)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     if not cli_arguments:
         cli_arguments = sys.argv
 
     if '--' in cli_arguments:
         kubemarine_args = cli_arguments[:cli_arguments.index('--')]
         remote_args = cli_arguments[cli_arguments.index('--') + 1:]
@@ -101,17 +103,17 @@
             ['stdout;level=error;colorize=true;correct_newlines=true']
         ],
         'config': configfile_path,
         'ignore_schema_errors': ignore_schema_errors
     })
     context['preserve_inventory'] = False
 
-    def node_group_provider(cluster: KubernetesCluster):
+    def node_group_provider(cluster: KubernetesCluster) -> NodeGroup:
         if arguments.get('node', None) is not None or arguments.get('group', None) is not None:
-            executor_lists = {
+            executor_lists: Dict[str, List[str]] = {
                     'node': [],
                     'group': []
             }
             for executors_type in executor_lists.keys():
                 executors_str = arguments.get(executors_type)
                 if executors_str:
                     if "," in executors_str:
@@ -119,15 +121,15 @@
                             executor_lists[executors_type].append(executor_name.strip())
                     else:
                         executor_lists[executors_type].append(executors_str.strip())
             return cluster.create_group_from_groups_nodes_names(executor_lists['group'], executor_lists['node'])
         else:
             return cluster.nodes['control-plane'].get_any_member()
 
-    no_stream = arguments.get('no_stream')
+    no_stream: bool = arguments['no_stream']
     action = CLIAction(node_group_provider, remote_args, no_stream)
     res = resources.DynamicResources(context, silent=True)
     flow.ActionsFlow([action]).run_flow(res, print_summary=False)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/install.py` & `kubemarine-0.19.0/kubemarine/procedures/install.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,81 +11,83 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
-from typing import Callable
+from types import FunctionType
+from typing import Callable, List, Dict, cast
 
-import fabric
 import yaml
 import os
 import io
 
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.errors import KME
 from kubemarine import system, sysctl, haproxy, keepalived, kubernetes, plugins, \
     kubernetes_accounts, selinux, thirdparties, admission, audit, coredns, cri, packages, apparmor
 from kubemarine.core import flow, utils, summary
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroup
+from kubemarine.core.group import NodeGroup, RunnersGroupResult, CollectorCallback
 from kubemarine.core.resources import DynamicResources
 
 
-def _applicable_for_new_nodes_with_roles(*roles):
+TASK_CALLABLE = Callable[[KubernetesCluster], None]
+DECORATED_GROUP_CALLABLE = Callable[[NodeGroup], None]
+
+
+def _applicable_for_new_nodes_with_roles(*roles: str) -> Callable[[DECORATED_GROUP_CALLABLE], TASK_CALLABLE]:
     """
     Decorator to annotate installation methods.
     If there are no new nodes with the specified roles to be added / installed to the cluster,
     the decorator skips execution of the method.
     Otherwise, it runs the annotated method with the calculated group of nodes with the specified roles.
     Note that the signature of annotated method should be f(NodeGroup),
     but the resulting wrapping method will be f(KubernetesCluster).
 
     :param roles: roles of nodes for which the annotated method is applicable.
     :return: new wrapping method.
     """
     if not roles:
         raise Exception(f'Roles are not defined')
 
-    def roles_wrapper(fn: Callable[[NodeGroup], None]):
-        def cluster_wrapper(cluster: KubernetesCluster):
+    def roles_wrapper(fn: DECORATED_GROUP_CALLABLE) -> TASK_CALLABLE:
+        def cluster_wrapper(cluster: KubernetesCluster) -> None:
             candidate_group = cluster.nodes['all'].get_new_nodes_or_self()
-            group = cluster.make_group([])
-            for role in roles:
-                group = group.include_group(cluster.nodes.get(role))
+            group = cluster.make_group_from_roles(roles)
             group = group.intersection_group(candidate_group)
             if not group.is_empty():
                 fn(group)
             else:
-                fn_name = fn.__module__ + '.' + fn.__qualname__
+                func = cast(FunctionType, fn)
+                fn_name = func.__module__ + '.' + func.__qualname__
                 cluster.log.debug(f"Skip running {fn_name} as no new node with roles {roles} has been found.")
 
         return cluster_wrapper
 
     return roles_wrapper
 
 
-def system_prepare_check_sudoer(cluster):
+def system_prepare_check_sudoer(cluster: KubernetesCluster):
     not_sudoers = []
     for host, node_context in cluster.context['nodes'].items():
         access_info = node_context['access']
         if access_info['online'] and access_info['sudo'] == 'Root':
             cluster.log.debug("%s online and has root" % host)
         else:
             not_sudoers.append(host)
 
     if not_sudoers:
         raise KME("KME0005", hostnames=not_sudoers)
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_check_system(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     cluster.log.debug(system.fetch_os_versions(cluster))
     for address, context in cluster.context["nodes"].items():
         if address not in group.nodes:
             continue
         if context["os"]["family"] == "unsupported":
             raise Exception('%s host operating system is unsupported' % address)
         if context["os"]["family"] == "unknown":
@@ -96,43 +98,43 @@
             raise Exception("%s running on unknown %s version. "
                             "Expected %s, got '%s'" % (address,
                                                        context["os"]["name"],
                                                        supported_os_versions,
                                                        context["os"]["version"]))
 
 
-def system_prepare_check_cluster_installation(cluster):
+def system_prepare_check_cluster_installation(cluster: KubernetesCluster):
     if kubernetes.is_cluster_installed(cluster):
         cluster.log.debug('Cluster already installed and available at %s' % cluster.context['controlplain_uri'])
     else:
         cluster.log.debug('There is no any installed cluster')
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_system_chrony(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     if cluster.inventory['services']['ntp'].get('chrony', {}).get('servers') is None:
         cluster.log.debug("Skipped - NTP servers from chrony is not defined in config file")
         return
     group.call(system.configure_chronyd)
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_system_timesyncd(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     if not cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('NTP') and \
             not cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('FallbackNTP'):
         cluster.log.debug("Skipped - NTP servers from timesyncd is not defined in config file")
         return
     group.call(system.configure_timesyncd)
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_system_sysctl(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     if cluster.inventory['services'].get('sysctl') is None or not cluster.inventory['services']['sysctl']:
         cluster.log.debug("Skipped - sysctl is not defined or empty in config file")
         return
     group.call_batch([
         sysctl.configure,
         sysctl.reload,
     ])
@@ -174,216 +176,206 @@
 
 
 @_applicable_for_new_nodes_with_roles('control-plane')
 def system_prepare_policy(group: NodeGroup):
     """
     Task generates rules for logging kubernetes and on audit
     """
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     api_server_extra_args = cluster.inventory['services']['kubeadm']['apiServer']['extraArgs']
     audit_log_dir = os.path.dirname(api_server_extra_args['audit-log-path'])
     audit_file_name = api_server_extra_args['audit-policy-file']
     audit_policy_dir = os.path.dirname(audit_file_name)
     group.sudo(f"mkdir -p {audit_log_dir} && sudo mkdir -p {audit_policy_dir}")
     policy_config = cluster.inventory['services']['audit'].get('cluster_policy')
-    collect_node = group.get_ordered_members_list(provide_node_configs=True)
+    collect_node = group.get_ordered_members_list()
 
     if policy_config:
         policy_config_file = yaml.dump(policy_config)
         utils.dump_file(cluster, policy_config_file, 'audit-policy.yaml')
         #download rules in cluster
         for node in collect_node:
-            node['connection'].put(io.StringIO(policy_config_file), audit_file_name, sudo=True, backup=True)
+            node.put(io.StringIO(policy_config_file), audit_file_name, sudo=True, backup=True)
         audit_config = True
         cluster.log.debug("Audit cluster policy config")
     else:
         audit_config = False
         cluster.log.debug("Audit cluster policy config is empty, nothing will be configured ")
 
     if kubernetes.is_cluster_installed(cluster) and audit_config is True and cluster.context['initial_procedure'] != 'add_node':
         for control_plane in collect_node:
-            config_new = (kubernetes.get_kubeadm_config(cluster.inventory))
+            node_config = control_plane.get_config()
+            config_new = kubernetes.get_kubeadm_config(cluster.inventory)
 
             # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
             # and only "else" branch remains
             if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
-                control_plane['connection'].put(io.StringIO(config_new), '/etc/kubernetes/audit-on-config.yaml', sudo=True)
+                control_plane.put(io.StringIO(config_new), '/etc/kubernetes/audit-on-config.yaml', sudo=True)
 
-                control_plane['connection'].sudo(f"kubeadm init phase control-plane apiserver "
-                                             f"--config=/etc/kubernetes/audit-on-config.yaml && "
-                                             f"sudo sed -i 's/--bind-address=.*$/--bind-address="
-                                             f"{control_plane['internal_address']}/' "
-                                             f"/etc/kubernetes/manifests/kube-apiserver.yaml")
+                control_plane.sudo(
+                    f"kubeadm init phase control-plane apiserver "
+                    f"--config=/etc/kubernetes/audit-on-config.yaml && "
+                    f"sudo sed -i 's/--bind-address=.*$/--bind-address="
+                    f"{node_config['internal_address']}/' "
+                    f"/etc/kubernetes/manifests/kube-apiserver.yaml")
             else:
                 # we need InitConfiguration in audit-on-config.yaml file to take into account kubeadm patch for apiserver
                 init_config = {
                     'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
                     'kind': 'InitConfiguration',
                     'localAPIEndpoint': {
-                        'advertiseAddress': control_plane['internal_address']
+                        'advertiseAddress': node_config['internal_address']
                     },
                     'patches': {
                         'directory': '/etc/kubernetes/patches'
                     }
                 }
 
                 config_new = config_new + "---\n" + yaml.dump(init_config, default_flow_style=False)
 
-                control_plane['connection'].put(io.StringIO(config_new), '/etc/kubernetes/audit-on-config.yaml', sudo=True)
+                control_plane.put(io.StringIO(config_new), '/etc/kubernetes/audit-on-config.yaml', sudo=True)
 
                 kubernetes.create_kubeadm_patches_for_node(cluster, control_plane)
 
-                control_plane['connection'].sudo(f"kubeadm init phase control-plane apiserver "
-                                             f"--config=/etc/kubernetes/audit-on-config.yaml ")
+                control_plane.sudo(f"kubeadm init phase control-plane apiserver "
+                                   f"--config=/etc/kubernetes/audit-on-config.yaml ")
 
             if cluster.inventory['services']['cri']['containerRuntime'] == 'containerd':
-                control_plane['connection'].call(utils.wait_command_successful,
-                                                 command="crictl rm -f $(sudo crictl ps --name kube-apiserver -q)")
+                control_plane.call(utils.wait_command_successful,
+                                   command="crictl rm -f $(sudo crictl ps --name kube-apiserver -q)")
             else:
-                control_plane['connection'].call(utils.wait_command_successful,
-                                                 command="docker stop $(sudo docker ps -q -f 'name=k8s_kube-apiserver'"
-                                                         " | awk '{print $1}')")
-            control_plane['connection'].call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
-            control_plane['connection'].sudo("kubeadm init phase upload-config kubeadm "
-                                             "--config=/etc/kubernetes/audit-on-config.yaml")
+                control_plane.call(utils.wait_command_successful,
+                                   command="docker stop $(sudo docker ps -q -f 'name=k8s_kube-apiserver'"
+                                           " | awk '{print $1}')")
+            control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
+            control_plane.sudo("kubeadm init phase upload-config kubeadm "
+                               "--config=/etc/kubernetes/audit-on-config.yaml")
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_dns_hostname(group: NodeGroup):
-    cluster = group.cluster
-    with RemoteExecutor(cluster):
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            cluster.log.debug("Changing hostname '%s' = '%s'" % (node["connect_to"], node["name"]))
-            node["connection"].sudo("hostnamectl set-hostname %s" % node["name"])
+    cluster: KubernetesCluster = group.cluster
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            cluster.log.debug("Changing hostname '%s' = '%s'" % (node.get_host(), node.get_node_name()))
+            node.sudo("hostnamectl set-hostname %s" % node.get_node_name())
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_dns_resolv_conf(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     if cluster.inventory["services"].get("resolv.conf") is None:
         cluster.log.debug("Skipped - resolv.conf section not defined in config file")
         return
 
     system.update_resolv_conf(group, config=cluster.inventory["services"].get("resolv.conf"))
     cluster.log.debug(group.sudo("ls -la /etc/resolv.conf; sudo lsattr /etc/resolv.conf"))
 
 
-def system_prepare_dns_etc_hosts(cluster):
-    config = system.generate_etc_hosts_config(cluster.inventory, cluster, 'etc_hosts')
-    config += system.generate_etc_hosts_config(cluster.inventory, cluster, 'etc_hosts_generated')
+def system_prepare_dns_etc_hosts(cluster: KubernetesCluster):
+    config = system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts')
+    config += system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts_generated')
 
     utils.dump_file(cluster, config, 'etc_hosts')
     cluster.log.debug("\nUploading...")
 
     group = cluster.nodes['all'].get_final_nodes()
 
     system.update_etc_hosts(group, config=config)
     cluster.log.debug(group.sudo("ls -la /etc/hosts"))
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_package_manager_configure(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     repositories = cluster.inventory['services']['packages']['package_manager'].get("repositories")
     if not repositories:
         cluster.log.debug("Skipped - no repositories defined for configuration")
         return
 
-    group.call_batch([
-        packages.backup_repo,
-        packages.add_repo
-    ], **{
-        "kubemarine.packages.add_repo": {
-            "repo_data": repositories,
-            "repo_filename": "predefined"
-        }
-    })
+    group.call(packages.backup_repo)
+    group.call(packages.add_repo, repo_data=repositories)
 
     cluster.log.debug("Nodes contain the following repositories:")
     cluster.log.debug(packages.ls_repofiles(group))
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_package_manager_manage_packages(group: NodeGroup):
     group.call_batch([
         manage_mandatory_packages,
         manage_custom_packages
     ])
 
 
-def manage_mandatory_packages(group: NodeGroup):
-    cluster = group.cluster
+def manage_mandatory_packages(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
 
-    with RemoteExecutor(cluster) as exe:
-        for node in group.get_ordered_members_list():
-            pkgs = []
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            pkgs: List[str] = []
             for package in cluster.inventory["services"]["packages"]['mandatory'].keys():
                 hosts_to_packages = packages.get_association_hosts_to_packages(node, cluster.inventory, package)
                 pkgs.extend(next(iter(hosts_to_packages.values()), []))
 
             if pkgs:
                 cluster.log.debug(f"Installing {pkgs} on {node.get_node_name()!r}")
-                packages.install(node, pkgs)
+                packages.install(node, include=pkgs, callback=collector)
 
-    return exe.get_merged_result()
+    return collector.result
 
 
-def manage_custom_packages(group: NodeGroup):
-    cluster = group.cluster
-    batch_tasks = []
-    batch_parameters = {}
+def manage_custom_packages(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
 
+    batch_results: Dict[str, RunnersGroupResult] = {}
     packages_section = cluster.inventory["services"].get("packages", {})
     if packages_section.get("remove", {}).get("include"):
-        batch_tasks.append(packages.remove)
-        batch_parameters["kubemarine.packages.remove"] = {
-            "include": packages_section['remove']['include'],
-            "exclude": packages_section['remove'].get('exclude')
-        }
+        cluster.log.debug("Running kubemarine.packages.remove: ")
+        remove = packages_section['remove']
+        batch_results['remove'] = results = packages.remove(
+            group, include=remove['include'], exclude=remove.get('exclude'))
+        cluster.log.debug(results)
 
     if packages_section.get("install", {}).get("include"):
-        batch_tasks.append(packages.install)
-        batch_parameters["kubemarine.packages.install"] = {
-            "include": packages_section['install']['include'],
-            "exclude": packages_section['install'].get('exclude')
-        }
+        cluster.log.debug("Running kubemarine.packages.install: ")
+        install = packages_section['install']
+        batch_results['install'] = results = packages.install(
+            group, include=install['include'], exclude=install.get('exclude'))
+        cluster.log.debug(results)
 
     if packages_section.get("upgrade", {}).get("include"):
-        batch_tasks.append(packages.upgrade)
-        batch_parameters["kubemarine.packages.upgrade"] = {
-            "include": packages_section['upgrade']['include'],
-            "exclude": packages_section['upgrade'].get('exclude')
-        }
+        cluster.log.debug("Running kubemarine.packages.upgrade: ")
+        upgrade = packages_section['upgrade']
+        batch_results['upgrade'] = results = packages.upgrade(
+            group, include=upgrade['include'], exclude=upgrade.get('exclude'))
+        cluster.log.debug(results)
 
-    if not batch_tasks:
+    if not batch_results:
         cluster.log.debug("Skipped - no packages configuration defined in config file")
-        return
-
-    try:
-        batch_results = group.call_batch(batch_tasks, **batch_parameters)
-    except fabric.group.GroupException:
-        cluster.log.verbose('Exception occurred! Trying to handle is there anything updated or not...')
-        # todo develop cases when we can continue even if exception occurs
-        raise
+        return None
 
     any_changes_found = False
     for action, results in batch_results.items():
         cluster.log.verbose('Verifying packages changes after \'%s\' action...' % action)
-        for conn, result in results.items():
-            node = cluster.make_group([conn])
+        for host, result in results.items():
+            node = cluster.make_group([host])
             if not packages.no_changes_found(node, action, result):
-                cluster.log.verbose('Packages changed at %s' % conn.host)
+                cluster.log.verbose('Packages changed at %s' % host)
                 any_changes_found = True
 
     if any_changes_found:
         cluster.log.verbose('Packages changed, scheduling nodes restart...')
         cluster.schedule_cumulative_point(system.reboot_nodes)
     else:
         cluster.log.verbose('No packages changed, nodes restart will not be scheduled')
 
+    return None
+
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
 def system_cri_install(group: NodeGroup):
     """
     Task which is used to install CRI. Could be skipped, if CRI already installed.
     """
     group.call(cri.install)
@@ -395,58 +387,58 @@
     Task which is used to configure CRI. Could be skipped, if CRI already configured.
     """
     group.call(cri.configure)
 
 
 @_applicable_for_new_nodes_with_roles('all')
 def system_prepare_thirdparties(group: NodeGroup):
-    cluster = group.cluster
+    cluster: KubernetesCluster = group.cluster
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
 
     group.call(thirdparties.install_all_thirparties)
 
 
 @_applicable_for_new_nodes_with_roles('balancer')
 def deploy_loadbalancer_haproxy_install(group: NodeGroup):
     group.call(haproxy.install)
 
 
-def deploy_loadbalancer_haproxy_configure(cluster):
+def deploy_loadbalancer_haproxy_configure(cluster: KubernetesCluster):
 
     if not cluster.inventory['services'].get('loadbalancer', {}) \
             .get('haproxy', {}).get('keep_configs_updated', True):
         cluster.log.debug('Skipped - haproxy balancers configs update manually disabled')
         return
 
     group = None
 
     if "balancer" in cluster.nodes:
 
         if cluster.context['initial_procedure'] != 'remove_node':
             group = cluster.nodes['balancer'].get_new_nodes_or_self()
 
-        if not cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_changed_nodes().is_empty():
+        if not cluster.make_group_from_roles(['control-plane', 'worker']).get_changed_nodes().is_empty():
             group = cluster.nodes['balancer'].get_final_nodes()
 
     if group is None or group.is_empty():
         cluster.log.debug('Skipped - no balancers to perform')
         return
 
-    with RemoteExecutor(cluster):
-        group.call_batch([
+    with group.new_executor() as exe:
+        exe.group.call_batch([
             haproxy.configure,
             haproxy.override_haproxy18,
         ])
 
     haproxy.restart(group)
 
 
-def deploy_loadbalancer_keepalived_install(cluster):
+def deploy_loadbalancer_keepalived_install(cluster: KubernetesCluster):
     group = None
     if 'vrrp_ips' in cluster.inventory and cluster.inventory['vrrp_ips']:
 
         group = cluster.nodes['keepalived']
 
         # if remove/add node, then reconfigure only new keepalives
         if cluster.context['initial_procedure'] != 'install':
@@ -462,15 +454,15 @@
         cluster.log.debug('Skipped - no VRRP IPs to perform')
         return
 
     # add_node will impact all keepalived
     group.call(keepalived.install)
 
 
-def deploy_loadbalancer_keepalived_configure(cluster):
+def deploy_loadbalancer_keepalived_configure(cluster: KubernetesCluster):
     group = None
     if 'vrrp_ips' in cluster.inventory and cluster.inventory['vrrp_ips']:
 
         group = cluster.nodes['keepalived'].get_final_nodes()
 
         # if remove/add node, then reconfigure only new keepalives
         if cluster.context['initial_procedure'] != 'install':
@@ -508,45 +500,44 @@
 def deploy_kubernetes_init(cluster: KubernetesCluster):
     cluster.nodes['control-plane'].call_batch([
         kubernetes.init_first_control_plane,
         kubernetes.join_other_control_planes
     ])
 
     if 'worker' in cluster.nodes:
-        cluster.nodes.get('worker').new_group(
-            apply_filter=lambda node: 'control-plane' not in node['roles']) \
+        cluster.nodes['worker'].exclude_group(cluster.nodes['control-plane']) \
             .call(kubernetes.init_workers)
 
     cluster.nodes['all'].call_batch([
         kubernetes.apply_labels,
         kubernetes.apply_taints
     ])
 
     kubernetes.schedule_running_nodes_report(cluster)
 
 
-def deploy_coredns(cluster):
+def deploy_coredns(cluster: KubernetesCluster):
     config = coredns.generate_configmap(cluster.inventory)
 
     cluster.log.debug('Applying patch...')
     cluster.log.debug(coredns.apply_patch(cluster))
 
     cluster.log.debug('Applying configmap...')
     cluster.log.debug(coredns.apply_configmap(cluster, config))
 
 
-def deploy_plugins(cluster):
+def deploy_plugins(cluster: KubernetesCluster):
     plugins.install(cluster)
 
 
-def deploy_accounts(cluster):
+def deploy_accounts(cluster: KubernetesCluster):
     kubernetes_accounts.install(cluster)
 
 
-def overview(cluster):
+def overview(cluster: KubernetesCluster):
     cluster.log.debug("Retrieving cluster status...")
     control_plane = cluster.nodes["control-plane"].get_final_nodes().get_first_member()
     cluster.log.debug("\nNAMESPACES:")
     control_plane.sudo("kubectl get namespaces", hide=False)
     cluster.log.debug("\nNODES:")
     control_plane.sudo("kubectl get nodes -o wide", hide=False)
     cluster.log.debug("\nPODS:")
@@ -651,15 +642,15 @@
     ]
 }
 
 
 class InstallAction(Action):
     def __init__(self):
         super().__init__('install')
-        self.target_version = None
+        self.target_version = "not supported"
 
     def run(self, res: DynamicResources):
         self.target_version = kubernetes.get_initial_kubernetes_version(res.raw_inventory())
         kubernetes.verify_supported_version(self.target_version, res.logger())
 
         flow.run_tasks(res, tasks, cumulative_points=cumulative_points)
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/manage_psp.py` & `kubemarine-0.19.0/kubemarine/procedures/manage_psp.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
+from typing import List
 
 from kubemarine import admission
 from kubemarine.core import flow
 from kubemarine.core.action import Action
 from kubemarine.core.resources import DynamicResources
 
 tasks = OrderedDict({
@@ -28,23 +29,23 @@
     "reconfigure_oob": admission.reconfigure_oob_task,
     "reconfigure_plugin": admission.reconfigure_plugin_task,
     "restart_pods": admission.restart_pods_task
 })
 
 
 class PSPAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('manage psp', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     cli_help = '''
     Script for managing psp on existing Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/manage_pss.py` & `kubemarine-0.19.0/kubemarine/procedures/manage_pss.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
+from typing import List
 
 from kubemarine import admission
 from kubemarine.core import flow
 from kubemarine.core.action import Action
 from kubemarine.core.resources import DynamicResources
 
 tasks = OrderedDict({
@@ -26,23 +27,23 @@
     "delete_default_pss": admission.delete_default_pss,
     "apply_default_pss": admission.apply_default_pss,
     "restart_pods": admission.restart_pods_task
 })
 
 
 class PSSAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('manage pss', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     cli_help = '''
     Script for managing pss on existing Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.19.0/kubemarine/procedures/migrate_cri.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,38 @@
 # limitations under the License.
 
 
 from collections import OrderedDict
 
 import io
 import uuid
+from typing import List, Callable
 
 from kubemarine import kubernetes, etcd, thirdparties, cri
-from kubemarine.core import flow, utils
+from kubemarine.core import flow
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 from kubemarine.cri import docker
 from kubemarine.procedures import install
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine import packages
 
 
-def enrich_inventory(inventory, cluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster):
     if cluster.context.get("initial_procedure") != "migrate_cri":
         return inventory
 
     os_family = cluster.get_os_family()
     if os_family in ('unknown', 'unsupported', 'multiple'):
         raise Exception("Migration of CRI is possible only for cluster "
                         "with all nodes having the same and supported OS family")
 
-    enrichment_functions = [
+    enrichment_functions: List[Callable[[KubernetesCluster, dict], dict]] = [
         _prepare_yum_repos,
         _prepare_packages,
         _configure_containerd_on_nodes,
         _prepare_crictl
     ]
     for enrichment_fn in enrichment_functions:
         cluster.log.verbose('Calling fn "%s"' % enrichment_fn.__qualname__)
@@ -117,184 +119,176 @@
     if inventory["services"]["cri"]["containerRuntime"] == cluster.procedure_inventory["cri"]["containerRuntime"]:
         raise Exception("You already have such cri or you should explicitly specify 'cri.containerRuntime: docker' in cluster.yaml")
 
     inventory = _merge_containerd(cluster, inventory)
     return inventory
 
 
-def _merge_containerd(cluster, inventory, finalization=False):
+def _merge_containerd(cluster: KubernetesCluster, inventory: dict, finalization=False):
     if not inventory["services"].get("cri", {}):
         inventory["services"]["cri"] = {}
 
     if inventory["services"]["cri"].get("dockerConfig", {}):
         del inventory["services"]["cri"]["dockerConfig"]
 
     default_merger.merge(inventory["services"]["cri"], cluster.procedure_inventory["cri"])
     return inventory
 
 
-def migrate_cri(cluster):
+def migrate_cri(cluster: KubernetesCluster):
     _migrate_cri(cluster, cluster.nodes["worker"].exclude_group(cluster.nodes["control-plane"])
-                 .get_ordered_members_list(provide_node_configs=True))
-    _migrate_cri(cluster, cluster.nodes["control-plane"].get_ordered_members_list(provide_node_configs=True))
+                 .get_ordered_members_list())
+    _migrate_cri(cluster, cluster.nodes["control-plane"].get_ordered_members_list())
 
 
-def _migrate_cri(cluster: KubernetesCluster, node_group: dict):
+def _migrate_cri(cluster: KubernetesCluster, node_group: List[NodeGroup]):
     """
     Migrate CRI from docker to already installed containerd.
     This method works node-by-node, configuring kubelet to use containerd.
     :param cluster: main object describing a cluster
     :param node_group: group of nodes to migrate
     """
 
     for node in node_group:
-        if "control-plane" in node["roles"]:
+        node_config = node.get_config()
+        node_name = node.get_node_name()
+        is_control_plane = "control-plane" in node_config["roles"]
+        if is_control_plane:
             control_plane = node
         else:
-            control_plane = cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
+            control_plane = cluster.nodes["control-plane"].get_first_member()
 
-        cluster.log.debug(f'Updating thirdparties for node "{node["connect_to"]}..."')
-        thirdparties.install_all_thirparties(node["connection"])
+        cluster.log.debug(f'Updating thirdparties for node "{node_name}"...')
+        thirdparties.install_all_thirparties(node)
 
         version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
-        cluster.log.debug("Migrating \"%s\"..." % node["name"])
-        drain_cmd = kubernetes.prepare_drain_command(cluster, node['name'], disable_eviction=True)
-        control_plane["connection"].sudo(drain_cmd, is_async=False, hide=False)
+        cluster.log.debug("Migrating \"%s\"..." % node_name)
+        drain_cmd = kubernetes.prepare_drain_command(cluster, node_name, disable_eviction=True)
+        control_plane.sudo(drain_cmd, hide=False)
 
         kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
-        kubeadm_flags = node["connection"].sudo(f"cat {kubeadm_flags_file}",
-                                                is_async=False).get_simple_out()
+        kubeadm_flags = node.sudo(f"cat {kubeadm_flags_file}").get_simple_out()
 
         #Removing the --network-plugin=cni switch after the cri migration procedure that was used to run Docker on the cluster.
         #Support for this key has been removed in kubernetes 1.24.
         if kubeadm_flags.find('--network-plugin=cni') != -1:
             kubeadm_flags = kubeadm_flags.replace('--network-plugin=cni', '')
 
         kubeadm_flags = edit_config(kubeadm_flags)
 
-        node["connection"].put(io.StringIO(kubeadm_flags), kubeadm_flags_file, backup=True, sudo=True)
+        node.put(io.StringIO(kubeadm_flags), kubeadm_flags_file, backup=True, sudo=True)
 
-        node["connection"].sudo("systemctl stop kubelet")
-        docker.prune(node["connection"])
+        node.sudo("systemctl stop kubelet")
+        docker.prune(node)
 
-        docker_associations = cluster.get_associations_for_node(node['connect_to'], 'docker')
-        node["connection"].sudo(f"systemctl disable {docker_associations['service_name']} --now; "
-                                 "sudo sh -c 'rm -rf /var/lib/docker/*'")
+        docker_associations = cluster.get_associations_for_node(node.get_host(), 'docker')
+        node.sudo(f"systemctl disable {docker_associations['service_name']} --now; "
+                  "sudo sh -c 'rm -rf /var/lib/docker/*'")
 
         cluster.log.debug('Reinstalling CRI...')
-        cri.install(node["connection"])
-        cri.configure(node["connection"])
+        cri.install(node)
+        cri.configure(node)
 
-        cluster.log.debug(f'CRI configured! Restoring pods on node "{node["connect_to"]}"')
+        cluster.log.debug(f'CRI configured! Restoring pods on node "{node_name}"')
 
         # if there is a disk for docker in "/etc/fstab", then use this disk for containerd
-        docker_disk_result = node["connection"].sudo("cat /etc/fstab | grep ' /var/lib/docker '", warn=True)
+        docker_disk_result = node.sudo("cat /etc/fstab | grep ' /var/lib/docker '", warn=True)
         docker_disk = list(docker_disk_result.values())[0].stdout.strip()
         if docker_disk:
-            node['connection'].sudo("umount /var/lib/docker && "
-                                    "sudo sed -i 's/ \/var\/lib\/docker / \/var\/lib\/containerd /' /etc/fstab && "
-                                    "sudo sh -c 'rm -rf /var/lib/containerd/*' && "
-                                    "sudo mount -a && "
-                                    "sudo systemctl restart containerd")
+            node.sudo(
+                "umount /var/lib/docker && "
+                "sudo sed -i 's/ \/var\/lib\/docker / \/var\/lib\/containerd /' /etc/fstab && "
+                "sudo sh -c 'rm -rf /var/lib/containerd/*' && "
+                "sudo mount -a && "
+                "sudo systemctl restart containerd")
 
         # flushing iptables to delete old cri's rules,
         # existence of those rules could lead to services unreachable
-        node["connection"].sudo("sudo iptables -t nat -F && "
-                                "sudo iptables -t raw -F && "
-                                "sudo iptables -t filter -F && "
-                                # hotfix for Ubuntu 22.04
-                                "sudo systemctl stop kubepods-burstable.slice || true && "
-                                "sudo systemctl restart containerd && "
-                                # start kubelet
-                                "sudo systemctl restart kubelet")
+        node.sudo(
+            "sudo iptables -t nat -F && "
+            "sudo iptables -t raw -F && "
+            "sudo iptables -t filter -F && "
+            # hotfix for Ubuntu 22.04
+            "sudo systemctl stop kubepods-burstable.slice || true && "
+            "sudo systemctl restart containerd && "
+            # start kubelet
+            "sudo systemctl restart kubelet")
 
-        if "control-plane" in node["roles"]:
-            kubernetes.wait_uncordon(node["connection"])
+        if is_control_plane:
+            kubernetes.wait_uncordon(node)
         else:
-            control_plane["connection"].sudo(f"kubectl uncordon {node['name']}", is_async=False, hide=False)
+            control_plane.sudo(f"kubectl uncordon {node_name}", hide=False)
 
-        if "control-plane" in node["roles"]:
+        if is_control_plane:
             # hotfix for Ubuntu 22.04 and Kubernetes v1.21.2
             if version == "v1.21.2":
-                node['connection'].sudo("sleep 30 && "
-                                        "sudo kubectl -n kube-system  delete pod "
-                                        "$(sudo kubectl -n kube-system get pod --field-selector='status.phase=Pending' | "
-                                        "grep 'kube-proxy' | awk '{ print $1 }') || true")
-            kubernetes.wait_for_any_pods(cluster, node["connection"], apply_filter=node["name"])
+                node.sudo(
+                    "sleep 30 && "
+                    "sudo kubectl -n kube-system  delete pod "
+                    "$(sudo kubectl -n kube-system get pod --field-selector='status.phase=Pending' | "
+                    "grep 'kube-proxy' | awk '{ print $1 }') || true")
+            kubernetes.wait_for_any_pods(cluster, node, apply_filter=node_name)
             # check ETCD health
-            etcd.wait_for_health(cluster, node["connection"])
+            etcd.wait_for_health(cluster, node)
 
         packages_list = []
         for package_name in docker_associations['package_name']:
             if not package_name.startswith('containerd'):
                 packages_list.append(package_name)
         cluster.log.warning("The following packages will be removed: %s" % packages_list)
         if packages_list:
-            packages.remove(node["connection"], include=packages_list, warn=True, hide=False)
+            packages.remove(node, include=packages_list, warn=True, hide=False)
 
         # change annotation for cri-socket
-        control_plane["connection"].sudo(f"sudo kubectl annotate node {node['name']} "
-                                  f"--overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock",
-                                  is_async=False, hide=True)
+        control_plane.sudo(f"sudo kubectl annotate node {node_name} "
+                           f"--overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock")
 
         # delete docker socket
-        node["connection"].sudo("rm -rf /var/run/docker.sock", hide=False)
+        node.sudo("rm -rf /var/run/docker.sock", hide=False)
 
 
-def release_calico_leaked_ips(cluster):
+def release_calico_leaked_ips(cluster: KubernetesCluster):
     """
     During drain command we ignore daemon sets, as result this such pods as ingress-nginx-controller arent't deleted before migration.
     For this reason their ips can stay in calico ipam despite they aren't used. You can check this, if you run "calicoctl ipam check --show-problem-ips" right after apply_new_cri task.
     Those ips are cleaned by calico garbage collector, but it can take about 20 minutes.
     This task releases problem ips with force.
     """
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     cluster.log.debug("Getting leaked ips...")
     random_report_name = "/tmp/%s.json" % uuid.uuid4().hex
-    result = first_control_plane.sudo(f"calicoctl ipam check --show-problem-ips -o {random_report_name} | grep 'leaked' || true", is_async=False, hide=False)
+    result = first_control_plane.sudo(f"calicoctl ipam check --show-problem-ips -o {random_report_name} | grep 'leaked' || true", hide=False)
     leaked_ips = result.get_simple_out()
     leaked_ips_count = leaked_ips.count('leaked')
     cluster.log.debug(f"Found {leaked_ips_count} leaked ips")
     if leaked_ips_count != 0:
-        first_control_plane.sudo(f"calicoctl ipam release --from-report={random_report_name} --force", is_async=False, hide=False)
+        first_control_plane.sudo(f"calicoctl ipam release --from-report={random_report_name} --force", hide=False)
         cluster.log.debug("Leaked ips was released")
-    first_control_plane.sudo(f"rm {random_report_name}", is_async=False, hide=False)
-    
+    first_control_plane.sudo(f"rm {random_report_name}", hide=False)
 
-def edit_config(kubeadm_flags):
-    kubeadm_flags = _config_changer(kubeadm_flags, "--container-runtime=remote")
-    return _config_changer(kubeadm_flags,
-                           "--container-runtime-endpoint=unix:///run/containerd/containerd.sock")
 
+def edit_config(kubeadm_flags: str):
+    kubeadm_flags = kubernetes._config_changer(kubeadm_flags, "--container-runtime=remote")
+    return kubernetes._config_changer(kubeadm_flags,
+                           "--container-runtime-endpoint=unix:///run/containerd/containerd.sock")
 
-def _config_changer(config, word):
-    equal_pos = word.find("=") + 1
-    param_begin_pos = config.find(word[:equal_pos])
-    if param_begin_pos != -1:
-        param_end_pos = config[param_begin_pos:].find(" ")
-        if param_end_pos == -1:
-            return config[:param_begin_pos] + word + "\""
-        return config[:param_begin_pos] + word + config[param_end_pos + param_begin_pos:]
-    else:
-        param_end_pos = config.rfind("\"")
-        return config[:param_end_pos] + " " + word[:] + "\""
 
+def migrate_cri_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
 
-def migrate_cri_finalize_inventory(cluster, inventory_to_finalize):
     if cluster.context.get("initial_procedure") != "migrate_cri":
         return inventory_to_finalize
-    finalize_functions = [
+    finalize_functions: List[Callable[[KubernetesCluster, dict, bool], dict]] = [
         _prepare_yum_repos,
         _prepare_packages,
         _prepare_crictl,
         _merge_containerd
     ]
     for finalize_fn in finalize_functions:
         cluster.log.verbose('Calling fn "%s"' % finalize_fn.__qualname__)
-        inventory_to_finalize = finalize_fn(cluster, inventory_to_finalize, finalization=True)
+        inventory_to_finalize = finalize_fn(cluster, inventory_to_finalize, True)
 
     return inventory_to_finalize
 
 
 tasks = OrderedDict({
     "add_repos": install.system_prepare_package_manager_configure,
     "apply_new_cri": migrate_cri,
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.19.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import argparse
 import re
 from abc import ABC, abstractmethod
 from textwrap import dedent
-from typing import List
+from typing import List, Union
 
 import yaml
 
 import kubemarine.patches
 from kubemarine import kubernetes, plugins, cri, packages, etcd, thirdparties, haproxy, keepalived
 from kubemarine.core import flow, static, utils, errors
 from kubemarine.core.action import Action
@@ -27,69 +28,69 @@
 from kubemarine.core.patch import Patch, _SoftwareUpgradePatch
 from kubemarine.core.resources import DynamicResources
 
 SOFTWARE_UPGRADE_PATH = utils.get_internal_resource_path("patches/software_upgrade.yaml")
 
 
 class SoftwareUpgradeAction(Action, ABC):
-    def __init__(self, software_name: str, k8s_versions: List[str]):
+    def __init__(self, software_name: str, k8s_versions: List[str]) -> None:
         super().__init__(f'Upgrade {software_name}')
         self.software_name = software_name
         self.k8s_versions = k8s_versions
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         # We should not call DynamicResources.cluster() and should only access the raw inventory,
         # because otherwise enrichment will start with probably not relevant validation.
         version = kubernetes.get_initial_kubernetes_version(res.raw_inventory())
         if version not in self.k8s_versions:
             res.logger().info(f"Patch is not relevant for Kubernetes {version}")
             return
 
         self.specific_run(res)
         res.make_final_inventory()
 
     @abstractmethod
-    def specific_run(self, res: DynamicResources):
+    def specific_run(self, res: DynamicResources) -> None:
         pass
 
 
 class ThirdpartyUpgradeAction(SoftwareUpgradeAction):
-    def __init__(self, software_name: str, k8s_versions: List[str]):
+    def __init__(self, software_name: str, k8s_versions: List[str]) -> None:
         super().__init__(software_name, k8s_versions)
         self._destination = thirdparties.get_thirdparty_destination(self.software_name)
 
-    def specific_run(self, res: DynamicResources):
+    def specific_run(self, res: DynamicResources) -> None:
         logger = res.logger()
         cluster = res.cluster()
         if self._destination not in cluster.inventory['services']['thirdparties']:
             version = kubernetes.get_initial_kubernetes_version(cluster.inventory)
             cri_impl = cri.get_initial_cri_impl(cluster.inventory)
             logger.info(f"Patch is not relevant for Kubernetes {version}, based on {cri_impl}")
             return
 
         self.recreate_inventory = True
         logger.info(f"Reinstalling third-party {self._destination!r}")
         self._run(cluster)
 
-    def _run(self, cluster: KubernetesCluster):
+    def _run(self, cluster: KubernetesCluster) -> None:
         thirdparties.install_thirdparty(cluster.nodes['all'], self._destination)
 
     def prepare_context(self, context: dict) -> None:
         context['upgrading_thirdparty'] = self._destination
 
     def reset_context(self, context: dict) -> None:
         del context['upgrading_thirdparty']
 
 
 class CriUpgradeAction(Action):
-    def __init__(self, upgrade_config: dict):
+    def __init__(self, upgrade_config: dict) -> None:
         super().__init__(f'Upgrade CRI')
         self.upgrade_config = upgrade_config
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         # Access only to raw inventory to prepare context
         cri_impl = cri.get_initial_cri_impl(res.raw_inventory())
         res.context['upgrading_package'] = cri_impl
 
         if not self.associations_changed(res):
             return
 
@@ -103,42 +104,42 @@
         self._run(cluster)
 
         res.make_final_inventory()
 
     def reset_context(self, context: dict) -> None:
         del context['upgrading_package']
 
-    def _run(self, cluster: KubernetesCluster):
+    def _run(self, cluster: KubernetesCluster) -> None:
         if 'worker' in cluster.nodes:
             self.upgrade_cri(cluster.nodes["worker"].exclude_group(cluster.nodes["control-plane"]), workers=True)
         self.upgrade_cri(cluster.nodes["control-plane"], workers=False)
 
-    def upgrade_cri(self, group: NodeGroup, workers: bool):
-        cluster = group.cluster
+    def upgrade_cri(self, group: NodeGroup, workers: bool) -> None:
+        cluster: KubernetesCluster = group.cluster
 
         drain_timeout = cluster.procedure_inventory.get('drain_timeout')
         grace_period = cluster.procedure_inventory.get('grace_period')
         disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
 
         for node in group.get_ordered_members_list():
             node_name = node.get_node_name()
             control_plane = node
             if workers:
                 control_plane = cluster.nodes["control-plane"].get_first_member()
 
             drain_cmd = kubernetes.prepare_drain_command(
                 cluster, node_name,
                 disable_eviction=disable_eviction, drain_timeout=drain_timeout, grace_period=grace_period)
-            control_plane.sudo(drain_cmd, is_async=False, hide=False)
+            control_plane.sudo(drain_cmd, hide=False)
 
             kubernetes.upgrade_cri_if_required(node)
             node.sudo('systemctl restart kubelet')
 
             if workers:
-                control_plane.sudo(f"kubectl uncordon {node_name}", is_async=False, hide=False)
+                control_plane.sudo(f"kubectl uncordon {node_name}", hide=False)
             else:
                 kubernetes.wait_uncordon(node)
 
             if not workers:
                 kubernetes.wait_for_any_pods(cluster, node, apply_filter=node_name)
                 etcd.wait_for_health(cluster, node)
 
@@ -168,45 +169,45 @@
             res.logger().info(f"Patch is not relevant for Kubernetes {version}, "
                               f"based on {cri_impl} and {os_family!r} OS family")
 
         return changes_detected
 
 
 class BalancerUpgradeAction(Action):
-    def __init__(self, upgrade_config: dict, package_name: str):
+    def __init__(self, upgrade_config: dict, package_name: str) -> None:
         super().__init__(f'Upgrade {package_name}')
         self.upgrade_config = upgrade_config
         self.package_name = package_name
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         if not self.associations_changed(res):
             return
 
         # Only now the cluster is initialized and full enrichment is run.
         cluster = res.cluster()
         logger = res.logger()
         if self.package_name not in cluster.context['packages']['upgrade_required']:
             logger.info(f"Nothing has changed in associations of {self.package_name!r}. Upgrade is not required.")
             return
 
         role = 'balancer' if self.package_name == 'haproxy' else 'keepalived'
-        group = cluster.create_group_from_groups_nodes_names([role], [])
+        group = cluster.make_group_from_roles([role])
         if group.is_empty():
             logger.info(f"No nodes to install {self.package_name!r}.")
             return
 
         logger.info(f"Reinstalling {self.package_name} on nodes: {group.get_nodes_names()}")
         self.recreate_inventory = True
 
         self._run(group)
         res.make_final_inventory()
 
-    def _run(self, group: NodeGroup):
-        cluster = group.cluster
-        packages.install(group, cluster.get_package_association(self.package_name, 'package_name'))
+    def _run(self, group: NodeGroup) -> None:
+        cluster: KubernetesCluster = group.cluster
+        packages.install(group, include=cluster.get_package_association(self.package_name, 'package_name'))
         if self.package_name == 'haproxy':
             haproxy.restart(group)
         else:
             keepalived.restart(group)
 
     def associations_changed(self, res: DynamicResources) -> bool:
         """
@@ -216,55 +217,55 @@
         nodes_context = res.get_nodes_context()
         os_families = list({ctx['os']['family'] for ctx in nodes_context.values()})
         if len(os_families) != 1 or os_families[0] not in packages.get_associations_os_family_keys():
             raise errors.KME("KME0012")
         os_family = os_families[0]
         version_key = packages.get_compatibility_version_key(os_family)
 
-        changes_detected = self.upgrade_config['packages'][self.package_name][version_key]
+        changes_detected: Union[List[str], bool] = self.upgrade_config['packages'][self.package_name][version_key]
         if not changes_detected:
             res.logger().info(f"Patch is not relevant for {os_family!r} OS family")
 
-        return changes_detected
+        return bool(changes_detected)
 
     def prepare_context(self, context: dict) -> None:
         context['upgrading_package'] = self.package_name
 
     def reset_context(self, context: dict) -> None:
         del context['upgrading_package']
 
 
 class PluginUpgradeAction(SoftwareUpgradeAction):
-    def specific_run(self, res: DynamicResources):
+    def specific_run(self, res: DynamicResources) -> None:
         self.recreate_inventory = True
 
         cluster = res.cluster()
         # TODO despite that we are sure that the recommended version has changed,
         #  upgrade might still be not required if the effective configuration did not change.
         upgrade_candidates = {
             self.software_name: cluster.inventory['plugins'][self.software_name]
         }
         self._run(cluster, upgrade_candidates)
 
-    def _run(self, cluster: KubernetesCluster, upgrade_candidates: dict):
+    def _run(self, cluster: KubernetesCluster, upgrade_candidates: dict) -> None:
         plugins.install(cluster, upgrade_candidates)
 
     def prepare_context(self, context: dict) -> None:
         context['upgrading_plugin'] = self.software_name
         if self.software_name == 'calico':
             context['upgrading_thirdparty'] = thirdparties.get_thirdparty_destination('calicoctl')
 
     def reset_context(self, context: dict) -> None:
         del context['upgrading_plugin']
         if self.software_name == 'calico':
             del context['upgrading_thirdparty']
 
 
 class ThirdpartyUpgradePatch(_SoftwareUpgradePatch):
-    def __init__(self, thirdparty_name: str, k8s_versions: List[str]):
+    def __init__(self, thirdparty_name: str, k8s_versions: List[str]) -> None:
         super().__init__(f"upgrade_{thirdparty_name}")
         self.thirdparty_name = thirdparty_name
         self.k8s_versions = k8s_versions
 
     @property
     def action(self) -> Action:
         return ThirdpartyUpgradeAction(self.thirdparty_name, self.k8s_versions)
@@ -280,15 +281,15 @@
             Roughly equivalent to 'kubemarine install --tasks=prepare.thirdparties'
             provided that all third-parties except the {self.thirdparty_name!r} are already actual.
             """.rstrip()
         ).format(versions_list=versions_list)
 
 
 class CriUpgradePatch(_SoftwareUpgradePatch):
-    def __init__(self, upgrade_config: dict):
+    def __init__(self, upgrade_config: dict) -> None:
         super().__init__(f"upgrade_cri")
         self.upgrade_config = upgrade_config
 
     @property
     def action(self) -> Action:
         return CriUpgradeAction(self.upgrade_config)
 
@@ -301,15 +302,15 @@
             {SOFTWARE_UPGRADE_PATH}.
             Upgrade procedure is similar to 'kubemarine upgrade --tasks=kubernetes', but without the Kubernetes upgrade.
             """.rstrip()
         )
 
 
 class BalancerUpgradePatch(_SoftwareUpgradePatch):
-    def __init__(self, upgrade_config: dict, package_name: str):
+    def __init__(self, upgrade_config: dict, package_name: str) -> None:
         super().__init__(f"upgrade_{package_name}")
         self.upgrade_config = upgrade_config
         self.package_name = package_name
 
     @property
     def action(self) -> Action:
         return BalancerUpgradeAction(self.upgrade_config, self.package_name)
@@ -322,15 +323,15 @@
             Roughly equivalent to 'kubemarine install --tasks=deploy.loadbalancer.{self.package_name}.install',
             as if it is run in a clean environment.
             """.rstrip()
         )
 
 
 class PluginUpgradePatch(_SoftwareUpgradePatch):
-    def __init__(self, plugin_name: str, k8s_versions: List[str]):
+    def __init__(self, plugin_name: str, k8s_versions: List[str]) -> None:
         super().__init__(f"upgrade_{re.sub(r'-', '_', plugin_name)}")
         self.plugin_name = plugin_name
         self.k8s_versions = k8s_versions
 
     @property
     def action(self) -> Action:
         return PluginUpgradeAction(self.plugin_name, self.k8s_versions)
@@ -346,15 +347,16 @@
             Roughly equivalent to 'kubemarine install --tasks=deploy.plugins' with all plugins disabled except the {self.plugin_name!r}.
             """.rstrip()
         ).format(versions_list=versions_list)
 
 
 def load_upgrade_config() -> dict:
     with utils.open_internal(SOFTWARE_UPGRADE_PATH) as stream:
-        return yaml.safe_load(stream)
+        upgrade_config: dict = yaml.safe_load(stream)
+        return upgrade_config
 
 
 def resolve_upgrade_patches() -> List[_SoftwareUpgradePatch]:
     upgrade_config = load_upgrade_config()
 
     upgrade_patches: List[_SoftwareUpgradePatch] = []
 
@@ -377,38 +379,43 @@
     for package_name in ['haproxy', 'keepalived']:
         if any(upgrade_config['packages'][package_name].get(v_key)
                for v_key in ('version_rhel', 'version_rhel8', 'version_debian')):
             upgrade_patches.append(BalancerUpgradePatch(upgrade_config, package_name))
 
     default_plugins = static.DEFAULTS['plugins']
     plugins = list(default_plugins)
-    plugins.sort(key=lambda p: default_plugins[p]['installation']['priority'])
+    plugins.sort(key=get_default_plugin_prioriry)
     for plugin_name in plugins:
         k8s_versions = upgrade_config['plugins'][plugin_name]
         if k8s_versions:
             verify_allowed_kubernetes_versions(k8s_versions)
             upgrade_patches.append(PluginUpgradePatch(plugin_name, k8s_versions))
 
     return upgrade_patches
 
 
-def verify_allowed_kubernetes_versions(kubernetes_versions: List[str]):
+def get_default_plugin_prioriry(plugin: str) -> int:
+    priority: int = static.DEFAULTS['plugins'][plugin]['installation']['priority']
+    return priority
+
+
+def verify_allowed_kubernetes_versions(kubernetes_versions: List[str]) -> None:
     not_allowed_versions = set(kubernetes_versions) - set(static.KUBERNETES_VERSIONS['compatibility_map'])
     if not_allowed_versions:
         raise Exception(f"Kubernetes versions {', '.join(map(repr, not_allowed_versions))} are not allowed.")
 
 
 def load_patches() -> List[Patch]:
     patches = list(kubemarine.patches.patches)
     patches.extend(resolve_upgrade_patches())
     patches.sort(key=lambda p: p.priority())
     return patches
 
 
-def new_parser():
+def new_parser() -> argparse.ArgumentParser:
     cli_help = '''
     Script for automated update of the environment for the current version of Kubemarine.
 
     How to use:
 
     '''
 
@@ -430,15 +437,15 @@
 
     parser.add_argument('procedure_config', metavar='procedure_config',
                         type=str, help='config file for the procedure', nargs='?')
 
     return parser
 
 
-def run(context: dict):
+def run(context: dict) -> None:
     args = context['execution_arguments']
 
     patches = load_patches()
     patch_ids = [patch.identifier for patch in patches]
 
     if args['list']:
         if patch_ids:
@@ -488,15 +495,15 @@
     if not actions:
         print("No patches to apply")
         exit(0)
 
     flow.ActionsFlow(actions).run_flow(context)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     parser = new_parser()
     context = flow.create_context(parser, cli_arguments, procedure="migrate_kubemarine")
     run(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/reboot.py` & `kubemarine-0.19.0/kubemarine/procedures/reboot.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,57 +11,59 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
+from typing import List
 
 from kubemarine.core import flow
 from kubemarine.core.action import Action
+from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 from kubemarine import system
 
 
-def reboot(cluster):
+def reboot(cluster: KubernetesCluster) -> None:
     if cluster.context.get('initial_procedure') != 'reboot':
         raise ImportError('Invalid reboot.py usage, please use system.reboot_nodes')
 
     if not cluster.procedure_inventory.get("nodes"):
         cluster.log.verbose('No nodes defined in procedure: all nodes will be rebooted')
     else:
         cluster.log.verbose('There are nodes defined in procedure: only defined will be rebooted')
 
     nodes = []
 
     cluster.log.verbose('The following nodes will be rebooted:')
-    for node in cluster.procedure_inventory.get("nodes", cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True)):
+    for node in cluster.procedure_inventory.get("nodes", cluster.inventory['nodes']):
         nodes.append(node['name'])
         cluster.log.verbose('  - ' + node['name'])
 
     system.reboot_group(cluster.make_group_from_nodes(nodes),
                         try_graceful=cluster.procedure_inventory.get("graceful_reboot"))
 
 
 tasks = OrderedDict({
     "reboot": reboot,
     "overview": install.overview,
 })
 
 
 class RebootAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('reboot')
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
     Script for Kubernetes nodes graceful rebooting.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/remove_node.py` & `kubemarine-0.19.0/kubemarine/procedures/remove_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
+from typing import Optional
 
-from kubemarine import kubernetes, haproxy, keepalived, coredns
+from kubemarine import kubernetes, haproxy, keepalived
 from kubemarine.core import flow, summary
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 
 
-def _get_active_nodes(node_type: str, cluster: KubernetesCluster) -> NodeGroup:
+def _get_active_nodes(node_type: str, cluster: KubernetesCluster) -> Optional[NodeGroup]:
     all_nodes = None
     if cluster.nodes.get(node_type) is not None:
         all_nodes = cluster.nodes[node_type].get_nodes_for_removal()
     if all_nodes is None or all_nodes.is_empty():
         cluster.log.debug("Skipped - no %s to remove" % node_type)
-        return
+        return None
     active_nodes = all_nodes.get_online_nodes(True)
     disabled_nodes = all_nodes.exclude_group(active_nodes)
     if active_nodes.is_empty():
-        cluster.log.debug("Skipped - %s nodes are inactive: %s" % (node_type, ", ".join(disabled_nodes.nodes.keys())))
-        return
+        cluster.log.debug("Skipped - %s nodes are inactive: %s" % (node_type, ", ".join(disabled_nodes.nodes)))
+        return None
     if not disabled_nodes.is_empty():
         cluster.log.debug("Partly Skipped - several %s nodes are inactive: %s"
-                          % (node_type, ", ".join(disabled_nodes.nodes.keys())))
+                          % (node_type, ", ".join(disabled_nodes.nodes)))
     return active_nodes
 
 
 def loadbalancer_remove_haproxy(cluster: KubernetesCluster):
     nodes = _get_active_nodes("balancer", cluster)
     if nodes is None:
         return
@@ -54,15 +55,15 @@
     nodes = _get_active_nodes("keepalived", cluster)
     if nodes is None:
         return
     nodes.call(keepalived.disable)
 
 
 def remove_kubernetes_nodes(cluster: KubernetesCluster):
-    group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_nodes_for_removal()
+    group = cluster.make_group_from_roles(['control-plane', 'worker']).get_nodes_for_removal()
 
     if group.is_empty():
         cluster.log.debug("No kubernetes nodes to perform")
         return
 
     group.call(kubernetes.reset_installation_env)
     kubernetes.schedule_running_nodes_report(cluster)
@@ -83,15 +84,15 @@
             from kubemarine import keepalived
             hosts = keepalived.get_default_node_names(inventory_to_finalize)
 
         for host in hosts:
             host_name = host
             if isinstance(host_name, dict):
                 host_name = host['name']
-            if final_nodes.get_first_member(apply_filter={"name": host_name}) is None:
+            if not final_nodes.has_node(host_name):
                 hosts.remove(host)
         if not hosts:
             del inventory_to_finalize['vrrp_ips'][i]
         else:
             if inventory_to_finalize['vrrp_ips'][i].get('hosts', []):
                 inventory_to_finalize['vrrp_ips'][i]['hosts'] = hosts
 
@@ -100,15 +101,15 @@
     for i in range(size):
         for j, node in enumerate(inventory_to_finalize['nodes']):
             if nodes_for_removal.has_node(node["name"]):
                 del inventory_to_finalize['nodes'][j]
                 break
 
     if inventory_to_finalize['services'].get('kubeadm', {}).get('apiServer', {}).get('certSANs'):
-        for node in nodes_for_removal.get_ordered_members_list(provide_node_configs=True):
+        for node in nodes_for_removal.get_ordered_members_configs_list():
             hostnames = [node['name'], node['internal_address']]
             if node.get('address') is not None:
                 hostnames.append(node['address'])
             for name in hostnames:
                 if name in inventory_to_finalize['services']['kubeadm']['apiServer']['certSANs']:
                     inventory_to_finalize['services']['kubeadm']['apiServer']['certSANs'].remove(name)
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/restore.py` & `kubemarine-0.19.0/kubemarine/procedures/restore.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,28 @@
 import time
 from collections import OrderedDict
 import yaml
 
 from kubemarine.core import utils, flow, defaults
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install, backup
 from kubemarine import system, kubernetes, etcd
-from kubemarine.core.executor import RemoteExecutor
 
 
 def missing_or_empty(file):
     if not os.path.exists(file):
         return True
     content = utils.read_external(file)
     if re.search(r'^\s*$', content):
         return True
 
 
-def replace_config_from_backup_if_needed(procedure_inventory_filepath, config):
+def replace_config_from_backup_if_needed(procedure_inventory_filepath: str, config: str):
     if missing_or_empty(config):
         print('Config is missing or empty - retrieving config from backup archive...')
         with utils.open_external(procedure_inventory_filepath, 'r') as stream:
             procedure = yaml.safe_load(stream)
         backup_location = procedure.get("backup_location")
         if not backup_location:
             raise Exception('Backup location is not specified in procedure')
@@ -51,15 +49,15 @@
         print('Unpacking cluster.yaml...')
         with tarfile.open(backup_location, 'r:gz') as tar:
             member = tar.getmember('original_cluster.yaml')
             tar.makefile(member, config)
             tar.close()
 
 
-def unpack_data(cluster):
+def unpack_data(cluster: KubernetesCluster):
     backup_tmp_directory = backup.prepare_backup_tmpdir(cluster)
     backup_file_source = cluster.procedure_inventory.get('backup_location')
 
     if not backup_file_source:
         raise Exception('Backup source not specified in procedure')
 
     backup_file_source = utils.get_external_resource_path(backup_file_source)
@@ -85,15 +83,15 @@
     if not os.path.isfile(descriptor_filepath):
         raise FileNotFoundError('Descriptor not found in backup file')
 
     with utils.open_external(descriptor_filepath, 'r') as stream:
         cluster.context['backup_descriptor'] = yaml.safe_load(stream)
 
 
-def verify_backup_data(cluster):
+def verify_backup_data(cluster: KubernetesCluster):
     if not cluster.context['backup_descriptor'].get('kubernetes', {}).get('version'):
         cluster.log.debug('Not possible to verify Kubernetes version, because descriptor do not contain such information')
         return
 
     if cluster.context['backup_descriptor']['kubernetes']['version'] != cluster.inventory['services']['kubeadm']['kubernetesVersion']:
         cluster.log.warning('Installed kubernetes versions do not match version from backup')
         cluster.log.verbose('Cluster re-parse required')
@@ -103,15 +101,15 @@
             cluster.raw_inventory['services']['kubeadm'] = {}
         cluster.raw_inventory['services']['kubeadm']['kubernetesVersion'] = cluster.context['backup_descriptor']['kubernetes']['version']
         cluster._inventory = defaults.enrich_inventory(cluster, cluster.raw_inventory)
     else:
         cluster.log.debug('Kubernetes version from backup is correct')
 
 
-def stop_cluster(cluster):
+def stop_cluster(cluster: KubernetesCluster):
     cluster.log.debug('Stopping the existing cluster...')
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
     if cri_impl == "docker":
         result = cluster.nodes['control-plane'].sudo('systemctl stop kubelet; '
                                               'sudo docker kill $(sudo docker ps -q); '
                                               'sudo docker rm -f $(sudo docker ps -a -q); '
                                               'sudo docker ps -a; '
@@ -122,41 +120,42 @@
                                               'sudo crictl rm -fa; '
                                               'sudo crictl ps -a; '
                                               'sudo rm -rf /var/lib/etcd; '
                                               'sudo mkdir -p /var/lib/etcd', warn=True)
     cluster.log.verbose(result)
 
 
-def restore_thirdparties(cluster):
+def restore_thirdparties(cluster: KubernetesCluster):
     custom_thirdparties = cluster.procedure_inventory.get('restore_plan', {}).get('thirdparties', {})
     if custom_thirdparties:
         for name, value in custom_thirdparties.items():
             cluster.inventory['services']['thirdparties'][name]['source'] = value['source']
             if value.get('sha1'):
                 cluster.inventory['services']['thirdparties'][name]['sha1'] = value['sha1']
 
     install.system_prepare_thirdparties(cluster)
 
 
-def import_nodes(cluster):
-    for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
-        node['connection'].put(os.path.join(cluster.context['backup_tmpdir'], 'nodes_data', '%s.tar.gz' % node['name']),
-                               '/tmp/kubemarine-backup.tar.gz')
-        cluster.log.debug('Backup \'%s\' uploaded' % node['name'])
+def import_nodes(cluster: KubernetesCluster):
+    with cluster.nodes['all'].new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            node_name = node.get_node_name()
+            cluster.log.debug('Uploading backup for \'%s\'' % node_name)
+            node.put(os.path.join(cluster.context['backup_tmpdir'], 'nodes_data', '%s.tar.gz' % node_name),
+                     '/tmp/kubemarine-backup.tar.gz')
 
     cluster.log.debug('Unpacking backup...')
 
-    with RemoteExecutor(cluster) as exe:
-        for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
-            cmd = f"readlink /etc/resolv.conf ;" \
-                  f"if [ $? -ne 0 ]; then sudo chattr -i /etc/resolv.conf; sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite && sudo chattr +i /etc/resolv.conf; else sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite; fi "
-            node['connection'].sudo(cmd)
+    unpack_cmd = "sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite"
+    result = cluster.nodes['all'].sudo(
+        f"readlink /etc/resolv.conf ; "
+        f"if [ $? -ne 0 ]; then sudo chattr -i /etc/resolv.conf; {unpack_cmd} && sudo chattr +i /etc/resolv.conf; "
+        f"else {unpack_cmd}; fi ")
 
-    result = exe.get_last_results_str()
-    cluster.log.debug('%s',result)
+    cluster.log.debug(result)
 
 
 def import_etcd(cluster: KubernetesCluster):
     etcd_all_certificates = cluster.procedure_inventory.get('restore_plan', {}).get('etcd', {}).get('certificates', {})
     etcd_cert = etcd_all_certificates.get('cert', cluster.globals['etcd']['default_arguments']['cert'])
     etcd_key = etcd_all_certificates.get('key', cluster.globals['etcd']['default_arguments']['key'])
     etcd_cacert = etcd_all_certificates.get('cacert', cluster.globals['etcd']['default_arguments']['cacert'])
@@ -174,28 +173,28 @@
 
     cluster.log.debug('Uploading ETCD snapshot...')
     snap_name = '/var/lib/etcd/etcd-snapshot%s.db' % int(round(time.time() * 1000))
     cluster.nodes['control-plane'].put(os.path.join(cluster.context['backup_tmpdir'], 'etcd.db'), snap_name, sudo=True)
 
     initial_cluster_list = []
     initial_cluster_list_without_names = []
-    for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
+    for control_plane in cluster.nodes['control-plane'].get_ordered_members_configs_list():
         initial_cluster_list.append(control_plane['name'] + '=https://' + control_plane["internal_address"] + ":2380")
         initial_cluster_list_without_names.append(control_plane["internal_address"] + ":2379")
     initial_cluster = ','.join(initial_cluster_list)
 
     if "docker" == cluster.inventory['services']['cri']['containerRuntime']:
         cont_runtime = "docker"
     else:
         cont_runtime = "podman"
 
     etcd_instances = 0
-    for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
+    for control_plane in cluster.nodes['control-plane'].get_ordered_members_configs_list():
         cluster.log.debug('Restoring ETCD member ' + control_plane['name'])
-        control_plane_conn: NodeGroup = control_plane['connection']
+        control_plane_conn = cluster.make_group([control_plane['connect_to']])
         control_plane_conn.sudo(
             f'chmod 777 {snap_name} && '
             f'sudo ls -la {snap_name} && '
             f'sudo etcdctl snapshot restore {snap_name} '
             f'--name={control_plane["name"]} '
             f'--data-dir=/var/lib/etcd/snapshot '
             f'--initial-cluster={initial_cluster} '
@@ -248,15 +247,15 @@
             if expected_dbsize > real_dbsize:
                 raise Exception('ETCD member "%s" has invalid DB size' % item.get('endpoint'))
         cluster.log.debug('DB size "%s" is correct' % expected_dbsize)
     else:
         cluster.log.verbose('It is not possible to verify db size - descriptor do not contain such information')
 
 
-def reboot(cluster):
+def reboot(cluster: KubernetesCluster):
     system.reboot_group(cluster.nodes['all'], try_graceful=False)
     kubernetes.wait_for_nodes(cluster.nodes['control-plane'])
 
 
 tasks = OrderedDict({
     "prepare": {
         "unpack": unpack_data,
```

### Comparing `kubemarine-0.18.2/kubemarine/procedures/upgrade.py` & `kubemarine-0.19.0/kubemarine/procedures/upgrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,35 +23,36 @@
 import toml
 
 from kubemarine import kubernetes, plugins
 from kubemarine.core import flow
 from kubemarine.core import utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
+from kubemarine.core.group import CollectorCallback
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 
 
-def system_prepare_thirdparties(cluster):
+
+def system_prepare_thirdparties(cluster: KubernetesCluster):
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
 
     install.system_prepare_thirdparties(cluster)
 
 
-def prepull_images(cluster):
+def prepull_images(cluster: KubernetesCluster):
     cluster.log.debug("Prepulling Kubernetes images...")
     fix_cri_socket(cluster)
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
     upgrade_group.call(kubernetes.images_grouped_prepull)
 
 
-def kubernetes_upgrade(cluster):
+def kubernetes_upgrade(cluster: KubernetesCluster):
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
     grace_period = cluster.procedure_inventory.get('grace_period')
     disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
     drain_kwargs = {
         'disable_eviction': disable_eviction, 'drain_timeout': drain_timeout, 'grace_period': grace_period
@@ -68,15 +69,15 @@
     if cluster.nodes.get('worker', []):
         kubernetes.upgrade_workers(upgrade_group, cluster, **drain_kwargs)
 
     cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     cluster.context['cached_nodes_versions_cleaned'] = True
 
 
-def kubernetes_cleanup_nodes_versions(cluster):
+def kubernetes_cleanup_nodes_versions(cluster: KubernetesCluster):
     if not cluster.context.get('cached_nodes_versions_cleaned', False):
         cluster.log.verbose('Cached nodes versions required')
         cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     else:
         cluster.log.verbose('Cached nodes versions already cleaned')
     kubernetes_apply_taints(cluster)
 
@@ -85,15 +86,15 @@
     upgrade_version = cluster.context["upgrade_version"]
 
     packages = cluster.procedure_inventory.get(upgrade_version, {}).get("packages", {})
     if packages.get("install") is not None or packages.get("upgrade") is not None or packages.get("remove") is not None:
         install.manage_custom_packages(cluster.nodes['all'])
 
 
-def upgrade_plugins(cluster):
+def upgrade_plugins(cluster: KubernetesCluster):
     upgrade_version = cluster.context["upgrade_version"]
 
     # upgrade_candidates is a source of upgradeable plugins, not list of plugins to upgrade.
     # Some plugins from upgrade_candidates will not be upgraded, because they have "install: false"
     upgrade_candidates = {}
     defined_plugins = cluster.procedure_inventory.get(upgrade_version, {}).get("plugins", {}).keys()
     for plugin in chain(defined_plugins, plugins.oob_plugins):
@@ -133,25 +134,34 @@
                 if not isinstance(value, dict):
                     config_string += f"{toml.dumps({key: value})}"
             for key, value in containerd_config.items():
                 # next we process all "complex" `key: dict_value` pairs, representing named sections
                 if isinstance(value, dict):
                     config_string += f"\n[{key}]\n{toml.dumps(value)}"
             utils.dump_file(cluster, config_string, 'containerd-config.toml')
-            with RemoteExecutor(cluster) as exe:
-                for node in cluster.nodes['control-plane'].include_group(
-                        cluster.nodes.get('worker')).get_ordered_members_list(
-                        provide_node_configs=True):
-                    os_specific_associations = cluster.get_associations_for_node(node['connect_to'], 'containerd')
-                    node['connection'].put(StringIO(config_string), os_specific_associations['config_location'],
-                                           backup=True,
-                                           sudo=True, mkdir=True)
-                    node['connection'].sudo(f"sudo systemctl restart {os_specific_associations['service_name']} && "
-                                            f"systemctl status {os_specific_associations['service_name']}")
-            return exe.get_last_results_str()
+
+            kubernetes_nodes = cluster.make_group_from_roles(['control-plane', 'worker'])
+            collector = CollectorCallback(cluster)
+            for member_node in kubernetes_nodes.get_ordered_members_list():
+                kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
+                kubeadm_flags = member_node.sudo(f"cat {kubeadm_flags_file}").get_simple_out()
+                updated_kubeadm_flags = kubernetes._config_changer(kubeadm_flags, f"--pod-infra-container-image={sandbox}")
+                member_node.put(StringIO(updated_kubeadm_flags), kubeadm_flags_file, backup=True, sudo=True)
+
+            with kubernetes_nodes.new_executor() as exe:
+                for node in exe.group.get_ordered_members_list():
+                    os_specific_associations = cluster.get_associations_for_node(node.get_host(), 'containerd')
+                    node.put(StringIO(config_string), os_specific_associations['config_location'],
+                             backup=True, sudo=True, mkdir=True)
+                    node.sudo(
+                        f"sudo systemctl restart {os_specific_associations['service_name']} && "
+                        f"systemctl status {os_specific_associations['service_name']} && " 
+                        f"sudo systemctl restart kubelet",
+                        callback=collector)
+            return collector.result
 
 
 tasks = OrderedDict({
     "verify_upgrade_versions": kubernetes.verify_upgrade_versions,
     "thirdparties": system_prepare_thirdparties,
     "prepull_images": prepull_images,
     "configure_policy": install.system_prepare_policy,
@@ -163,21 +173,21 @@
     "overview": install.overview
 
 })
 
 
 class UpgradeFlow(flow.Flow):
     def __init__(self):
-        self.target_version = None
+        self.target_version = "not supported"
 
     def _run(self, resources: DynamicResources):
         logger = resources.logger()
 
         previous_version = kubernetes.get_initial_kubernetes_version(resources.raw_inventory())
-        upgrade_plan = resources.procedure_inventory().get('upgrade_plan')
+        upgrade_plan = resources.procedure_inventory()['upgrade_plan']
         upgrade_plan = verify_upgrade_plan(previous_version, upgrade_plan)
         logger.debug(f"Loaded upgrade plan: current ({previous_version}) ⭢ {' ⭢ '.join(upgrade_plan)}")
 
         self.target_version = upgrade_plan[-1]
         kubernetes.verify_supported_version(self.target_version, logger)
 
         args = resources.context['execution_arguments']
@@ -230,30 +240,29 @@
     for version in upgrade_plan:
         kubernetes.test_version_upgrade_possible(previous_version, version)
         previous_version = version
 
     return upgrade_plan
 
 
-def fix_cri_socket(cluster):
+def fix_cri_socket(cluster: KubernetesCluster):
     """
     This method fixs the issue with 'kubeadm.alpha.kubernetes.io/cri-socket' node annotation
     and delete the docker socket if it exists
     """
 
     if cluster.inventory["services"]["cri"]["containerRuntime"] == "containerd":
-        control_plane = cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
-        control_plane["connection"].sudo(f"sudo kubectl annotate nodes --all \
-                                     --overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock"
-                                         , is_async=False, hide=True)
+        control_plane = cluster.nodes["control-plane"].get_first_member()
+        control_plane.sudo(f"sudo kubectl annotate nodes --all "
+                           f"--overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock")
         upgrade_group = kubernetes.get_group_for_upgrade(cluster)
         upgrade_group.sudo("rm -rf /var/run/docker.sock")
 
 
-def kubernetes_apply_taints(cluster):
+def kubernetes_apply_taints(cluster: KubernetesCluster):
     # Apply taints after upgrade
     group = cluster.nodes['control-plane']
     kubernetes.apply_taints(group)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     apiVersion: kubelet.config.k8s.io/v1beta1
     kind: KubeletConfiguration
     readOnlyPort: 0
     enableDebuggingHandlers: true
     protectKernelDefaults: true
     podPidsLimit: 4096
     cgroupDriver: systemd
+    serializeImagePulls: false
   kubeadm_flags:
     ignorePreflightErrors: Port-6443,CoreDNSUnsupportedPlugins
   kubeadm:
     # for patches functionality we need v1beta3 which is available since k8s v1.22 only
     apiVersion: '{% if "v1.21" in services["kubeadm"]["kubernetesVersion"] %}kubeadm.k8s.io/v1beta2{% else %}kubeadm.k8s.io/v1beta3{% endif %}'
     kind: ClusterConfiguration
     kubernetesVersion: v1.26.3
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.19.0/kubemarine/resources/configurations/globals.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     - CreateContainerConfigError
 nodes:
   expect:
     kubernetes_version:
       timeout: 10
       retries: 30
   boot:
-    reboot_command: 'reboot 2>/dev/null >/dev/null &'
+    reboot_command: 'systemctl stop sshd && sudo reboot 2>/dev/null >/dev/null'
     defaults:
       delay_period: 5
   drain:
     timeout: 10
     grace_period: 60
   remove:
     check_active_timeout: 30
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-All files and directories inside kubemarine/patches directory should participate only in patching mechanism,
-and relate to the current Kubemarine version.
+# Check url availability script.
+# The script is for testing purpose only.
+# The first argv parameter is source. The second argv parameter is the timeout.
 
-The whole directory is automatically cleared and reset after new version of Kubemarine is released.
-"""
+import sys
 
-from typing import List
+major_version = sys.version_info.major
+if major_version == 3:
+    import urllib.request as urllib
+else:
+    import urllib2 as urllib  # type: ignore[import, no-redef]
 
-from kubemarine.core.patch import Patch
-
-patches: List[Patch] = [
-]
-"""
-List of patches that is sorted according to the Patch.priority() before execution.
-Patches that have the same priority, are executed in the declared order.
-"""
+try:
+    source = sys.argv[1]
+    timeout = int(sys.argv[2])
+    status_code = urllib.urlopen(source, timeout=timeout).getcode()
+    if status_code != 200:
+        sys.stderr.write("Error status code: %s" % status_code)
+        exit(1)
+except Exception as e:
+    sys.stderr.write(str(e))
+    exit(1)
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.19.0/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/psp/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.19.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/psp/default.yaml` & `kubemarine-0.19.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.19.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.19.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/reports/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/reports/check_report.css` & `kubemarine-0.19.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/backup.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8392857142857143%*

 * *Differences: {"'oneOf'": "[OrderedDict([('required', ['keyfile'])]), OrderedDict([('required', ['password'])])]",*

 * * "'required'": '{delete: [3]}'}*

```diff
@@ -1,14 +1,26 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "allOf": [
         {
             "$ref": "node_defaults.json#/definitions/SSHAccessCommonProperties"
         }
     ],
+    "oneOf": [
+        {
+            "required": [
+                "keyfile"
+            ]
+        },
+        {
+            "required": [
+                "password"
+            ]
+        }
+    ],
     "properties": {
         "address": {
             "description": "Gateway node's IP or hostname address for connection",
             "type": "string"
         },
         "name": {
             "description": "Gateway node name",
@@ -27,12 +39,11 @@
                 ]
             }
         ]
     },
     "required": [
         "name",
         "address",
-        "username",
-        "keyfile"
+        "username"
     ],
     "type": "object"
 }
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'definitions'": "{'SSHAccessCommonProperties': {'properties': {'password': OrderedDict([('type', "*

 * *                  "'string'), ('description', 'Password for SSH-access the remote "*

 * *                  "machine(s)')])}}, 'SSHAccessCommonPropertyNames': {'enum': {insert: [(1, "*

 * *                  "'password')]}}}"}*

```diff
@@ -63,24 +63,29 @@
                     "minimum": 1,
                     "type": "integer"
                 },
                 "keyfile": {
                     "description": "Absolute path to keyfile on local machine to access the remote machine(s)",
                     "type": "string"
                 },
+                "password": {
+                    "description": "Password for SSH-access the remote machine(s)",
+                    "type": "string"
+                },
                 "username": {
                     "default": "root",
                     "description": "Username for SSH-access the remote machine(s)",
                     "type": "string"
                 }
             }
         },
         "SSHAccessCommonPropertyNames": {
             "enum": [
                 "keyfile",
+                "password",
                 "username",
                 "connection_port",
                 "connection_timeout"
             ]
         }
     },
     "description": "Section to hold the parameters to be applied by default to each record in the nodes section",
```

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/restore.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.19.0/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.19.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.19.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.19.0/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/selinux.py` & `kubemarine-0.19.0/kubemarine/selinux.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import re
+from typing import Tuple, Optional, Dict, List
 
 from kubemarine import system
-from kubemarine.core import utils
-
+from kubemarine.core import utils, log
+from kubemarine.core.group import NodeGroup, RunnersGroupResult
 
 # Common regexp should support the following schemes:
 # SELinux status:                 enabled
 # SELinuxfs mount:                /selinux
 # Policy version:                 23
 
 # Commong regexp
@@ -58,77 +59,80 @@
 #
 # > keepalived_t
 # > something_else_t
 #
 permissive_types_regex = re.compile("Customized Permissive Types\\s*([\\w_\\s]*)\\s*", re.M)
 
 
-def get_expected_state(inventory):
-    return inventory['services']['kernel_security'].get('selinux', {}).get('state', 'enforcing')
+def get_expected_state(inventory: dict) -> str:
+    state: str = inventory['services']['kernel_security'].get('selinux', {}).get('state', 'enforcing')
+    return state
 
 
-def get_expected_policy(inventory):
-    return inventory['services']['kernel_security'].get('selinux', {}).get('policy', 'targeted')
+def get_expected_policy(inventory: dict) -> str:
+    policy: str = inventory['services']['kernel_security'].get('selinux', {}).get('policy', 'targeted')
+    return policy
 
 
-def get_expected_permissive(inventory):
-    return inventory['services']['kernel_security'].get('selinux', {}).get('permissive', [])
+def get_expected_permissive(inventory: dict) -> List[str]:
+    permissive: List[str] = inventory['services']['kernel_security'].get('selinux', {}).get('permissive', [])
+    return permissive
 
 
-def parse_selinux_status(log, stdout):
-    result = {}
+def parse_selinux_status(logger: log.EnhancedLogger, stdout: str) -> Dict[str, str]:
+    result: Dict[str, str] = {}
     if stdout is not None and stdout.strip() != '':
         for regex, key in parsed_names_map.items():
-            matches = re.findall(regex, stdout)
+            matches: List[str] = re.findall(regex, stdout)
             if matches:
                 result[key] = matches[0].strip()
-    log.verbose('Parsed status: %s' % result)
+    logger.verbose('Parsed status: %s' % result)
     return result
 
 
-def parse_selinux_permissive_types(log, stdout):
+def parse_selinux_permissive_types(logger: log.EnhancedLogger, stdout: str) -> List[str]:
     if stdout is None or stdout.strip() == '':
-        log.verbose('Permissive types pattern not found - presented stdout is empty')
+        logger.verbose('Permissive types pattern not found - presented stdout is empty')
         return []
 
-    matches = re.findall(permissive_types_regex, stdout)
+    matches: List[str] = re.findall(permissive_types_regex, stdout)
     if not matches:
-        log.verbose('Permissive types pattern not found')
+        logger.verbose('Permissive types pattern not found')
         return []
 
     types_string = matches[0]
     if types_string.strip() == '':
-        log.verbose('Permissive types pattern found, but value is empty')
+        logger.verbose('Permissive types pattern found, but value is empty')
         return []
 
     result = types_string.split('\n')
-    log.verbose('Permissive types parsed: %s' % result)
+    logger.verbose('Permissive types parsed: %s' % result)
     return result
 
 
-def get_selinux_status(group):
+def get_selinux_status(group: NodeGroup) -> Tuple[RunnersGroupResult, Dict[str, dict]]:
     log = group.cluster.log
 
     result = group.sudo("sestatus && sudo semanage permissive -l")
 
-    parsed_result = {}
-    for connection, node_result in result.items():
-        log.verbose('Parsing status for %s...' % connection.host)
-        parsed_result[connection] = parse_selinux_status(log, node_result.stdout)
-        parsed_result[connection]['permissive_types'] = parse_selinux_permissive_types(log, node_result.stdout)
+    parsed_result: Dict[str, dict] = {}
+    for host, node_result in result.items():
+        log.verbose('Parsing status for %s...' % host)
+        parsed_result[host] = parse_selinux_status(log, node_result.stdout)
+        parsed_result[host]['permissive_types'] = parse_selinux_permissive_types(log, node_result.stdout)
     log.verbose("Parsed remote sestatus summary:\n%s" % parsed_result)
     return result, parsed_result
 
 
-def is_config_valid(group, state=None, policy=None, permissive=None):
+def is_config_valid(group: NodeGroup, state: str = None, policy: str = None, permissive: List[str] = None) \
+        -> Tuple[bool, RunnersGroupResult, Dict[str, dict]]:
     log = group.cluster.log
 
     if group.get_nodes_os() == 'debian':
-        log.debug("Skipped - selinux is not supported on Ubuntu/Debian os family")
-        return
+        raise Exception("Selinux is not supported on Ubuntu/Debian os family")
 
     log.verbose('Verifying selinux configs...')
 
     if state is None:
         state = get_expected_state(group.cluster.inventory)
 
     if policy is None:
@@ -136,52 +140,52 @@
 
     if permissive is None:
         permissive = get_expected_permissive(group.cluster.inventory)
 
     result, parsed_result = get_selinux_status(group)
     valid = True
 
-    for connection, selinux_status in parsed_result.items():
+    for host, selinux_status in parsed_result.items():
 
         if selinux_status['status'] == 'disabled' and state == 'disabled':
             continue
 
         # for some different selinux versions some statuses may be absent
         # that is why such construction was made - when no status, then cause true
         if state != selinux_status.get('mode', state) or \
                 state != selinux_status.get('mode_from_file', state) or \
                 policy != selinux_status.get('policy_from_file', policy) or \
                 policy != selinux_status.get('policy', policy):
             valid = False
-            log.verbose('Selinux configs are not matched at %s' % connection.host)
+            log.verbose('Selinux configs are not matched at %s' % host)
             break
 
         if permissive:
             for permissive_type in permissive:
                 if permissive_type not in selinux_status['permissive_types']:
                     valid = False
                     log.verbose('Permissive type %s not found in types %s at %s '
-                                % (permissive_type, selinux_status['permissive_types'], connection.host))
+                                % (permissive_type, selinux_status['permissive_types'], host))
                     break
             # if no break was called in previous for loop, then else called and no break will be called in current loop
             else:
                 continue
             # if break was called in previous for loop, then do break in current loop
             break
 
     return valid, result, parsed_result
 
 
-def setup_selinux(group):
+def setup_selinux(group: NodeGroup) -> Optional[RunnersGroupResult]:
     log = group.cluster.log
 
     # this method handles cluster with multiple os, suppressing should be enabled
     if group.get_nodes_os() not in ['rhel', 'rhel8']:
         log.debug("Skipped - selinux is not supported on Ubuntu/Debian os family")
-        return
+        return None
 
     expected_state = get_expected_state(group.cluster.inventory)
     expected_policy = get_expected_policy(group.cluster.inventory)
     expected_permissive = get_expected_permissive(group.cluster.inventory)
 
     valid, result, parsed_result = is_config_valid(group,
                                                    state=expected_state,
@@ -205,7 +209,8 @@
         semanage_commands = semanage_commands + 'semanage permissive -a %s' % item
     log.verbose("The following command will be executed to configure permissive:\n%s" % semanage_commands)
 
     group.sudo(semanage_commands)
 
     group.cluster.schedule_cumulative_point(system.reboot_nodes)
     group.cluster.schedule_cumulative_point(system.verify_system)
+    return None
```

### Comparing `kubemarine-0.18.2/kubemarine/sysctl.py` & `kubemarine-0.19.0/kubemarine/sysctl.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 This module works with sysctl on remote systems.
 Using this module you can generate new sysctl configs, install and apply them.
 """
 
 import io
 
 from kubemarine.core import utils
-from kubemarine.core.group import NodeGroup, NodeGroupResult
+from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import NodeGroup, RunnersGroupResult
 
 
-def make_config(cluster):
+def make_config(cluster: KubernetesCluster) -> str:
     """
     Converts parameters from inventory['services']['sysctl'] to a string in the format of systcl.conf.
     """
     config = ""
     if cluster.inventory['services'].get('sysctl') is not None:
         for key, value in cluster.inventory['services']['sysctl'].items():
             if isinstance(value, str):
@@ -57,30 +58,30 @@
             if pid_max > 2**22:
                 raise Exception("Calculated 'pid_max' value = '%s' is greater than the maximum allowable '%s'"
                                 % (pid_max, 2**22))
             config += "%s = %s\n" % ("kernel.pid_max", pid_max)
     return config
 
 
-def configure(group: NodeGroup) -> NodeGroupResult:
+def configure(group: NodeGroup) -> RunnersGroupResult:
     """
     Generates and uploads sysctl configuration to the group.
     The configuration will be placed in sysctl daemon directory.
     """
     config = make_config(group.cluster)
     group.sudo('rm -f /etc/sysctl.d/98-*-sysctl.conf')
     utils.dump_file(group.cluster, config, '98-kubemarine-sysctl.conf')
     group.put(io.StringIO(config), '/etc/sysctl.d/98-kubemarine-sysctl.conf', backup=True, sudo=True)
     return group.sudo('ls -la /etc/sysctl.d/98-kubemarine-sysctl.conf')
 
 
-def reload(group: NodeGroup) -> NodeGroupResult:
+def reload(group: NodeGroup) -> RunnersGroupResult:
     """
     Reloads sysctl configuration in the specified group.
     """
     return group.sudo('sysctl -p /etc/sysctl.d/98-*-sysctl.conf')
 
 
-def get_pid_max(inventory):
-    max_pods = inventory["services"]["kubeadm_kubelet"].get("maxPods", 110)
-    pod_pids_limit = inventory["services"]["kubeadm_kubelet"].get("podPidsLimit", 4096)
+def get_pid_max(inventory: dict) -> int:
+    max_pods: int = inventory["services"]["kubeadm_kubelet"].get("maxPods", 110)
+    pod_pids_limit: int = inventory["services"]["kubeadm_kubelet"].get("podPidsLimit", 4096)
     return max_pods * pod_pids_limit + 2048
```

### Comparing `kubemarine-0.18.2/kubemarine/system.py` & `kubemarine-0.19.0/kubemarine/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,41 +14,44 @@
 
 import configparser
 import io
 import paramiko
 import re
 import socket
 import time
-from typing import Dict
+from typing import Dict, Tuple, Optional, List
 
 from dateutil.parser import parse
-import fabric
 from ordered_set import OrderedSet
 
 from kubemarine import selinux, kubernetes, apparmor
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.executor import RemoteExecutor
-from kubemarine.core.group import NodeGroupResult, NodeGroup
+from kubemarine.core.executor import RunnersResult, Token, GenericResult, Callback, RawExecutor
+from kubemarine.core.group import (
+    GenericGroupResult, RunnersGroupResult, GroupResultException,
+    NodeGroup, DeferredGroup, AbstractGroup, GROUP_RUN_TYPE, CollectorCallback
+)
 from kubemarine.core.annotations import restrict_empty_group
 
 ERROR_UNSUPPORTED_KERNEL_MODULES_VERSIONS_DETECTED = \
         "Kernel modules are not available for the current OS family"
 
-def verify_inventory(inventory, cluster):
+
+def verify_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
 
     if cluster.inventory['services']['ntp'].get('chrony', {}).get('servers') \
         and (cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('NTP') or
              cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('FallbackNTP')):
         raise Exception('chrony and timesyncd configured both at the same time')
 
     return inventory
 
 
-def enrich_etc_hosts(inventory, cluster):
+def enrich_etc_hosts(inventory: dict, cluster: KubernetesCluster) -> dict:
 # enrich only etc_hosts_generated object, etc_hosts remains as it is
 
     # if by chance cluster.yaml contains non empty etc_hosts_generated we have to reset it
     inventory['services']['etc_hosts_generated'] = {}
 
     control_plain = inventory['control_plain']['internal']
 
@@ -58,33 +61,33 @@
     control_plain_names = list(OrderedSet(control_plain_names))
     inventory['services']['etc_hosts_generated'][control_plain] = control_plain_names
 
     for node in cluster.inventory['nodes']:
         if 'remove_node' in node['roles']:
             continue
 
-        internal_node_ip_names = inventory['services']['etc_hosts_generated'].get(node['internal_address'], [])  
+        internal_node_ip_names: List[str] = inventory['services']['etc_hosts_generated'].get(node['internal_address'], [])
 
         internal_node_ip_names.append("%s.%s" % (node['name'], cluster.inventory['cluster_name']))
         internal_node_ip_names.append(node['name'])
         internal_node_ip_names = list(OrderedSet(internal_node_ip_names))
         inventory['services']['etc_hosts_generated'][node['internal_address']] = internal_node_ip_names
 
         if node.get('address'):
-            external_node_ip_names = inventory['services']['etc_hosts_generated'].get(node['address'], []) 
+            external_node_ip_names: List[str] = inventory['services']['etc_hosts_generated'].get(node['address'], [])
 
             external_node_ip_names.append("%s-external.%s" % (node['name'], cluster.inventory['cluster_name']))
             external_node_ip_names.append(node['name'] + "-external")
             external_node_ip_names = list(OrderedSet(external_node_ip_names))
             inventory['services']['etc_hosts_generated'][node['address']] = external_node_ip_names
 
     return inventory
 
 
-def enrich_kernel_modules(inventory: dict, cluster: KubernetesCluster):
+def enrich_kernel_modules(inventory: dict, cluster: KubernetesCluster) -> dict:
     """
     The method enrich the list of kernel modules ('services.modprobe') according to OS family
     """
     
     os_family = cluster.get_os_family()
     if os_family in ["unknown", "unsupported"]:
         raise Exception(ERROR_UNSUPPORTED_KERNEL_MODULES_VERSIONS_DETECTED)
@@ -100,37 +103,37 @@
         for item in os_families:
             modprobe[item] = inventory["services"]["modprobe"][item]
         inventory["services"]["modprobe"] = modprobe
 
     return inventory
 
 
-def fetch_os_versions(cluster: KubernetesCluster):
+def fetch_os_versions(cluster: KubernetesCluster) -> RunnersGroupResult:
     group = cluster.nodes['all'].get_accessible_nodes()
     '''
     For Red Hat, CentOS, Oracle Linux, and Ubuntu information in /etc/os-release /etc/redhat-release is sufficient but,
     Debian stores the full version in a special file. sed transforms version string, eg 10.10 becomes DEBIAN_VERSION="10.10"  
     '''
 
     return group.run(
         "cat /etc/*elease; cat /etc/debian_version 2> /dev/null | sed 's/\\(.\\+\\)/DEBIAN_VERSION=\"\\1\"/' || true")
 
 
-def detect_os_family(cluster):
+def detect_os_family(cluster: KubernetesCluster) -> None:
     results = fetch_os_versions(cluster)
 
-    for connection, result in results.items():
+    for host, result in results.items():
         stdout = result.stdout.lower()
 
         version = None
         lines = ''
 
         version_regex = re.compile("\\s\\d*\\.\\d*", re.M)
         for line in stdout.split("\n"):
-            if 'centos' in line or 'rhel' or 'rocky' in line:
+            if 'centos' in line or 'rhel' in line or 'rocky' in line:
                 # CentOS and Red Hat have a major version in VERSION_ID string
                 matches = re.findall(version_regex, line)
                 if matches:
                     version = matches[0].strip()
             if '=' in line:
                 lines += line + "\n"
 
@@ -146,15 +149,15 @@
 
         cluster.log.debug("Distribution: %s; Version: %s" % (name, version))
 
         os_family = detect_of_family_by_name_version(name, version)
 
         cluster.log.debug("OS family: %s" % os_family)
 
-        cluster.context["nodes"][connection.host]["os"] = {
+        cluster.context["nodes"][host]["os"] = {
             'name': name,
             'version': version,
             'family': os_family
         }
 
 
 def detect_of_family_by_name_version(name: str, version: str) -> str:
@@ -166,35 +169,32 @@
             if version in os_family_item["versions"]:
                 os_family = os_family_item["os_family"]
                 break
 
     return os_family
 
 
-def update_resolv_conf(group, config=None):
-    if config is None:
-        raise Exception("Data can't be empty")
-
+def update_resolv_conf(group: NodeGroup, config: dict) -> None:
     # TODO: Use Jinja template
     buffer = get_resolv_conf_buffer(config)
     utils.dump_file(group.cluster, buffer, 'resolv.conf')
-    group.put(buffer, "/etc/resolv.conf", backup=True, immutable=True, sudo=True, hide=True)
+    group.put(buffer, "/etc/resolv.conf", backup=True, immutable=True, sudo=True)
 
 
-def get_resolv_conf_buffer(config):
+def get_resolv_conf_buffer(config: dict) -> io.StringIO:
     buffer = io.StringIO()
     if config.get("search") is not None:
         buffer.write("search %s\n" % config["search"])
     if config.get("nameservers") is not None:
-        for address in config.get("nameservers"):
+        for address in config["nameservers"]:
             buffer.write("nameserver %s\n" % address)
     return buffer
 
 
-def generate_etc_hosts_config(inventory, cluster=None, etc_hosts_part='etc_hosts_generated'):
+def generate_etc_hosts_config(inventory: dict, etc_hosts_part: str = 'etc_hosts_generated') -> str:
 # generate records for /etc/hosts from services.etc_hosts or services.etc_hosts_generated
 
     result = ""
 
     max_len_ip = 0
 
     for ip in list(inventory['services'][etc_hosts_part].keys()):
@@ -210,110 +210,112 @@
                 continue
             names = " ".join(names)
         result += "%s%s  %s\n" % (ip, " " * (max_len_ip - len(ip)), names)
 
     return result
 
 
-def update_etc_hosts(group, config=None):
-    if config is None:
-        raise Exception("Data can't be empty")
+def update_etc_hosts(group: NodeGroup, config: str) -> None:
     utils.dump_file(group.cluster, config, 'etc_hosts')
-    group.put(io.StringIO(config), "/etc/hosts", backup=True, sudo=True, hide=True)
+    group.put(io.StringIO(config), "/etc/hosts", backup=True, sudo=True)
 
 
-def stop_service(group: NodeGroup, name: str) -> NodeGroupResult:
-    return group.sudo('systemctl stop %s' % name)
+def stop_service(group: AbstractGroup[GROUP_RUN_TYPE], name: str, callback: Callback = None) -> GROUP_RUN_TYPE:
+    return group.sudo('systemctl stop %s' % name, callback=callback)
 
 
-def start_service(group: NodeGroup, name: str) -> NodeGroupResult:
-    return group.sudo('systemctl start %s' % name)
+def start_service(group: AbstractGroup[GROUP_RUN_TYPE], name: str, callback: Callback = None) -> GROUP_RUN_TYPE:
+    return group.sudo('systemctl start %s' % name, callback=callback)
 
 
-def restart_service(group, name=None):
+def restart_service(group: AbstractGroup[GROUP_RUN_TYPE], name: str = None,
+                    callback: Callback = None) -> GROUP_RUN_TYPE:
     if name is None:
         raise Exception("Service name can't be empty")
-    return group.sudo('systemctl restart %s' % name)
+    return group.sudo('systemctl restart %s' % name, callback=callback)
 
 
-def enable_service(group, name=None, now=True):
+def enable_service(group: AbstractGroup[GROUP_RUN_TYPE], name: str = None,
+                   now: bool = True, callback: Callback = None) -> GROUP_RUN_TYPE:
     if name is None:
         raise Exception("Service name can't be empty")
 
     cmd = 'systemctl enable %s' % name
     if now:
         cmd = cmd + " --now"
-    return group.sudo(cmd)
+    return group.sudo(cmd, callback=callback)
 
 
-def disable_service(group, name=None, now=True):
+def disable_service(group: AbstractGroup[GROUP_RUN_TYPE], name: str = None,
+                    now: bool = True, callback: Callback = None) -> GROUP_RUN_TYPE:
     if name is None:
         raise Exception("Service name can't be empty")
 
     cmd = 'systemctl disable %s' % name
     if now:
         cmd = cmd + " --now"
-    return group.sudo(cmd)
+    return group.sudo(cmd, callback=callback)
 
 
-def patch_systemd_service(group: NodeGroup, service_name: str, patch_source: str):
+def patch_systemd_service(group: DeferredGroup, service_name: str, patch_source: str) -> None:
     group.sudo(f"mkdir -p /etc/systemd/system/{service_name}.service.d")
     group.put(io.StringIO(utils.read_internal(patch_source)),
               f"/etc/systemd/system/{service_name}.service.d/{service_name}.conf",
               sudo=True)
     group.sudo("systemctl daemon-reload")
 
 
-def fetch_firewalld_status(group: NodeGroup) -> NodeGroupResult:
+def fetch_firewalld_status(group: NodeGroup) -> RunnersGroupResult:
     return group.sudo("systemctl status firewalld", warn=True)
 
 
-def is_firewalld_disabled(group):
+def is_firewalld_disabled(group: NodeGroup) -> Tuple[bool, RunnersGroupResult]:
     result = fetch_firewalld_status(group)
     disabled_status = True
 
     for node_result in list(result.values()):
         if node_result.return_code != 4 and "disabled" not in node_result.stdout:
             disabled_status = False
 
     return disabled_status, result
 
 
-def disable_firewalld(group):
-    log = group.cluster.log
+def disable_firewalld(group: NodeGroup) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
     already_disabled, result = is_firewalld_disabled(group)
 
     if already_disabled:
         log.debug("Skipped - FirewallD already disabled or not installed")
         return result
 
     log.verbose("Trying to stop and disable FirewallD...")
 
     result = disable_service(group, name='firewalld', now=True)
 
-    group.cluster.schedule_cumulative_point(reboot_nodes)
-    group.cluster.schedule_cumulative_point(verify_system)
+    cluster.schedule_cumulative_point(reboot_nodes)
+    cluster.schedule_cumulative_point(verify_system)
 
     return result
 
 
-def is_swap_disabled(group):
+def is_swap_disabled(group: NodeGroup) -> Tuple[bool, RunnersGroupResult]:
     result = group.sudo("cat /proc/swaps", warn=True)
     disabled_status = True
 
     for node_result in list(result.values()):
         # is there any other lines excluding first head line?
         if node_result.stdout.strip().split('\n')[1:]:
             disabled_status = False
 
     return disabled_status, result
 
 
-def disable_swap(group):
+def disable_swap(group: NodeGroup) -> Optional[RunnersGroupResult]:
     log = group.cluster.log
 
     already_disabled, result = is_swap_disabled(group)
 
     if already_disabled:
         log.debug("Skipped - swap already disabled")
         return result
@@ -322,78 +324,80 @@
 
     group.sudo('swapoff -a', warn=True)
     group.sudo('sed -i.bak \'/swap/d\' /etc/fstab', warn=True)
 
     group.cluster.schedule_cumulative_point(reboot_nodes)
     group.cluster.schedule_cumulative_point(verify_system)
 
+    return None
+
 
-def reboot_nodes(cluster: KubernetesCluster):
+def reboot_nodes(cluster: KubernetesCluster) -> None:
     cluster.nodes["all"].get_new_nodes_or_self().call(reboot_group)
 
 
-def reboot_group(group: NodeGroup, try_graceful=None):
-    log = group.cluster.log
+def reboot_group(group: NodeGroup, try_graceful: bool = None) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
+    log = cluster.log
 
     if try_graceful is None:
-        if 'controlplain_uri' not in group.cluster.context.keys():
-            kubernetes.is_cluster_installed(group.cluster)
+        if 'controlplain_uri' not in cluster.context.keys():
+            kubernetes.is_cluster_installed(cluster)
 
     graceful_reboot = try_graceful is True or \
-                      (try_graceful is None and group.cluster.context['controlplain_uri'] is not None)
+                      (try_graceful is None and cluster.context['controlplain_uri'] is not None)
 
     if not graceful_reboot:
         return perform_group_reboot(group)
 
     log.verbose('Graceful reboot required')
 
-    first_control_plane = group.cluster.nodes['control-plane'].get_first_member()
-    results = NodeGroupResult(group.cluster)
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
+    results: Dict[str, RunnersResult] = {}
 
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        cordon_required = 'control-plane' in node['roles'] or 'worker' in node['roles']
+    for node in group.get_ordered_members_list():
+        node_config = node.get_config()
+        node_name = node.get_node_name()
+        cordon_required = 'control-plane' in node_config['roles'] or 'worker' in node_config['roles']
         if cordon_required:
             res = first_control_plane.sudo(
-                kubernetes.prepare_drain_command(group.cluster, node["name"], disable_eviction=False),
+                kubernetes.prepare_drain_command(cluster, node_name, disable_eviction=False),
                 warn=True)
             log.verbose(res)
-        log.debug(f'Rebooting node "{node["name"]}"')
-        raw_results = perform_group_reboot(node['connection'])
+        log.debug(f'Rebooting node "{node_name}"')
+        raw_results = perform_group_reboot(node)
         if cordon_required:
-            res = first_control_plane.sudo(f'kubectl uncordon {node["name"]}', warn=True)
+            res = first_control_plane.sudo(f'kubectl uncordon {node_name}', warn=True)
             log.verbose(res)
         results.update(raw_results)
 
-    return results
+    return RunnersGroupResult(cluster, results)
 
 
-def get_reboot_history(group: NodeGroup):
+def get_reboot_history(group: NodeGroup) -> RunnersGroupResult:
     return group.sudo('last reboot')
 
 
-def perform_group_reboot(group: NodeGroup):
+def perform_group_reboot(group: NodeGroup) -> RunnersGroupResult:
     log = group.cluster.log
 
     initial_boot_history = get_reboot_history(group)
     result = group.sudo(group.cluster.globals['nodes']['boot']['reboot_command'], warn=True)
     log.debug("Waiting for boot up...")
+    log.verbose("Initial boot history:\n%s" % initial_boot_history)
     group.wait_for_reboot(initial_boot_history)
     return result
 
 
-def reload_systemctl(group):
+def reload_systemctl(group: AbstractGroup[GROUP_RUN_TYPE]) -> GROUP_RUN_TYPE:
     return group.sudo('systemctl daemon-reload')
 
 
-def add_to_path(group, string):
-    # TODO: Also update PATH in ~/.bash_profile
-    group.sudo("export PATH=$PATH:%s" % string)
-
-def configure_chronyd(group, retries=60):
-    cluster = group.cluster
+def configure_chronyd(group: NodeGroup, retries: int = 60) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
     chronyd_config = ''
 
     for server in cluster.inventory['services']['ntp']['chrony']['servers']:
         chronyd_config += "server " + server + "\n"
 
     if cluster.inventory['services']['ntp']['chrony'].get('makestep'):
@@ -407,15 +411,15 @@
     group.sudo('systemctl restart chronyd')
     while retries > 0:
         log.debug("Waiting for time sync, retries left: %s" % retries)
         results = group.sudo('chronyc tracking && sudo chronyc sources')
         if results.stdout_contains("Normal"):
             log.verbose("NTP service reported successful time synchronization, validating...")
 
-            current_node_time, nodes_time, time_diff = get_nodes_time(group)
+            _, _, time_diff = get_nodes_time(group)
             if time_diff > cluster.globals['nodes']['max_time_difference']:
                 log.debug("Time is not synced yet")
                 log.debug(results)
             else:
                 log.debug("Time synced!")
                 return results
 
@@ -424,16 +428,16 @@
             log.debug(results)
         time.sleep(1)
         retries -= 1
 
     raise Exception("Time not synced, but timeout is reached")
 
 
-def configure_timesyncd(group, retries=120):
-    cluster = group.cluster
+def configure_timesyncd(group: NodeGroup, retries: int = 120) -> RunnersGroupResult:
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
     timesyncd_config = ''
 
     for section, options in cluster.inventory['services']['ntp']['timesyncd'].items():
         timesyncd_config += '[%s]' % section
         for option_name, option_value in options.items():
             if isinstance(option_value, list):
@@ -452,15 +456,15 @@
     log.verbose(res)
     while retries > 0:
         log.debug("Waiting for time sync, retries left: %s" % retries)
         results = group.sudo('timedatectl timesync-status && sudo timedatectl status')
         if results.stdout_contains("synchronized: yes"):
             log.verbose("NTP service reported successful time synchronization, validating...")
 
-            current_node_time, nodes_time, time_diff = get_nodes_time(group)
+            _, _, time_diff = get_nodes_time(group)
             if time_diff > cluster.globals['nodes']['max_time_difference']:
                 log.debug("Time is not synced yet")
                 log.debug(results)
             else:
                 log.debug("Time synced!")
                 return results
 
@@ -469,22 +473,22 @@
             log.debug(results)
         time.sleep(1)
         retries -= 1
 
     raise Exception("Time not synced, but timeout is reached")
 
 
-def setup_modprobe(group):
+def setup_modprobe(group: NodeGroup) -> Optional[RunnersGroupResult]:
     log = group.cluster.log
 
     os_family = group.get_nodes_os()
     if group.cluster.inventory['services'].get('modprobe') is None \
             or not group.cluster.inventory['services']['modprobe']:
         log.debug('Skipped - no modprobe configs in inventory')
-        return
+        return None
 
     is_valid, result = is_modprobe_valid(group)
 
     if is_valid:
         log.debug("Skipped - all necessary kernel modules are presented")
         return result
 
@@ -494,38 +498,40 @@
         module_name = module_name.strip()
         if module_name is not None and module_name != '':
             config += module_name + "\n"
             raw_config += module_name + " "
 
     log.debug("Uploading config...")
     utils.dump_file(group.cluster, config, 'modprobe_predefined.conf')
-    group.put(io.StringIO(config), "/etc/modules-load.d/predefined.conf", backup=True, sudo=True, hide=True)
+    group.put(io.StringIO(config), "/etc/modules-load.d/predefined.conf", backup=True, sudo=True)
     group.sudo("modprobe -a %s" % raw_config)
 
     group.cluster.schedule_cumulative_point(reboot_nodes)
     group.cluster.schedule_cumulative_point(verify_system)
 
+    return None
+
 
-def is_modprobe_valid(group):
+def is_modprobe_valid(group: NodeGroup) -> Tuple[bool, RunnersGroupResult]:
     log = group.cluster.log
 
     verify_results = group.sudo("lsmod", warn=True)
     is_valid = True
 
     os_family = group.get_nodes_os()
     for module_name in group.cluster.inventory['services']['modprobe'][os_family]:
-        for conn, result in verify_results.items():
+        for host, result in verify_results.items():
             if module_name not in result.stdout:
-                log.debug('Kernel module %s not found at %s' % (module_name, conn.host))
+                log.debug('Kernel module %s not found at %s' % (module_name, host))
                 is_valid = False
 
     return is_valid, verify_results
 
 
-def verify_system(cluster: KubernetesCluster):
+def verify_system(cluster: KubernetesCluster) -> None:
     group = cluster.nodes["all"].get_new_nodes_or_self()
     log = cluster.log
     # this method handles clusters with multiple OS
     os_family = group.get_nodes_os()
 
     if os_family in ['rhel', 'rhel8'] and cluster.is_task_completed('prepare.system.setup_selinux'):
         log.debug("Verifying Selinux...")
@@ -539,15 +545,15 @@
             raise Exception("Selinux is still not configured")
     else:
         log.debug('Selinux verification skipped - origin task was not completed')
 
     if cluster.is_task_completed('prepare.system.setup_apparmor') and os_family == 'debian':
         log.debug("Verifying Apparmor...")
         expected_profiles = cluster.inventory['services']['kernel_security'].get('apparmor', {})
-        apparmor_configured, result = apparmor.is_state_valid(group, expected_profiles)
+        apparmor_configured = apparmor.is_state_valid(group, expected_profiles)
         if not apparmor_configured:
             raise Exception("Apparmor is still not configured")
     else:
         log.debug('Apparmor verification skipped - origin task was not completed')
 
     if cluster.is_task_completed('prepare.system.disable_firewalld'):
         log.debug("Verifying FirewallD...")
@@ -573,119 +579,112 @@
         log.debug(modprobe_result)
         if not modprobe_valid:
             raise Exception("Required kernel modules are not presented")
     else:
         log.debug('Modprobe verification skipped - origin setup task was not completed')
 
 
-def detect_active_interface(cluster: KubernetesCluster):
+def detect_active_interface(cluster: KubernetesCluster) -> None:
     group = cluster.nodes['all'].get_accessible_nodes()
-    with RemoteExecutor(cluster) as exe:
-        for node in group.get_ordered_members_list(provide_node_configs=True):
-            detect_interface_by_address(node['connection'], node['internal_address'])
-    for cxn, host_results in exe.get_last_results().items():
-        try:
-            interface = list(host_results.values())[0].stdout.strip()
-        except Exception:
-            interface = None
-        cluster.context['nodes'][cxn.host]['active_interface'] = interface
+    collector = CollectorCallback(cluster)
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            detect_interface_by_address(node, node.get_config()['internal_address'], collector=collector)
+    for host, result in collector.result.items():
+        interface = result.stdout.strip()
+        cluster.context['nodes'][host]['active_interface'] = interface
 
-    return exe.get_last_results_str()
 
+def detect_interface_by_address(group: DeferredGroup, address: str, collector: CollectorCallback) -> Token:
+    return group.run("/usr/sbin/ip -o a | grep %s | awk '{print $2}'" % address, callback=collector)
 
-def detect_interface_by_address(group: NodeGroup, address: str):
-    return group.run("/usr/sbin/ip -o a | grep %s | awk '{print $2}'" % address)
 
-
-def _detect_nodes_access_info(cluster: KubernetesCluster):
+def _detect_nodes_access_info(cluster: KubernetesCluster) -> None:
     nodes_context = cluster.context['nodes']
     hosts_unknown_status = [host for host, node_context in nodes_context.items() if 'access' not in node_context]
     group_unknown_status = cluster.make_group(hosts_unknown_status)
     if group_unknown_status.is_empty():
         return
 
     check_active_timeout = int(cluster.globals["nodes"]["remove"]["check_active_timeout"])
     exc = None
+    results: GenericGroupResult[GenericResult]
     try:
         # This should invoke sudo last reboot
         results = group_unknown_status.wait_and_get_boot_history(timeout=check_active_timeout)
-    except fabric.group.GroupException as e:
+    except GroupResultException as e:
         exc = e
         results = e.result
 
-    for connection, result in results.items():
+    for host, result in results.items():
         access_info = {
             'online': False,
             'accessible': False,
             'sudo': 'No'
         }
-        nodes_context[connection.host]['access'] = access_info
+        nodes_context[host]['access'] = access_info
 
         if isinstance(result, Exception):
-            if NodeGroup.is_require_nopasswd_exception(result):
+            if RawExecutor.is_require_nopasswd_exception(result):
                 # The error is thrown only if connection is successful, but something is wrong with sudo access.
                 # In general, sudo password is incorrect. In our case, user is not a sudoer, or not a nopasswd sudoer.
                 access_info['online'] = True
                 access_info['accessible'] = True
             elif isinstance(result, socket.timeout):
                 # Usually when node is off. All statuses are unchecked.
                 pass
             elif isinstance(result, paramiko.ssh_exception.SSHException):
                 # At least, node is on, but something is wrong with ssh credentials (user / identity key)
                 access_info['online'] = True
             elif isinstance(result, paramiko.ssh_exception.NoValidConnectionsError):
                 # Internal socket error, for example, when ssh daemon is off. All statuses are unchecked.
                 pass
-            else:
+            elif isinstance(exc, Exception):
                 raise exc
         else:
             access_info['online'] = True
             access_info['accessible'] = True
             access_info['sudo'] = "Yes"
 
 
-def whoami(cluster: KubernetesCluster) -> NodeGroupResult:
+def whoami(cluster: KubernetesCluster) -> RunnersGroupResult:
     '''
     Determines different nodes access information, such as if the node is online, ssh credentials are correct, etc.
     '''
     _detect_nodes_access_info(cluster)
 
     results = cluster.nodes["all"].get_sudo_nodes().sudo("whoami")
-    for connection, result in results.items():
-        node_ctx = cluster.context['nodes'][connection.host]
+    for host, result in results.items():
+        node_ctx = cluster.context['nodes'][host]
         node_ctx['access']['sudo'] = 'Root' if result.stdout.strip() == "root" else 'Yes'
     return results
 
 
 @restrict_empty_group
-def get_nodes_time(group: NodeGroup) -> (float, Dict[fabric.connection.Connection, float], float):
+def get_nodes_time(group: NodeGroup) -> Tuple[float, Dict[str, float], float]:
     """
     Polls the time from the specified group of nodes, parses it and returns tuple with results.
     :param group: Group of nodes, where timestamps should be detected.
     :return: tuple with max timestamp, dict of parsed timestamps per node and max found time difference.
 
     Max time required for comparing dates computed on nodes, because we can not detect real time between nodes.
     Max nodes time should be less than minimal compared time from future.
 
     Timestamp - is a time in milliseconds since epoch.
     """
 
     # Please, note: this method can not detect time on nodes precisely, since Kubemarine can execute commands not at the
     # same time depending on various factors, for example, restrictions on the number of open sockets.
 
-    parsed_time_per_node: Dict[fabric.connection.Connection, float] = {}
-
-    min_time = None
-    max_time = None
+    parsed_time_per_node: Dict[str, float] = {}
 
     # TODO: request and parse more accurate timestamp in milliseconds
 
     raw_results = group.run('date')
     for host, result in raw_results.items():
         parsed_time = parse(result.stdout.strip()).timestamp() * 1000
         parsed_time_per_node[host] = parsed_time
-        if min_time is None or min_time > parsed_time:
-            min_time = parsed_time
-        if max_time is None or max_time < parsed_time:
-            max_time = parsed_time
+
+    min_time = min(parsed_time_per_node.values())
+    max_time = max(parsed_time_per_node.values())
 
     return max_time, parsed_time_per_node, max_time-min_time
```

### Comparing `kubemarine-0.18.2/kubemarine/templates/__init__.py` & `kubemarine-0.19.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.19.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.19.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.19.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.19.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/kubemarine/testsuite.py` & `kubemarine-0.19.0/kubemarine/testsuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import textwrap
 from traceback import *
 import csv
 from datetime import datetime
+from typing import Dict
+
 from kubemarine.core import utils, log
-import fabric
+
+from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.group import GroupException
 
 TC_UNKNOWN = -1
 TC_PASSED = 0
 TC_FAILED = 1
 TC_WARNED = 2
 TC_EXCEPTED = 3
 
@@ -44,23 +48,19 @@
             if self.status is TC_UNKNOWN:
                 self.success()
         elif type is TestFailure:
             self.fail(value)
         elif type is TestWarn:
             self.warn(value)
         else:
-            if isinstance(value, fabric.group.GroupException):
-                value.result.print()
-            else:
-                print_exc()
             self.exception(value)
         print(self.get_summary(show_hint=True))
         return True
 
-    def __init__(self, cluster, id, category, name, default_results=None, minimal=None, recommended=None):
+    def __init__(self, cluster: KubernetesCluster, id, category, name, default_results=None, minimal=None, recommended=None):
         self.include_in_ts(cluster.context['testsuite'])
         self.category = category
         self.id = str(id)
         self.name = name
         self.status = TC_UNKNOWN
         self.results = default_results
         self.minimal = minimal
@@ -85,15 +85,20 @@
     def warn(self, results):
         self.status = TC_WARNED
         self.results = results
         return self
 
     def exception(self, results):
         self.status = TC_EXCEPTED
-        self.results = results
+        if isinstance(results, GroupException):
+            self.cluster.log.debug(results)
+            self.results = "Remote group exception"
+        else:
+            print_exc()
+            self.results = results
         return self
 
     def get_summary(self, show_description=False, show_hint=False, show_minimal=False, show_recommended=False):
         output = ""
 
         output += " " * (15 - len(self.category))
         output += self.category + "  "
@@ -264,15 +269,15 @@
         if self.is_any_test_warned():
             log.warning("\nTEST PASSED WITH WARNINGS"
                         "\nThe environment meets the minimal requirements, but is not as recommended. Try to check the test report and resolve the issues.")
             return
         log.info("\nTEST PASSED")
 
     def get_stats_data(self):
-        results = {}
+        results: Dict[str, int] = {}
         for tc in self.tcs:
             key = 'unknown'
             if tc.is_succeeded():
                 key = 'succeeded'
             elif tc.is_failed():
                 key = 'failed'
             elif tc.is_warned():
```

### Comparing `kubemarine-0.18.2/kubemarine/thirdparties.py` & `kubemarine-0.19.0/kubemarine/thirdparties.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 from copy import deepcopy
-from typing import Tuple, Optional, Dict, List
+from typing import Tuple, Optional, Dict, List, Union
 
 from kubemarine.core import utils, static, errors
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import NodeGroupResult, NodeGroup
+from kubemarine.core.group import NodeGroup, RunnersGroupResult
 from kubemarine.core.yaml_merger import default_merger
 
 
-def is_default_thirdparty(destination: str):
+def is_default_thirdparty(destination: str) -> bool:
     return destination in static.GLOBALS['thirdparties']
 
 
 def get_default_thirdparties() -> List[str]:
     return list(static.GLOBALS['thirdparties'])
 
 
@@ -40,15 +40,15 @@
     if 'version' in software_settings:
         return software_settings['version']
     else:
         # kubeadm, kubelet, kubectl
         return kubernetes_version
 
 
-def get_default_thirdparty_source(destination: str, version: str, in_public: bool):
+def get_default_thirdparty_source(destination: str, version: str, in_public: bool) -> str:
     """
     :param destination: absolute path of default third-party
     :param version: version of third-party
     :param in_public: flag whether to return third-party URL in public resources.
     :return: URL of the third-party source.
     """
     if not is_default_thirdparty(destination):
@@ -79,24 +79,26 @@
 
     version = get_default_thirdparty_version(kubernetes_version, destination)
     source = get_default_thirdparty_source(destination, version, in_public)
 
     return source, sha1
 
 
-def _get_software_settings_for_thirdparty(kubernetes_version: str, destination: str) -> dict:
+def _get_software_settings_for_thirdparty(kubernetes_version: str, destination: str) -> Dict[str, str]:
     if not is_default_thirdparty(destination):
         raise Exception(f"{destination} is not a default 3rd-party")
 
     thirdparty_settings = static.GLOBALS['thirdparties'][destination]
     software_name = thirdparty_settings['software_name']
-    return static.GLOBALS['compatibility_map']['software'][software_name][kubernetes_version]
+    software_settings: Dict[str, str] = static.GLOBALS['compatibility_map']['software'][software_name][kubernetes_version]
+    return software_settings
 
 
 def get_thirdparty_destination(software_name: str) -> str:
+    destination: str
     for destination, thirdparty_settings in static.GLOBALS['thirdparties'].items():
         if thirdparty_settings['software_name'] == software_name:
             return destination
     else:
         raise Exception(f"Failed to find third-party destination for {software_name!r}")
 
 
@@ -110,29 +112,29 @@
                                                          destination, in_public=True)
     cluster.log.verbose(f"Recommended sha for thirdparty {destination} was calculated: {recommended_sha}")
 
     return recommended_sha
 
 
 def _convert_thirdparty(thirdparties: dict, destination: str) -> dict:
-    config = thirdparties.setdefault(destination, {})
+    config: Union[str, dict] = thirdparties.setdefault(destination, {})
     if isinstance(config, str):
         thirdparties[destination] = config = {
             'source': config
         }
 
     return config
 
 
 def _get_upgrade_plan(cluster: KubernetesCluster) -> List[Tuple[str, dict]]:
     context = cluster.context
     if context.get("initial_procedure") == "upgrade":
         upgrade_version = context["upgrade_version"]
         upgrade_plan = []
-        for version in cluster.procedure_inventory.get('upgrade_plan'):
+        for version in cluster.procedure_inventory['upgrade_plan']:
             if utils.version_key(version) < utils.version_key(upgrade_version):
                 continue
 
             upgrade_plan.append((version, cluster.procedure_inventory.get(version, {}).get("thirdparties", {})))
 
     elif context.get("initial_procedure") == "migrate_kubemarine" and 'upgrading_thirdparty' in context:
         upgrade_thirdparties = cluster.procedure_inventory.get('upgrade', {}).get("thirdparties", {})
@@ -166,15 +168,15 @@
 
     _verify_upgrade_plan(inventory, previous_version, thirdparties_verify, upgrade_plan)
 
     return generic_upgrade_inventory(cluster, inventory)
 
 
 def _verify_upgrade_plan(inventory: dict, previous_version: str,
-                         thirdparties_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+                         thirdparties_verify: List[str], upgrade_plan: List[Tuple[str, dict]]) -> None:
 
     thirdparties = deepcopy(inventory["services"]['thirdparties'])
     sensitive_keys = ['source', 'sha1']
 
     for version, upgrade_thirdparties in upgrade_plan:
         upgrade_thirdparties = deepcopy(upgrade_thirdparties)
 
@@ -263,15 +265,15 @@
     if cri_name == "docker" and \
             crictl_key not in cluster.raw_inventory.get('services', {}).get('thirdparties', {}):
         del(thirdparties[crictl_key])
 
     return inventory
 
 
-def get_install_group(cluster: KubernetesCluster, config: dict):
+def get_install_group(cluster: KubernetesCluster, config: dict) -> NodeGroup:
     return cluster.create_group_from_groups_nodes_names(
         config.get('groups', []), config.get('nodes', []))
 
 
 def get_group_require_unzip(cluster: KubernetesCluster, inventory: dict) -> NodeGroup:
     thirdparties: dict = inventory['services']['thirdparties']
 
@@ -283,27 +285,27 @@
 
         install_group = get_install_group(cluster, config)
         group = group.include_group(install_group)
 
     return group
 
 
-def install_thirdparty(filter_group: NodeGroup, destination: str) -> NodeGroupResult or None:
+def install_thirdparty(filter_group: NodeGroup, destination: str) -> Optional[RunnersGroupResult]:
     cluster = filter_group.cluster
     config = cluster.inventory['services'].get('thirdparties', {}).get(destination)
 
     if config is None:
         raise Exception('Not possible to install thirdparty %s - not found in configfile' % destination)
 
     common_group = get_install_group(cluster, config)
     common_group = common_group.intersection_group(filter_group)
 
     if common_group.is_empty():
         cluster.log.verbose(f'No destination nodes to install thirdparty {destination!r}')
-        return
+        return None
 
     cluster.log.debug("Thirdparty \"%s\" will be installed" % destination)
     is_curl = config['source'][:4] == 'http' and '://' in config['source'][4:8]
 
     # all commands will be grouped to single run
     remote_commands = ''
 
@@ -367,16 +369,16 @@
                            % (destination, config['owner'], config['unpack'])
             remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo ls -la %s/FILE' % (destination, config['unpack'])
 
 
     return common_group.sudo(remote_commands)
 
 
-def install_all_thirparties(group):
-    cluster = group.cluster
+def install_all_thirparties(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     if not cluster.inventory['services'].get('thirdparties', {}):
         return
 
     for destination in cluster.inventory['services']['thirdparties'].keys():
         skip_thirdparty = False
```

### Comparing `kubemarine-0.18.2/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.19.0/kubemarine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.2
+Version: 0.19.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -20,49 +20,50 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ansible
+Provides-Extra: mypy
 License-File: LICENSE
 
 ![Kubemarine_1280х640_3_JPEG](https://user-images.githubusercontent.com/5212888/162978291-63d55f19-7dc0-4126-ad39-cd69191e7e19.jpg)
 [![GitHub stars](https://img.shields.io/github/v/release/Netcracker/Kubemarine)](https://github.com/Netcracker/KubeMarine/releases)
 [![GitHub stars](https://img.shields.io/badge/contributions-welcome-orange.svg)](https://github.com/Netcracker/KubeMarine/blob/main/CONTRIBUTING.md)
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +81,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +100,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,27 +129,28 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.2/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.19.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
+     password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
 
    nodes:
      - name: "k8s-control-plane-1"
@@ -173,42 +175,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.2/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.19.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.2/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.19.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.2/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.19.0/LICENSE)
```

### Comparing `kubemarine-0.18.2/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.19.0/kubemarine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.2/setup.py` & `kubemarine-0.19.0/setup.py`

 * *Files identical despite different names*

