# Comparing `tmp/pktperf-0.4.1.tar.gz` & `tmp/pktperf-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pktperf-0.4.1.tar", last modified: Thu May 25 12:11:55 2023, max compression
+gzip compressed data, was "pktperf-0.5.3.tar", last modified: Mon Jun  5 07:40:13 2023, max compression
```

## Comparing `pktperf-0.4.1.tar` & `pktperf-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-25 12:11:36.000000 pktperf-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-25 12:11:55.198103 pktperf-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-25 12:11:36.000000 pktperf-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/pktperf/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/pktperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 12:11:36.000000 pktperf-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:11:55.198103 pktperf-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 12:11:36.000000 pktperf-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.284232 pktperf-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.280232 pktperf-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.280232 pktperf-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 07:40:02.000000 pktperf-0.5.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-05 07:40:02.000000 pktperf-0.5.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 07:40:02.000000 pktperf-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-05 07:40:02.000000 pktperf-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-05 07:40:02.000000 pktperf-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-05 07:40:13.284232 pktperf-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-05 07:40:02.000000 pktperf-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-05 07:40:02.000000 pktperf-0.5.3/example.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.280232 pktperf-0.5.3/pktperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/ethtoolsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.280232 pktperf-0.5.3/pktperf/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/module/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/module/common.mk
+-rw-r--r--   0 runner    (1001) docker     (123)   141227 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/module/pktgen_5.4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23005 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/pktgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/pktperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-05 07:40:02.000000 pktperf-0.5.3/pktperf/pktsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:40:13.280232 pktperf-0.5.3/pktperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 07:40:13.000000 pktperf-0.5.3/pktperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 07:40:02.000000 pktperf-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:40:13.284232 pktperf-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-05 07:40:02.000000 pktperf-0.5.3/setup.py
```

### Comparing `pktperf-0.4.1/LICENSE` & `pktperf-0.5.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2021 junka<wan.junjie@foxmail.com>
+Copyright 2021 - 2023 junka<wan.junjie@foxmail.com>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pktperf-0.4.1/pktperf/pktgen.py` & `pktperf-0.5.3/pktperf/pktgen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 # -*- coding: UTF-8 -*-
 """
 classes provide functions for pktgen operation
 """
 import sys
 import re
 import os
+import math
 import ipaddress
+import subprocess
+import configparser
 from .pktsar import PktSar
 
 
 def open_write_error(filename, flag, mode="r+"):
     """open and write a flag to file"""
     try:
         with open(filename, mode, encoding='utf-8') as fp_dev:
             fp_dev.write("%s\n" % flag)
     except IOError:
         print("Error: Cannot open %s" % (filename))
+        raise Exception("Error writing flag %s", flag)
         sys.exit(1)
 
 
+def modinfo_check() -> str:
+    """ check module version """
+    p = subprocess.run(['modinfo', 'pktgen'], stdout=subprocess.PIPE, check=True)
+    if p.returncode != 0:
+        return ""
+    ret = p.stdout.decode('utf-8')
+    ver = re.search(r'version:[\t\ ]+([\d\.]+)', ret)
+    if ver is not None:
+        return ver.group(1)
+    return ""
+
+
 class Pktgen:
     """Pktgen class
 
     pktgen api class, responsible for operation on
     /proc/net/pktgen/pgctrl
     /proc/net/pktgen/kpktgend_X
     /proc/net/pktgen/ethX
@@ -44,37 +60,44 @@
             threads: number of threads to start
             first_thread: index of first thread to start
             clone: number of skb clones sent before alloc new skb
             num: number of packets to send per thread, 0 means indefinitely
             burst: hw level bursting of skbs
             verbose: verbose
             debug: debug
-            ipv6: send IPv6 packets
             flows: limit number of flows
             flow_len: packets number a flow will send
             tx_delay: tx delay value in ns
             append: script will not reset generator state, append its config
             queue: queue mapping with irq affinity
+
+            tos, traffic_class, vni should be hex for pktgen
         """
         if self.os_check() is False:
             print("pktperf Can Only run in Linux system!")
             sys.exit()
         if os.getuid() != 0:
             print("pktperf should be run as root!")
             sys.exit()
