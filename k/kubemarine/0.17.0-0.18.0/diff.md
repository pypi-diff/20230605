# Comparing `tmp/kubemarine-0.17.0.tar.gz` & `tmp/kubemarine-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.17.0.tar", last modified: Mon May 15 10:01:30 2023, max compression
+gzip compressed data, was "kubemarine-0.18.0.tar", last modified: Fri Jun  2 11:14:55 2023, max compression
```

## Comparing `kubemarine-0.17.0.tar` & `kubemarine-0.18.0.tar`

### file list

```diff
@@ -1,237 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.492222 kubemarine-0.17.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-15 10:01:16.000000 kubemarine-0.17.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-15 10:01:16.000000 kubemarine-0.17.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12413 2023-05-15 10:01:30.492222 kubemarine-0.17.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-05-15 10:01:16.000000 kubemarine-0.17.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.460221 kubemarine-0.17.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-05-15 10:01:16.000000 kubemarine-0.17.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-15 10:01:16.000000 kubemarine-0.17.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.464221 kubemarine-0.17.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8195 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    44406 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15462 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23611 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    15921 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    18873 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    39980 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    12720 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8286 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    20944 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7067 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    19878 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10879 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11275 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    63792 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    19658 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1037 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/patches/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    38251 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14938 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    18795 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.472221 kubemarine-0.17.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4919 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20638 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2629 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50500 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    74067 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5081 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26620 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1769 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1667 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    15479 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2380 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6074 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13653 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13619 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3605 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     3849 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     5903 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3020 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    27351 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     9468 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.456221 kubemarine-0.17.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1037 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/etalons/patches/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3096 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      585 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4092 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5128 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1881 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2826 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    31848 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.492222 kubemarine-0.17.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    10441 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    13898 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.464221 kubemarine-0.17.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12413 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8938 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2554 2023-05-15 10:01:16.000000 kubemarine-0.17.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 10:01:30.492222 kubemarine-0.17.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 11:14:41.000000 kubemarine-0.18.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-02 11:14:41.000000 kubemarine-0.18.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-02 11:14:55.455617 kubemarine-0.18.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-06-02 11:14:41.000000 kubemarine-0.18.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.427617 kubemarine-0.18.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-02 11:14:41.000000 kubemarine-0.18.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-02 11:14:41.000000 kubemarine-0.18.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    45051 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    14424 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    20072 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    65136 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    29985 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    40081 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    19568 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    19510 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    13653 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5037 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    25005 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.423617 kubemarine-0.18.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26444 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11284 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    17436 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-02 11:14:41.000000 kubemarine-0.18.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 11:14:55.455617 kubemarine-0.18.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/setup.py
```

### Comparing `kubemarine-0.17.0/LICENSE` & `kubemarine-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/PKG-INFO` & `kubemarine-0.18.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.17.0
+Version: 0.18.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.17.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#documentation).
 
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
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.17.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.17.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.17.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.0/LICENSE)
```

### Comparing `kubemarine-0.17.0/README.md` & `kubemarine-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/bin/kubemarine` & `kubemarine-0.18.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/bin/kubemarine.cmd` & `kubemarine-0.18.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/__init__.py` & `kubemarine-0.18.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/__main__.py` & `kubemarine-0.18.0/kubemarine/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,16 +217,16 @@
 
     from kubemarine import demo
 
     demo.new_cluster(demo.generate_inventory(**demo.FULLHA))
 
     print('\nValidating patch duplicates ...')
 
-    from kubemarine import patches
-    patches = patches.patches
+    module = import_procedure('migrate_kubemarine')
+    patches = module.load_patches()
     patch_ids = [patch.identifier for patch in patches]
     unique = set()
     duplicates = [p_id for p_id in patch_ids if p_id in unique or unique.add(p_id)]
     if duplicates:
         raise Exception(f'Patches identifiers {duplicates} are duplicated ')
 
     print("Finished")
```

### Comparing `kubemarine-0.17.0/kubemarine/admission.py` & `kubemarine-0.18.0/kubemarine/admission.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,30 +316,30 @@
     final_admission_plugins_list = list(result.values())[0]
 
     # update api-server config on all control-planes
     cluster.log.debug("Updating kube-apiserver configs on control-planes")
     cluster.nodes["control-plane"].call(update_kubeapi_config, options_list=final_admission_plugins_list)
 
 
-def restart_pods_task(cluster, disable_eviction=False):
+def restart_pods_task(cluster):
     if cluster.context.get('initial_procedure') == 'manage_pss':
         # check if pods restart is enabled
         is_restart = cluster.procedure_inventory.get("restart-pods", False)
         if not is_restart:
             cluster.log.debug("'restart-pods' is disabled, pods won't be restarted")
             return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Drain-Uncordon all nodes to restart pods")
     kube_nodes = cluster.nodes["control-plane"].include_group(cluster.nodes["worker"])
     for node in kube_nodes.get_ordered_members_list(provide_node_configs=True):
         first_control_plane.sudo(
-            kubernetes.prepare_drain_command(node, cluster.inventory['services']['kubeadm']['kubernetesVersion'],
-                                             cluster.globals, disable_eviction, cluster.nodes), hide=False)
+            kubernetes.prepare_drain_command(cluster, node["name"], disable_eviction=False),
+            hide=False)
         first_control_plane.sudo("kubectl uncordon %s" % node["name"], hide=False)
 
     cluster.log.debug("Restarting daemon-sets...")
     daemon_sets = ruamel.yaml.YAML().load(list(first_control_plane.sudo("kubectl get ds -A -o yaml").values())[0].stdout)
     for ds in daemon_sets["items"]:
         first_control_plane.sudo("kubectl rollout restart ds %s -n %s" % (ds["metadata"]["name"], ds["metadata"]["namespace"]))
 
@@ -792,14 +792,24 @@
     if "defaults" in procedure_config:
         default_merger.merge(current_config.setdefault("defaults", {}), procedure_config["defaults"])
     if "exemptions" in procedure_config:
         default_merger.merge(current_config.setdefault("exemptions", {}), procedure_config["exemptions"])
 
     return inventory_to_finalize
 
+# update PSP/PSS fields in the inventory dumped to cluster_finalized.yaml
+def update_finalized_inventory(cluster, inventory_to_finalize):
+    if cluster.context.get('initial_procedure') == 'manage_pss':
+        current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("pss", {})
+        current_config["pod-security"] = cluster.procedure_inventory["pss"].get("pod-security", current_config.get("pod-security", "enabled"))
+    elif cluster.context.get('initial_procedure') == 'manage_psp':
+        current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("psp", {})
+        current_config["pod-security"] = cluster.procedure_inventory["psp"].get("pod-security", current_config.get("pod-security", "enabled"))
+
+    return inventory_to_finalize
 
 def copy_pss(group):
     if  group.cluster.inventory['rbac']['admission'] !=  "pss":
         return
     if group.cluster.context.get('initial_procedure') == 'manage_pss':
         if not is_security_enabled(group.cluster.inventory) and \
                 group.cluster.procedure_inventory["pss"]["pod-security"] != "enabled":
```

### Comparing `kubemarine-0.17.0/kubemarine/apparmor.py` & `kubemarine-0.18.0/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/apt.py` & `kubemarine-0.18.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/audit.py` & `kubemarine-0.18.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/controlplane.py` & `kubemarine-0.18.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/__init__.py` & `kubemarine-0.18.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/action.py` & `kubemarine-0.18.0/kubemarine/core/action.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,20 +29,35 @@
         :param recreate_inventory specifies if inventory should be recreated after the action succeeds.
         """
 
         self.identifier = identifier
         self.recreate_inventory = recreate_inventory
 
     @abstractmethod
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         """
-        Do some work based on provided DynamicResources.
+        Do some work based on provided DynamicResources. If any action fails, further actions are not run.
 
         Avoid direct exiting in case of exceptions (for example using utils.do_fail),
         unless it is the only action being executed.
         Otherwise, correct exception handling will not be performed.
         """
         pass
 
-    def prepare_context(self, context: dict):
-        """Called first before any work with the action"""
+    def prepare_context(self, context: dict) -> None:
+        """
+        Enrich context if necessary before the action is run.
+        The changes are remained after action is executed, and will be visible to further actions.
+        To revert the changes, implement Action.reset_context().
+
+        :param context: mutable context instance.
+        """
+        return
+
+    def reset_context(self, context: dict) -> None:
+        """
+        Reset changes in the context if necessary.
+        The method is called only if the action is executed successfully.
+
+        :param context: mutable context instance.
+        """
         return
```

### Comparing `kubemarine-0.17.0/kubemarine/core/annotations.py` & `kubemarine-0.18.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/cluster.py` & `kubemarine-0.18.0/kubemarine/core/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
             raise Exception(f'Failed to get association "{association_key}" for package "{package}"')
         if not isinstance(association_value, str) and not isinstance(association_value, list):
             raise Exception(f'Unsupported association "{association_key}" value type for package "{package}", '
                             f'got: {str(association_value)}')
 
         return association_value
 
-    def get_package_association(self, package: str, association_key: str) -> str or list:
+    def get_package_association(self, package: str, association_key: str) -> Union[str, List[str]]:
         """
         Returns the specified association for the specified package from inventory for the cluster.
         The method can be used only if cluster has nodes with the same and supported OS family.
 
         :param package: The package name to get the association for
         :param association_key: Association key to get
         :return: Association string or list value
@@ -315,21 +315,22 @@
         """
         os_family = self.get_os_family_for_node(host)
         return self._get_package_associations_for_os(os_family, package, association_key)
 
     def make_finalized_inventory(self):
         from kubemarine.core import defaults
         from kubemarine.procedures import remove_node
-        from kubemarine import controlplane, cri, packages
+        from kubemarine import admission, controlplane, cri, packages
 
         cluster_finalized_functions = {
             packages.cache_package_versions,
             packages.remove_unused_os_family_associations,
             cri.remove_invalid_cri_config,
             remove_node.remove_node_finalize_inventory,
+            admission.update_finalized_inventory,
             defaults.escape_jinja_characters_for_inventory,
             controlplane.controlplane_finalize_inventory,
         }
 
         # copying is currently not necessary, but it is possible in general.
         prepared_inventory = self.inventory
         for finalize_fn in cluster_finalized_functions:
@@ -338,16 +339,15 @@
         return defaults.prepare_for_dump(prepared_inventory, copy=False)
 
     def dump_finalized_inventory(self):
         inventory_for_dump = self.make_finalized_inventory()
         data = yaml.dump(inventory_for_dump)
         finalized_filename = "cluster_finalized.yaml"
         utils.dump_file(self, data, finalized_filename)
-        with utils.open_external(finalized_filename, 'w') as f:
-            f.write(data)
+        utils.dump_file(self, data, finalized_filename, dump_location=False)
 
     def preserve_inventory(self):
         self.log.debug("Start preserving of the information about the procedure.")
         cluster_storage = utils.ClusterStorage(self)
         cluster_storage.make_dir()
         if self.context.get('initial_procedure') == 'add_node':
             cluster_storage.upload_info_new_control_planes()
```

### Comparing `kubemarine-0.17.0/kubemarine/core/connections.py` & `kubemarine-0.18.0/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/defaults.py` & `kubemarine-0.18.0/kubemarine/core/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,37 +17,37 @@
 from typing import Optional
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.errors import KME
 from kubemarine import jinja
-from kubemarine.core import utils, static
+from kubemarine.core import utils, static, log, os
 from kubemarine.core.yaml_merger import default_merger
 
 # All enrichment procedures should not connect to any node.
 # The information about nodes should be collected within KubernetesCluster#detect_nodes_context().
 DEFAULT_ENRICHMENT_FNS = [
     "kubemarine.core.schema.verify_inventory",
     "kubemarine.core.defaults.merge_defaults",
     "kubemarine.kubernetes.verify_initial_version",
     "kubemarine.admission.enrich_default_admission",
     "kubemarine.kubernetes.add_node_enrichment",
     "kubemarine.kubernetes.remove_node_enrichment",
     "kubemarine.controlplane.controlplane_node_enrichment",
     "kubemarine.core.defaults.append_controlplain",
     "kubemarine.kubernetes.enrich_upgrade_inventory",
-    "kubemarine.plugins.enrich_upgrade_inventory",
-    "kubemarine.packages.enrich_inventory_associations",
-    "kubemarine.packages.enrich_inventory_packages",
-    "kubemarine.system.enrich_upgrade_inventory",
     "kubemarine.core.defaults.compile_inventory",
     "kubemarine.core.defaults.manage_true_false_values",
+    "kubemarine.plugins.enrich_upgrade_inventory",
+    "kubemarine.packages.enrich_inventory",
+    "kubemarine.packages.enrich_upgrade_inventory",
+    "kubemarine.packages.enrich_inventory_apply_defaults",
+    "kubemarine.thirdparties.enrich_upgrade_inventory",
     "kubemarine.admission.manage_enrichment",
-    "kubemarine.thirdparties.enrich_inventory_apply_upgrade_defaults",
     "kubemarine.procedures.migrate_cri.enrich_inventory",
     "kubemarine.core.defaults.apply_registry",
     "kubemarine.core.defaults.calculate_node_names",
     "kubemarine.core.defaults.verify_node_names",
     "kubemarine.core.defaults.apply_defaults",
     "kubemarine.keepalived.enrich_inventory_apply_defaults",
     "kubemarine.haproxy.enrich_inventory",
@@ -408,20 +408,21 @@
         from kubemarine import controlplane
         inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, prepare_for_dump(inventory))
         utils.dump_file(cluster, yaml.dump(inventory_for_dump, ), "cluster.yaml")
 
     return inventory
 
 
-def compile_inventory(inventory, cluster):
+def compile_inventory(inventory: dict, cluster: KubernetesCluster):
 
     # convert references in yaml to normal values
     iterations = 100
     root = deepcopy(inventory)
     root['globals'] = static.GLOBALS
+    root['env'] = os.Environ()
 
     while iterations > 0:
 
         cluster.log.verbose('Inventory is not rendered yet...')
         inventory = compile_object(cluster.log, inventory, root)
 
         temp_dump = yaml.dump(inventory)
@@ -442,46 +443,49 @@
     inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, prepare_for_dump(inventory))
     merged_inventory = yaml.dump(inventory_for_dump)
     utils.dump_file(cluster, merged_inventory, "cluster_precompiled.yaml")
 
     return inventory
 
 
-def compile_object(log, struct, root, ignore_jinja_escapes=True):
+def compile_object(logger: log.EnhancedLogger, struct: object, root: dict, ignore_jinja_escapes=True) -> object:
     if isinstance(struct, list):
         new_struct = []
         for i, v in enumerate(struct):
-            struct[i] = compile_object(log, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
+            struct[i] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
             # delete empty list entries, which can appear after jinja compilation
             if struct[i] != '':
                 new_struct.append(struct[i])
         struct = new_struct
     elif isinstance(struct, dict):
         for k, v in struct.items():
-            struct[k] = compile_object(log, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
+            struct[k] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
     elif isinstance(struct, str) and ('{{' in struct or '{%' in struct):
-        struct = compile_string(log, struct, root, ignore_jinja_escapes=ignore_jinja_escapes)
+        struct = compile_string(logger, struct, root, ignore_jinja_escapes=ignore_jinja_escapes)
+
     return struct
 
 
-def compile_string(log, struct, root, ignore_jinja_escapes=True):
-    log.verbose("Rendering \"%s\"" % struct)
+def compile_string(logger: log.EnhancedLogger, struct: str, root: dict,
+                   ignore_jinja_escapes=True) -> str:
+    logger.verbose("Rendering \"%s\"" % struct)
 
     if ignore_jinja_escapes:
         iterator = escaped_expression_regex.finditer(struct)
         struct = re.sub(escaped_expression_regex, '', struct)
-        struct = jinja.new(log, root).from_string(struct).render(**root)
+        struct = jinja.new(logger, True, root).from_string(struct).render(**root)
 
+        # TODO this does not work for {raw}{jinja}{raw}{jinja}
         for match in iterator:
             span = match.span()
             struct = struct[:span[0]] + match.group() + struct[span[0]:]
     else:
-        struct = jinja.new(log, root).from_string(struct).render(**root)
+        struct = jinja.new(logger, True, root).from_string(struct).render(**root)
 
-    log.verbose("\tRendered as \"%s\"" % struct)
+    logger.verbose("\tRendered as \"%s\"" % struct)
     return struct
 
 
 def escape_jinja_characters_for_inventory(cluster: KubernetesCluster, obj):
     if isinstance(obj, dict):
         for key, value in obj.items():
             obj[key] = escape_jinja_characters_for_inventory(cluster, value)
```

### Comparing `kubemarine-0.17.0/kubemarine/core/environment.py` & `kubemarine-0.18.0/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/executor.py` & `kubemarine-0.18.0/kubemarine/core/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 import fabric
 import invoke
 
 from fabric.connection import Connection
 from concurrent.futures.thread import ThreadPoolExecutor
 
+from kubemarine.core import log
+
 GRE = ContextVar('KubemarineGlobalRemoteExecutor', default=None)
 
 
 class RemoteExecutor:
 
     def __init__(self, cluster,
                  warn=False,
@@ -183,18 +185,26 @@
     def queue(self, target, action: Tuple, callback: Callable = None) -> int or dict:
         # TODO support callbacks
         callback = None
         executor = self._get_active_executor()
         executor._last_token = token = executor._last_token + 1
 
         if isinstance(target, Connection):
-            target = [Connection]
+            target = [target]
         if isinstance(target, dict):
             target = list(target.values())
 
+        kwargs = action[2]
+        if 'out_stream' in kwargs or 'err_stream' in kwargs:
+            if executor.lazy:
+                raise ValueError("Custom out/err streams are supported only for non-lazy execution")
+
+            if len(target) != 1:
+                raise ValueError("Custom out/err streams are supported only for the single node")
+
         if not target:
             executor.cluster.log.verbose('Connections list is empty, nothing to queue')
         else:
             for connection in target:
                 if not executor.connections_queue.get(connection):
                     executor.connections_queue[connection] = []
                 executor.connections_queue[connection].append((action, callback, token))
@@ -366,19 +376,30 @@
                     do_type, args, kwargs = action
                     executor.cluster.log.verbose('Executing %s %s with options: %s' % (do_type, args, kwargs))
                     safe_exec(futures, cxn.host, lambda: TPE.submit(getattr(cxn, do_type), *args, **kwargs))
 
                 for host, future in futures.items():
                     safe_exec(results, host, lambda: future.result(timeout=executor.timeout))
 
+                self._flush_logger_writers(batch)
+
                 parsed_results = executor.reparse_results(results, batch)
                 for host, tokenized_results in parsed_results.items():
                     if not batch_results.get(host):
                         batch_results[host] = {}
                     for token, res in tokenized_results.items():
                         batch_results[host][token] = res
 
         executor.connections_queue_history.append(executor.connections_queue)
         executor.reset_queue()
         executor.results.append(batch_results)
 
         return batch_results
+
+    def _flush_logger_writers(self, batch):
+        for cxn, payload in batch.items():
+            action, _, _ = payload
+            _, _, kwargs = action
+            if isinstance(kwargs.get('out_stream'), log.LoggerWriter):
+                kwargs.get('out_stream').flush(remainder=True)
+            if isinstance(kwargs.get('err_stream'), log.LoggerWriter):
+                kwargs.get('err_stream').flush(remainder=True)
```

### Comparing `kubemarine-0.17.0/kubemarine/core/flow.py` & `kubemarine-0.18.0/kubemarine/core/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
             if resources.procedure_inventory_filepath:
                 with utils.open_external(resources.procedure_inventory_filepath, "r") as stream:
                     utils.dump_file(context, stream, "procedure.yaml")
         try:
             logger.info(f"Running action '{act.identifier}'")
             act.run(resources)
+            act.reset_context(context)
             successfully_performed.append(act.identifier)
         except Exception:
             if successfully_performed:
                 _post_process_actions_group(last_cluster, context, successfully_performed, failed=True)
 
             raise
```

### Comparing `kubemarine-0.17.0/kubemarine/core/group.py` & `kubemarine-0.18.0/kubemarine/core/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from datetime import datetime
 from typing import Callable, Dict, List, Union, IO
 
 import fabric
 import invoke
 from invoke import UnexpectedExit
 
-from kubemarine.core import utils
+from kubemarine.core import utils, log
 from kubemarine.core.connections import Connections
 from kubemarine.core.executor import RemoteExecutor
 
 _GenericResult = Union[Exception, fabric.runners.Result, fabric.transfer.Result]
 _HostToResult = Dict[str, _GenericResult]
 
 
@@ -304,14 +304,52 @@
 
         return True
 
     def __ne__(self, other) -> bool:
         return not self == other
 
 
+def _handle_internal_logging(fn: callable) -> callable:
+    """
+    Method is a decorator that handles internal streaming of output (hide=False) of fabric (invoke).
+    Note! This decorator should be the outermost.
+
+    :param fn: Origin function to apply annotation to
+    :return: Validation wrapper function
+    """
+    def do(self: 'NodeGroup', *args, logging_stream_level: int = None, **kwargs):
+        if logging_stream_level is not None and 'hide' in kwargs:
+            raise ValueError("'hide' and 'logging_stream_level' should not be combined")
+
+        logger = self.cluster.log
+        if logging_stream_level is not None:
+            # We want to stream output immediately to logging framework, thus not hide.
+            kwargs['hide'] = False
+
+            caller = log.caller_info(logger)
+            out = log.LoggerWriter(logger, logging_stream_level, caller, '[remote] ')
+            err = log.LoggerWriter(logger, logging_stream_level, caller, '[stderr] ')
+
+            return fn(self, *args, out_stream=out, err_stream=err, **kwargs)
+
+        results = None
+        try:
+            results = fn(self, *args, **kwargs)
+            return results
+        except fabric.group.GroupException as e:
+            results = e.result
+            raise
+        finally:
+            # if hide is False, we already logged only to stdout, and should log to other handlers.
+            if results is not None and not kwargs.get('hide', True):
+                logger.debug(results, extra={'ignore_stdout': True})
+
+    return do
+
+
 class NodeGroup:
 
     def __init__(self, connections: Connections, cluster):
         from kubemarine.core.cluster import KubernetesCluster
 
         self.cluster: KubernetesCluster = cluster
         self.nodes = connections
@@ -356,17 +394,19 @@
         group_result = self._make_result(results)
 
         if failed_hosts:
             raise fabric.group.GroupException(group_result)
 
         return group_result
 
+    @_handle_internal_logging
     def run(self, *args, **kwargs) -> Union[NodeGroupResult, int]:
         return self.do("run", *args, **kwargs)
 
+    @_handle_internal_logging
     def sudo(self, *args, **kwargs) -> Union[NodeGroupResult, int]:
         return self.do("sudo", *args, **kwargs)
 
     def put(self, local_file: Union[io.StringIO, str], remote_file: str, **kwargs):
         if isinstance(local_file, io.StringIO):
             self.cluster.log.verbose("Text is being transferred to remote file \"%s\" on nodes %s with options %s"
                                      % (remote_file, list(self.nodes.keys()), kwargs))
@@ -474,20 +514,15 @@
     def get(self, *args, **kwargs):
         return self.do("get", *args, **kwargs)
 
     def do(self, do_type, *args, **kwargs) -> Union[NodeGroupResult, int]:
         raw_results = self._do_with_wa(do_type, *args, **kwargs)
         if isinstance(raw_results, int):
             return raw_results
-        group_results = self._make_result_or_fail(raw_results, lambda host, result: isinstance(result, Exception))
-
-        if not kwargs.get('hide', True):
-            self.cluster.log.debug(group_results, extra={'ignore_stdout': True})
-
-        return group_results
+        return self._make_result_or_fail(raw_results, lambda host, result: isinstance(result, Exception))
 
     def _do_with_wa(self, do_type, *args, **kwargs) -> Union[_HostToResult, int]:
         # by default all code is async, but can be set False forcibly
         is_async = kwargs.pop("is_async", True) is not False
 
         left_nodes = self.nodes
         retry = 0
```

### Comparing `kubemarine-0.17.0/kubemarine/core/log.py` & `kubemarine-0.18.0/kubemarine/core/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,69 +78,90 @@
     logging.ERROR: 'error',
     logging.CRITICAL: 'critical'
 }
 
 
 class VerboseLogger(ABC):
     @abstractmethod
-    def verbose(self, msg: str, *args, **kwargs):
+    def verbose(self, msg, *args, **kwargs):
         pass
 
 
 class EnhancedLogger(logging.Logger, VerboseLogger):
     def __init__(self, name, level=logging.NOTSET):
         super().__init__(name, level)
         logging.addLevelName(VERBOSE, 'VERBOSE')
 
     def verbose(self, msg, *args, **kwargs):
         if self.isEnabledFor(VERBOSE):
             self._log(VERBOSE, msg, args, **kwargs)
 
+    def makeRecord(self, name: str, level: int, fn: str, lno: int, msg: object, args,
+                   exc_info, func=None, extra=None,
+                   sinfo=None) -> logging.LogRecord:
+        record = super().makeRecord(name, level, fn, lno, msg, args, exc_info, func, extra, sinfo)
+        caller = record.__dict__.get('real_caller')
+        if caller is not None:
+            record.__dict__.update(record.__dict__.pop('real_caller'))
+
+        return record
+
+
+class EnhancedLogRecord(logging.LogRecord):
+    def getMessage(self) -> str:
+        message = super().getMessage()
+        prefix = self.__dict__.get('prefix')
+        if prefix is not None:
+            message = prefix + message
+        return message
+
 
 logging.setLoggerClass(EnhancedLogger)
+logging.setLogRecordFactory(EnhancedLogRecord)
 
 
 class LogFormatter(logging.Formatter):
     def __init__(self, fmt=None, datefmt=None, style='%', colorize=False, correct_newlines=False):
         super().__init__(fmt, datefmt, style)
         self.colorize = colorize
         self.correct_newlines = correct_newlines
 
     def _format(self, record):
         s = super().format(record)
         if self.colorize and record.levelname in COLORS_SCHEME:
-            s = '$__COLOR_' + COLORS_SCHEME[record.levelname] + s + '$__COLOR_RESET'
-        for color_name, color_code in COLORS.items():
-            if self.colorize:
-                s = s.replace('$__COLOR_' + color_name, color_code)
-            else:
-                s = s.replace('$__COLOR_' + color_name, '')
+            s = COLORS[COLORS_SCHEME[record.levelname]] + s + COLORS['RESET']
         return s
 
     def format(self, record):
-        messages = str(record.msg).split('\n')
-        if self.correct_newlines and len(messages):
-            subrecord = logging.makeLogRecord(record.__dict__)
+        if self.correct_newlines:
+            messages = str(record.msg).split('\n')
+            if len(messages) == 1:
+                return self._format(record)
+        else:
+            return self._format(record)
+
+        orig_msg = record.msg
+        try:
             s = ''
             for message in messages:
                 if s != '':
                     s += '\n'
-                subrecord.msg = message
-                s += self._format(subrecord)
+                record.msg = message
+                s += self._format(record)
             return s
-        else:
-            return self._format(record)
+        finally:
+            record.msg = orig_msg
 
 
 class StdoutHandler(logging.StreamHandler):
     def __init__(self):
         super().__init__(sys.stdout)
 
     def emit(self, record):
-        if hasattr(record, 'ignore_stdout') and getattr(record, 'ignore_stdout'):
+        if 'ignore_stdout' in record.__dict__:
             return
         super().emit(record)
         # TODO: if output stuck, then add here self.flush()
         # More about, see at https://stackoverflow.com/questions/16633911
 
 
 class FileHandlerWithHeader(logging.FileHandler):
@@ -270,14 +291,38 @@
             handler.append_to_logger(self._logger)
 
     @property
     def logger(self) -> EnhancedLogger:
         return self._logger
 
 
+class LoggerWriter:
+    def __init__(self, logger: EnhancedLogger, level, caller: dict, prefix: str):
+        self.logger = logger
+        self.level = level
+        self.caller = caller
+        self.prefix = prefix
+        self.buf = ""
+
+    def write(self, message):
+        lines = message.split('\n')
+        for line in lines[:-1]:
+            self.buf = self.buf + line
+            self._log()
+        self.buf = self.buf + lines[-1]
+
+    def flush(self, remainder=False):
+        if remainder and self.buf:
+            self._log()
+
+    def _log(self):
+        self.logger.log(self.level, self.buf, extra={'real_caller': self.caller, 'prefix': self.prefix})
+        self.buf = ""
+
+
 def parse_log_argument(argument: str) -> LogHandler:
     """
     Parse raw CLI arguments and verify for required parameters
     :param argument: Raw CLI argument string. For example: test.log;level=verbose;colorize=true
     :return: Initialized LogHandler
     """
     parameters = {}
@@ -333,18 +378,29 @@
     debug_filepath = get_dump_debug_filepath(context)
     if debug_filepath:
         handlers.append(LogHandler(target=debug_filepath,
                                    **globals['logging']['default_targets']['dump']))
 
     if not stdout_specified:
         stdout_settings = deepcopy(globals['logging']['default_targets']['stdout'])
-        # Globals lacks of colorize property, so calculated value for Windows is "false".
-        # But it is still convenient to specify the value explicitly even for Windows for debugging purpose.
-        if 'colorize' not in stdout_settings:
-            stdout_settings['colorize'] = (os.name != 'nt')
         handlers.append(LogHandler(target='stdout', **stdout_settings))
 
     log = Log(raw_inventory, handlers)
 
     log.logger.verbose('Using the following loggers: \n\t%s' % "\n\t".join("- " + str(x) for x in handlers))
 
     return log
+
+
+def caller_info(logger: EnhancedLogger) -> dict:
+    """
+    Catches and returns invocation metadata of the method that calls caller_info()
+    """
+    fn, lno, func, sinfo = logger.findCaller()
+    record: logging.LogRecord = logger.makeRecord(None, None, fn, lno, "", (), None, func=func, extra=None, sinfo=sinfo)
+    return dict(item for item in record.__dict__.items()
+                if item[0] in (
+                    # record's fields describing invocation origin
+                    'pathname', 'filename', 'module', 'lineno', 'funcName', 'stack_info',
+                    # record's fields describing initial process and thread context
+                    'thread', 'threadName', 'process', 'processName'
+                ))
```

### Comparing `kubemarine-0.17.0/kubemarine/core/patch.py` & `kubemarine-0.18.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC, abstractmethod
-
-from kubemarine.core.action import Action
-
-
-class Patch(ABC):
-    def __init__(self, identifier: str):
-        self.identifier = identifier
-
-    @property
-    @abstractmethod
-    def action(self) -> Action:
-        pass
-
-    @property
-    @abstractmethod
-    def description(self) -> str:
-        pass
+# Check url availability script.
+# The script is for testing purpose only.
+# The first argv parameter is source. The second argv parameter is the timeout.
+
+import sys
+
+major_version = sys.version_info.major
+if major_version == 3:
+    import urllib.request as urllib
+else:
+    import urllib2 as urllib
+
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

### Comparing `kubemarine-0.17.0/kubemarine/core/resources.py` & `kubemarine-0.18.0/kubemarine/core/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,24 +107,27 @@
 
         Avoid using it directly, because cluster object and previous inventory will be lost,
         and post processing of actions may work incorrectly.
         """
         if self._formatted_inventory is None:
             return
 
