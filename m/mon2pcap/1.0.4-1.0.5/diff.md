# Comparing `tmp/mon2pcap-1.0.4.tar.gz` & `tmp/mon2pcap-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mon2pcap-1.0.4.tar", max compression
+gzip compressed data, was "mon2pcap-1.0.5.tar", max compression
```

## Comparing `mon2pcap-1.0.4.tar` & `mon2pcap-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.4/LICENSE
--rw-r--r--   0        0        0     2338 2023-06-04 11:37:08.244034 mon2pcap-1.0.4/README.md
--rw-r--r--   0        0        0      230 2023-06-05 07:10:39.716916 mon2pcap-1.0.4/mon2pcap/__init__.py
--rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.4/mon2pcap/common.py
--rw-r--r--   0        0        0     2850 2023-06-04 11:23:50.048354 mon2pcap-1.0.4/mon2pcap/console.py
--rw-r--r--   0        0        0     3213 2023-06-04 10:03:27.795673 mon2pcap-1.0.4/mon2pcap/constants.py
--rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.4/mon2pcap/errors.py
--rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.4/mon2pcap/helpers.py
--rw-r--r--   0        0        0     7537 2023-06-04 10:13:54.030726 mon2pcap-1.0.4/mon2pcap/mon2pcap.py
--rw-r--r--   0        0        0    56507 2023-06-04 10:03:28.174218 mon2pcap-1.0.4/mon2pcap/packets.py
--rw-r--r--   0        0        0     1017 2023-06-05 07:10:46.965199 mon2pcap-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 mon2pcap-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3378 2023-06-05 14:39:35.620745 mon2pcap-1.0.5/README.md
+-rw-r--r--   0        0        0      230 2023-06-05 07:10:39.716916 mon2pcap-1.0.5/mon2pcap/__init__.py
+-rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.5/mon2pcap/common.py
+-rw-r--r--   0        0        0     2850 2023-06-04 11:23:50.048354 mon2pcap-1.0.5/mon2pcap/console.py
+-rw-r--r--   0        0        0     3261 2023-06-05 14:05:37.872613 mon2pcap-1.0.5/mon2pcap/constants.py
+-rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.5/mon2pcap/errors.py
+-rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.5/mon2pcap/helpers.py
+-rw-r--r--   0        0        0     7537 2023-06-05 14:36:44.763690 mon2pcap-1.0.5/mon2pcap/mon2pcap.py
+-rw-r--r--   0        0        0    60553 2023-06-05 14:29:47.705500 mon2pcap-1.0.5/mon2pcap/packets.py
+-rw-r--r--   0        0        0     1017 2023-06-05 14:37:31.916503 mon2pcap-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 mon2pcap-1.0.5/PKG-INFO
```

### Comparing `mon2pcap-1.0.4/LICENSE` & `mon2pcap-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.4/mon2pcap/console.py` & `mon2pcap-1.0.5/mon2pcap/console.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.4/mon2pcap/constants.py` & `mon2pcap-1.0.5/mon2pcap/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         ("PPP", 0),
         ("DHCP", 0),
         ("L3_TUNNEL", 0),
         ("PFCP", 0),
         ("GTPP", 0),
         ("SLS", 0),
         ("SCTP", 0),
+        ("LMISF", 0),
         ("Ignored", 0),
         ("Filtered", 0),
     ]
 )
 
 RE_HEXDUMP = re.compile(r"^([0-9a-f]{2,4}\s?){1,8}$", re.IGNORECASE)
 RE_HEXDUMP_ASCII = re.compile(
@@ -127,9 +128,10 @@
         "221302": "PFCP",
         "52000": "GTPP",
         "52001": "GTPP",
         "206301": "SLS",
         "206302": "SLS",
         "87301": "SCTP",
         "87302": "SCTP",
+        "69126": "LMISF",
     }
     return table.get(eventid)