+        ver = modinfo_check()
+        if ver == "":
+            print("pktgen is not enabled in kernel")
+            sys.exit()
         mod = "/proc/net/pktgen"
         is_exists = os.path.exists(mod)
         if is_exists is False:
             print("No pktgen module\nPlease do \'modprobe pktgen\'")
             sys.exit(0)
         self.pgdev = args.interface
         self.pkt_size = int(args.size)
         self.dst_mac = args.mac
-        self.__init_ip_dst(args.ipv6, args.dest)
-        self.__init_port_range(args.portrange)
+        self.dst_ip_min, self.dst_ip_max = self.__init_ip_input(args.dst)
+        self.src_ip_min, self.src_ip_max = self.__init_ip_input(args.src)
+        self.dst_port_min, self.dst_port_max = self.__init_port_range(args.portrange)
+        self.src_port_min, self.src_port_max = 9, 1009
         self.frags = None
         self.csum = args.txcsum
         self.debug = args.debug
         self.verbose = args.verbose
         self.append = args.append
         if args.clone is not None:
             self.clone = int(args.clone)
@@ -86,70 +109,121 @@
         self.stats = []
         if args.firstthread is not None:
             self.first_thread = int(args.firstthread)
         if args.delay is not None:
             self.tx_delay = int(args.delay)
         if args.flows is not None:
             self.flows = int(args.flows)
-        if args.flowpkt is not None:
-            self.flow_len = int(args.flowpkt)
+        if args.flowpkts is not None:
+            self.flow_len = int(args.flowpkts)
         self.__init_irq(args.queuemap)
         if args.tos is not None:
             self.tos = int(args.tos)
         self.bps_rate = args.bps
         self.pps_rate = args.pps
         if args.frags is not None:
             self.frags = int(args.frags)
         self.vlan = args.vlan
         self.svlan = args.svlan
+        self.tun_vni = args.vni
+        self.tun_udpport = args.tundport
+        self.tun_dst_min, self.tun_dst_max = self.__init_ip_input(args.tundst)
+        self.tun_src_min, self.tun_src_max = self.__init_ip_input(args.tunsrc)
+        self.inner_dmac = args.innerdmac
+        self.inner_smac = args.innersmac
+        self.microburst = args.microburst
+        self.imixweight = args.imix
+        self.__read_config_file(args.file)
+
+    def __read_config_file(self, file):
+        cfg = configparser.ConfigParser()
+        if file is not None:
+            # cfg.read(file)
+            with open(file, 'r') as f:
+                config_string = '[dummy]\n' + f.read()
+                cfg.read_string(config_string)
+        else:
+            return
+        if cfg.has_option('dummy', 'pkt_size'):
+            self.pkt_size = cfg.getint('dummy', 'pkt_size')
+        if cfg.has_option('dummy', 'pkt_num'):
+            self.num = cfg.get_int('dummy', 'pkt_num')
+        if cfg.has_option('dummy', 'dst_ip'):
+            self.dst_ip_min, self.dst_ip_max = self.__init_ip_input(cfg.get('dummy', 'dst_ip'))
+        if cfg.has_option('dummy', 'src_ip'):
+            self.src_ip_min, self.src_ip_max = self.__init_ip_input(cfg.get('dummy', 'src_ip'))
+        if cfg.has_option('dummy', 'dstmac'):
+            self.dst_mac = cfg.get('dummy', 'dstmac')
+        if cfg.has_option('dummy', 'vlan'):
+            self.vlan = cfg.get('dummy', 'vlan')
+        if cfg.has_option('dummy', 'svlan'):
+            self.svlan = cfg.get('dummy', 'svlan')
+        if cfg.has_option('dummy', 'udp_src_port'):
+            self.src_port_min, self.src_port_max = self.__init_port_range(cfg.get('dummy', 'udp_src_port'))
+        if cfg.has_option('dummy', 'udp_dst_port'):
+            self.dst_port_min, self.dst_port_max = self.__init_port_range(cfg.get('dummy', 'udp_dst_port'))
+        if cfg.has_option('dummy', 'tos'):
+            self.tos = cfg['tos']
+        if cfg.has_option('dummy', 'tun_vni'):
+            self.tun_vni = cfg.get('dummy', 'tun_vni')
+        if cfg.has_option('dummy', 'tun_udp_port'):
+            self.tun_udpport = cfg.get('dummy', 'tun_udp_port')
+        if cfg.has_option('dummy', 'tun_src_ip'):
+            self.tun_src_min, self.tun_src_max = self.__init_ip_input(cfg.get('dummy', 'tun_src_ip'))
+        if cfg.has_option('dummy', 'tun_dst_ip'):
+            self.tun_dst_min, self.tun_dst_max = self.__init_ip_input(cfg.get('dummy', 'tun_dst_ip'))
+        if cfg.has_option('dummy', 'inner_dstmac'):
+            self.inner_dmac = cfg.get('dummy', 'inner_dstmac')
+        if cfg.has_option('dummy', 'inner_srcmac'):
+            self.inner_smac = cfg.get('dummy', 'inner_srcmac')
+        if cfg.has_option('dummy', 'micro_burst'):
+            self.microburst = cfg.get('dummy', 'micro_burst')
+        if cfg.has_option('dummy', 'imix_weight'):
+            self.imixweight = cfg.get('dummy', 'imix_weight')
 