-        # replace initial inventory file with changed inventory
-        with utils.open_external(self.inventory_filepath, "w+") as stream:
-            utils.yaml_structure_preserver().dump(self.formatted_inventory(), stream)
+        self._store_inventory()
 
         self._raw_inventory = None
         self._formatted_inventory = None
         # no need to clear _nodes_context as it should not change after cluster is reinitialized.
         # should not clear working_context as it can be inspected after execution.
         self._cluster = None
 
+    def _store_inventory(self):
+        # replace initial inventory file with changed inventory
+        with utils.open_external(self.inventory_filepath, "w+") as stream:
+            utils.yaml_structure_preserver().dump(self.formatted_inventory(), stream)
+
     def cluster_if_initialized(self) -> Optional[c.KubernetesCluster]:
         return self._cluster
 
     def cluster(self) -> c.KubernetesCluster:
         """Returns already initialized cluster object or initializes new real cluster object."""
         if self._cluster is None:
             self.working_context = deepcopy(self.context)
@@ -157,15 +160,15 @@
         except errors.FailException:
             raise
         except Exception as exc:
             raise errors.FailException("Failed to proceed inventory file", exc)
 
     def _create_cluster(self, context):
         log = self.logger()
-        context['nodes'] = deepcopy(self._get_nodes_context())
+        context['nodes'] = deepcopy(self.get_nodes_context())
         with self._handle_enrichment_error():
             cluster = self._new_cluster_instance(context)
             cluster.enrich()
 
         if not self._silent:
             log.debug("Inventory file loaded:")
             for role in cluster.roles:
@@ -175,25 +178,25 @@
 
         args = context['execution_arguments']
         if 'ansible_inventory_location' in args:
             utils.make_ansible_inventory(args['ansible_inventory_location'], cluster)
 
         return cluster
 
-    def _get_nodes_context(self):
+    def get_nodes_context(self):
         if self._nodes_context is None:
             with self._handle_enrichment_error():
                 # temporary cluster instance to detect initial nodes context.
                 light_cluster = self._new_cluster_instance(deepcopy(self.context))
                 light_cluster.enrich(custom_enrichment_fns=light_cluster.get_facts_enrichment_fns())
                 self._nodes_context = light_cluster.detect_nodes_context()
 
         return self._nodes_context
 
-    def _new_cluster_instance(self, context: dict):
+    def _new_cluster_instance(self, context: dict) -> c.KubernetesCluster:
         return _provide_cluster(self.raw_inventory(), context,
                                 procedure_inventory=self.procedure_inventory(),
                                 logger=self.logger())
 
     def _create_logger(self):
         return log.init_log_from_context_args(static.GLOBALS, self.context, self.raw_inventory()).logger
```

### Comparing `kubemarine-0.17.0/kubemarine/core/schema.py` & `kubemarine-0.18.0/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/static.py` & `kubemarine-0.18.0/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/summary.py` & `kubemarine-0.18.0/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/core/utils.py` & `kubemarine-0.18.0/kubemarine/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 import json
 import os
 import shutil
 import sys
 import time
 import tarfile
 
-from typing import Union, Tuple
+from typing import Tuple
 
 import yaml
 import ruamel.yaml
 from copy import deepcopy
 from datetime import datetime
 from collections import OrderedDict
 
 from ruamel.yaml import CommentedMap
 
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.errors import pretty_print_error
 
 
-def do_fail(message='', reason: Union[str, Exception] = '', hint='', log=None):
+def do_fail(message='', reason: Exception = None, hint='', log=None):
 
     if log:
         log.critical('FAILURE!')
         if message != "":
             log.critical(message)
     else:
         sys.stderr.write("\033[91mFAILURE!")
@@ -148,36 +148,38 @@
     config_compiled = ''
     for section_name, strings in config.items():
         config_compiled += '[%s]' % section_name
         for string in strings:
             config_compiled += '\n' + string
         config_compiled += '\n\n'
 
-    with open_external(location, 'w') as configfile:
-        configfile.write(config_compiled)
+    dump_file({}, config_compiled, location, dump_location=False)
 
 
 def get_current_timestamp_formatted():
     return datetime.now().strftime("%Y%m%d-%H%M%S")
 
 
 def get_final_inventory(cluster, initial_inventory=None):
     if initial_inventory is None:
         inventory = deepcopy(cluster.inventory)
     else:
         inventory = deepcopy(initial_inventory)
 
-    from kubemarine import admission
+    from kubemarine import admission, kubernetes, packages, plugins, thirdparties
     from kubemarine.plugins import nginx_ingress
-    from kubemarine.procedures import add_node, remove_node, upgrade, migrate_cri
+    from kubemarine.procedures import add_node, remove_node, migrate_cri
 
     inventory_finalize_functions = {
         add_node.add_node_finalize_inventory,
         remove_node.remove_node_finalize_inventory,
-        upgrade.upgrade_finalize_inventory,
+        kubernetes.upgrade_finalize_inventory,
+        thirdparties.upgrade_finalize_inventory,
+        plugins.upgrade_finalize_inventory,
+        packages.upgrade_finalize_inventory,
         admission.finalize_inventory,
         nginx_ingress.finalize_inventory,
         migrate_cri.migrate_cri_finalize_inventory
     }
 
     for finalize_fn in inventory_finalize_functions:
         inventory = finalize_fn(cluster, inventory)
@@ -191,47 +193,54 @@
     else:
         inventory["vrrp_ips"] = procedure_inventory["vrrp_ips"]
 
     if isinstance(inventory, OrderedDict):
         inventory.move_to_end("vrrp_ips", last=False)
 
 
-def dump_file(context, data, filename):
-    if not isinstance(context, dict):
-        # cluster is passed instead of the context directly
-        cluster = context
-        context = cluster.context
+def dump_file(context, data: object, filename: str,
+              *, dump_location=True):
+    if dump_location:
+        if not isinstance(context, dict):
+            # cluster is passed instead of the context directly
+            cluster = context
+            context = cluster.context
+
+        args = context['execution_arguments']
+        if args.get('disable_dump', True) \
+                and not (filename in ClusterStorage.PRESERVED_DUMP_FILES and context['preserve_inventory']):
+            return
+
+        prepare_dump_directory(args.get('dump_location'), reset_directory=False)
+        target_path = get_dump_filepath(context, filename)
+    else:
+        target_path = get_external_resource_path(filename)
 
     if isinstance(data, io.StringIO):
         data = data.getvalue()
     if isinstance(data, io.TextIOWrapper):
         data = data.read()
 
-    args = context['execution_arguments']
-    if not args.get('disable_dump', True) \
-            or (filename in ClusterStorage.PRESERVED_DUMP_FILES and context['preserve_inventory']):
-
-        prepare_dump_directory(args.get('dump_location'), reset_directory=False)
-        with open_utf8(get_dump_filepath(context, filename), 'w') as file:
-            file.write(data)
+    with open_utf8(target_path, 'w') as file:
+        file.write(data)
 
 
 def get_dump_filepath(context, filename):
     if context.get("dump_filename_prefix"):
         filename = f"{context['dump_filename_prefix']}_{filename}"
 
     return get_external_resource_path(os.path.join(context['execution_arguments']['dump_location'], 'dump', filename))
 
 
-def wait_command_successful(group, command, retries=15, timeout=5, warn=True, hide=False):
+def wait_command_successful(group, command, retries=15, timeout=5, warn=True, hide=False, is_async=True):
     log = group.cluster.log
 
     while retries > 0:
         log.debug("Waiting for command to succeed, %s retries left" % retries)
-        result = group.sudo(command, warn=warn, hide=hide)
+        result = group.sudo(command, warn=warn, hide=hide, is_async=is_async)
         exit_code = list(result.values())[0].exited
         if exit_code == 0:
             log.debug("Command succeeded")
             return
         retries = retries - 1
         time.sleep(timeout)
     raise Exception("Command failed")
```

### Comparing `kubemarine-0.17.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.18.0/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/coredns.py` & `kubemarine-0.18.0/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/cri/__init__.py` & `kubemarine-0.18.0/kubemarine/cri/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from kubemarine.core import static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroupResult
 from kubemarine.cri import docker, containerd
 
 
 def enrich_inventory(inventory, cluster):
     if cluster.context.get("initial_procedure") == "migrate_cri":
@@ -28,14 +29,22 @@
     for key, value in forbidden_cri_sections.items():
         if value in cluster.raw_inventory.get('services', {}).get('cri', {}):
             raise Exception(f"{key} is not used, please remove {value} config from `services.cri` section")
 
     return inventory
 
 
+def get_initial_cri_impl(inventory: dict) -> str:
+    cri_impl = inventory.get("services", {}).get("cri", {}).get("containerRuntime")
+    if cri_impl is None:
+        cri_impl = static.DEFAULTS['services']['cri']['containerRuntime']
+
+    return cri_impl
+
+
 def remove_invalid_cri_config(cluster: KubernetesCluster, inventory: dict):
     if inventory['services']['cri']['containerRuntime'] == 'docker':
         if inventory['services']['cri'].get('containerdConfig'):
             del inventory['services']['cri']['containerdConfig']
     elif inventory['services']['cri'].get('dockerConfig'):
         del inventory['services']['cri']['dockerConfig']
```

### Comparing `kubemarine-0.17.0/kubemarine/cri/containerd.py` & `kubemarine-0.18.0/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/cri/docker.py` & `kubemarine-0.18.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/demo.py` & `kubemarine-0.18.0/kubemarine/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
 import io
 import re
 import threading
 from copy import deepcopy
-from typing import List, Dict, Union, Any, IO
+from typing import List, Dict, Union, Any, IO, Optional
 
 import fabric
 from invoke import UnexpectedExit
 
+from kubemarine import system
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core import group, flow, connections
 from kubemarine.core.connections import Connections
 from kubemarine.core.group import NodeGroup, NodeGroupResult, _GenericResult, _HostToResult
 from kubemarine.core.resources import DynamicResources
 
 ShellResult = Dict[str, Union[NodeGroupResult, Any]]
@@ -32,15 +33,15 @@
 
 class FakeShell:
     def __init__(self):
         self.results: Dict[str, List[ShellResult]] = {}
         self.history: Dict[str, List[ShellResult]] = {}
         self._lock = threading.Lock()
 
-    def __deepcopy__(self, memodict={}):
+    def __deepcopy__(self, memodict: dict):
         cls = self.__class__
         result = cls.__new__(cls)
         memodict[id(self)] = result
         result.results = deepcopy(self.results, memodict)
         result.history = deepcopy(self.history, memodict)
         result._lock = threading.Lock()
         return result
@@ -113,15 +114,15 @@
 
 
 class FakeFS:
     def __init__(self):
         self.storage: Dict[str, Dict[str, str]] = {}
         self._lock = threading.Lock()
 
-    def __deepcopy__(self, memodict={}):
+    def __deepcopy__(self, memodict: dict):
         cls = self.__class__
         result = cls.__new__(cls)
         memodict[id(self)] = result
         result.storage = deepcopy(self.storage, memodict)
         result._lock = threading.Lock()
         return result
 
@@ -189,33 +190,40 @@
 
     def preserve_inventory(self):
         return
 
 
 class FakeResources(DynamicResources):
     def __init__(self, context, raw_inventory: dict, procedure_inventory: dict = None,
-                 cluster: KubernetesCluster = None,
+                 nodes_context: dict = None,
                  fake_shell: FakeShell = None, fake_fs: FakeFS = None):
         super().__init__(context, True)
         self.inventory_filepath = None
         self.procedure_inventory_filepath = None
-        self._raw_inventory = raw_inventory
-        self._formatted_inventory = raw_inventory
+        self.stored_inventory = raw_inventory
+        self.last_cluster: Optional[FakeKubernetesCluster] = None
+        self.fake_shell = fake_shell if fake_shell else FakeShell()
+        self.fake_fs = fake_fs if fake_fs else FakeFS()
+        self._nodes_context = nodes_context
         self._procedure_inventory = procedure_inventory
-        self._cluster = cluster
-        if cluster:
-            self._logger = cluster.log
-        self._fake_shell = fake_shell if fake_shell else FakeShell()
-        self._fake_fs = fake_fs if fake_fs else FakeFS()
-
-    def _new_cluster_instance(self, context: dict):
-        return FakeKubernetesCluster(self.raw_inventory(), context,
-                                     procedure_inventory=self.procedure_inventory(),
-                                     logger=self.logger(),
-                                     fake_shell=self._fake_shell, fake_fs=self._fake_fs)
+
+    def _load_inventory(self):
+        self._raw_inventory = deepcopy(self.stored_inventory)
+        self._formatted_inventory = deepcopy(self.stored_inventory)
+
+    def _store_inventory(self):
+        self.stored_inventory = deepcopy(self._formatted_inventory)
+
+    def _new_cluster_instance(self, context: dict) -> FakeKubernetesCluster:
+        self.last_cluster = FakeKubernetesCluster(
+            self.raw_inventory(), context,
+            procedure_inventory=self.procedure_inventory(), logger=self.logger(),
+            fake_shell=self.fake_shell, fake_fs=self.fake_fs
+        )
+        return self.last_cluster
 
 
 class FakeConnection(fabric.connection.Connection):
 
     def __init__(self, ip, cluster: FakeKubernetesCluster, **kw):
         super().__init__(ip, **kw)
         self.fake_shell = cluster.fake_shell
@@ -393,20 +401,15 @@
         cluster = KubernetesCluster(inventory, context, procedure_inventory=procedure_inventory)
 
     cluster.enrich()
     return cluster
 
 
 def generate_nodes_context(inventory: dict, os_name='centos', os_version='7.9', net_interface='eth0') -> dict:
