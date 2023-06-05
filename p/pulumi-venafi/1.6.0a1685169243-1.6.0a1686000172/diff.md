# Comparing `tmp/pulumi_venafi-1.6.0a1685169243.tar.gz` & `tmp/pulumi_venafi-1.6.0a1686000172.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.6.0a1685169243.tar", last modified: Sat May 27 06:41:03 2023, max compression
+gzip compressed data, was "pulumi_venafi-1.6.0a1686000172.tar", last modified: Mon Jun  5 21:30:11 2023, max compression
```

## Comparing `pulumi_venafi-1.6.0a1685169243.tar` & `pulumi_venafi-1.6.0a1686000172.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:41:03.787789 pulumi_venafi-1.6.0a1685169243/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-27 06:41:03.787789 pulumi_venafi-1.6.0a1685169243/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:41:03.783789 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:41:03.783789 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:41:03.783789 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:41:03.787789 pulumi_venafi-1.6.0a1685169243/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-27 06:41:03.000000 pulumi_venafi-1.6.0a1685169243/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48936 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:30:11.523269 pulumi_venafi-1.6.0a1686000172/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-05 21:30:11.000000 pulumi_venafi-1.6.0a1686000172/setup.py
```

### Comparing `pulumi_venafi-1.6.0a1685169243/PKG-INFO` & `pulumi_venafi-1.6.0a1686000172/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.6.0a1685169243
+Version: 1.6.0a1686000172
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-venafi/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-venafi/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fvenafi.svg)](https://www.npmjs.com/package/@pulumi/venafi)
 [![Python version](https://badge.fury.io/py/pulumi-venafi.svg)](https://pypi.org/project/pulumi-venafi)
 [![NuGet version](https://badge.fury.io/nu/pulumi.venafi.svg)](https://badge.fury.io/nu/pulumi.venafi)
```

### Comparing `pulumi_venafi-1.6.0a1685169243/README.md` & `pulumi_venafi-1.6.0a1686000172/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/__init__.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/certificate.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
                to request a new certificate.  Defaults to `168`.
         :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
                issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
                "Entrust", and "Microsoft".
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
         :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
+               Useful when working with resources like
+               azurerm_key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
         :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
                Applies when `algorithm=RSA`.  Defaults to `2048`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
                subjects of the certificate.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
                alternative subjects of the certificate.
@@ -231,14 +234,19 @@
     @nickname.setter
     def nickname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nickname", value)
 
     @property
     @pulumi.getter
     def pkcs12(self) -> Optional[pulumi.Input[str]]:
+        """
+        A base64-encoded PKCS#12 keystore secured by the `key_password`.
+        Useful when working with resources like
+        azurerm_key_vault_certificate.
+        """
         return pulumi.get(self, "pkcs12")
 
     @pkcs12.setter
     def pkcs12(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pkcs12", value)
 
     @property
@@ -371,14 +379,17 @@
         :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
                to request a new certificate.  Defaults to `168`.
         :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
                issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
                "Entrust", and "Microsoft".
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
         :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
+               Useful when working with resources like
+               azurerm_key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
         :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
                Applies when `algorithm=RSA`.  Defaults to `2048`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
                subjects of the certificate.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
                alternative subjects of the certificate.
@@ -587,14 +598,19 @@
     @nickname.setter
     def nickname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nickname", value)
 
     @property
     @pulumi.getter
     def pkcs12(self) -> Optional[pulumi.Input[str]]:
+        """
+        A base64-encoded PKCS#12 keystore secured by the `key_password`.
+        Useful when working with resources like
+        azurerm_key_vault_certificate.
+        """
         return pulumi.get(self, "pkcs12")
 
     @pkcs12.setter
     def pkcs12(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pkcs12", value)
 
     @property
@@ -727,14 +743,17 @@
         :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
                to request a new certificate.  Defaults to `168`.
         :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
                issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
                "Entrust", and "Microsoft".
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
         :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
+               Useful when working with resources like
+               azurerm_key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
         :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
                Applies when `algorithm=RSA`.  Defaults to `2048`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
                subjects of the certificate.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
                alternative subjects of the certificate.
@@ -872,14 +891,17 @@
         :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
                to request a new certificate.  Defaults to `168`.
         :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
                issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
                "Entrust", and "Microsoft".
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
         :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
+               Useful when working with resources like
+               azurerm_key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
         :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
                Applies when `algorithm=RSA`.  Defaults to `2048`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
                subjects of the certificate.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
                alternative subjects of the certificate.
@@ -1020,14 +1042,19 @@
         Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
         """
         return pulumi.get(self, "nickname")
 
     @property
     @pulumi.getter
     def pkcs12(self) -> pulumi.Output[str]:
+        """
+        A base64-encoded PKCS#12 keystore secured by the `key_password`.
+        Useful when working with resources like
+        azurerm_key_vault_certificate.
+        """
         return pulumi.get(self, "pkcs12")
 
     @property
     @pulumi.getter(name="privateKeyPem")
     def private_key_pem(self) -> pulumi.Output[str]:
         """
         The private key in PEM format.
```

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/policy.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         internal_policy = venafi.Policy("internalPolicy",
             zone="My Business App\\\\Enterprise Trusted Certs",
             policy_specification=(lambda path: open(path).read())("/path-to/internal-policy.json"))
         ```
 
         ## Import
 
-        The `venafi_policy` resource supports the Terraform [import](https://www.terraform.io/docs/cli/import/index.html) method.
+        The `venafi_policy` resource supports the Terraform import method.
 
         When used, the `zone` and `policy_specification` resource arguments are not required since the zone is a required parameter of the import method and the policy specification is populated from the existing infrastructure. Policy that is successfully imported is also output to a file named after the zone that was specified. hcl resource "venafi_policy" "existing_policy" {}
 
         ```sh
          $ pulumi import venafi:index/policy:Policy existing_policy" "My Business App\\\\Enterprise Trusted Certs"
         ```
 
@@ -165,15 +165,15 @@
         internal_policy = venafi.Policy("internalPolicy",
             zone="My Business App\\\\Enterprise Trusted Certs",
             policy_specification=(lambda path: open(path).read())("/path-to/internal-policy.json"))
         ```
 
         ## Import
 
-        The `venafi_policy` resource supports the Terraform [import](https://www.terraform.io/docs/cli/import/index.html) method.
+        The `venafi_policy` resource supports the Terraform import method.
 
         When used, the `zone` and `policy_specification` resource arguments are not required since the zone is a required parameter of the import method and the policy specification is populated from the existing infrastructure. Policy that is successfully imported is also output to a file named after the zone that was specified. hcl resource "venafi_policy" "existing_policy" {}
 
         ```sh
          $ pulumi import venafi:index/policy:Policy existing_policy" "My Business App\\\\Enterprise Trusted Certs"
         ```
```

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/provider.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-venafi
-Version: 1.6.0a1685169243
+Version: 1.6.0a1686000172
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-venafi/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-venafi/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fvenafi.svg)](https://www.npmjs.com/package/@pulumi/venafi)
 [![Python version](https://badge.fury.io/py/pulumi-venafi.svg)](https://pypi.org/project/pulumi-venafi)
 [![NuGet version](https://badge.fury.io/nu/pulumi.venafi.svg)](https://badge.fury.io/nu/pulumi.venafi)
```

### Comparing `pulumi_venafi-1.6.0a1685169243/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.6.0a1686000172/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1685169243/setup.py` & `pulumi_venafi-1.6.0a1686000172/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.6.0a1685169243"
-PLUGIN_VERSION = "1.6.0-alpha.1685169243+f1c3dab5"
+VERSION = "1.6.0a1686000172"
+PLUGIN_VERSION = "1.6.0-alpha.1686000172+1b89455a"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'venafi', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "venafi Pulumi Package - Development Version"
 
 
 setup(name='pulumi_venafi',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing venafi cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