-    def __init_ip_dst(self, is_ipv6, dest_ip):
+    def __init_ip_input(self, ipstr):
         """ Init pktgen module ip dst """
-        self.ipv6 = is_ipv6
-        if dest_ip is None:
-            if self.ipv6 is True:
-                dest_ip = "FD00::1"
-            else:
-                dest_ip = "198.18.0.42"
+        if ipstr is None:
+            return "", ""
         net = None
         try:
-            net = ipaddress.ip_network(dest_ip, strict=False)
+            net = ipaddress.ip_network(ipstr, strict=False)
         except (ValueError, TypeError):
-            ip_list = dest_ip.split('-')
+            ip_list = ipstr.split('-')
             try:
-                self.dst_ip_min = ipaddress.ip_address(ip_list[0])
+                ip_min = ipaddress.ip_address(ip_list[0])
             except (ValueError, TypeError):
                 print("invalid ip address format")
                 sys.exit()
             if len(ip_list) == 2:
                 try:
-                    self.dst_ip_max = ipaddress.ip_address(ip_list[1])
+                    ip_max = ipaddress.ip_address(ip_list[1])
                 except (ValueError, TypeError):
                     print("invalid ip address format")
                     sys.exit()
             elif len(ip_list) == 1:
-                self.dst_ip_max = self.dst_ip_min
+                ip_max = ip_min
         if net is not None:
             ip_list = list(net)
-            if ip_list[0].version == 6:
-                self.ipv6 = True
-            self.dst_ip_min = ip_list[0]
-            self.dst_ip_max = ip_list[-1]
+            ip_min = ip_list[0]
+            ip_max = ip_list[-1]
+        return ip_min, ip_max
 
-    def __init_port_range(self, portrange) -> None:
+    def __init_port_range(self, portrange):
         """init port range for pktgen"""
-        self.dst_port_max = None
-        self.dst_port_min = None
+        port_max = 65535
+        port_min = 65535
         if portrange is not None:
             ports = portrange.split('-')
             if len(ports) == 2:
-                self.dst_port_max = int(ports[1])
+                port_max = int(ports[1])
             elif len(ports) == 1:
-                self.dst_port_max = int(ports[0])
-            self.dst_port_min = int(ports[0])
+                port_max = int(ports[0])
+            port_min = int(ports[0])
+        return port_min, port_max
 
     def __init_irq(self, queuemap) -> None:
         """init irq affinity if queue mapping enabled"""
         self.queue = queuemap
         if queuemap is True:
             numa = self.__get_dev_numa()
             self.irq_list = self.__get_irqs()
@@ -205,17 +279,17 @@
         if self.debug is True:
             print("irq %d is set affinity to %d" % (irq, thread))
 
     def __config_tos(self, dev) -> None:
         """config tos """
         if self.tos is not None and self.tos != 0:
             if self.ipv6 is True:
-                self.pg_set(dev, "traffic_class %x" % self.tos)
+                self.pg_set(dev, "traffic_class %0x" % self.tos)
             else:
-                self.pg_set(dev, "tos %s" % self.tos)
+                self.pg_set(dev, "tos %0x" % self.tos)
 
     def __config_vlan(self, dev) -> None:
         """config vlan related parameter """
         if self.vlan is not None and 0 <= int(self.vlan) < 4096:
             self.pg_set(dev, "vlan_id %d" % int(self.vlan))
         if self.svlan is not None and 0 <= int(self.svlan) < 4096:
             self.pg_set(dev, "svlan_id %d" % int(self.svlan))
@@ -228,19 +302,68 @@
             self.pg_set(dev, "udp_dst_min %d" % (self.dst_port_min))
             self.pg_set(dev, "udp_dst_max %d" % (self.dst_port_max))
 
         if self.csum is True:
             self.pg_set(dev, "flag UDPCSUM")
 
         # Setup random UDP port src range
-        udp_src_min = 9
-        udp_src_max = 1009
         self.pg_set(dev, "flag UDPSRC_RND")
-        self.pg_set(dev, "udp_src_min %d" % (udp_src_min))
-        self.pg_set(dev, "udp_src_max %d" % (udp_src_max))
+        self.pg_set(dev, "udp_src_min %d" % (self.src_port_min))
+        self.pg_set(dev, "udp_src_max %d" % (self.src_port_max))
+
+    def __config_ip_dst(self, dev) -> None:
+        # Destination
+        if self.dst_ip_min.version == 6:
+            self.pg_set(dev, "dst_min6 %s" % (self.dst_ip_min))
+            self.pg_set(dev, "dst_max6 %s" % (self.dst_ip_max))
+        else:
+            self.pg_set(dev, "dst_min %s" % (self.dst_ip_min))
+            self.pg_set(dev, "dst_max %s" % (self.dst_ip_max))
+
+    def __config_ip_src(self, dev) -> None:
+        if self.src_ip_min == "":
+            return None
+        if self.src_ip_min.version == 6:
+            self.pg_set(dev, "src_min6 %s" % (self.src_ip_min))
+            self.pg_set(dev, "src_max6 %s" % (self.src_ip_max))
+        else:
+            self.pg_set(dev, "src_min %s" % (self.src_ip_min))
+            self.pg_set(dev, "src_max %s" % (self.src_ip_max))
+
+    def __config_imix(self, dev) -> None:
+        if self.imixweight is not None:
+            self.pg_set(dev, "imix_weights %s" % self.imixweight.replace(",", " ").replace(":", ","))
+
+    def __config_microburst(self, dev) -> None:
+        if self.microburst is not None:
+            self.pg_set(dev, "micro_burst %s" % self.microburst)
+
+    def __config_tun_meta(self, dev) -> None:
+        if self.tun_vni is not None:
+            self.pg_set(dev, "tun_meta %06x" % int(self.tun_vni))
+            self.pg_set(dev, "tun_udp_dst %d" % int(self.tun_udpport))
+            if self.tun_src_min != "":
+                self.pg_set(dev, "tun_src_min %s" % self.tun_src_min)
+            if self.tun_src_max != "":
+                self.pg_set(dev, "tun_src_max %s" % self.tun_src_max)
+            if self.tun_dst_min != "":
+                self.pg_set(dev, "tun_dst_min %s" % self.tun_dst_min)
+            if self.tun_dst_max != "":
+                self.pg_set(dev, "tun_dst_max %s" % self.tun_dst_max)
+            if self.inner_smac is not None:
+                self.pg_set(dev, "inner_src_mac %s" % self.inner_smac)
+            if self.inner_dmac is not None:
+                self.pg_set(dev, "inner_dst_mac %s" % self.inner_dmac)
+
+    def __config_ratelimit(self, dev) -> None:
+        # rate limit
+        if self.bps_rate is not None:
+            self.pg_set(dev, "rate %s" % (self.bps_rate))
+        if self.pps_rate is not None:
+            self.pg_set(dev, "ratep %s" % (self.pps_rate))
 
     def config_queue(self) -> None:
         """configure queues for pktgen"""
         # General cleanup everything since last run
         self.reset()
 
         # Threads are specified with parameter -t value in $THREADS