-    os_family = None
-
-    if os_name in ['centos', 'rhel']:
-        os_family = 'rhel'
-    elif os_name in ['ubuntu', 'debian']:
-        os_family = 'debian'
+    os_family = system.detect_of_family_by_name_version(os_name, os_version)
 
     context = {}
     for node in inventory['nodes']:
         node_context = {
             'access': {
                 'online': True,
                 'accessible': True,
```

### Comparing `kubemarine-0.17.0/kubemarine/etcd.py` & `kubemarine-0.18.0/kubemarine/etcd.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             command = "etcdctl member remove " + etcd_members[node_name]
             log.verbose(f"Removing found etcd member {node_name}...")
             managing_control_plane.sudo(command)
         else:
             log.verbose(f"Skipping {node_name} as it is not among etcd members.")
 
 
-def wait_for_health(cluster: KubernetesCluster, connection: fabric.connection.Connection) -> List[Dict]:
+def wait_for_health(cluster: KubernetesCluster, connection: NodeGroup) -> List[Dict]:
     """
     The method checks etcd endpoints health until all endpoints are healthy or retries are exhausted
     if all member are healthy the method checks the leader.
     """
     log = cluster.log
     init_timeout = cluster.globals['etcd']['health']['init_timeout']
     timeout = cluster.globals['etcd']['health']['timeout']
```

### Comparing `kubemarine-0.17.0/kubemarine/haproxy.py` & `kubemarine-0.18.0/kubemarine/haproxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import io
 import time
 
 from jinja2 import Template
 
 from kubemarine import system, packages
-from kubemarine.core import utils
+from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroupResult, NodeGroup
 
 ERROR_VRRP_IS_NOT_CONFIGURED = \
     'Balancer is combined with other role, but there is no VRRP IP configured for node \'%s\'.'
 
@@ -150,22 +150,24 @@
     return installation_result
 
 
 def uninstall(group):
     return packages.remove(group, include=['haproxy', 'rh-haproxy18'])
 
 
-def restart(group):
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        service_name = _get_associations_for_node(node)['service_name']
-        system.restart_service(node['connection'], name=service_name)
-    RemoteExecutor(group.cluster).flush()
-    group.cluster.log.debug("Sleep while haproxy comes-up...")
-    time.sleep(group.cluster.globals['haproxy']['restart_wait'])
-    return
+def restart(group: NodeGroup):
+    cluster = group.cluster
+    cluster.log.debug("Restarting haproxy in all group...")
+    with RemoteExecutor(cluster):
+        for node in group.get_ordered_members_list(provide_node_configs=True):
+            service_name = _get_associations_for_node(node)['service_name']
+            system.restart_service(node['connection'], name=service_name)
+
+    cluster.log.debug("Sleep while haproxy comes-up...")
+    time.sleep(static.GLOBALS['haproxy']['restart_wait'])
 
 
 def disable(group):
     with RemoteExecutor(group.cluster):
         for node in group.get_ordered_members_list(provide_node_configs=True):
             service_name = _get_associations_for_node(node)['service_name']
             system.disable_service(node['connection'], name=service_name)
```

### Comparing `kubemarine-0.17.0/kubemarine/k8s_certs.py` & `kubemarine-0.18.0/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/keepalived.py` & `kubemarine-0.18.0/kubemarine/keepalived.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import io
 import random
 import time
 
 from jinja2 import Template
 
 from kubemarine import system, packages
-from kubemarine.core import utils
+from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroup, NodeGroupResult
 
 
 def autodetect_interface(cluster: KubernetesCluster, name):
     for node in cluster.inventory['nodes']:
@@ -189,22 +189,24 @@
 
 
 def uninstall(group):
     return packages.remove(group, include='keepalived')
 
 
 def restart(group: NodeGroup):
-    results = NodeGroupResult(group.cluster)
-    for node in group.get_ordered_members_list(provide_node_configs=True):
-        service_name = group.cluster.get_package_association_for_node(
-            node['connect_to'], 'keepalived', 'service_name')
-        results.update(system.restart_service(node['connection'], name=service_name))
-        group.cluster.log.debug("Sleep while keepalived comes-up...")
-        time.sleep(group.cluster.globals['keepalived']['restart_wait'])
-    return results
+    cluster = group.cluster
+    cluster.log.debug("Restarting keepalived in all group...")
+    with RemoteExecutor(cluster):
+        for node in group.get_ordered_members_list(provide_node_configs=True):
+            service_name = group.cluster.get_package_association_for_node(
+                node['connect_to'], 'keepalived', 'service_name')
+            system.restart_service(node['connection'], name=service_name)
+
+    cluster.log.debug("Sleep while keepalived comes-up...")
+    time.sleep(static.GLOBALS['keepalived']['restart_wait'])
 
 
 def enable(group: NodeGroup):
     with RemoteExecutor(group.cluster):
         for node in group.get_ordered_members_list(provide_node_configs=True):
             service_name = group.cluster.get_package_association_for_node(
                 node['connect_to'], 'keepalived', 'service_name')
@@ -272,11 +274,10 @@
             config = generate_config(group.cluster.inventory, node)
             utils.dump_file(group.cluster, config, 'keepalived_%s.conf' % node['name'])
 
             node['connection'].put(io.StringIO(config), package_associations['config_location'], sudo=True)
 
     log.debug(group.sudo('ls -la %s' % package_associations['config_location']))
 
-    log.debug("Restarting keepalived in all group...")
     restart(group)
 
     return group.sudo('systemctl status %s' % package_associations['service_name'], warn=True)
```

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.18.0/kubemarine/kubernetes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import math
 import os
 import time
+import uuid
+from contextlib import contextmanager
 from copy import deepcopy
-from typing import List, Dict, Tuple
+from typing import List, Dict, Tuple, ContextManager
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 import ipaddress
 
 from kubemarine import system, plugins, admission, etcd, packages
@@ -63,26 +65,35 @@
     for i, node in enumerate(inventory['nodes']):
         if node['name'] in node_names_to_remove:
             inventory['nodes'][i]['roles'].append('remove_node')
 
     return inventory
 
 
-def enrich_upgrade_inventory(inventory, cluster):
+def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get('initial_procedure') == 'upgrade':
-        if not inventory.get('services'):
-            inventory['services'] = {}
-        if not inventory['services'].get('kubeadm'):
-            inventory['services']['kubeadm'] = {}
         cluster.context['initial_kubernetes_version'] = inventory['services']['kubeadm']['kubernetesVersion']
-        inventory['services']['kubeadm']['kubernetesVersion'] = cluster.context['upgrade_version']
 
         cluster.log.info(
             '------------------------------------------\nUPGRADING KUBERNETES %s ⭢ %s\n------------------------------------------' % (
             cluster.context['initial_kubernetes_version'], cluster.context['upgrade_version']))
+
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def upgrade_finalize_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def generic_upgrade_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    if cluster.context.get("initial_procedure") != "upgrade":
+        return inventory
+
+    upgrade_version = cluster.context.get("upgrade_version")
+    inventory.setdefault("services", {}).setdefault("kubeadm", {})['kubernetesVersion'] = upgrade_version
     return inventory
 
 
 def enrich_inventory(inventory, cluster):
     repository = inventory['services']['kubeadm'].get('imageRepository', "")
     if repository:
         inventory['services']['kubeadm']['dns'] = {}
@@ -272,18 +283,18 @@
 
     stdout = list(result.values())[0].stdout
     log.verbose("Detected the following nodes in cluster:\n%s" % stdout)
 
     for node in group.get_ordered_members_list(provide_node_configs=True):
         if node["name"] in stdout:
             log.debug("Draining node %s..." % node["name"])
-            control_plane.sudo(prepare_drain_command(node, group.cluster.inventory['services']['kubeadm']['kubernetesVersion'],
-                                              group.cluster.globals, disable_eviction, group.cluster.nodes,
-                                              drain_timeout, grace_period),
-                        hide=False)
+            drain_cmd = prepare_drain_command(
+                group.cluster, node["name"],
+                disable_eviction=disable_eviction, drain_timeout=drain_timeout, grace_period=grace_period)
+            control_plane.sudo(drain_cmd, hide=False)
         else:
             log.warning("Node %s is not found in cluster and can't be drained" % node["name"])
 
     return control_plane.sudo("kubectl get nodes")
 
 
 def delete_nodes(group):
@@ -433,14 +444,31 @@
             node['connection'].sudo("systemctl restart kubelet")
             copy_admin_config(log, node['connection'])
        
 
     wait_for_any_pods(group.cluster, node['connection'], apply_filter=node['name'])
 
 
+@contextmanager
+def local_admin_config(node: NodeGroup) -> ContextManager[str]:
+    temp_filepath = "/tmp/%s" % uuid.uuid4().hex
+
+    cluster_name = node.cluster.inventory['cluster_name']
+    internal_address = node.get_first_member(provide_node_configs=True)['internal_address']
+    if type(ipaddress.ip_address(internal_address)) is ipaddress.IPv6Address:
+        internal_address = f"[{internal_address}]"
+
+    try:
+        node.sudo(f"cp /root/.kube/config {temp_filepath} "
+                  f"&& sudo sed -i 's/{cluster_name}/{internal_address}/' {temp_filepath}")
+        yield temp_filepath
+    finally:
+        node.sudo(f'rm -f {temp_filepath}')
+
+
 def copy_admin_config(log, nodes):
     log.debug("Setting up admin-config...")
     nodes.sudo("mkdir -p /root/.kube && sudo cp -f /etc/kubernetes/admin.conf /root/.kube/config")
 
 
 def fetch_admin_config(cluster: KubernetesCluster) -> str:
     log = cluster.log
@@ -455,17 +483,15 @@
     if public_cluster_ip:
         if type(ipaddress.ip_address(public_cluster_ip)) is ipaddress.IPv6Address:
             public_cluster_ip = f"[{public_cluster_ip}]"
         cluster_name = cluster.inventory['cluster_name']
         kubeconfig = kubeconfig.replace(cluster_name, public_cluster_ip)
 
     kubeconfig_filename = os.path.abspath("kubeconfig")
-    with utils.open_external(kubeconfig_filename, 'w') as f:
-        f.write(kubeconfig)
-
+    utils.dump_file(cluster.context, kubeconfig, kubeconfig_filename, dump_location=False)
     cluster.log.debug(f"Kubeconfig saved to {kubeconfig_filename}")
 
     return kubeconfig_filename
 
 
 def get_join_dict(group):
     first_control_plane = group.cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
@@ -582,14 +608,25 @@
         'kube-scheduler',
         'etcd'
     ], node=connection, apply_filter=apply_filter,
                         timeout=cluster.inventory['globals']['expect']['pods']['kubernetes']['timeout'],
                         retries=cluster.inventory['globals']['expect']['pods']['kubernetes']['retries'])
 
 
+def wait_uncordon(node: NodeGroup):
+    cluster = node.cluster
+    timeout_config = cluster.inventory['globals']['expect']['pods']['kubernetes']
+    # This forces to use local API server and waits till it is up.
+    with local_admin_config(node) as kubeconfig:
+        utils.wait_command_successful(node, f"kubectl --kubeconfig {kubeconfig} uncordon {node.get_node_name()}",
+                                      is_async=False, hide=False,
+                                      timeout=timeout_config['timeout'],
+                                      retries=timeout_config['retries'])
+
+
 def wait_for_nodes(group: NodeGroup):
     log = group.cluster.log
 
     first_control_plane = group.cluster.nodes["control-plane"].get_first_member()
     node_names = group.get_nodes_names()
 
     wait_conditions = {
@@ -746,16 +783,17 @@
 
 
 def get_kubeadm_config(inventory):
     kubeadm_kubelet = yaml.dump(inventory["services"]["kubeadm_kubelet"], default_flow_style=False)
     kubeadm = yaml.dump(inventory["services"]["kubeadm"], default_flow_style=False)
     return f'{kubeadm_kubelet}---\n{kubeadm}'
 
-def upgrade_first_control_plane(version, upgrade_group, cluster, kubeadm_file,
-                                minor_version, drain_timeout=None, grace_period=None):
+
+def upgrade_first_control_plane(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+    version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
 
     if not upgrade_group.has_node(first_control_plane['name']):
         cluster.log.debug("First control-plane \"%s\" upgrade is not required" % first_control_plane['name'])
         return
 
     cluster.log.debug("Upgrading first control-plane \"%s\"" % first_control_plane)
@@ -769,63 +807,56 @@
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s'" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
     else:
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s' --patches=/etc/kubernetes/patches" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
 
     if patch_kubeadm_configmap(first_control_plane, cluster):
         flags += " --config /tmp/kubeadm_config.yaml"
 
-    disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
-    drain_cmd = prepare_drain_command(first_control_plane, version, cluster.globals, disable_eviction, cluster.nodes,
-                                      drain_timeout, grace_period)
+    drain_cmd = prepare_drain_command(cluster, first_control_plane['name'], **drain_kwargs)
     first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
     upgrade_cri_if_required(first_control_plane['connection'])
 
     # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
-
-    if minor_version == 27:
-        fix_flag_kubelet(first_control_plane, kubeadm_file)
+    fix_flag_kubelet(cluster, first_control_plane)
 
     first_control_plane['connection'].sudo(f"sudo kubeadm upgrade apply {version} {flags} && "
                                     f"sudo kubectl uncordon {first_control_plane['name']} && "
                                     f"sudo systemctl restart kubelet", is_async=False, hide=False)
 
     copy_admin_config(cluster.log, first_control_plane['connection'])
 
     expect_kubernetes_version(cluster, version, apply_filter=first_control_plane['name'])
     wait_for_any_pods(cluster, first_control_plane['connection'], apply_filter=first_control_plane['name'])
     exclude_node_from_upgrade_list(first_control_plane['connection'], first_control_plane['name'])
 
 
-def upgrade_other_control_planes(version, upgrade_group, cluster, kubeadm_file,
-                                 minor_version, drain_timeout=None, grace_period=None):
+def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+    version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
 
     for node in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
         if node['name'] != first_control_plane['name']:
 
             if not upgrade_group.has_node(node['name']):
                 cluster.log.debug("Control-plane \"%s\" upgrade is not required" % node['name'])
                 continue
 
             cluster.log.debug("Upgrading control-plane \"%s\"" % node['name'])
 
             # put control-plane patches
             create_kubeadm_patches_for_node(cluster, node)
 
-            disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
-            drain_cmd = prepare_drain_command(node, version, cluster.globals, disable_eviction, cluster.nodes,
-                                              drain_timeout, grace_period)
+            drain_cmd = prepare_drain_command(cluster, node['name'], **drain_kwargs)
             node['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
             upgrade_cri_if_required(node['connection'])
 
             # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
-            if minor_version == 27:
-                fix_flag_kubelet(node, kubeadm_file)
+            fix_flag_kubelet(cluster, node)
 
             # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
             # and only "else" branch remains
             if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
                 node['connection'].sudo(f"sudo kubeadm upgrade node --certificate-renewal=true && "
                                     f"sudo sed -i 's/--bind-address=.*$/--bind-address={node['internal_address']}/' "
                                     f"/etc/kubernetes/manifests/kube-apiserver.yaml && "
@@ -880,39 +911,37 @@
     ryaml.dump(cluster_config, updated_config)
     result_config = kubelet_config + "---\n" + updated_config.getvalue()
     first_control_plane["connection"].put(io.StringIO(result_config), "/tmp/kubeadm_config.yaml", sudo=True)
 
     return True
 
 
-def upgrade_workers(version, upgrade_group, cluster, kubeadm_file, minor_version, drain_timeout=None, grace_period=None):
+def upgrade_workers(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+    version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
 
     for node in cluster.nodes.get('worker').exclude_group(cluster.nodes['control-plane']).get_ordered_members_list(
             provide_node_configs=True):
 
         if not upgrade_group.has_node(node['name']):
             cluster.log.debug("Worker \"%s\" upgrade is not required" % node['name'])
             continue
 
         cluster.log.debug("Upgrading worker \"%s\"" % node['name'])
 
         # put control-plane patches
         create_kubeadm_patches_for_node(cluster, node)
 
-        disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
-        drain_cmd = prepare_drain_command(node, version, cluster.globals, disable_eviction, cluster.nodes,
-                                          drain_timeout, grace_period)
+        drain_cmd = prepare_drain_command(cluster, node['name'], **drain_kwargs)
         first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
         upgrade_cri_if_required(node['connection'])
 
         # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
-        if minor_version == 27:
-            fix_flag_kubelet(node, kubeadm_file)
+        fix_flag_kubelet(cluster, node)
 
         # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
         # and only "else" branch remains
         if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
             node['connection'].sudo("kubeadm upgrade node --certificate-renewal=true && "
                                 "sudo systemctl restart kubelet")
         else:
@@ -922,40 +951,44 @@
         first_control_plane['connection'].sudo("kubectl uncordon %s" % node['name'], is_async=False, hide=False)
 
         expect_kubernetes_version(cluster, version, apply_filter=node['name'])
         # workers do not have system pods to wait for their start
         exclude_node_from_upgrade_list(first_control_plane, node['name'])
 
 
-def prepare_drain_command(node, version: str, globals, disable_eviction: bool, nodes,
+def prepare_drain_command(cluster: KubernetesCluster, node_name: str,
+                          *,
+                          disable_eviction=False,
                           drain_timeout: int = None, grace_period: int = None):
-    drain_globals = globals['nodes']['drain']
+    drain_globals = static.GLOBALS['nodes']['drain']
     if drain_timeout is None:
-        drain_timeout = recalculate_proper_timeout(nodes, drain_globals['timeout'])
+        drain_timeout = recalculate_proper_timeout(cluster.nodes, drain_globals['timeout'])
+
     if grace_period is None:
         grace_period = drain_globals['grace_period']
-    drain_cmd = f"kubectl drain {node['name']} --force --ignore-daemonsets --delete-emptydir-data " \
+
+    drain_cmd = f"kubectl drain {node_name} --force --ignore-daemonsets --delete-emptydir-data " \
                 f"--timeout={drain_timeout}s --grace-period={grace_period}"
-    if version and disable_eviction:
+    if disable_eviction:
         drain_cmd += " --disable-eviction=true"
     return drain_cmd
 
 
-def upgrade_cri_if_required(group):
+def upgrade_cri_if_required(group: NodeGroup):
     # currently it is invoked only for single node
     cluster = group.cluster
     log = cluster.log
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
 
     if cri_impl in cluster.context["packages"]["upgrade_required"]:
         cri_packages = cluster.get_package_association_for_node(group.get_host(), cri_impl, 'package_name')
 
-        log.debug(f"Installing {cri_packages}")
+        log.debug(f"Installing {cri_packages} on node: {group.get_node_name()}")
         packages.install(group, include=cri_packages)
-        log.debug(f"Restarting all containers on nodes: {group.get_nodes_names()}")
+        log.debug(f"Restarting all containers on node: {group.get_node_name()}")
         if cri_impl == "docker":
             group.sudo("docker container rm -f $(sudo docker container ls -q)", warn=True)
         else:
             group.sudo("crictl rm -fa", warn=True)
     else:
         log.debug(f"{cri_impl} upgrade is not required")
 
@@ -1348,14 +1381,20 @@
             node['connection'].put(io.StringIO(control_plane_patch + "\n"), '/etc/kubernetes/patches/' +
                                  control_plane_patch_files[control_plane_item], sudo=True)
             node['connection'].sudo('chmod 644 /etc/kubernetes/patches/' +
                                  control_plane_patch_files[control_plane_item])
 
     return
 
-def fix_flag_kubelet(node, kubeadm_file):
-
+def fix_flag_kubelet(cluster: KubernetesCluster, node: dict):
     #Deprecated flag removal function for kubelet
+    kubeadm_file = "/var/lib/kubelet/kubeadm-flags.env"
+    version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
+
+    if utils.version_key(version) < utils.version_key("v1.27.0"):
+        # Target version is lower than v1.27.0. Flag is actual and should not be removed.
+        return
+
     kubeadm_flags = node['connection'].sudo(f"cat {kubeadm_file}", is_async=False).get_simple_out()
     if kubeadm_flags.find('--container-runtime=remote') != -1:
         kubeadm_flags = kubeadm_flags.replace('--container-runtime=remote', '')
-        node['connection'].put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
+        node['connection'].put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
```

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.18.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.18.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/object.py` & `kubemarine-0.18.0/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.18.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.18.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.18.0/kubemarine/kubernetes_accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,13 +113,12 @@
             'name': account['name'],
             'role': account['role'],
             'namespace': account['namespace'],
             'token': token,
         })
 
     cluster.log.debug('\nSaving tokens...')
-    token_filename = os.path.abspath('account-tokens.yaml')
-    with utils.open_external(token_filename, 'w') as tokenfile:
-        tokenfile.write(yaml.dump(tokens, default_flow_style=False))
-        cluster.log.debug('Tokens saved to %s' % token_filename)
+    token_filename = utils.get_external_resource_path('account-tokens.yaml')
+    utils.dump_file(cluster.context, yaml.dump(tokens), token_filename, dump_location=False)
+    cluster.log.debug('Tokens saved to %s' % token_filename)
 
     summary.schedule_report(cluster.context, summary.SummaryItem.ACCOUNT_TOKENS, token_filename)
```

### Comparing `kubemarine-0.17.0/kubemarine/packages.py` & `kubemarine-0.18.0/kubemarine/packages.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from copy import deepcopy
-from typing import List, Dict
+from typing import List, Dict, Tuple
 
 import fabric
 
 from kubemarine import yum, apt
+from kubemarine.core import errors, utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroup, NodeGroupResult
 from kubemarine.core.yaml_merger import default_merger
 
 
 ERROR_GLOBAL_ASSOCIATIONS_REDEFINED_MULTIPLE_OS = \
@@ -32,14 +33,21 @@
     "Multiple package versions detected %s for package '%s'. " \
     "Align them to the single version manually or using corresponding task of install procedure. " \
     "Alternatively, specify cache_versions=false for corresponding association."
 
 ERROR_SEMANAGE_NOT_MANAGED_DEBIAN = "semanage is not managed for debian OS family by KubeMarine"
 
 
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
+    enrich_inventory_associations(inventory, cluster)
+    enrich_inventory_packages(inventory, cluster)
+
+    return inventory
+
+
 def enrich_inventory_associations(inventory, cluster: KubernetesCluster):
     associations: dict = inventory['services']['packages']['associations']
     enriched_associations = {}
 
     # Move associations for OS families and merge with globals
     for association_name in get_associations_os_family_keys():
         os_associations: dict = deepcopy(cluster.globals['packages']['common_associations'])
@@ -60,37 +68,231 @@
             default_merger.merge(enriched_associations[os_family], associations)
 
     if 'semanage' in enriched_associations['debian']:
         raise Exception(ERROR_SEMANAGE_NOT_MANAGED_DEBIAN)
 
     inventory['services']['packages']['associations'] = enriched_associations
 
-    return inventory
-
 
 def enrich_inventory_packages(inventory: dict, _):
     for _type in ['install', 'upgrade', 'remove']:
         packages_list = inventory['services']['packages'].get(_type)
         if isinstance(packages_list, list):
             inventory['services']['packages'][_type] = {
                 'include': packages_list
             }
 
+
+def enrich_inventory_apply_defaults(inventory: dict, _) -> dict:
+    kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
+
+    for os_family in get_associations_os_family_keys():
+        cluster_associations = inventory["services"]["packages"]["associations"][os_family]
+        for package in static.GLOBALS['packages'][os_family]:
+            if cluster_associations[package].get('package_name') is None:
+                cluster_associations[package]['package_name'] = \
+                    get_default_package_names(os_family, package, kubernetes_version)
+
+    return inventory
+
+
+def _get_associations_upgrade_plan(cluster: KubernetesCluster, inventory: dict) -> List[Tuple[str, dict]]:
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        upgrade_version = context["upgrade_version"]
+        upgrade_plan = []
+        for version in cluster.procedure_inventory.get('upgrade_plan'):
+            if utils.version_key(version) < utils.version_key(upgrade_version):
+                continue
+
+            upgrade_associations = cluster.procedure_inventory.get(version, {}).get("packages", {}).get("associations", {})
+            upgrade_associations = dict(item for item in upgrade_associations.items()
+                                        if item[0] in _get_system_packages_support_upgrade(inventory))
+            upgrade_plan.append((version, upgrade_associations))
+
+    elif context.get("initial_procedure") == "migrate_kubemarine" and "upgrading_package" in context:
+        upgrade_associations = cluster.procedure_inventory.get('upgrade', {}).get("packages", {}).get("associations", {})
+        upgrade_associations = dict(item for item in upgrade_associations.items()
+                                    if item[0] == context["upgrading_package"])
+        upgrade_plan = [("", upgrade_associations)]
+    else:
+        upgrade_plan = []
+
+    return upgrade_plan
+
+
+def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
+    upgrade_plan = _get_associations_upgrade_plan(cluster, inventory)
+    if not upgrade_plan:
+        return inventory
+
+    os_family = cluster.get_os_family()
+    if os_family not in get_associations_os_family_keys():
+        raise errors.KME("KME0012")
+
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        previous_version = context["initial_kubernetes_version"]
+        packages_verify = _get_system_packages_support_upgrade(inventory)
+    else:  # migrate_kubemarine procedure
+        previous_version = ""
+        packages_verify = [context["upgrading_package"]]
+
+    cluster_associations = inventory["services"]["packages"]["associations"][os_family]
+    _verify_upgrade_plan(cluster_associations, previous_version, packages_verify, upgrade_plan)
+
+    upgrade_required = get_system_packages_for_upgrade(cluster, inventory)
+    context["packages"] = {"upgrade_required": upgrade_required}
+
+    # Merge procedure associations with the OS family specific section of associations in the inventory.
+    upgrade_inventory_associations(cluster, inventory, enrich_global=False)
+    upgrade_inventory_packages(cluster, inventory)
+
     return inventory
 
 