```

### Comparing `mon2pcap-1.0.4/mon2pcap/helpers.py` & `mon2pcap-1.0.5/mon2pcap/helpers.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.4/mon2pcap/mon2pcap.py` & `mon2pcap-1.0.5/mon2pcap/mon2pcap.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.4/mon2pcap/packets.py` & `mon2pcap-1.0.5/mon2pcap/packets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1741,34 +1741,131 @@
                 src="00:00:00:00:00:00", dst="00:00:00:00:00:00", type=0x0800
             ) / bytes.fromhex(self.hexdump)
 
         scapy_packet.time = self.arrive_time
         return scapy_packet
 
 
+class Lmisf(Packet):
+    """LMISF packet
+
+    :param raw_text: list: Lines in list of packet text
+    StarOS does not decode correctly LIMSF protocol!!
+
+    Sample:
+    Monday June 05 2023
+    <<<<OUTBOUND  08:54:53:397 Eventid:69126(3)
+    [Unknown(0)]GTPv2C Tx PDU, from :0 to :0 (154)
+    ---------------------------Packet Dump [154 Bytes]---------------------------
+    40 02 01 34 00 0c 00 04  39 31 39 33 32 36 37 33        @..4.... 91932673
+    37 37 33 33 00 04 00 9d  05 00 00 80 00 01 00 a0        7733.... ........
+    00 00 08 00 5c 64 7d db  1d 00 06 06 9e 00 0f 00        ....\d}. ........
+    05 38 30 39 32 37 39 35  33 31 32 31 33 39 30 36        .8092795 31213906
+    00 10 00 06 31 31 32 32  33 33 34 34 35 35 36 36        ....1122 33445566
+    37 37 38 38 00 06 00 0b  08 12 54 63 12 34 00 01        7788.... ..Tc.4..
+    00 26 05 00 12 00 50 08  05 00 00 00 00 00 00 00        .&....P. ........
+    00 00 00 00 00 00 00 00  00 00 0b 00 08 73 74 61        ........ .....sta
+    72 65 6e 74 2e 63 6f 6d  00 01 00 53 00 00 04 00        rent.com ...S....
+    a3 21 7b 31 01 00 01 00  5d 01                          .!{1.... ].
+    
+    0x0000   4002 0134 000c 0004 3931 3933 3236 3733        @..4....91932673
+    0x0010   3737 3333 0004 009d 0500 0080 0001 00a0        7733............
+    0x0020   0000 0800 5c64 7ddb 1d00 0606 9e00 0f00        ....\d}.........
+    0x0030   0538 3039 3237 3935 3331 3231 3339 3036        .809279531213906
+    0x0040   0010 0006 3131 3232 3333 3434 3535 3636        ....112233445566
+    0x0050   3737 3838 0006 000b 0812 5463 1234 0001        7788......Tc.4..
+    0x0060   0026 0500 1200 5008 0500 0000 0000 0000        .&....P.........
+    0x0070   0000 0000 0000 0000 0000 0b00 0873 7461        .............sta
+    0x0080   7265 6e74 2e63 6f6d 0001 0053 0000 0400        rent.com...S....
+    0x0090   a321 7b31 0100 0100 5d01                       .!{1....].
+
+    GTPv2C decoder :(
+
+    Eth / IP / UDP layers added.
+    IP src = IP dst = 0.0.0.0
+    UDP sport = 9201
+    UDP dport = 9200
+
+    TODO: parse IP and Transport layers when we'll have the decoder.
+    """
+
+    def __init__(self, raw_text: list):
+        super().__init__(raw_text)
+        self._validate_content()
+        #an_ip_address = self.raw_text[2].split()[4]
+        #self.ip_version = self._probe_ip_ver(an_ip_address)
+        self.ip_version = 4
+        self.direction = self._get_direction()
+        self.arrive_time = self._get_arrive_time()
+        (
+            self.ip_src,
+            self.ip_dst,
+            self.sport,
+            self.dport,
+            self.length,
+        ) = self._get_l3_l4_data()
+        self.hexdump = self._get_hexdump(self.length)
+        self._hexdump_sanity_check(self.hexdump, self.length)
+        self.scapy_packet = self._get_scapy_packet()
+
+    def _get_l3_l4_data(self):
+        """ """
+        line = self.raw_text[2].split()
+        ip_src = "0.0.0.0"
+        ip_dst = "0.0.0.0"
+        sport = 9201
+        dport = 9200
+        length = int(line[-1].split("(")[1][:-1])
+
+
+        return ip_src, ip_dst, sport, dport, length
+
+    def _get_scapy_packet(self):
+        """ """
+        if self.ip_version == 4:
+            scapy_packet = (
+                Ether(src="00:00:00:00:00:00", dst="00:00:00:00:00:00", type=0x0800)
+                / IP(src=self.ip_src, dst=self.ip_dst)
+                / UDP(sport=self.sport, dport=self.dport)
+                / bytes.fromhex(self.hexdump)
+            )
+
+        if self.ip_version == 6:
+            scapy_packet = (
+                Ether(src="00:00:00:00:00:00", dst="00:00:00:00:00:00", type=0x86DD)
+                / IPv6(src=self.ip_src, dst=self.ip_dst)
+                / UDP(sport=self.sport, dport=self.dport)
+                / bytes.fromhex(self.hexdump)
+            )
+
+        scapy_packet.time = self.arrive_time
+        return scapy_packet
+
+
 PARSERS = {
-    "GTPC": Gtpc,
-    "GTPCv2": GtpcV2,
-    "GTPU": Gtpu,
-    "RADIUS": Radius,
-    "USERL3": UserL3,
+    "GTPC"       : Gtpc,
+    "GTPCv2"     : GtpcV2,
+    "GTPU"       : Gtpu,
+    "RADIUS"     : Radius,
+    "USERL3"     : UserL3,
     "USERL3_IPV6": UserL3,
-    "CSS": Css,
-    "DIAMETER": Diameter,
-    "RANAP": Ranap,
-    "RUA": Rua,
-    "S1AP": S1Ap,
-    "SGS": SGs,
-    "BSSGP": Bssgp,
-    "TCAP": Tcap,
-    "SCCP": Sccp,
-    "IKEv2": IkeV2,
-    "L2TP": L2tp,
-    "PPP": Ppp,
-    "DNS": Dns,
-    "DHCP": Dhcp,
-    "L3_TUNNEL": L3Tunnel,
-    "PFCP": Pfcp,
-    "GTPP": Gtpp,
-    "SLS": Sls,
-    "SCTP": Sctp,
+    "CSS"        : Css,
+    "DIAMETER"   : Diameter,
+    "RANAP"      : Ranap,
+    "RUA"        : Rua,
+    "S1AP"       : S1Ap,
+    "SGS"        : SGs,
+    "BSSGP"      : Bssgp,
+    "TCAP"       : Tcap,
+    "SCCP"       : Sccp,
+    "IKEv2"      : IkeV2,
+    "L2TP"       : L2tp,
+    "PPP"        : Ppp,
+    "DNS"        : Dns,
+    "PFCP"       : Pfcp,
+    "DHCP"       : Dhcp,
+    "L3_TUNNEL"  : L3Tunnel,
+    "GTPP"       : Gtpp,
+    "SLS"        : Sls,
+    "SCTP"       : Sctp,
+    "LMISF"      : Lmisf, 
 }
```

### Comparing `mon2pcap-1.0.4/pyproject.toml` & `mon2pcap-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mon2pcap"
-version = "1.0.4"
+version = "1.0.5"
 description = "Convert StarOS \"monitor subscriber\" or \"monitor protocol\" ASCII dump to PCAP"
 authors = ["Artur Russu <arussu@cisco.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/arussu/mon2pcap"
 keywords = ["scapy", "mon2pcap"]
 classifiers = [
```