@@ -268,47 +391,41 @@
                 self.pg_set(dev, "queue_map_max %d" % qid)
 
             # Notice config queue to map to cpu (mirrors smp_processor_id())
             # It is beneficial to map IRQ /proc/irq/*/smp_affinity 1:1 to CPU
             self.pg_set(dev, "flag QUEUE_MAP_CPU")
 
             # Base config of dev
-            self.pg_set(dev, "count %d" % self.num)
+            self.pg_set(dev, "count %d" % math.ceil(self.num / self.threads))
             self.pg_set(dev, "clone_skb %d" % self.clone)
             self.pg_set(dev, "pkt_size %d" % self.pkt_size)
             if self.frags is not None and self.frags != 1:
                 self.pg_set(dev, "frags %d" % self.frags)
             self.pg_set(dev, "delay %d" % self.tx_delay)
 
             self.__config_tos(dev)
 
             # Flag example disabling timestamping
             self.pg_set(dev, "flag NO_TIMESTAMP")
 
-            # Destination
+            self.__config_tun_meta(dev)
             self.pg_set(dev, "dst_mac %s" % (self.dst_mac))
-            if self.ipv6 is True:
-                self.pg_set(dev, "dst_min6 %s" % (self.dst_ip_min))
-                self.pg_set(dev, "dst_max6 %s" % (self.dst_ip_max))
-            else:
-                self.pg_set(dev, "dst_min %s" % (self.dst_ip_min))
-                self.pg_set(dev, "dst_max %s" % (self.dst_ip_max))
-
+            self.__config_ip_dst(dev)
+            self.__config_ip_src(dev)
             self.__config_udp_portrange(dev)
             self.__config_vlan(dev)
 
             # hw burst
             if self.burst is not None and self.burst > 0:
                 self.pg_set(dev, "burst %d" % self.burst)
 
-            # rate limit
-            if self.bps_rate is not None:
-                self.pg_set(dev, "rate %s" % (self.bps_rate))
-            if self.pps_rate is not None:
-                self.pg_set(dev, "ratep %s" % (self.pps_rate))
+            self.__config_ratelimit(dev)
+
+            self.__config_imix(dev)
+            self.__config_microburst(dev)
 
     def reset(self) -> None:
         """ reset pktgen"""
         if self.append is False:
             self.pg_ctrl("reset")
 
     def start(self) -> None:
@@ -366,15 +483,15 @@
             pps, bps = pkt_sar.get_stats()
             print_cb(
                 "Core%3d send %18d pkts: %18f pps %18f bps %6d errors" %
                 (core_id, int(sofar.group(1)), pps, bps, int(sofar.group(2))))
             return int(sofar.group(1)), pps, bps, int(sofar.group(2))
         return 0, 0, 0, 0
 
-    def result(self, last, print_cb) -> None:
+    def result(self, last, print_cb) -> int:
         """ Print results """
         if last is True:
             print("%d cores enabled" % self.threads)
         need_init = False
         total_pkts = 0
         total_pps = 0
         total_bps = 0
@@ -391,14 +508,17 @@
                         i, fp_dev, print_cb)
                 total_pkts += sg_pkts
                 total_pps += sg_pps
                 total_bps += sg_bps
                 total_err += sg_err
         print_cb("Total   send %18d pkts: %18d pps %18d bps %6d errors" %
                  (total_pkts, total_pps, total_bps, total_err))
+        if last is False and self.num > 0 and total_pkts >= self.num:
+            return 1
+        return 0
 
     def __get_dev_numa(self) -> int:
         """ __get_dev_numa returns the numa node of the device"""
         numa_path = "/sys/class/net/%s/device/numa_node" % self.pgdev
         try:
             with open(numa_path, "r") as fp_numa:
                 node = fp_numa.read().rstrip('\n')
```

### Comparing `pktperf-0.4.1/pktperf/pktsar.py` & `pktperf-0.5.3/pktperf/pktsar.py`

 * *Files identical despite different names*