+def upgrade_inventory_associations(cluster: KubernetesCluster, inventory: dict,
+                                   *, enrich_global: bool):
+    # pass enriched 'cluster.inventory' instead of 'inventory' that is being finalized
+    upgrade_plan = _get_associations_upgrade_plan(cluster, cluster.inventory)
+    if not upgrade_plan:
+        return
+
+    _, upgrade_associations = upgrade_plan[0]
+    if upgrade_associations:
+        cluster_associations = inventory.setdefault("services", {}).setdefault("packages", {}) \
+            .setdefault("associations", {})
+        if not enrich_global:
+            cluster_associations = cluster_associations.setdefault(cluster.get_os_family(), {})
+        default_merger.merge(cluster_associations, upgrade_associations)
+
+
+def upgrade_inventory_packages(cluster: KubernetesCluster, inventory: dict):
+    if cluster.context.get("initial_procedure") != "upgrade":
+        return
+
+    upgrade_version = cluster.context["upgrade_version"]
+    for _type in ['install', 'upgrade', 'remove']:
+        packages_section = cluster.procedure_inventory.get(upgrade_version, {}).get("packages", {})
+        upgrade_packages = packages_section.get(_type)
+        if upgrade_packages is None:
+            continue
+        if isinstance(upgrade_packages, list):
+            upgrade_packages = {'include': upgrade_packages}
+
+        packages_section = inventory.setdefault("services", {}).setdefault("packages", {})
+        inventory_packages = packages_section.setdefault(_type, {})
+        if isinstance(inventory_packages, list):
+            packages_section[_type] = inventory_packages = {
+                'include': inventory_packages
+            }
+
+        default_merger.merge(inventory_packages, upgrade_packages)
+
+
+def _verify_upgrade_plan(cluster_associations: dict, previous_version: str,
+                         packages_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+    cluster_associations = deepcopy(cluster_associations)
+
+    # validate all packages sections in procedure inventory
+    for version, upgrade_associations in upgrade_plan:
+        for package in packages_verify:
+            upgrade_package_name = upgrade_associations.get(package, {}).get('package_name')
+            # Here default package names are not yet enriched and thus hold the custom supplied package names.
+            if cluster_associations[package].get('package_name') and not upgrade_package_name:
+                raise errors.KME("KME0010", package=package,
+                                 previous_version_spec=f' for version {previous_version}' if previous_version else "",
+                                 next_version_spec=f' for version {version}' if version else "")
+            if upgrade_package_name:
+                cluster_associations[package]['package_name'] = upgrade_package_name
+        previous_version = version
+
+
+def get_default_package_names(os_family: str, package: str, kubernetes_version: str) -> List[str]:
+    version_key = get_compatibility_version_key(os_family)
+    compatibility = static.GLOBALS['compatibility_map']['software']
+    packages_names = static.GLOBALS['packages'][os_family][package]['package_name']
+
+    package_versions = []
+    for kv in packages_names:
+        package_name, software_name = list(kv.items())[0]
+        if software_name in ('haproxy', 'keepalived'):
+            version = compatibility[software_name][version_key]
+        else:
+            version = compatibility[software_name][kubernetes_version][version_key]
+
+        package_versions.append(f"{package_name}{get_package_version_separator(os_family)}{version}")
+
+    return package_versions
+
+
+def get_system_packages_for_upgrade(cluster: KubernetesCluster, inventory: dict) -> List[str]:
+    undefined_package_name = object()
+
+    context = cluster.context
+    os_family = cluster.get_os_family()
+
+    cluster_associations = inventory['services']['packages']['associations'][os_family]
+    _, upgrade_associations = _get_associations_upgrade_plan(cluster, inventory)[0]
+
+    # Resolve old and new packages with versions and schedule for upgrade if they are not equal.
+    system_packages = _get_system_packages_support_upgrade(inventory)
+    upgrade_required = []
+    for package in system_packages:
+        # Here default package names are not yet enriched and thus hold the custom supplied package names.
+        old_package_name = cluster_associations[package].get('package_name')
+        if old_package_name is None:
+            # Trying enrichment before upgrade
+            if context.get("initial_procedure") == "migrate_kubemarine":
+                # Recommended versions have changed, and we forgot about what versions were previously recommended.
+                old_package_name = undefined_package_name
+            else:
+                # upgrade procedure
+                previous_ver = context["initial_kubernetes_version"]
+                old_package_name = get_default_package_names(os_family, package, previous_ver)
+
+        new_package_name = cluster_associations[package].get('package_name')
+        # associations from procedure inventory have priority
+        upgrade_package_name = upgrade_associations.get(package, {}).get('package_name')
+        if upgrade_package_name:
+            new_package_name = upgrade_package_name
+        if new_package_name is None:
+            # For upgrade procedure, services.kubeadm.kubernetesVersion is equal to 'upgrade_version',
+            # because the version was already enriched.
+            upgrade_ver = inventory['services']['kubeadm']['kubernetesVersion']
+            new_package_name = get_default_package_names(os_family, package, upgrade_ver)
+
+        if old_package_name is undefined_package_name or old_package_name != new_package_name:
+            upgrade_required.append(package)
+
+    return upgrade_required
+
+
+def _get_system_packages_support_upgrade(inventory: dict):
+    return [inventory['services']['cri']['containerRuntime'], 'haproxy', 'keepalived']
+
+
 def enrich_inventory_include_all(inventory: dict, _):
     for _type in ['upgrade', 'remove']:
         packages: dict = inventory['services']['packages'].get(_type)
         if packages is not None:
             packages.setdefault('include', ['*'])
 
     return inventory
 
 
+def upgrade_finalize_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    # Despite we enrich OS specific section inside enrich_upgrade_inventory(),
+    # we still merge global associations section because it has priority during enrichment.
+    upgrade_inventory_associations(cluster, inventory, enrich_global=True)
+    upgrade_inventory_packages(cluster, inventory)
+
+    return inventory
+
+
 def cache_package_versions(cluster: KubernetesCluster, inventory: dict, by_initial_nodes=False) -> dict:
     os_ids = cluster.get_os_identifiers()
     different_os = list(set(os_ids.values()))
     if len(different_os) > 1:
         cluster.log.debug(f"Final nodes have different OS families or versions, packages will not be cached. "
                           f"List of (OS family, version): {different_os}")
         return inventory
@@ -283,14 +485,26 @@
     return inventory
 
 
 def get_associations_os_family_keys():
     return {'debian', 'rhel', 'rhel8'}
 
 
+def get_compatibility_version_key(os_family: str) -> str:
+    """
+    Get os-specific version key to be used in software compatibility map.
+    :param os_family: one of supported OS families
+    :return: String to use as version key.
+    """
+    if os_family in get_associations_os_family_keys():
+        return f"version_{os_family}"
+    else:
+        raise ValueError(f"Unsupported {os_family!r} OS family")
+
+
 def get_package_manager(group: NodeGroup) -> apt or yum:
     os_family = group.get_nodes_os()
 
     if os_family in ['rhel', 'rhel8']:
         return yum
     elif os_family == 'debian':
         return apt
@@ -415,23 +629,27 @@
         for i, package in enumerate(packages_list):
             node_detected_package = _parse_node_detected_package(multiple_results[i], package)
             results.setdefault(package, {}).setdefault(node_detected_package, []).append(host)
 
     return results
 
 
+def get_package_version_separator(os_family: str) -> str:
+    return '=' if os_family == 'debian' else '-'
+
+
 def get_package_name(os_family: str, package: str) -> str:
     """
     Return the pure package name, without any part of version
     """
 
     import re
 
     package_name = ""
-    
+
     if package:
         if os_family in ["rhel", "rhel8"]:
             # regexp is needed to split package and its version, the pattern start with '-' then should be number or '*'
             package_name = re.split(r'-[\d,\*]', package)[0]
         else:
             # in ubuntu it is much easier to parse package name
             package_name = package.split("=")[0]
```

### Comparing `kubemarine-0.17.0/kubemarine/patches/__init__.py` & `kubemarine-0.18.0/kubemarine/patches/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 
 from typing import List
 
 from kubemarine.core.patch import Patch
 
 patches: List[Patch] = [
 ]
-"""List of patches which can be executed strictly in the declared order"""
+"""
+List of patches that is sorted according to the Patch.priority() before execution.
+Patches that have the same priority, are executed in the declared order.
+"""
```

### Comparing `kubemarine-0.17.0/kubemarine/plugins/__init__.py` & `kubemarine-0.18.0/kubemarine/plugins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import glob
 import importlib.util
 import io
+import logging
 import os
 import re
 import shutil
 import ssl
 import subprocess
 import sys
 import tarfile
@@ -33,15 +34,15 @@
 from itertools import chain
 from typing import Dict, List, Tuple
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine import jinja, thirdparties
-from kubemarine.core import utils, static
+from kubemarine.core import utils, static, errors, os as kos
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.group import NodeGroup, NodeGroupResult
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.kubernetes.replicaset import ReplicaSet
 from kubemarine.kubernetes.statefulset import StatefulSet
 
@@ -64,57 +65,108 @@
         for i, step in enumerate(plugin_item.get('installation', {}).get('procedures', [])):
             for procedure_type, configs in step.items():
                 if procedure_types[procedure_type].get('convert') is not None:
                     step[procedure_type] = procedure_types[procedure_type]['convert'](cluster, configs)
     return inventory
 
 
-def enrich_upgrade_inventory(inventory, cluster):
-    if cluster.context.get("initial_procedure") != "upgrade":
+def _get_upgrade_plan(cluster: KubernetesCluster) -> List[Tuple[str, dict]]:
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        upgrade_version = context["upgrade_version"]
+        upgrade_plan = []
+        for version in cluster.procedure_inventory.get('upgrade_plan'):
+            if utils.version_key(version) < utils.version_key(upgrade_version):
+                continue
+
+            upgrade_plan.append((version, cluster.procedure_inventory.get(version, {}).get("plugins", {})))
+
+    elif context.get("initial_procedure") == "migrate_kubemarine" and 'upgrading_plugin' in context:
+        upgrade_plugins = cluster.procedure_inventory.get('upgrade', {}).get("plugins", {})
+        upgrade_plugins = dict(item for item in upgrade_plugins.items()
+                               if item[0] == context['upgrading_plugin'])
+        upgrade_plan = [("", upgrade_plugins)]
+    else:
+        upgrade_plan = []
+
+    return upgrade_plan
+
+
+def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
+    upgrade_plan = _get_upgrade_plan(cluster)
+    if not upgrade_plan:
         return inventory
 
-    base_plugins = static.DEFAULTS["plugins"]
-    current_plugins = deepcopy(inventory["plugins"])
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        previous_version = context['initial_kubernetes_version']
+        plugins_verify = oob_plugins
+    else:  # migrate_kubemarine procedure
+        previous_version = ""
+        plugins_verify = [context['upgrading_plugin']]
+
+    _verify_upgrade_plan(cluster.raw_inventory, previous_version, plugins_verify, upgrade_plan)
+
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def _verify_upgrade_plan(raw_inventory: dict, previous_version: str,
+                         plugins_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+    raw_plugins = deepcopy(raw_inventory.get('plugins', {}))
 
     # validate all plugin sections in procedure inventory
-    upgrade_plan = cluster.procedure_inventory.get('upgrade_plan')
-    previous_version = cluster.context['initial_kubernetes_version']
-    for version in upgrade_plan:
-        upgrade_plugins = cluster.procedure_inventory.get(version, {}).get("plugins", {})
-        for oob_plugin in oob_plugins:
-            verify_image_redefined(oob_plugin,
+    for version, upgrade_plugins in upgrade_plan:
+        for plugin_name in plugins_verify:
+            verify_image_redefined(plugin_name,
                                    previous_version,
-                                   base_plugins[oob_plugin],
-                                   current_plugins[oob_plugin],
-                                   upgrade_plugins.get(oob_plugin, {}))
-        default_merger.merge(current_plugins, upgrade_plugins)
+                                   version,
+                                   raw_plugins.get(plugin_name, {}),
+                                   upgrade_plugins.get(plugin_name, {}))
+        default_merger.merge(raw_plugins, upgrade_plugins)
         previous_version = version
 
-    upgrade_plugins = cluster.procedure_inventory.get(cluster.context["upgrade_version"], {}).get("plugins", {})
-    default_merger.merge(inventory["plugins"], upgrade_plugins)
-    return inventory
-
 
-def verify_image_redefined(plugin_name, previous_version, base_plugin, cluster_plugin, upgrade_plugin):
+def verify_image_redefined(plugin_name, previous_version, next_version, raw_plugins, upgrade_plugin):
     """
     If some image in "cluster_plugin" is different from image in "base_plugin",
     i.e. redefined, then "upgrade_plugin" should have this image explicitly
     redefined too.
     """
-    for key, value in base_plugin.items():
+    sensitive_keys = ['image', 'helper-pod-image', 'version']
+    for key, value in raw_plugins.items():
         if isinstance(value, dict):
             verify_image_redefined(plugin_name,
                                    previous_version,
-                                   base_plugin[key],
-                                   cluster_plugin[key],
+                                   next_version,
+                                   value,
                                    upgrade_plugin.get(key, {}))
-        elif key == "image" and base_plugin["image"] != cluster_plugin["image"] and not upgrade_plugin.get("image"):
-            raise Exception(f"Image is redefined for {plugin_name} in cluster.yaml for version {previous_version}, "
-                            f"but not present in procedure inventory for next version(s). "
-                            f"Please, specify required plugin version explicitly in procedure inventory.")
+        elif key not in sensitive_keys:
+            continue
+        elif value and not upgrade_plugin.get(key):
+            raise errors.KME("KME0009",
+                             key=key, plugin_name=plugin_name,
+                             previous_version_spec=f" for version {previous_version}" if previous_version else "",
+                             next_version_spec=f" for next version {next_version}" if next_version else ""
+            )
+
+
+def upgrade_finalize_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def generic_upgrade_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    upgrade_plan = _get_upgrade_plan(cluster)
+    if not upgrade_plan:
+        return inventory
+
+    _, upgrade_plugins = upgrade_plan[0]
+    if upgrade_plugins:
+        default_merger.merge(inventory.setdefault("plugins", {}), upgrade_plugins)
+
+    return inventory
 
 
 def install(cluster, plugins=None):
     if not plugins:
         plugins = cluster.inventory["plugins"]
     plugins_queue: List[str] = []
     max_priority = 0
@@ -747,26 +799,25 @@
     if config_values_file is not None:
         with utils.open_external(config_values_file) as stream:
             file_values = yaml.safe_load(stream)
 
     if config_values is None and file_values is None:
         return
 
-    with utils.open_external(os.path.join(local_chart_path, 'values.yaml'), 'r+') as stream:
+    chart_values = os.path.join(local_chart_path, 'values.yaml')
+    with utils.open_external(chart_values, 'r') as stream:
         merged_values = yaml.safe_load(stream)
 
-        if file_values is not None:
-            merged_values = default_merger.merge(merged_values, file_values)
-        # Values from 'values' section have priority over values in 'values_file' section
-        if config_values is not None:
-            merged_values = default_merger.merge(merged_values, config_values)
-
-        stream.seek(0)
-        stream.write(yaml.dump(merged_values))
-        stream.truncate()
+    if file_values is not None:
+        merged_values = default_merger.merge(merged_values, file_values)
+    # Values from 'values' section have priority over values in 'values_file' section
+    if config_values is not None:
+        merged_values = default_merger.merge(merged_values, config_values)
+
+    utils.dump_file({}, yaml.dump(merged_values), chart_values, dump_location=False)
 
 
 def get_local_chart_path(log, config):
     chart_path = config.get('chart_path')
 
     is_curl = chart_path[:4] == 'http' and '://' in chart_path[4:8]
 
@@ -883,15 +934,15 @@
         if do_render:
             # templates usually have '.j2' extension, which we want to remove from resulting filename
             # but we also support usual '.yaml' files without '.j2' extension, in this case we do not want to remove extension
             split_extension = os.path.splitext(source_filename)
             if split_extension[1] == ".j2":
                 source_filename = split_extension[0]
 
-            render_vars = {**cluster.inventory, 'runtime_vars': cluster.context['runtime_vars']}
+            render_vars = {**cluster.inventory, 'runtime_vars': cluster.context['runtime_vars'], 'env': kos.Environ()}
             with utils.open_utf8(file, 'r') as template_stream:
                 generated_data = jinja.new(log).from_string(template_stream.read()).render(**render_vars)
 
             utils.dump_file(cluster, generated_data, source_filename)
             source = io.StringIO(generated_data)
         elif not is_external:
             with utils.open_utf8(file, 'r') as config_stream:
@@ -936,15 +987,15 @@
     destination_common_group.put(source, destination_path, backup=True, sudo=use_sudo)
 
     if apply_required:
         method = apply_common_group.run
         if use_sudo:
             method = apply_common_group.sudo
         cluster.log.debug("Applying yaml...")
-        method(apply_command, hide=False)
+        method(apply_command, logging_stream_level=logging.DEBUG)
     else:
         cluster.log.debug('Apply is not required')
 
 
 procedure_types = {
     'template': {
         'convert': convert_template,
```

### Comparing `kubemarine-0.17.0/kubemarine/plugins/builtin.py` & `kubemarine-0.18.0/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/calico.py` & `kubemarine-0.18.0/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.18.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.18.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/manifest.py` & `kubemarine-0.18.0/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.18.0/kubemarine/plugins/nginx_ingress.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,14 +245,28 @@
         else:
             raise Exception("Failed to find '--publish-service' argument in ingress-nginx-controller container specification.")
 
         extra_args = [
             ('--watch-ingress-without-class=', 'true')
         ]
         ssl_options = self.inventory['plugins']['nginx-ingress-controller']['controller']['ssl']
+        additional_args = self.inventory['plugins']['nginx-ingress-controller']['controller'].get('args')
+
+        if additional_args:
+            for arg in additional_args:
+                pars_arg = arg.split('=')
+                for i, container_arg in enumerate(container_args):
+                    if container_arg.startswith(pars_arg[0]):
+                       raise Exception(
+                           f"{pars_arg[0]!r} argument is already defined in ingress-nginx-controller container specification.")
+                else:
+                    container_args.append(arg)
+                    self.log.verbose(f"The {arg!r} argument has been added to "
+                                     f"'spec.template.spec.containers.[{container_pos}].args' in the {key}")
+
         if ssl_options['enableSslPassthrough']:
             extra_args.append(('--enable-ssl-passthrough',))
         if ssl_options.get('default-certificate'):
             extra_args.append(('--default-ssl-certificate=', 'kube-system/default-ingress-cert'))
 
         for extra_arg in extra_args:
             for i, arg in enumerate(container_args):
```

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/__init__.py` & `kubemarine-0.18.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/add_node.py` & `kubemarine-0.18.0/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/backup.py` & `kubemarine-0.18.0/kubemarine/procedures/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,16 +280,15 @@
     found_resources_results = result.split(resource_separator)
     for i, result in enumerate(found_resources_results):
         resource = resources[i]
         resource_file_path = os.path.join(location, '%s.yaml' % resource)
         result = result.strip()
         if result and result != '':
             actual_resources.append(resource)
-            with utils.open_external(resource_file_path, 'w') as resource_file_stream:
-                resource_file_stream.write(result)
+            utils.dump_file({}, result, resource_file_path, dump_location=False)
 
     return actual_resources
 
 
 def export_kubernetes(cluster):
     backup_directory = prepare_backup_tmpdir(cluster)
     control_plane = cluster.nodes['control-plane'].get_any_member()
```

### Comparing `kubemarine-0.17.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.18.0/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.18.0/kubemarine/procedures/check_iaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.resources import DynamicResources
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.core.group import NodeGroupResult
 
 def connection_ssh_connectivity(cluster):
-    with TestCase(cluster.context['testsuite'], '001', 'SSH', 'Connectivity', default_results='Connected'):
+    with TestCase(cluster, '001', 'SSH', 'Connectivity', default_results='Connected'):
         failed_nodes = []
         for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
             try:
                 cluster.log.verbose(node['connection'].run("echo 1"))
             except fabric.group.GroupException as e:
                 failed_nodes.append(node['name'])
                 cluster.log.error("Connection test failed for node \"%s\"" % node['name'])
@@ -50,15 +50,15 @@
             raise TestFailure("Failed to connect to %s nodes" % len(failed_nodes),
                               hint="Failed to connect from the deploy node to the remote node of the cluster. Check that "
                                    "the inventory details (key, username, and nodes addresses) are entered correctly, and verify "
                                    "the access to remote nodes.")
 
 
 def connection_ssh_latency_single(cluster):
-    with TestCase(cluster.context['testsuite'], '002',  'SSH', 'Latency - Single Thread',
+    with TestCase(cluster, '002',  'SSH', 'Latency - Single Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 5:
             i += 1
             for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
@@ -78,15 +78,15 @@
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
 def connection_ssh_latency_multiple(cluster):
-    with TestCase(cluster.context['testsuite'], '003',  'SSH', 'Latency - Multi Thread',
+    with TestCase(cluster, '003',  'SSH', 'Latency - Multi Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 10:
             i += 1
             time_start = time.time()
@@ -105,15 +105,15 @@
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
 def connection_sudoer_access(cluster):
-    with TestCase(cluster.context['testsuite'], '004', 'SSH', 'Sudoer Access', default_results='Access provided'):
+    with TestCase(cluster, '004', 'SSH', 'Sudoer Access', default_results='Access provided'):
         non_root = []
         for host, node_context in cluster.context['nodes'].items():
             access_info = node_context['access']
             if access_info['online'] and access_info['sudo'] == 'Root':
                 cluster.log.debug("%s online and has root" % host)
             else:
                 non_root.append(host)
@@ -126,15 +126,15 @@
 def hardware_members_amount(cluster, group_name):
     beauty_name = group_name.capitalize()
     if group_name == 'vip':
         beauty_name = 'VIP'
     if group_name == 'all':
         beauty_name = 'Total Node'
 
-    with TestCase(cluster.context['testsuite'], '005',  'Hardware', '%ss Amount' % beauty_name,
+    with TestCase(cluster, '005',  'Hardware', '%ss Amount' % beauty_name,
                   minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount'],
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['amount']) as tc:
         amount = 0
         if group_name == 'vip':
             amount = len(cluster.inventory.get('vrrp_ips', []))
         else:
             group = cluster.nodes.get(group_name)
@@ -164,15 +164,15 @@
         tc.success("%s item%s" % (amount, s))
 
 
 def hardware_cpu(cluster, group_name):
     minimal_cpu = cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'] \
         if group_name == 'balancer' or cluster.nodes.get('all').nodes_amount() > 1 \
         else cluster.globals['compatibility_map']['hardware']['minimal']['control-plane']['vcpu']
-    with TestCase(cluster.context['testsuite'], '006',  'Hardware', 'VCPUs Amount - %ss' % group_name.capitalize(),
+    with TestCase(cluster, '006',  'Hardware', 'VCPUs Amount - %ss' % group_name.capitalize(),
                   minimal=minimal_cpu,
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
             return tc.success(results='Skipped')
         results = cluster.nodes[group_name].sudo("nproc --all")
         cluster.log.verbose(results)
         minimal_amount = None
@@ -201,15 +201,15 @@
             raise TestWarn("Less than recommended. Detected %s VCPU%s" % (minimal_amount, s),
                            hint="Increase the number of VCPUs in the node configuration up to %s VCPUs."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'])
         tc.success(results='%s VCPU%s' % (minimal_amount, s))
 
 
 def hardware_ram(cluster, group_name):
-    with TestCase(cluster.context['testsuite'], '007',  'Hardware', 'RAM Amount - %ss' % group_name.capitalize(),
+    with TestCase(cluster, '007',  'Hardware', 'RAM Amount - %ss' % group_name.capitalize(),
                   minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'],
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
             return tc.success(results='Skipped')
         results = cluster.nodes[group_name].sudo("cat /proc/meminfo | awk '/DirectMap/ { print $2 }'")
         cluster.log.verbose(results)
         minimal_amount = None
@@ -233,15 +233,15 @@
             raise TestWarn("Less than recommended. Detected %sGB" % minimal_amount,
                            hint="Increase the number of RAM in the node configuration up to %s GB."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'])
         tc.success(results='%sGB' % minimal_amount)
 
 
 def system_distributive(cluster):
-    with TestCase(cluster.context['testsuite'], '008', 'System', 'Distibutive') as tc:
+    with TestCase(cluster, '008', 'System', 'Distibutive') as tc:
         supported_distributives = cluster.globals['compatibility_map']['distributives'].keys()
 
         cluster.log.debug(system.fetch_os_versions(cluster))
 
         detected_unsupported_os = []
         detected_supported_os = []
         detected_unsupported_version = []
@@ -288,15 +288,15 @@
         tc.success(results=", ".join(detected_supported_os))
 
 
 def check_kernel_version(cluster):
     """
     This method compares the linux kernel version with the bad version
     """
-    with TestCase(cluster.context['testsuite'], '015', "Software", "Kernel version") as tc:
+    with TestCase(cluster, '015', "Software", "Kernel version") as tc:
         bad_results = {}
         unstable_kernel_ubuntu = cluster.globals['compatibility_map']['distributives']['ubuntu'][0].get('unstable_kernel')
         unstable_kernel_centos = []
         group = cluster.nodes['all']
         result_group = group.run('uname -r')
         for connection, results in result_group.items():
             os_name = cluster.context['nodes'][connection.host]['os']['name']
@@ -314,15 +314,15 @@
             cluster.log.debug(f"Update the linux kernel version to 5.4.0-135-generic")
             raise TestWarn("Kernel version unstable")
         else:
             tc.success("All kernel have stable versions")
 
 
 def check_access_to_thirdparties(cluster: KubernetesCluster):
-    with TestCase(cluster.context['testsuite'], '012', 'Software', 'Thirdparties Availability') as tc:
+    with TestCase(cluster, '012', 'Software', 'Thirdparties Availability') as tc:
         detect_preinstalled_python(cluster)
         broken = []
         nodes_without_python = set()
 
         # Load script for checking sources
         all_group = cluster.nodes['all']
         check_script = utils.read_internal("resources/scripts/check_url_availability.py")
@@ -410,15 +410,15 @@
             nodes_context[conn.host]["package_repos_are_actual"] = not list(results.values())[-1].failed
 
         # Remove temp .repo file
         group.sudo("rm %s" % random_repos_conf_path)
 
 
 def check_access_to_package_repositories(cluster: KubernetesCluster):
-    with TestCase(cluster.context['testsuite'], '013', 'Software', 'Package Repositories') as tc:
+    with TestCase(cluster, '013', 'Software', 'Package Repositories') as tc:
         detect_preinstalled_python(cluster)
         check_resolv_conf(cluster)
         broken = []
         warnings = []
 
         # Collect repository urls
         # TODO: think about better parsing
@@ -503,15 +503,15 @@
             raise TestFailure('Found problems for package repositories', hint=yaml.safe_dump(broken))
         elif warnings:
             raise TestWarn('Found potential problems for package repositories or nodes', hint=yaml.safe_dump(warnings))
         tc.success('All package repositories are correct and available')
 
 
 def check_access_to_packages(cluster: KubernetesCluster):
-    with TestCase(cluster.context['testsuite'], '014', 'Software', 'Package Availability') as tc:
+    with TestCase(cluster, '014', 'Software', 'Package Availability') as tc:
         check_package_repositories(cluster)
         broken = []
         warnings = []
         group = cluster.nodes['all']
         hosts_to_packages = packages.get_all_managed_packages_for_group(group, cluster.inventory)
         with RemoteExecutor(cluster) as exe:
             for host, packages_to_check in hosts_to_packages.items():
@@ -669,15 +669,15 @@
 
     if skipped_nodes:
         raise TestWarn(f"Cannot perform check on {skipped_nodes}: subnet is already in use. "
                        f"Use check_paas procedure if you already have installed cluster.")
 
 
 def pod_subnet_connectivity(cluster):
-    with TestCase(cluster.context['testsuite'], '009', 'Network', 'PodSubnet', default_results='Connected'),\
+    with TestCase(cluster, '009', 'Network', 'PodSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         pod_subnet = cluster.inventory['services']['kubeadm']['networking']['podSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, pod_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
             failed_nodes = check_tcp_connect_between_all_nodes(cluster, list(nodes.values()), tcp_ports, host_to_ip)
@@ -685,15 +685,15 @@
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Traffic is not allowed for the pod subnet({pod_subnet}) "
                                        f"on nodes: {failed_nodes}.")
 
 
 def service_subnet_connectivity(cluster):
-    with TestCase(cluster.context['testsuite'], '010', 'Network', 'ServiceSubnet', default_results='Connected'),\
+    with TestCase(cluster, '010', 'Network', 'ServiceSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         service_subnet = cluster.inventory['services']['kubeadm']['networking']['serviceSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, service_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
             failed_nodes = check_tcp_connect_between_all_nodes(cluster, list(nodes.values()), tcp_ports, host_to_ip)
@@ -857,15 +857,15 @@
 
     if nodes_without_python:
         cluster.log.warning(f"Nodes without python: {nodes_without_python.keys()}")
         raise TestWarn(f"Cannot perform check on {list(nodes_without_python.keys())}: python doesn't exist.")
 
 
 def check_tcp_ports(cluster):
-    with TestCase(cluster.context['testsuite'], '011', 'Network', 'TCPPorts', default_results='Connected'),\
+    with TestCase(cluster, '011', 'Network', 'TCPPorts', default_results='Connected'),\
             suspend_firewalld(cluster):
         tcp_ports = ["80", "443", "179", "5473", "6443", "8443", "2379", "2380", "9091", "9094", "10250", "10254",
                      "10257", "10259", "30001", "30002"]
         nodes = {node["connect_to"]: node
                  for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True)}
         host_to_ip = {host: node['internal_address'] for host, node in nodes.items()}
         with install_tcp_listener(cluster, nodes, tcp_ports):
```

### Comparing `kubemarine-0.17.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.18.0/kubemarine/procedures/check_paas.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 import uuid
 
 from kubemarine import packages as pckgs, system, selinux, etcd, thirdparties, apparmor, kubernetes
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import check_iaas
-from kubemarine.core import flow
+from kubemarine.core import flow, static
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.coredns import generate_configmap
 from deepdiff import DeepDiff
 
 
 def services_status(cluster: KubernetesCluster, service_type: str):
-    with TestCase(cluster.context['testsuite'], '201', "Services", "%s Status" % service_type.capitalize(),
+    with TestCase(cluster, '201', "Services", "%s Status" % service_type.capitalize(),
                   default_results='active (running)'):
         service_name = service_type
 
         if cluster.get_os_family() != 'multiple' and service_type != 'kubelet':
             service_name = cluster.get_package_association(service_type, 'service_name')
 
         group = cluster.nodes['all']
@@ -105,76 +105,59 @@
 
 def recommended_system_package_versions(cluster: KubernetesCluster, pckg_alias: str):
     """
     Function that checks if defined package are compatible with the configured k8s version and OS.
     Raise Warn if unable to detect the OS family, configured not recommended k8s version or
     if configured not recommended system packages versions.
     """
-    version_key = system.get_compatibility_version_key(cluster)
-    if not version_key:
+    os_family = cluster.get_os_family()
+    if os_family not in pckgs.get_associations_os_family_keys():
         raise TestFailure("OS is unknown or multiple OS present")
-    k8s_version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
-    compatibility = cluster.globals["compatibility_map"]["software"]
-    if k8s_version not in compatibility["kubeadm"]:
-        raise TestWarn(f"Using not recommended k8s version: {k8s_version}")
-
-    # Mapping "system_package_alias -> expected_packages_names -> expected_versions"
-    # We assume that system packages have word "haproxy"/"keepalived"/"docker"/"containerd"/"podman" in their name,
-    # if not - then we may miss such package
-    if pckg_alias == "haproxy":
-        expected_system_packages = {"haproxy": compatibility["haproxy"][version_key]}
-    elif pckg_alias == "keepalived":
-        expected_system_packages = {"keepalived": compatibility["keepalived"][version_key]}
-    elif pckg_alias == "containerd":
-        expected_system_packages = {"podman": compatibility["podman"][k8s_version][version_key]}
-        if version_key in ["version_rhel", "version_rhel8"]:
-            expected_system_packages["containerd.io"] = compatibility["containerdio"][k8s_version][version_key]
-        else:
-            expected_system_packages["containerd"] = compatibility["containerd"][k8s_version][version_key]
-    elif pckg_alias == "docker":
-        expected_system_packages = {
-            "docker": compatibility["docker"][k8s_version][version_key],
-            "containerd.io": compatibility["containerdio"][k8s_version][version_key]
-        }
-    else:
+
+    recommended_packages = list(static.GLOBALS['packages'][os_family])
+    if pckg_alias not in recommended_packages:
         raise TestWarn(f"Package {pckg_alias} doesn't have recommended version")
 
+    k8s_version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
+    expected_system_packages = pckgs.get_default_package_names(os_family, pckg_alias, k8s_version)
+
     good_results = set()
     bad_results = []
     actual_packages = cluster.get_package_association(pckg_alias, "package_name")
     if not isinstance(actual_packages, list):
         actual_packages = [actual_packages]
-    for expected_pckg, version in expected_system_packages.items():
-        version = version.replace("*", "")
-        is_found = False
+    for expected_pckg in expected_system_packages:
+        expected_pckg_name = pckgs.get_package_name(os_family, expected_pckg)
         for actual_pckg in actual_packages:
-            if expected_pckg in actual_pckg:
-                is_found = True
-                if f"-{version}" in actual_pckg or f"={version}" in actual_pckg:
+            actual_pckg_name = pckgs.get_package_name(os_family, actual_pckg)
+            if expected_pckg_name == actual_pckg_name:
+                if actual_pckg.startswith(expected_pckg.replace("*", "")):
                     good_results.add(actual_pckg)
                 else:
-                    cluster.log.debug(f"Package {actual_pckg} is not recommended, recommended version is {version}")
+                    cluster.log.debug(f"Package {actual_pckg} is not recommended, recommended is {expected_pckg}")
                     bad_results.append(actual_pckg)
-        if not is_found:
-            cluster.log.debug(f"Package {expected_pckg} is not found in inventory")
-            bad_results.append(expected_pckg)
+
+                break
+        else:
+            cluster.log.debug(f"Package {expected_pckg_name} is not found in inventory")
+            bad_results.append(expected_pckg_name)
 
     if bad_results:
         raise TestWarn(f"Detected not recommended packages versions: {bad_results}")
     cluster.log.debug(f"Detected packages with recommended versions: {good_results}")
 
 
 def system_packages_versions(cluster: KubernetesCluster, pckg_alias: str):
     """
     Verifies that system packages are installed on required nodes and have equal versions.
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     :param pckg_alias: system package alias to retrieve "package_name" association.
     """
-    with TestCase(cluster.context['testsuite'], '205', "Services", f"{pckg_alias} version") as tc:
+    with TestCase(cluster, '205', "Services", f"{pckg_alias} version") as tc:
         _check_same_os(cluster)
         hosts_to_packages = pckgs.get_association_hosts_to_packages(cluster.nodes['all'], cluster.inventory, pckg_alias)
         if not hosts_to_packages:
             raise TestWarn(f"No nodes to check {pckg_alias!r} version")
         check_packages_versions(cluster, tc, hosts_to_packages, raise_successful=False)
 
         if pckg_alias in ["haproxy", "keepalived", "containerd", "docker"]:
@@ -184,15 +167,15 @@
 
 def mandatory_packages_versions(cluster: KubernetesCluster):
     """
     Verifies that mandatory packages are installed on required nodes and have equal versions.
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     """
-    with TestCase(cluster.context['testsuite'], '205', "Services", "Mandatory package versions") as tc:
+    with TestCase(cluster, '205', "Services", "Mandatory package versions") as tc:
         _check_same_os(cluster)
         hosts_to_packages = {}
         group = cluster.nodes['all']
         for package in cluster.inventory["services"]["packages"]['mandatory'].keys():
             packages = pckgs.get_association_hosts_to_packages(group, cluster.inventory, package)
 
             for host, packages_list in packages.items():
@@ -205,15 +188,15 @@
 
 
 def generic_packages_versions(cluster: KubernetesCluster):
     """
     Verifies that user-provided packages are installed on required nodes and have equal versions.
     Warning is shown if check is not successful.
     """
-    with TestCase(cluster.context['testsuite'], '206', "Services", f"Generic packages version") as tc:
+    with TestCase(cluster, '206', "Services", f"Generic packages version") as tc:
         _check_same_os(cluster)
         packages = cluster.inventory['services']['packages'].get('install', {}).get('include', [])
         hosts_to_packages = {host: packages for host in cluster.nodes['all'].get_hosts()}
         return check_packages_versions(cluster, tc, hosts_to_packages, warn_on_bad_result=True)
 
 
 def check_packages_versions(cluster, tc, hosts_to_packages: Dict[str, List[str]],
@@ -238,15 +221,15 @@
         version = list(version_map.keys())[0]
         if "not installed" in version:
             cluster.log.debug(f"Package {package} is not installed on some nodes:")
             cluster.log.debug(version_map[version])
             bad_results.append(package)
         else:
             package_name = package.replace("*", "")
-            if package_name in version:
+            if version.startswith(package_name):
                 good_results.append(version)
             else:
                 bad_results.append(version)
 
     if bad_results:
         hint_message = f'Check the presence and correctness of the version of the following packages on the ' \
                        f'system: {bad_results}'
@@ -259,15 +242,15 @@
 
 
 def get_nodes_description(cluster):
     return kubernetes.get_nodes_description(cluster)
 
 
 def kubelet_version(cluster):
-    with TestCase(cluster.context['testsuite'], '203', "Services", "Kubelet Version",
+    with TestCase(cluster, '203', "Services", "Kubelet Version",
                   default_results=cluster.inventory['services']['kubeadm']['kubernetesVersion']):
         nodes_description = get_nodes_description(cluster)
         bad_versions = []
         for node_description in nodes_description['items']:
             node_name = node_description['metadata']['name']
             kubelet_version = node_description['status']['nodeInfo']['kubeletVersion']
             cluster.log.debug("Node \"%s\" running kubelet %s" % (node_name, kubelet_version))
@@ -284,15 +267,15 @@
 def thirdparties_hashes(cluster):
     """
     Task which is used to verify configured thirdparties hashes agains actual hashes on nodes.
     If thirdparty is an archive, then archive files hashes are also verified.
     If hash is not specified, then thirdparty is skipped.
     If there is no thirdparties with hashes, then warning is shown.
     """
-    with TestCase(cluster.context['testsuite'], '212', "Thirdparties", "Hashes") as tc:
+    with TestCase(cluster, '212', "Thirdparties", "Hashes") as tc:
         successful = []
         warnings = []
         broken = []
 
         #Create tmp dir for loading thirdparty without default sha
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
@@ -433,15 +416,15 @@
     for host, result in results.items():
         if result.failed:
             missing.append(host.host)
     return missing
 
 
 def kubernetes_nodes_existence(cluster):
-    with TestCase(cluster.context['testsuite'], '209', "Kubernetes", "Nodes Existence",
+    with TestCase(cluster, '209', "Kubernetes", "Nodes Existence",
                   default_results="All nodes presented"):
         nodes_description = get_nodes_description(cluster)
         nodes_names = kubernetes.get_actual_roles(nodes_description).keys()
         not_found = []
         for node in cluster.inventory['nodes']:
             if 'control-plane' in node['roles'] or 'worker' in node['roles']:
                 if node['name'] in nodes_names:
@@ -453,15 +436,15 @@
         if not_found:
             raise TestFailure("Nodes not found: %s" % ', '.join(not_found),
                               hint="The cluster must contain all the nodes that are described in the inventory. Add "
                                    "the missing nodes to the cluster.")
 
 
 def kubernetes_nodes_roles(cluster: KubernetesCluster):
-    with TestCase(cluster.context['testsuite'], '210', "Kubernetes", "Nodes Roles",
+    with TestCase(cluster, '210', "Kubernetes", "Nodes Roles",
                   default_results="All nodes have the correct roles"):
         nodes_description = get_nodes_description(cluster)
         nodes_roles = kubernetes.get_actual_roles(nodes_description)
         nodes_with_bad_roles = []
         for node_name, actual_roles in nodes_roles.items():
             node = cluster.get_node_by_name(node_name)
             if node is None:
@@ -480,15 +463,15 @@
         if nodes_with_bad_roles:
             raise TestFailure("Incorrect role detected at: %s" % ', '.join(nodes_with_bad_roles),
                               hint="Some nodes whose role differs from that specified in the "
                                    "inventory were detected. The configuration of these nodes should be fixed.")
 
 
 def kubernetes_nodes_condition(cluster, condition_type):
-    with TestCase(cluster.context['testsuite'], '211', "Kubernetes", "Nodes Condition - %s" % condition_type) as tc:
+    with TestCase(cluster, '211', "Kubernetes", "Nodes Condition - %s" % condition_type) as tc:
         nodes_description = get_nodes_description(cluster)
         expected_status = 'False'
         if condition_type == 'Ready':
             expected_status = 'True'
         positive_conditions = []
         negative_conditions = []
         nodes_conditions = kubernetes.get_nodes_conditions(nodes_description)
@@ -522,15 +505,15 @@
     cluster.log.verbose(result)
     return list(result.values())[0].stdout.strip()
 
 
 def kubernetes_pods_condition(cluster):
     system_namespaces = ["kube-system", "ingress-nginx", "kube-public", "kubernetes-dashboard", "default"]
     critical_states = cluster.globals['pods']['critical_states']
-    with TestCase(cluster.context['testsuite'], '207', "Kubernetes", "Pods Condition") as tc:
+    with TestCase(cluster, '207', "Kubernetes", "Pods Condition") as tc:
         pods_description = get_not_running_pods(cluster)
         total_failed_amount = len(pods_description.split('\n')[1:])
         critical_system_failed_amount = 0
 
         for pod_description in pods_description.split('\n')[1:]:
             split_description = pod_description.split(' ')
             if split_description[0] in system_namespaces and split_description[2] in critical_states:
@@ -552,15 +535,15 @@
                                 "try to wait, redeploy, reapply, or restart them. "
                                 "If this is not fixed, some deployed applications may not work or may work incorrectly.")
         else:
             tc.success(results="All pods are running")
 
 
 def kubernetes_dashboard_status(cluster):
-    with TestCase(cluster.context['testsuite'], '208', "Plugins", "Dashboard Availability") as tc:
+    with TestCase(cluster, '208', "Plugins", "Dashboard Availability") as tc:
         retries = 10
         test_succeeded = False
         i = 0
         while not test_succeeded and i < retries:
             i += 1
             if cluster.inventory['plugins']['kubernetes-dashboard']['install']:
                 results = cluster.nodes['control-plane'].get_first_member().sudo("kubectl get svc -n kubernetes-dashboard kubernetes-dashboard -o=jsonpath=\"{['spec.clusterIP']}\"", warn=True)
@@ -586,15 +569,15 @@
                 tc.success(results="skipped")
         if not test_succeeded:
             raise TestFailure("not available",
                               hint=f"Please verify the following Kubernetes Dashboard status and fix this issue:\n{status}")
 
 
 def nodes_pid_max(cluster):
-    with TestCase(cluster.context['testsuite'], '202', "Nodes", "Nodes pid_max correctly installed") as tc:
+    with TestCase(cluster, '202', "Nodes", "Nodes pid_max correctly installed") as tc:
         control_plane = cluster.nodes['control-plane'].get_any_member()
         yaml = ruamel.yaml.YAML()
         nodes_failed_pid_max_check = {}
         for node in cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_ordered_members_list(provide_node_configs=True):
 
             node_info = control_plane.sudo("kubectl get node %s -o yaml" % node["name"]).get_simple_out()
             config = yaml.load(node_info)
@@ -635,15 +618,15 @@
     the RHEL family.
     :param cluster: KubernetesCluster object
     :return: None
     """
     if cluster.get_os_family() not in ('rhel', 'rhel8'):
         return
 
-    with TestCase(cluster.context['testsuite'], '213', "Security", "Selinux security policy") as tc:
+    with TestCase(cluster, '213', "Security", "Selinux security policy") as tc:
         group = cluster.nodes['all']
         selinux_configured, selinux_result, selinux_parsed_result = \
             selinux.is_config_valid(group,
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         cluster.log.debug(selinux_result)
@@ -694,15 +677,15 @@
     the inventory or with the one by default. If the configuration does not match, the test will fail.
     :param cluster: KubernetesCluster object
     :return: None
     """
     if cluster.get_os_family() not in ('rhel', 'rhel8'):
         return
 
-    with TestCase(cluster.context['testsuite'], '214', "Security", "Selinux configuration") as tc:
+    with TestCase(cluster, '214', "Security", "Selinux configuration") as tc:
         group = cluster.nodes['all']
         selinux_configured, selinux_result, selinux_parsed_result = \
             selinux.is_config_valid(group,
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         cluster.log.debug(selinux_result)
@@ -717,15 +700,15 @@
 
 def verify_firewalld_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which verifies that the FirewallD is disabled on cluster nodes, otherwise the test will fail.
     :param cluster: KubernetesCluster object
     :return: None
     """
-    with TestCase(cluster.context['testsuite'], '215', "Security", "Firewalld status") as tc:
+    with TestCase(cluster, '215', "Security", "Firewalld status") as tc:
         group = cluster.nodes['all']
         firewalld_disabled, firewalld_result = system.is_firewalld_disabled(group)
         cluster.log.debug(firewalld_result)
         if firewalld_disabled:
             tc.success(results='disabled')
         else:
             raise TestFailure('enabled',
@@ -736,15 +719,15 @@
 
 def verify_time_sync(cluster: KubernetesCluster) -> None:
     """
     This method is a test that verifies that the time between all nodes does not lag behind.
     :param cluster: KubernetesCluster object
     :return: None
     """
-    with TestCase(cluster.context['testsuite'], '218', "System", "Time difference") as tc:
+    with TestCase(cluster, '218', "System", "Time difference") as tc:
         group = cluster.nodes['all']
         current_node_time, nodes_timestamp, time_diff = system.get_nodes_time(group)
         cluster.log.verbose('Current node time: %s' % current_node_time)
         cluster.log.verbose('Time difference: %s' % time_diff)
         cluster.log.verbose('Nodes time details:')
         for host, timestamp in nodes_timestamp.items():
             cluster.log.verbose(' - %s: %s' % (host.host, timestamp))
@@ -762,15 +745,15 @@
 def verify_swap_state(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which verifies that swap is disabled on all nodes in the cluster, otherwise the test will
     fail.
     :param cluster: KubernetesCluster object
     :return: None
     """
-    with TestCase(cluster.context['testsuite'], '216', "System", "Swap state") as tc:
+    with TestCase(cluster, '216', "System", "Swap state") as tc:
         group = cluster.nodes['all']
         swap_disabled, swap_result = system.is_swap_disabled(group)
         cluster.log.debug(swap_result)
         if swap_disabled:
             tc.success(results='disabled')
         else:
             raise TestFailure('enabled',
@@ -782,15 +765,16 @@
 def verify_modprobe_rules(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which compares the modprobe rules on the nodes with the rules specified in the inventory or
     with default rules. If rules does not match, the test will fail.
     :param cluster: KubernetesCluster object
     :return: None
     """
-    with TestCase(cluster.context['testsuite'], '217', "System", "Modprobe rules") as tc:
+    with TestCase(cluster, '217', "System", "Modprobe rules") as tc:
+        _check_same_os(cluster)
         group = cluster.nodes['all']
         modprobe_valid, modprobe_result = system.is_modprobe_valid(group)
         cluster.log.debug(modprobe_result)
         if modprobe_valid:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid',
@@ -800,15 +784,15 @@
 
 def etcd_health_status(cluster):
     """
     This method is a test, check ETCD health
     :param cluster: KubernetesCluster object
     :return: None
     """
-    with TestCase(cluster.context['testsuite'], '219', "ETCD", "Health status ETCD") as tc:
+    with TestCase(cluster, '219', "ETCD", "Health status ETCD") as tc:
         try:
             etcd_health_status = etcd.wait_for_health(cluster, cluster.nodes['control-plane'].get_any_member())
         except Exception as e:
             cluster.log.verbose('Failed to load and parse ETCD status')
             raise TestFailure('invalid',
                               hint=f"ETCD not ready, please check"
                                    f" because of {e} ")
@@ -818,15 +802,15 @@
 
 def control_plane_configuration_status(cluster):
     '''
     This test verifies the consistency of the configuration (image version, `extra_args`, `extra_volumes`) of static pods of Control Plain like `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
-    with TestCase(cluster.context['testsuite'], '220', "Control plane", "configuration status") as tc:
+    with TestCase(cluster, '220', "Control plane", "configuration status") as tc:
         results = []
         static_pod_names = {'kube-apiserver': 'apiServer',
                             'kube-controller-manager': 'controllerManager',
                             'kube-scheduler': 'scheduler'}
         static_pods_content = []
         not_presented_static_pods = []
         for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
@@ -923,15 +907,15 @@
 
 def control_plane_health_status(cluster):
     '''
     This test verifies the health of static pods `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
-    with TestCase(cluster.context['testsuite'], '221', "Control plane", "health status") as tc:
+    with TestCase(cluster, '221', "Control plane", "health status") as tc:
         static_pods = ['kube-apiserver', 'kube-controller-manager', 'kube-scheduler']
         static_pod_names = []
 
         for control_plane in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
             for static_pod in static_pods:
                 static_pod_names.append(static_pod + '-' + control_plane['name'])
 
@@ -955,15 +939,15 @@
 
 def default_services_configuration_status(cluster):
     '''
     In this test, the versions of the images of the default services, such as `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`, are checked, and the `coredns` configmap is also checked.
     :param cluster: KubernetesCluster object
     :return: None
     '''
-    with TestCase(cluster.context['testsuite'], '222', "Default services", "configuration status") as tc:
+    with TestCase(cluster, '222', "Default services", "configuration status") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         original_coredns_cm = generate_configmap(cluster.inventory)
         original_coredns_cm = yaml.safe_load(original_coredns_cm)
         coredns_cm = first_control_plane.sudo('kubectl get cm coredns -n kube-system -oyaml').get_simple_out()
         coredns_cm = yaml.safe_load(coredns_cm)
         ddiff = DeepDiff(coredns_cm['data'], original_coredns_cm['data'], ignore_order=True)
         coredns_result = ddiff.to_dict().get('values_changed', {}).get("root['Corefile']", {}).get('diff')
@@ -1007,15 +991,15 @@
 
 def default_services_health_status(cluster):
     '''
     This test verifies the health of pods `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
-    with TestCase(cluster.context['testsuite'], '223', "Default services", "health status") as tc:
+    with TestCase(cluster, '223', "Default services", "health status") as tc:
         entities_to_check = {"kube-system": [{"DaemonSet": ["calico-node", "kube-proxy"]},
                                              {"Deployment": ["calico-kube-controllers", "coredns"]}],
                              "ingress-nginx": [{"DaemonSet": ["ingress-nginx-controller"]}]}
 
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         not_ready_entities = []
         for namespace, types_dict in entities_to_check.items():
@@ -1044,15 +1028,15 @@
 
 def calico_config_check(cluster):
     '''
     This test checks the configuration of the `calico-node` envs, Calico's ConfigMap in case of `ipam`, and also performed `calicoctl ipam check`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
-    with TestCase(cluster.context['testsuite'], '224', "Calico", "configuration check") as tc:
+    with TestCase(cluster, '224', "Calico", "configuration check") as tc:
         message = ""
         correct_config = True
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         result = first_control_plane.sudo(f"kubectl get DaemonSet calico-node -n kube-system -oyaml")
         result = result.get_simple_out()
         result = yaml.safe_load(result)
         for env in result["spec"]["template"]["spec"]["containers"][0]["env"]:
@@ -1087,15 +1071,15 @@
 
 
 def kubernetes_admission_status(cluster):
     """
     The method checks status of Pod Security Admissions, default Pod Security Profile,
     and 'kube-apiserver.yaml' and 'kubeadm-config' consistancy
     """
-    with TestCase(cluster.context['testsuite'], '225', "Kubernetes", "Pod Security Admissions") as tc:
+    with TestCase(cluster, '225', "Kubernetes", "Pod Security Admissions") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         profile_inv = ""
         if cluster.inventory["rbac"]["admission"] == "pss" and \
                 cluster.inventory["rbac"]["pss"]["pod-security"] == "enabled":
             profile_inv = cluster.inventory["rbac"]["pss"]["defaults"]["enforce"]
         profile = ""
         result = first_control_plane.sudo("kubectl get cm kubeadm-config -n kube-system -o yaml")
@@ -1158,15 +1142,15 @@
         "dnsStatus": {"failed": []},
         "svcStatus": {"failed": [], "skipped": []},
         "podStatus": {"failed": [], "skipped": []}
     }
 
     # Here we actually collect information about all statuses, but report information about DNS only.
     # Other statuses are reported in other TestCases below. This is done for better UX.
-    with TestCase(cluster.context['testsuite'], '226', "Geo Monitor", "Geo check - DNS resolving") as tc_dns:
+    with TestCase(cluster, '226', "Geo Monitor", "Geo check - DNS resolving") as tc_dns:
         geo_monitor_inventory = cluster.procedure_inventory["geo-monitor"]
         namespace = geo_monitor_inventory["namespace"]
         service = geo_monitor_inventory["service"]
         control_plane_node = cluster.nodes['control-plane'].get_first_member()
 
         svc_result = control_plane_node.sudo("kubectl get svc -n %s %s -o yaml" % (namespace, service)).get_simple_out()
         svc = yaml.safe_load(io.StringIO(svc_result))
@@ -1206,26 +1190,26 @@
                 continue
 
         collected_results["statusCollected"] = True
         if collected_results["dnsStatus"]["failed"]:
             raise TestFailure("found failed DNS statuses", hint=yaml.safe_dump(collected_results["dnsStatus"]["failed"]))
         tc_dns.success("all peer names resolved")
 
-    with TestCase(cluster.context['testsuite'], '226', "Geo Monitor", "Geo check - Pod-to-service") as tc_svc:
+    with TestCase(cluster, '226', "Geo Monitor", "Geo check - Pod-to-service") as tc_svc:
         if not collected_results["statusCollected"]:
             raise TestFailure("configuration error", hint="DNS check failed with error, statuses not collected")
 
         if collected_results["svcStatus"]["failed"]:
             raise TestFailure("found unavailable peer services",
                               hint=yaml.safe_dump(collected_results["svcStatus"]["failed"]+collected_results["svcStatus"]["skipped"]))
         if collected_results["svcStatus"]["skipped"]:
             raise TestWarn("found skipped peer services", hint=yaml.safe_dump(collected_results["svcStatus"]["skipped"]))
         tc_svc.success("all peer services available")
 
-    with TestCase(cluster.context['testsuite'], '226', "Geo Monitor", "Geo check - Pod-to-pod") as tc_pod:
+    with TestCase(cluster, '226', "Geo Monitor", "Geo check - Pod-to-pod") as tc_pod:
         if not collected_results["statusCollected"]:
             raise TestFailure("configuration error", hint="DNS check failed with error, statuses not collected")
 
         if collected_results["podStatus"]["failed"]:
             raise TestFailure("found unavailable peer pod",
                               hint=yaml.safe_dump(collected_results["podStatus"]["failed"]+collected_results["podStatus"]["skipped"]))
         if collected_results["podStatus"]["skipped"]:
@@ -1239,15 +1223,15 @@
     This test is applicable only for systems of the Debian family.
     :param cluster: KubernetesCluster object
     :return: None
     """
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         return
 
-    with TestCase(cluster.context['testsuite'], '227', "Security", "Apparmor security policy") as tc:
+    with TestCase(cluster, '227', "Security", "Apparmor security policy") as tc:
         group = cluster.nodes['all'].get_accessible_nodes()
         results = group.sudo("aa-enabled")
         enabled_nodes = []
         invalid_nodes = []
         for connection, item in results.items():
             apparmor_status = item.stdout
             cluster.log.warning(f"Apparmor on node: {connection.host} enabled: {apparmor_status}")
@@ -1267,15 +1251,15 @@
     This test is applicable only for systems of the Debian family.
     :param cluster: KubernetesCluster object
     :return: None
     """
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         return
 
-    with TestCase(cluster.context['testsuite'], '228', "Security", "Apparmor security policy") as tc:
+    with TestCase(cluster, '228', "Security", "Apparmor security policy") as tc:
         expected_profiles = cluster.inventory['services']['kernel_security'].get('apparmor', {})
         group = cluster.nodes['all'].get_accessible_nodes()
         if expected_profiles:
             apparmor_configured, result = apparmor.is_state_valid(group, expected_profiles)
             if apparmor_configured:
                 cluster.log.verbose(f"Apparmor is configured properly on cluster")
                 tc.success(results='valid')
```

### Comparing `kubemarine-0.17.0/kubemarine/procedures/do.py` & `kubemarine-0.18.0/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/install.py` & `kubemarine-0.18.0/kubemarine/procedures/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,17 +433,18 @@
         cluster.log.debug('Skipped - no balancers to perform')
         return
 
     with RemoteExecutor(cluster):
         group.call_batch([
             haproxy.configure,
             haproxy.override_haproxy18,
-            haproxy.restart
         ])
 
+    haproxy.restart(group)
+
 
 def deploy_loadbalancer_keepalived_install(cluster):
     group = None
     if 'vrrp_ips' in cluster.inventory and cluster.inventory['vrrp_ips']:
 
         group = cluster.nodes['keepalived']
```

### Comparing `kubemarine-0.17.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.18.0/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.18.0/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.18.0/kubemarine/procedures/migrate_cri.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from collections import OrderedDict
 
 import io
 import uuid
 
 from kubemarine import kubernetes, etcd, thirdparties, cri
-from kubemarine.core import flow
+from kubemarine.core import flow, utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.cri import docker
 from kubemarine.procedures import install
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine import packages
@@ -153,26 +153,16 @@
             control_plane = cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
 
         cluster.log.debug(f'Updating thirdparties for node "{node["connect_to"]}..."')
         thirdparties.install_all_thirparties(node["connection"])
 
         version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
         cluster.log.debug("Migrating \"%s\"..." % node["name"])
-        disable_eviction = True
-        drain_cmd = kubernetes.prepare_drain_command(node, version, cluster.globals, disable_eviction, cluster.nodes)
+        drain_cmd = kubernetes.prepare_drain_command(cluster, node['name'], disable_eviction=True)
         control_plane["connection"].sudo(drain_cmd, is_async=False, hide=False)
-        # `kubectl drain` ignores system pods, delete them explicitly
-        if "control-plane" in node["roles"]:
-            node["connection"].sudo(f"kubectl -n kube-system delete pod etcd-{node['name']} "
-                                    f"kube-apiserver-{node['name']} "
-                                    f"kube-controller-manager-{node['name']} "
-                                    f"kube-scheduler-{node['name']} "
-                                    f"$(sudo kubectl describe node {node['name']} | "
-                                    "grep -E 'kube-system\\s+kube-proxy-[a-z,0-9]{{5}}' | awk '{{print $2}}')",
-                                    is_async=False, hide=False).get_simple_out()
 
         kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
         kubeadm_flags = node["connection"].sudo(f"cat {kubeadm_flags_file}",
                                                 is_async=False).get_simple_out()
 
         #Removing the --network-plugin=cni switch after the cri migration procedure that was used to run Docker on the cluster.
         #Support for this key has been removed in kubernetes 1.24.
@@ -212,15 +202,20 @@
                                 "sudo iptables -t raw -F && "
                                 "sudo iptables -t filter -F && "
                                 # hotfix for Ubuntu 22.04
                                 "sudo systemctl stop kubepods-burstable.slice || true && "
                                 "sudo systemctl restart containerd && "
                                 # start kubelet
                                 "sudo systemctl restart kubelet")
-        control_plane["connection"].sudo(f"sudo kubectl uncordon {node['name']}", is_async=False, hide=False)
+
+        if "control-plane" in node["roles"]:
+            kubernetes.wait_uncordon(node["connection"])
+        else:
+            control_plane["connection"].sudo(f"kubectl uncordon {node['name']}", is_async=False, hide=False)
+
         if "control-plane" in node["roles"]:
             # hotfix for Ubuntu 22.04 and Kubernetes v1.21.2
             if version == "v1.21.2":
                 node['connection'].sudo("sleep 30 && "
                                         "sudo kubectl -n kube-system  delete pod "
                                         "$(sudo kubectl -n kube-system get pod --field-selector='status.phase=Pending' | "
                                         "grep 'kube-proxy' | awk '{ print $1 }') || true")
```

### Comparing `kubemarine-0.17.0/kubemarine/procedures/reboot.py` & `kubemarine-0.18.0/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.18.0/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/restore.py` & `kubemarine-0.18.0/kubemarine/procedures/restore.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.18.0/kubemarine/procedures/upgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,30 +11,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
-from copy import deepcopy
 from distutils.util import strtobool
 from io import StringIO
 from itertools import chain
 from typing import List
 
 import toml
 
 from kubemarine import kubernetes, plugins
 from kubemarine.core import flow
 from kubemarine.core import utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.resources import DynamicResources
-from kubemarine.core.yaml_merger import default_merger
 from kubemarine.procedures import install
 
 
 def system_prepare_thirdparties(cluster):
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
@@ -46,35 +44,33 @@
     cluster.log.debug("Prepulling Kubernetes images...")
     fix_cri_socket(cluster)
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
     upgrade_group.call(kubernetes.images_grouped_prepull)
 
 
 def kubernetes_upgrade(cluster):
-    version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
-    minor_version = int(version.split('.')[1])
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
-    kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
-
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
     grace_period = cluster.procedure_inventory.get('grace_period')
+    disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
+    drain_kwargs = {
+        'disable_eviction': disable_eviction, 'drain_timeout': drain_timeout, 'grace_period': grace_period
+    }
 
-    kubernetes.upgrade_first_control_plane(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
-                                           drain_timeout=drain_timeout, grace_period=grace_period)
+    kubernetes.upgrade_first_control_plane(upgrade_group, cluster, **drain_kwargs)
 
     # After first control-plane upgrade is finished we may loose our CoreDNS changes.
     # Thus, we need to re-apply our CoreDNS changes immediately after first control-plane upgrade.
     install.deploy_coredns(cluster)
 
-    kubernetes.upgrade_other_control_planes(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
-                                            drain_timeout=drain_timeout, grace_period=grace_period)
+    kubernetes.upgrade_other_control_planes(upgrade_group, cluster, **drain_kwargs)
+
     if cluster.nodes.get('worker', []):
-        kubernetes.upgrade_workers(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
-                                   drain_timeout=drain_timeout, grace_period=grace_period)
+        kubernetes.upgrade_workers(upgrade_group, cluster, **drain_kwargs)
 
     cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     cluster.context['cached_nodes_versions_cleaned'] = True
 
 
 def kubernetes_cleanup_nodes_versions(cluster):
     if not cluster.context.get('cached_nodes_versions_cleaned', False):
@@ -165,53 +161,14 @@
     "upgrade_containerd": upgrade_containerd,
     "plugins": upgrade_plugins,
     "overview": install.overview
 
 })
 
 
-def upgrade_finalize_inventory(cluster, inventory):
-    if cluster.context.get("initial_procedure") != "upgrade":
-        return inventory
-    upgrade_version = cluster.context.get("upgrade_version")
-
-    inventory.setdefault("services", {}).setdefault("kubeadm", {})['kubernetesVersion'] = upgrade_version
-
-    # if thirdparties was not defined in procedure.yaml,
-    # then no need to forcibly place them: user may want to use default
-    if cluster.procedure_inventory.get(upgrade_version, {}).get('thirdparties'):
-        inventory['services']['thirdparties'] = cluster.procedure_inventory[upgrade_version]['thirdparties']
-
-    if cluster.procedure_inventory.get(upgrade_version, {}).get("plugins"):
-        inventory.setdefault("plugins", {})
-        default_merger.merge(inventory["plugins"], cluster.procedure_inventory[upgrade_version]["plugins"])
-
-    if cluster.procedure_inventory.get(upgrade_version, {}).get("packages"):
-        inventory['services'].setdefault("packages", {})
-        packages_section = deepcopy(cluster.procedure_inventory[upgrade_version]["packages"])
-        for _type in ['install', 'upgrade', 'remove']:
-            packages = packages_section.pop(_type, None)
-            if packages is None:
-                continue
-            if isinstance(packages, list):
-                packages = {'include': packages}
-
-            packages_list = inventory['services']['packages'].get(_type)
-            if isinstance(packages_list, list):
-                inventory['services']['packages'][_type] = {
-                    'include': packages_list
-                }
-            default_merger.merge(inventory["services"]["packages"].setdefault(_type, {}), packages)
-        # Despite we enrich OS specific section inside system.enrich_upgrade_inventory,
-        # we still merge global associations section because it has priority during enrichment.
-        default_merger.merge(inventory["services"]["packages"], packages_section)
-
-    return inventory
-
-
 class UpgradeFlow(flow.Flow):
     def __init__(self):
         self.target_version = None
 
     def _run(self, resources: DynamicResources):
         logger = resources.logger()
 
@@ -237,15 +194,15 @@
         super().__init__('upgrade to ' + upgrade_version, recreate_inventory=True)
         self.upgrade_version = upgrade_version
 
     def run(self, res: DynamicResources):
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
-    def prepare_context(self, context: dict):
+    def prepare_context(self, context: dict) -> None:
         context['upgrade_version'] = self.upgrade_version
         context['dump_filename_prefix'] = self.upgrade_version
 
 
 def main(cli_arguments=None):
     cli_help = '''
     Script for automated upgrade of the entire Kubernetes cluster to a new version.
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This configuration is partially generated and maintained by "scripts/thirdparties/sync.py"
 #
 # If new Kubernetes version is added, the compatibility mapping is taken from the previous Kubernetes versions.
 # The developer should manually change the required package versions if necessary.
+#
+# After any change, kubemarine/patches/software_upgrade.yaml should also be manually changed.
 docker:
   v1.21.2:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
   v1.21.5:
     version_rhel: 19.03*
@@ -61,57 +63,42 @@
     version_debian: 5:20.10.*
   v1.27.1:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
 containerd:
   v1.21.2:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.21.5:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.21.12:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.22.2:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.22.9:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.23.6:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.23.11:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.23.17:
-    version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.24.2:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.24.11:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.25.2:
-    version_rhel8: 1.6*
     version_debian: 1.6.*
   v1.25.7:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.26.3:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.26.4:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.27.1:
-    version_rhel8: 1.4*
     version_debian: 1.6.*
 containerdio:
   v1.21.2:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.5.*
   v1.21.5:
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -329,15 +329,15 @@
               type: A
               zone: '{{ cluster_name }}'
               data:
                 match: '^(.*\.)?{{ cluster_name }}\.$'
                 answer: '{% raw %}{{ .Name }}{% endraw %} 3600 IN A {{ control_plain["internal"] }}'
             reject-aaaa:
               enabled: '{{ nodes[0]["internal_address"]|isipv4 }}'
-              priority: 999
+              priority: 1
               class: IN
               type: AAAA
               data:
                 authority: '{% raw %}{{ .Name }}{% endraw %} 3600 IN SOA coredns.kube-system.svc.cluster.local. hostmaster.coredns.kube-system.svc.cluster.local. (3600 3600 3600 3600 3600)'
           forward:
             - .
             - /etc/resolv.conf
@@ -365,73 +365,49 @@
       openssl: true
       curl: true
       unzip: true
       semanage: true
       kmod: true
     package_manager:
       replace-repositories: false
+    # Associations for each OS family are merged with 'package.common_associations' section of globals.yaml.
+    # Packages for docker, containerd, haproxy, and keepalived are calculated based on
+    # 'package.<OS family>' sections of globals.yaml, target Kubernetes version, and the compatibility map.
     associations:
       debian:
-        docker:
-          package_name:
-            - 'docker-ce={{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_debian }}'
-            - 'docker-ce-cli={{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_debian }}'
-            - 'containerd.io={{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_debian }}'
-        containerd:
-          package_name:
-            - 'containerd={{ globals.compatibility_map.software.containerd[services.kubeadm.kubernetesVersion].version_debian }}'
-            - 'podman={{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_debian }}'
+        docker: {}
+        containerd: {}
         haproxy:
           executable_name: 'haproxy'
-          package_name: 'haproxy={{ globals.compatibility_map.software.haproxy.version_debian }}'
           service_name: 'haproxy'
-        keepalived:
-          package_name: 'keepalived={{ globals.compatibility_map.software.keepalived.version_debian }}'
+        keepalived: {}
         audit:
           package_name: 'auditd'
         conntrack:
           package_name: 'conntrack'
       rhel:
-        docker:
-          package_name:
-            - 'docker-ce-{{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_rhel }}'
-            - 'docker-ce-cli-{{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_rhel }}'
-            - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel }}'
-        containerd:
-          package_name:
-            - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel }}'
-            - 'podman-{{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_rhel }}'
+        docker: {}
+        containerd: {}
         haproxy:
           executable_name: '/opt/rh/rh-haproxy18/root/usr/sbin/haproxy'
-          package_name: 'rh-haproxy18-haproxy-{{ globals.compatibility_map.software.haproxy.version_rhel }}'
           service_name: 'rh-haproxy18-haproxy'
-        keepalived:
-          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived.version_rhel }}'
+        keepalived: {}
         audit:
           package_name: 'audit'
         conntrack:
           package_name: 'conntrack-tools'
         semanage:
           package_name: 'policycoreutils-python'
       rhel8:
-        docker:
-          package_name:
-            - 'docker-ce-{{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_rhel8 }}'
-            - 'docker-ce-cli-{{ globals.compatibility_map.software.docker[services.kubeadm.kubernetesVersion].version_rhel8 }}'
-            - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel8 }}'
-        containerd:
-          package_name:
-            - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel8 }}'
-            - 'podman-{{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_rhel8 }}'
+        docker: {}
+        containerd: {}
         haproxy:
           executable_name: '/usr/sbin/haproxy'
-          package_name: 'haproxy-{{ globals.compatibility_map.software.haproxy.version_rhel8 }}'
           service_name: 'haproxy'
-        keepalived:
-          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived.version_rhel8 }}'
+        keepalived: {}
         audit:
           package_name: 'audit'
         conntrack:
           package_name: 'conntrack-tools'
         semanage:
           package_name: 'policycoreutils-python-utils'
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.18.0/kubemarine/resources/configurations/globals.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -149,14 +149,62 @@
     software_name: crictl
     source_prefix:
       public: https://github.com/kubernetes-sigs/cri-tools/releases/download
       private: '{registry}/kubernetes-sigs/cri-tools'
     relative_path: '{version}/crictl-{version}-linux-amd64.tar.gz'
 
 packages:
+  debian:
+    docker:
+      package_name:
+        - docker-ce: docker
+        - docker-ce-cli: docker
+        - containerd.io: containerdio
+    containerd:
+      package_name:
+        - containerd: containerd
+        - podman: podman
+    haproxy:
+      package_name:
+        - haproxy: haproxy
+    keepalived:
+      package_name:
+        - keepalived: keepalived
+  rhel:
+    docker:
+      package_name:
+        - docker-ce: docker
+        - docker-ce-cli: docker
+        - containerd.io: containerdio
+    containerd:
+      package_name:
+        - containerd.io: containerdio
+        - podman: podman
+    haproxy:
+      package_name:
+        - rh-haproxy18-haproxy: haproxy
+    keepalived:
+      package_name:
+        - keepalived: keepalived
+  rhel8:
+    docker:
+      package_name:
+        - docker-ce: docker
+        - docker-ce-cli: docker
+        - containerd.io: containerdio
+    containerd:
+      package_name:
+        - containerd.io: containerdio
+        - podman: podman
+    haproxy:
+      package_name:
+        - haproxy: haproxy
+    keepalived:
+      package_name:
+        - keepalived: keepalived
   common_associations:
     docker:
       executable_name: 'docker'
       service_name: 'docker'
       config_location: '/etc/docker/daemon.json'
       groups:
         - control-plane
@@ -274,14 +322,15 @@
           - '7.8'
           - '7.9'
       - os_family: 'rhel8'
         versions:
           - '8.4'
           - '8.6'
           - '8.7'
+          - '8.8'
     rocky:
       - os_family: 'rhel8'
         versions:
           - '8.6'
           - '8.7'
     ubuntu:
       - os_family: 'debian'
@@ -331,16 +380,18 @@
         - 80
         - 443
 logging:
   default_targets:
     stdout:
       level: debug
       correct_newlines: True
+      colorize: true
+      format: "%(asctime)s %(levelname)s %(message)s"
     dump:
       level: verbose
-      format: "%(asctime)s %(process)s %(thread)s %(name)s %(levelname)s [%(module)s.%(funcName)s] %(message)s"
+      format: "%(asctime)s %(levelname)s [%(module)s.%(funcName)s] %(message)s"
       colorize: False
       correct_newlines: True
 
 prepull_group_size: 20
 accounts:
   retries: 10
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 
 from typing import List
 
 from kubemarine.core.patch import Patch
 
 patches: List[Patch] = [
 ]
-"""List of patches which can be executed strictly in the declared order"""
+"""
+List of patches that is sorted according to the Patch.priority() before execution.
+Patches that have the same priority, are executed in the declared order.
+"""
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.18.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.18.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.18.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.18.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.18.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998724489795918%*

 * *Differences: {"'properties'": "{'controller': {'properties': {'args': OrderedDict([('type', 'array'), "*

 * *                 "('description', 'Additional arguments.')])}}}"}*

```diff
@@ -46,14 +46,18 @@
             "description": "Customize or fine tune NGINX behavior",
             "type": "object"
         },
         "controller": {
             "additionalProperties": false,
             "description": "NGINX Ingress Controller configuration",
             "properties": {
+                "args": {
+                    "description": "Additional arguments.",
+                    "type": "array"
+                },
                 "image": {
                     "description": "Specifies the string for the NGINX Ingress Controller image",
                     "type": "string"
                 },
                 "nodeSelector": {
                     "$ref": "generic_plugin.json#/definitions/CommonNodeSelector"
                 },
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'definitions'": "{'DisableEviction': OrderedDict([('type', 'boolean'), ('default', True), "*

 * *                  "('description', 'If specified to false, enforces PDB rules during the "*

 * *                  "upgrade')])}"}*

```diff
@@ -1,10 +1,15 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
+        "DisableEviction": {
+            "default": true,
+            "description": "If specified to false, enforces PDB rules during the upgrade",
+            "type": "boolean"
+        },
         "DrainTimeout": {
             "description": "Time to wait for the pods' killing",
             "type": "integer"
         },
         "GracePeriod": {
             "default": 60,
             "description": "Time to wait in seconds for the pods' migration to other nodes during draining before killing them",
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9809027777777778%*

 * *Differences: {"'definitions'": "{'PackageAssociationsProperties': {'properties': {'package_name': {replace: "*

 * *                  "OrderedDict([('$ref', '#/definitions/PackageName')])}}}, 'PackageName': "*

 * *                  "OrderedDict([('description', 'Packages with versions to install if the "*

 * *                  "associated service is required for the cluster'), ('oneOf', "*

 * *                  "[OrderedDict([('type', 'string')]), OrderedDict([('$ref', "*

 * *                  "'../../common/utils.json#/definitions/NonEmptySetOf […]*

```diff
@@ -90,44 +90,45 @@
             "properties": {
                 "cache_versions": {
                     "default": true,
                     "description": "Specifies whether to install exactly the same package versions from package_name section during the add_node procedure",
                     "type": "boolean"
                 },
                 "package_name": {
-                    "description": "Packages with versions to install if the associated service is required for the cluster",
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "items": {
-                                "oneOf": [
-                                    {
-                                        "type": "string"
-                                    },
-                                    {
-                                        "$ref": "../../common/utils.json#/definitions/ListMergingSymbol"
-                                    }
-                                ]
-                            },
-                            "minItems": 1,
-                            "type": "array",
-                            "uniqueItems": true
-                        }
-                    ]
+                    "$ref": "#/definitions/PackageName"
                 }
             }
         },
         "PackageAssociationsPropertyNames": {
             "enum": [
                 "package_name",
                 "cache_versions"
             ]
         },
+        "PackageName": {
+            "description": "Packages with versions to install if the associated service is required for the cluster",
+            "oneOf": [
+                {
+                    "type": "string"
+                },
+                {
+                    "$ref": "../../common/utils.json#/definitions/NonEmptySetOfStrings"
+                }
+            ]
+        },
+        "PackageNameOnlyAssociations": {
+            "additionalProperties": false,
+            "description": "Associations related to specific package",
+            "properties": {
+                "package_name": {
+                    "$ref": "#/definitions/PackageName"
+                }
+            },
+            "type": "object"
+        },
         "ServicePackageAssociations": {
             "allOf": [
                 {
                     "$ref": "#/definitions/PackageAssociationsProperties"
                 }
             ],
             "description": "Associations related to specific package",
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9035218253968254%*

 * *Differences: {"'allOf'": "{0: {'$ref': '#/definitions/CustomPackages'}}",*

 * * "'definitions'": "{'CustomPackages': OrderedDict([('properties', OrderedDict([('install', "*

 * *                  "OrderedDict([('description', 'List of custom packages to install. Can be "*

 * *                  'specified as list or as two lists that are to be included and excluded during '*

 * *                  "processing.'), ('oneOf', [OrderedDict([('type', 'object'), ('allOf', "*

 * *                  "[OrderedDict([('$ref', '#/definitions/IncludeExcludeProp […]*

```diff
@@ -1,55 +1,20 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "allOf": [
         {
-            "$ref": "#/definitions/Properties"
+            "$ref": "#/definitions/CustomPackages"
         }
     ],
     "definitions": {
         "AptRepositories": {
             "$ref": "../common/utils.json#/definitions/NonEmptySetOfStrings"
         },
-        "IncludeExcludePermissive": {
-            "allOf": [
-                {
-                    "$ref": "#/definitions/IncludeExcludeProperties"
-                }
-            ],
-            "minProperties": 1,
-            "propertyNames": {
-                "$ref": "#/definitions/IncludeExcludePropertyNames"
-            },
-            "type": "object"
-        },
-        "IncludeExcludeProperties": {
-            "properties": {
-                "exclude": {
-                    "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
-                    "description": "List of packages to exclude from processing. Type of processing is defined by parent section."
-                },
-                "include": {
-                    "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
-                    "description": "List of packages to include in processing. Type of processing is defined by parent section."
-                }
-            }
-        },
-        "IncludeExcludePropertyNames": {
-            "enum": [
-                "include",
-                "exclude"
-            ]
-        },
-        "Properties": {
+        "CustomPackages": {
             "properties": {
-                "cache_versions": {
-                    "default": true,
-                    "description": "Specifies whether to install exactly the same package versions from associations section during the add_node procedure",
-                    "type": "boolean"
-                },
                 "install": {
                     "description": "List of custom packages to install. Can be specified as list or as two lists that are to be included and excluded during processing.",
                     "oneOf": [
                         {
                             "allOf": [
                                 {
                                     "$ref": "#/definitions/IncludeExcludeProperties"
@@ -88,20 +53,49 @@
                         {
                             "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings"
                         }
                     ]
                 }
             }
         },
-        "PropertyNames": {
+        "CustomPackagesPropertyNames": {
             "enum": [
                 "install",
                 "upgrade",
-                "remove",
-                "cache_versions"
+                "remove"
+            ]
+        },
+        "IncludeExcludePermissive": {
+            "allOf": [
+                {
+                    "$ref": "#/definitions/IncludeExcludeProperties"
+                }
+            ],
+            "minProperties": 1,
+            "propertyNames": {
+                "$ref": "#/definitions/IncludeExcludePropertyNames"
+            },
+            "type": "object"
+        },
+        "IncludeExcludeProperties": {
+            "properties": {
+                "exclude": {
+                    "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
+                    "description": "List of packages to exclude from processing. Type of processing is defined by parent section."
+                },
+                "include": {
+                    "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
+                    "description": "List of packages to include in processing. Type of processing is defined by parent section."
+                }
+            }
+        },
+        "IncludeExcludePropertyNames": {
+            "enum": [
+                "include",
+                "exclude"
             ]
         },
         "YumRepositories": {
             "additionalProperties": {
                 "properties": {
                     "baseurl": {
                         "type": "string"
@@ -123,14 +117,19 @@
     },
     "description": "Section for packages and their management",
     "properties": {
         "associations": {
             "$ref": "packages/associations.json",
             "description": "Configure predefined associations of package objects. If configured in the common section, the associations are automatically switched to the section corresponding to your operating system."
         },
+        "cache_versions": {
+            "default": true,
+            "description": "Specifies whether to install exactly the same package versions from associations section during the add_node procedure",
+            "type": "boolean"
+        },
         "mandatory": {
             "additionalProperties": false,
             "description": "Specify whether to install or skip mandatory packages",
             "properties": {
                 "conntrack": {
                     "default": true,
                     "type": "boolean"
@@ -188,20 +187,21 @@
             },
             "type": "object"
         }
     },
     "propertyNames": {
         "anyOf": [
             {
-                "$ref": "#/definitions/PropertyNames"
+                "$ref": "#/definitions/CustomPackagesPropertyNames"
             },
             {
                 "enum": [
                     "package_manager",
                     "mandatory",
-                    "associations"
+                    "associations",
+                    "cache_versions"
                 ]
             }
         ]
     },
     "type": "object"
 }
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.18.0/kubemarine/resources/schemas/upgrade.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915332031249999%*

 * *Differences: {"'additionalProperties'": "{'properties': {'packages': {'allOf': {0: {'$ref': "*

 * *                           "'definitions/services/packages.json#/definitions/CustomPackages'}}, "*

 * *                           "'properties': {'associations': {'properties': {'docker': {'$ref': "*

 * *                           "'definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations'}, "*

 * *                           "'containerd': {'$ref': "*

 * *                           "'definitions/services/packages/as […]*

```diff
@@ -3,37 +3,37 @@
     "additionalProperties": {
         "additionalProperties": false,
         "description": "Configuration for the upgrade to the particular version from the 'upgrade_plan'",
         "properties": {
             "packages": {
                 "allOf": [
                     {
-                        "$ref": "definitions/services/packages.json#/definitions/Properties"
+                        "$ref": "definitions/services/packages.json#/definitions/CustomPackages"
                     }
                 ],
                 "description": "Section for packages and their management during upgrade",
                 "properties": {
                     "associations": {
                         "additionalProperties": false,
                         "description": "Configure associations of package objects to be used during upgrade",
                         "properties": {
                             "containerd": {
-                                "$ref": "definitions/services/packages/associations.json#/definitions/ServicePackageAssociations"
+                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
                             },
                             "docker": {
-                                "$ref": "definitions/services/packages/associations.json#/definitions/ServicePackageAssociations"
+                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
                             }
                         },
                         "type": "object"
                     }
                 },
                 "propertyNames": {
                     "anyOf": [
                         {
-                            "$ref": "definitions/services/packages.json#/definitions/PropertyNames"
+                            "$ref": "definitions/services/packages.json#/definitions/CustomPackagesPropertyNames"
                         },
                         {
                             "enum": [
                                 "associations"
                             ]
                         }
                     ]
@@ -47,17 +47,15 @@
                 "$ref": "definitions/services/thirdparties.json"
             }
         },
         "type": "object"
     },
     "properties": {
         "disable-eviction": {
-            "default": true,
-            "description": "If specified to false, enforces PDB rules during the upgrade",
-            "type": "boolean"
+            "$ref": "definitions/procedures.json#/definitions/DisableEviction"
         },
         "drain_timeout": {
             "$ref": "definitions/procedures.json#/definitions/DrainTimeout"
         },
         "grace_period": {
             "$ref": "definitions/procedures.json#/definitions/GracePeriod"
         },
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.18.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.18.0/kubemarine/core/os.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,34 @@
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
 
-# Check url availability script.
-# The script is for testing purpose only.
-# The first argv parameter is source. The second argv parameter is the timeout.
-
-import sys
-
-major_version = sys.version_info.major
-if major_version == 3:
-    import urllib.request as urllib
-else:
-    import urllib2 as urllib
-
-try:
-    source = sys.argv[1]
-    timeout = int(sys.argv[2])
-    status_code = urllib.urlopen(source, timeout=timeout).getcode()
-    if status_code != 200:
-        sys.stderr.write("Error status code: %s" % status_code)
-        exit(1)
-except Exception as e:
-    sys.stderr.write(str(e))
-    exit(1)
+import os
+from typing import Iterator, Mapping
+
+
+class Environ(Mapping[str, str]):
+    """
+    Read-only view of os.environ.
+    """
+
+    def __getitem__(self, name: str) -> str:
+        # check presence of the variable and throw KeyError if necessary
+        return os.environ[name]
+
+    def __len__(self) -> int:
+        return len(os.environ)
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(os.environ)
+
+    __slots__ = []
```

### Comparing `kubemarine-0.17.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.18.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.18.0/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/selinux.py` & `kubemarine-0.18.0/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/sysctl.py` & `kubemarine-0.18.0/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/system.py` & `kubemarine-0.18.0/kubemarine/system.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,28 +14,25 @@
 
 import configparser
 import io
 import paramiko
 import re
 import socket
 import time
-from copy import deepcopy
 from typing import Dict
 
 from dateutil.parser import parse
 import fabric
-import yaml
 from ordered_set import OrderedSet
 
 from kubemarine import selinux, kubernetes, apparmor
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroupResult, NodeGroup
-from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.annotations import restrict_empty_group
 
 ERROR_UNSUPPORTED_KERNEL_MODULES_VERSIONS_DETECTED = \
         "Kernel modules are not available for the current OS family"
 
 def verify_inventory(inventory, cluster):
 
@@ -79,67 +76,14 @@
             external_node_ip_names.append(node['name'] + "-external")
             external_node_ip_names = list(OrderedSet(external_node_ip_names))
             inventory['services']['etc_hosts_generated'][node['address']] = external_node_ip_names
 
     return inventory
 
 
-def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster):
-    if cluster.context.get("initial_procedure") != "upgrade":
-        return inventory
-
-    os_family = cluster.get_os_family()
-    if os_family in ('unknown', 'unsupported', 'multiple'):
-        raise Exception("Upgrade is possible only for cluster "
-                        "with all nodes having the same and supported OS family")
-
-    # validate all packages sections in procedure inventory
-    base_associations = static.DEFAULTS["services"]["packages"]["associations"][os_family]
-
-    cluster_associations = deepcopy(inventory["services"]["packages"]["associations"][os_family])
-    previous_ver = cluster.context["initial_kubernetes_version"]
-    upgrade_plan = cluster.procedure_inventory.get('upgrade_plan')
-    for version in upgrade_plan:
-        upgrade_associations = cluster.procedure_inventory.get(version, {}).get("packages", {}).get("associations", {})
-        for package in get_system_packages(cluster):
-            if base_associations[package]["package_name"] != cluster_associations[package]["package_name"] \
-                    and not upgrade_associations.get(package, {}).get("package_name"):
-                raise Exception(f"Associations are redefined for {package} in cluster.yaml for version {previous_ver}, "
-                                f"but not present in procedure inventory for version {version}. "
-                                f"Please, specify required associations explicitly in procedure inventory "
-                                f"for all versions since {previous_ver}.")
-            if upgrade_associations.get(package, {}).get("package_name"):
-                cluster_associations[package]["package_name"] = upgrade_associations[package]["package_name"]
-        previous_ver = version
-
-    upgrade_required = get_system_packages_for_upgrade(cluster)
-    cluster.context["packages"] = {"upgrade_required": upgrade_required}
-
-    upgrade_ver = cluster.context["upgrade_version"]
-    packages_section = deepcopy(cluster.procedure_inventory.get(upgrade_ver, {}).get("packages", {}))
-    # Move associations to the OS family specific section, and then merge with associations from procedure.
-    # This effectively allows to specify only global section but not for specific OS family.
-    # This restriction is because system.enrich_upgrade_inventory goes after packages.enrich_inventory_associations,
-    # but in future the restriction can be eliminated.
-    associations = packages_section.pop("associations", {})
-    default_merger.merge(inventory["services"]["packages"]["associations"][os_family], associations)
-
-    for _type in ['install', 'upgrade', 'remove']:
-        packages = packages_section.pop(_type, None)
-        if packages is None:
-            continue
-        if isinstance(packages, list):
-            packages = {'include': packages}
-        default_merger.merge(inventory["services"]["packages"].setdefault(_type, {}), packages)
-
-    # merge remained packages section
-    default_merger.merge(inventory["services"]["packages"], packages_section)
-
-    return inventory
-
 def enrich_kernel_modules(inventory: dict, cluster: KubernetesCluster):
     """
     The method enrich the list of kernel modules ('services.modprobe') according to OS family
     """
     
     os_family = cluster.get_os_family()
     if os_family in ["unknown", "unsupported"]:
@@ -155,41 +99,14 @@
             os_families.add(cluster.get_os_family_for_node(node))
         for item in os_families:
             modprobe[item] = inventory["services"]["modprobe"][item]
         inventory["services"]["modprobe"] = modprobe
 
     return inventory
 
-def get_system_packages_for_upgrade(cluster):
-    upgrade_ver = cluster.context["upgrade_version"]
-    previous_ver = cluster.context["initial_kubernetes_version"]
-    compatibility = cluster.globals["compatibility_map"]["software"]
-
-    # handle special cases in which upgrade is not required for particular package
-    cluster_associations = cluster.inventory["services"]["packages"]["associations"][cluster.get_os_family()]
-    upgrade_associations = cluster.procedure_inventory.get(upgrade_ver, {}).get("packages", {}).get("associations", {})
-    system_packages = get_system_packages(cluster)
-    upgrade_required = list(system_packages)
-    for package in system_packages:
-        defined_association = upgrade_associations.get(package, {}).get("package_name")
-        if defined_association and defined_association == cluster_associations[package]['package_name']:
-            # case 1: package_name is defined in upgrade inventory but is equal to one already defined in cluster.yaml
-            upgrade_required.remove(package)
-        elif compatibility.get(package) and compatibility[package][upgrade_ver] == compatibility[package][previous_ver] \
-                and not defined_association:
-            # case 2: package_name is not defined in upgrade inventory and default versions are equal
-            upgrade_required.remove(package)
-
-    # all other packages should be updated
-    return upgrade_required
-
-
-def get_system_packages(cluster):
-    return [cluster.inventory['services']['cri']['containerRuntime']]
-
 
 def fetch_os_versions(cluster: KubernetesCluster):
     group = cluster.nodes['all'].get_accessible_nodes()
     '''
     For Red Hat, CentOS, Oracle Linux, and Ubuntu information in /etc/os-release /etc/redhat-release is sufficient but,
     Debian stores the full version in a special file. sed transforms version string, eg 10.10 becomes DEBIAN_VERSION="10.10"  
     '''
@@ -225,51 +142,36 @@
                 version = os_release.get("system", "debian_version").replace('"', '')
             else:
                 # Oracle Linux and Ubuntu have full version in VERSION_ID string
                 version = os_release.get("system", "version_id").replace('"', '')
 
         cluster.log.debug("Distribution: %s; Version: %s" % (name, version))
 
-        os_family = 'unsupported'
-        if name in cluster.globals["compatibility_map"]["distributives"]:
-            os_family = 'unknown'
-            os_family_list = cluster.globals["compatibility_map"]["distributives"][name]
-            for os_family_item in os_family_list:
-                if version in os_family_item["versions"]:
-                    os_family = os_family_item["os_family"]
-                    break
+        os_family = detect_of_family_by_name_version(name, version)
 
         cluster.log.debug("OS family: %s" % os_family)
 
         cluster.context["nodes"][connection.host]["os"] = {
             'name': name,
             'version': version,
             'family': os_family
         }
 
 
-def get_compatibility_version_key(cluster: KubernetesCluster) -> str or None:
-    """
-    Get os-specific version key to be used in software compatibility map.
-    :param cluster: Cluster object for which to resolve compatibility version key.
-    :return: String to use as version key. None if OS is unknown or multiple OS present.
-    """
-    """
-    Return os-specific version compatibility key.
-    If OS is unknown or multiple OS, then returns None.
-    """
-    os = cluster.get_os_family()
-    if os == "rhel":
-        return "version_rhel"
-    elif os == "rhel8":
-        return "version_rhel8"
-    elif os == "debian":
-        return "version_debian"
-    else:
-        return None
+def detect_of_family_by_name_version(name: str, version: str) -> str:
+    os_family = 'unsupported'
+    if name in static.GLOBALS["compatibility_map"]["distributives"]:
+        os_family = 'unknown'
+        os_family_list = static.GLOBALS["compatibility_map"]["distributives"][name]
+        for os_family_item in os_family_list:
+            if version in os_family_item["versions"]:
+                os_family = os_family_item["os_family"]
+                break
+
+    return os_family
 
 
 def update_resolv_conf(group, config=None):
     if config is None:
         raise Exception("Data can't be empty")
 
     # TODO: Use Jinja template
@@ -447,16 +349,16 @@
     first_control_plane = group.cluster.nodes['control-plane'].get_first_member()
     results = NodeGroupResult(group.cluster)
 
     for node in group.get_ordered_members_list(provide_node_configs=True):
         cordon_required = 'control-plane' in node['roles'] or 'worker' in node['roles']
         if cordon_required:
             res = first_control_plane.sudo(
-                kubernetes.prepare_drain_command(node, group.cluster.inventory['services']['kubeadm']['kubernetesVersion'],
-                                                 group.cluster.globals, False, group.cluster.nodes), warn=True)
+                kubernetes.prepare_drain_command(group.cluster, node["name"], disable_eviction=False),
+                warn=True)
             log.verbose(res)
         log.debug(f'Rebooting node "{node["name"]}"')
         raw_results = perform_group_reboot(node['connection'])
         if cordon_required:
             res = first_control_plane.sudo(f'kubectl uncordon {node["name"]}', warn=True)
             log.verbose(res)
         results.update(raw_results)
```

### Comparing `kubemarine-0.17.0/kubemarine/templates/__init__.py` & `kubemarine-0.18.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.18.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.18.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.18.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.18.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine/testsuite.py` & `kubemarine-0.18.0/kubemarine/testsuite.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import io
 import textwrap
 from traceback import *
 import csv
 from datetime import datetime
-from kubemarine.core import utils
+from kubemarine.core import utils, log
 import fabric
 
 TC_UNKNOWN = -1
 TC_PASSED = 0
 TC_FAILED = 1
 TC_WARNED = 2
 TC_EXCEPTED = 3
@@ -52,23 +52,24 @@
                 value.result.print()
             else:
                 print_exc()
             self.exception(value)
         print(self.get_summary(show_hint=True))
         return True
 
-    def __init__(self, ts, id, category, name, default_results=None, minimal=None, recommended=None):
-        self.include_in_ts(ts)
+    def __init__(self, cluster, id, category, name, default_results=None, minimal=None, recommended=None):
+        self.include_in_ts(cluster.context['testsuite'])
         self.category = category
         self.id = str(id)
         self.name = name
         self.status = TC_UNKNOWN
         self.results = default_results
         self.minimal = minimal
         self.recommended = recommended
+        self.cluster = cluster
 
     def include_in_ts(self, ts):
         ts.register_tc(self)
         return self
 
     def success(self, results=None):
         if self.results is None:
@@ -95,33 +96,48 @@
         output = ""
 
         output += " " * (15 - len(self.category))
         output += self.category + "  "
 
         color = ""
         if self.is_succeeded():
-            color = "\x1b[38;5;041m"
-            output += " \x1b[48;5;041m\x1b[38;5;232m   OK   \x1b[49m\x1b[39m  "
+            if self.check_color():
+                color = "\x1b[38;5;041m"
+                output += " \x1b[48;5;041m\x1b[38;5;232m   OK   \x1b[49m\x1b[39m  "
+            else:
+                output += "    OK     "
         if self.is_failed():
-            color = "\x1b[38;5;196m"
-            output += " \x1b[48;5;196m\x1b[38;5;231m  FAIL  \x1b[49m\x1b[39m  "
+            if self.check_color():
+                color = "\x1b[38;5;196m"
+                output += " \x1b[48;5;196m\x1b[38;5;231m  FAIL  \x1b[49m\x1b[39m  "
+            else:
+                output += "   FAIL    "
         if self.is_warned():
-            color = "\x1b[38;5;208m"
-            output += " \x1b[48;5;208m\x1b[38;5;231m  WARN  \x1b[49m\x1b[39m  "
+            if self.check_color():
+                color = "\x1b[38;5;208m"
+                output += " \x1b[48;5;208m\x1b[38;5;231m  WARN  \x1b[49m\x1b[39m  "
+            else:
+                output += "   WARN    "
         if self.is_excepted():
-            color = "\x1b[31m"
-            output += " \x1b[41m ERROR? \x1b[49m  "
+            if self.check_color():
+                color = "\x1b[31m"
+                output += " \x1b[41m ERROR? \x1b[49m  "
+            else:
+                output += "  ERROR?   "
 
         output += self.id + "  "
         output += self.name + " "
 
         results = " " + str(self.results)
 
         output += "." * (146 - len(output) - len(results))
-        output += "%s%s\x1b[39m" % (color, results)
+        if self.check_color():
+            output += "%s%s\x1b[39m" % (color, results)
+        else:
+            output += "%s" % (results)
 
         if show_minimal:
             if self.minimal is None:
                 output += ' ' * 15
             else:
                 minimal = str(self.minimal)
                 output += ' ' * (15-len(minimal)) + minimal
@@ -134,14 +150,20 @@
                 output += ' ' * (14-len(recommended)) + recommended
 
         if show_hint and (isinstance(self.results, TestFailure) or isinstance(self.results, TestWarn)) and self.results.hint is not None:
             output += "\n                  HINT:\n" + textwrap.indent(str(self.results.hint), "                       ")
 
         return output
 
+    def check_color(self):
+        for handler in self.cluster.log.handlers:
+            if isinstance(handler, log.StdoutHandler) and handler.formatter.colorize:
+                return True
+        return False
+
     def get_readable_status(self):
         if self.is_succeeded():
             return 'ok'
         if self.is_failed():
             return 'fail'
         if self.is_warned():
             return 'warning'
@@ -213,23 +235,26 @@
         for tc in self.tcs:
             result += "\n" + tc.get_summary(show_minimal=show_minimal, show_recommended=show_recommended)
 
         result += "\n\nOVERALL RESULTS: "
 
         for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
             colors = ''
-            if key == 'succeeded':
-                colors = "\x1b[48;5;041m\x1b[38;5;232m"
-            if key == 'failed':
-                colors = "\x1b[48;5;196m\x1b[38;5;231m"
-            if key == 'warned':
-                colors = "\x1b[48;5;208m\x1b[38;5;231m"
-            if key == 'excepted':
-                colors = "\x1b[41m"
-            result += "%s %s %s \x1b[49m\x1b[39m " % (colors, value ,key.upper())
+            if tc.check_color():
+                if key == 'succeeded':
+                    colors = "\x1b[48;5;041m\x1b[38;5;232m"
+                if key == 'failed':
+                    colors = "\x1b[48;5;196m\x1b[38;5;231m"
+                if key == 'warned':
+                    colors = "\x1b[48;5;208m\x1b[38;5;231m"
+                if key == 'excepted':
+                    colors = "\x1b[41m"
+                result += "%s %s %s \x1b[49m\x1b[39m " % (colors, value ,key.upper())
+            else:
+                result += "%s %s  " % (value ,key.upper())
 
         result += "\n"
 
         return result
 
     def print_final_status(self, log):
         if self.is_any_test_failed():
@@ -255,51 +280,57 @@
             elif tc.is_excepted():
                 key = 'excepted'
             value = results.get(key, 0) + 1
             results[key] = value
         return results
 
     def save_csv(self, destination_file_path, delimiter=';'):
-        with utils.open_external(destination_file_path, mode='w') as stream:
-            csv_writer = csv.writer(stream, delimiter=delimiter, quotechar='"', quoting=csv.QUOTE_MINIMAL)
-            csv_writer.writerow(['group', 'status', 'test_id', 'test_name', 'current_result', 'minimal_result', 'recommended_result'])
-            for tc in self.tcs:
-                csv_writer.writerow([
-                    tc.category.lower(),
-                    tc.get_readable_status(),
-                    tc.id,
-                    tc.name,
-                    tc.results,
-                    tc.minimal,
-                    tc.recommended
-                ])
+        stream = io.StringIO()
+
+        csv_writer = csv.writer(stream, delimiter=delimiter, quotechar='"', quoting=csv.QUOTE_MINIMAL)
+        csv_writer.writerow(['group', 'status', 'test_id', 'test_name', 'current_result', 'minimal_result', 'recommended_result'])
+        for tc in self.tcs:
+            csv_writer.writerow([
+                tc.category.lower(),
+                tc.get_readable_status(),
+                tc.id,
+                tc.name,
+                tc.results,
+                tc.minimal,
+                tc.recommended
+            ])
+
+        utils.dump_file({}, stream, destination_file_path, dump_location=False)
 
     def save_html(self, destination_file_path, check_type, append_styles=True):
-        with utils.open_external(destination_file_path, mode='w') as stream:
-            stream.write('<!DOCTYPE html><html><head><meta charset="utf-8"><title>%s Check Report</title></head><body><div id="date">%s</div><div id="stats">' % (check_type, datetime.utcnow()))
-            for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
-                stream.write('<div class="%s">%s %s</div>' % (key, value, key))
-            stream.write('</div><h1>%s Check Report</h1><table>' % check_type)
-            stream.write('<thead><tr><td>Group</td><td>Status</td><td>ID</td><td>Test</td><td>Actual Result</td><td>Minimal</td><td>Recommended</td></tr></thead><tbody>')
-            for tc in self.tcs:
-                minimal = tc.minimal
-                if minimal is None:
-                    minimal = ''
-                recommended = tc.recommended
-                if recommended is None:
-                    recommended = ''
-                stream.write('<tr class="%s"><td>%s</td><td><div>%s</div></td><td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>' %
-                             (tc.get_readable_status(),
-                              tc.category.lower(),
-                              tc.get_readable_status(),
-                              tc.id,
-                              tc.name,
-                              tc.results,
-                              minimal,
-                              recommended
-                              ))
-            stream.write('</tbody></table>')
-            if append_styles:
-                css = utils.read_internal('resources/reports/check_report.css')
-                stream.write('<style>\n%s\n</style>' % css)
+        stream = io.StringIO()
+
+        stream.write('<!DOCTYPE html><html><head><meta charset="utf-8"><title>%s Check Report</title></head><body><div id="date">%s</div><div id="stats">' % (check_type, datetime.utcnow()))
+        for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
+            stream.write('<div class="%s">%s %s</div>' % (key, value, key))
+        stream.write('</div><h1>%s Check Report</h1><table>' % check_type)
+        stream.write('<thead><tr><td>Group</td><td>Status</td><td>ID</td><td>Test</td><td>Actual Result</td><td>Minimal</td><td>Recommended</td></tr></thead><tbody>')
+        for tc in self.tcs:
+            minimal = tc.minimal
+            if minimal is None:
+                minimal = ''
+            recommended = tc.recommended
+            if recommended is None:
+                recommended = ''
+            stream.write('<tr class="%s"><td>%s</td><td><div>%s</div></td><td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>' %
+                         (tc.get_readable_status(),
+                          tc.category.lower(),
+                          tc.get_readable_status(),
+                          tc.id,
+                          tc.name,
+                          tc.results,
+                          minimal,
+                          recommended
+                          ))
+        stream.write('</tbody></table>')
+        if append_styles:
+            css = utils.read_internal('resources/reports/check_report.css')
+            stream.write('<style>\n%s\n</style>' % css)
+
+        stream.write('</body></html>')
 
-            stream.write('</body></html>')
+        utils.dump_file({}, stream, destination_file_path, dump_location=False)
```

### Comparing `kubemarine-0.17.0/kubemarine/thirdparties.py` & `kubemarine-0.18.0/kubemarine/thirdparties.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 from copy import deepcopy
 from typing import Tuple, Optional, Dict, List
 
-from kubemarine.core import utils, static
+from kubemarine.core import utils, static, errors
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroupResult, NodeGroup
+from kubemarine.core.yaml_merger import default_merger
 
 
 def is_default_thirdparty(destination: str):
     return destination in static.GLOBALS['thirdparties']
 
 
 def get_default_thirdparties() -> List[str]:
@@ -87,59 +88,147 @@
         raise Exception(f"{destination} is not a default 3rd-party")
 
     thirdparty_settings = static.GLOBALS['thirdparties'][destination]
     software_name = thirdparty_settings['software_name']
     return static.GLOBALS['compatibility_map']['software'][software_name][kubernetes_version]
 
 
+def get_thirdparty_destination(software_name: str) -> str:
+    for destination, thirdparty_settings in static.GLOBALS['thirdparties'].items():
+        if thirdparty_settings['software_name'] == software_name:
+            return destination
+    else:
+        raise Exception(f"Failed to find third-party destination for {software_name!r}")
+
+
 def get_thirdparty_recommended_sha(destination: str, cluster: KubernetesCluster) -> Optional[str]:
     if not is_default_thirdparty(destination):
         # 3rd-party is not managed by Kubemarine
         return None
 
     cluster.log.verbose("Calculate recommended sha for thirdparty %s..." % destination)
     _, recommended_sha = get_default_thirdparty_identity(cluster.inventory,
                                                          destination, in_public=True)
     cluster.log.verbose(f"Recommended sha for thirdparty {destination} was calculated: {recommended_sha}")
 
     return recommended_sha
 
 
-def enrich_inventory_apply_upgrade_defaults(inventory, cluster):
-    if cluster.context.get('initial_procedure') == 'upgrade':
-        upgrade_version = cluster.context["upgrade_version"]
-        upgrade_thirdparties = cluster.procedure_inventory.get(upgrade_version, {}).get('thirdparties')
-        if upgrade_thirdparties:
-            upgrade_thirdparties = deepcopy(upgrade_thirdparties)
-            default_thirdparties = static.DEFAULTS['services']['thirdparties']
-
-            # keep some configurations (unpack) from default thirdparties, if they are not re-defined
-            for destination, config in upgrade_thirdparties.items():
-                if destination in default_thirdparties and 'unpack' in default_thirdparties[destination]\
-                        and 'unpack' not in config:
-                    config['unpack'] = deepcopy(default_thirdparties[destination]['unpack'])
-
-            inventory['services']['thirdparties'] = upgrade_thirdparties
-        else:
-            cluster.log.warning('New thirdparties for upgrade procedure is not set in procedure config - default will be used')
+def _convert_thirdparty(thirdparties: dict, destination: str) -> dict:
+    config = thirdparties.setdefault(destination, {})
+    if isinstance(config, str):
+        thirdparties[destination] = config = {
+            'source': config
+        }
+
+    return config
+
+
+def _get_upgrade_plan(cluster: KubernetesCluster) -> List[Tuple[str, dict]]:
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        upgrade_version = context["upgrade_version"]
+        upgrade_plan = []
+        for version in cluster.procedure_inventory.get('upgrade_plan'):
+            if utils.version_key(version) < utils.version_key(upgrade_version):
+                continue
+
+            upgrade_plan.append((version, cluster.procedure_inventory.get(version, {}).get("thirdparties", {})))
+
+    elif context.get("initial_procedure") == "migrate_kubemarine" and 'upgrading_thirdparty' in context:
+        upgrade_thirdparties = cluster.procedure_inventory.get('upgrade', {}).get("thirdparties", {})
+        upgrade_thirdparties = dict(item for item in upgrade_thirdparties.items()
+                                    if item[0] == context['upgrading_thirdparty'])
+        upgrade_plan = [("", upgrade_thirdparties)]
+    else:
+        upgrade_plan = []
+
+    return upgrade_plan
+
+
+def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
+    upgrade_plan = _get_upgrade_plan(cluster)
+    if not upgrade_plan:
+        return inventory
+
+    context = cluster.context
+    if context.get("initial_procedure") == "upgrade":
+        previous_version = context['initial_kubernetes_version']
+        # Validation is currently turned off for backward compatibility.
+        # It is possible to redefine all thirdparties with templates depending on Kubernetes version and the compatibility map.
+        # This technically allows to not supply new thirdparties during upgrade.
+        # The validation is turned on for new functionality of thirdparty upgrade during Kubemarine migration.
+        #
+        # thirdparties_verify = get_default_thirdparties()
+        thirdparties_verify = []
+    else:  # migrate_kubemarine procedure
+        previous_version = ""
+        thirdparties_verify = [context['upgrading_thirdparty']]
+
+    _verify_upgrade_plan(inventory, previous_version, thirdparties_verify, upgrade_plan)
+
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def _verify_upgrade_plan(inventory: dict, previous_version: str,
+                         thirdparties_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+
+    thirdparties = deepcopy(inventory["services"]['thirdparties'])
+    sensitive_keys = ['source', 'sha1']
+
+    for version, upgrade_thirdparties in upgrade_plan:
+        upgrade_thirdparties = deepcopy(upgrade_thirdparties)
+
+        for destination in thirdparties_verify:
+            config = _convert_thirdparty(thirdparties, destination)
+            upgrade_config = _convert_thirdparty(upgrade_thirdparties, destination)
+
+            for key in sensitive_keys:
+                if config.get(key) and not upgrade_config.get(key):
+                    raise errors.KME("KME0011",
+                                     key=key, thirdparty=destination,
+                                     previous_version_spec=f" for version {previous_version}" if previous_version else "",
+                                     next_version_spec=f" for next version {version}" if version else "")
+
+            default_merger.merge(config, upgrade_config)
+
+        previous_version = version
+
+
+def upgrade_finalize_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    return generic_upgrade_inventory(cluster, inventory)
+
+
+def generic_upgrade_inventory(cluster: KubernetesCluster, inventory: dict) -> dict:
+    upgrade_plan = _get_upgrade_plan(cluster)
+    if not upgrade_plan:
+        return inventory
+
+    _, upgrade_thirdparties = upgrade_plan[0]
+    if upgrade_thirdparties:
+        thirdparties = inventory.setdefault("services", {}).setdefault("thirdparties", {})
+        upgrade_thirdparties = deepcopy(upgrade_thirdparties)
+
+        for destination in upgrade_thirdparties:
+            config = _convert_thirdparty(thirdparties, destination)
+            upgrade_config = _convert_thirdparty(upgrade_thirdparties, destination)
+            default_merger.merge(config, upgrade_config)
+
     return inventory
 
 
 def enrich_inventory_apply_defaults(inventory: dict, cluster: KubernetesCluster) -> dict:
     thirdparties: Dict[str, dict] = inventory['services'].get('thirdparties', {})
     # if thirdparties is empty, then nothing to do
     if not thirdparties:
         return inventory
 
-    for destination, config in thirdparties.items():
+    for destination in thirdparties:
 
-        if isinstance(config, str):
-            config = {
-                'source': config
-            }
+        config = _convert_thirdparty(thirdparties, destination)
 
         if config.get('mode') is None:
             config['mode'] = 700
 
         if config.get('owner') is None:
             config['owner'] = 'root'
 
@@ -164,16 +253,14 @@
 
         if is_default_thirdparty(destination) and 'source' not in config:
             source, sha1 = get_default_thirdparty_identity(cluster.inventory, destination, in_public=True)
             config['source'] = source
             if 'sha1' not in config:
                 config['sha1'] = sha1
 
-        thirdparties[destination] = config
-
     # remove "crictl" from thirdparties when docker is used, but ONLY IF it is NOT explicitly specified in cluster.yaml
     cri_name = inventory['services']['cri']['containerRuntime']
     crictl_key = '/usr/bin/crictl.tar.gz'
     if cri_name == "docker" and \
             crictl_key not in cluster.raw_inventory.get('services', {}).get('thirdparties', {}):
         del(thirdparties[crictl_key])
```

### Comparing `kubemarine-0.17.0/kubemarine/yum.py` & `kubemarine-0.18.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.17.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.18.0/kubemarine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.17.0
+Version: 0.18.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.17.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#documentation).
 
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
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.17.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.17.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.17.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.0/LICENSE)
```

### Comparing `kubemarine-0.17.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.18.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 kubemarine/core/defaults.py
 kubemarine/core/environment.py
 kubemarine/core/errors.py
 kubemarine/core/executor.py
 kubemarine/core/flow.py
 kubemarine/core/group.py
 kubemarine/core/log.py
+kubemarine/core/os.py
 kubemarine/core/patch.py
 kubemarine/core/resources.py
 kubemarine/core/schema.py
 kubemarine/core/static.py
 kubemarine/core/summary.py
 kubemarine/core/utils.py
 kubemarine/core/yaml_merger.py
@@ -59,14 +60,15 @@
 kubemarine/kubernetes/__init__.py
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
+kubemarine/patches/software_upgrade.yaml
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
@@ -106,14 +108,15 @@
 kubemarine/resources/configurations/compatibility/internal/packages.yaml
 kubemarine/resources/configurations/compatibility/internal/plugins.yaml
 kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
 kubemarine/resources/drop_ins/__init__.py
 kubemarine/resources/drop_ins/haproxy.conf
 kubemarine/resources/drop_ins/keepalived.conf
 kubemarine/resources/etalons/patches/__init__.py
+kubemarine/resources/etalons/patches/software_upgrade.yaml
 kubemarine/resources/psp/__init__.py
 kubemarine/resources/psp/anyuid.yaml
 kubemarine/resources/psp/default.yaml
 kubemarine/resources/psp/host-network.yaml
 kubemarine/resources/psp/privileged.yaml
 kubemarine/resources/reports/__init__.py
 kubemarine/resources/reports/check_report.css
@@ -121,14 +124,15 @@
 kubemarine/resources/schemas/backup.json
 kubemarine/resources/schemas/cert_renew.json
 kubemarine/resources/schemas/check_paas.json
 kubemarine/resources/schemas/cluster.json
 kubemarine/resources/schemas/manage_psp.json
 kubemarine/resources/schemas/manage_pss.json
 kubemarine/resources/schemas/migrate_cri.json
+kubemarine/resources/schemas/migrate_kubemarine.json
 kubemarine/resources/schemas/reboot.json
 kubemarine/resources/schemas/remove_node.json
 kubemarine/resources/schemas/restore.json
 kubemarine/resources/schemas/upgrade.json
 kubemarine/resources/schemas/definitions/gateway_node.json
 kubemarine/resources/schemas/definitions/globals.json
 kubemarine/resources/schemas/definitions/node.json
```

### Comparing `kubemarine-0.17.0/pyproject.toml` & `kubemarine-0.18.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "0.17.0"
+current_version = "0.18.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.17.0/setup.py` & `kubemarine-0.18.0/setup.py`

 * *Files identical despite different names*

