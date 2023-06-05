# Comparing `tmp/cloudview-0.3.8.tar.gz` & `tmp/cloudview-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudview-0.3.8.tar", last modified: Wed Feb  9 22:34:24 2022, max compression
+gzip compressed data, was "cloudview-0.3.9.tar", last modified: Wed May 25 15:00:53 2022, max compression
```

## Comparing `cloudview-0.3.8.tar` & `cloudview-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-02-09 22:34:24.919284 cloudview-0.3.8/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     9881 2022-02-09 22:34:24.919284 cloudview-0.3.8/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7535 2021-06-15 18:17:20.000000 cloudview-0.3.8/README.md
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-02-09 22:34:24.919284 cloudview-0.3.8/_cloudview/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      104 2022-02-09 22:34:02.000000 cloudview-0.3.8/_cloudview/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2261 2021-10-17 13:57:10.000000 cloudview-0.3.8/_cloudview/amazon.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4969 2021-10-17 13:57:10.000000 cloudview-0.3.8/_cloudview/az.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      986 2022-02-09 21:52:18.000000 cloudview-0.3.8/_cloudview/exceptions.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5272 2022-02-09 22:25:03.000000 cloudview-0.3.8/_cloudview/gcp.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2911 2021-10-17 13:57:10.000000 cloudview-0.3.8/_cloudview/openstack.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     3354 2022-02-09 21:52:18.000000 cloudview-0.3.8/_cloudview/output.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      844 2021-10-17 13:57:10.000000 cloudview-0.3.8/_cloudview/singleton.py
--rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)    16032 2022-02-09 21:52:18.000000 cloudview-0.3.8/cloudview
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-02-09 22:34:24.919284 cloudview-0.3.8/cloudview.egg-info/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     9881 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      397 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/not-zip-safe
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1321 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/requires.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       11 2022-02-09 22:34:24.000000 cloudview-0.3.8/cloudview.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2022-02-09 22:34:24.919284 cloudview-0.3.8/setup.cfg
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1595 2022-02-09 21:52:18.000000 cloudview-0.3.8/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-05-25 15:00:53.340900 cloudview-0.3.9/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1071 2019-04-17 16:00:33.000000 cloudview-0.3.9/LICENSE
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8640 2022-05-25 15:00:53.340900 cloudview-0.3.9/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7608 2022-02-18 16:59:22.000000 cloudview-0.3.9/README.md
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-05-25 15:00:53.340900 cloudview-0.3.9/cloudview/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      104 2022-05-25 15:00:16.000000 cloudview-0.3.9/cloudview/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2286 2022-04-16 17:39:16.000000 cloudview-0.3.9/cloudview/aws.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4967 2022-04-15 14:42:52.000000 cloudview-0.3.9/cloudview/az.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    12117 2022-04-16 17:39:16.000000 cloudview-0.3.9/cloudview/cloudview.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      986 2022-02-17 19:55:18.000000 cloudview-0.3.9/cloudview/exceptions.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     3938 2022-02-17 20:55:40.000000 cloudview-0.3.9/cloudview/filters.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5302 2022-04-15 14:40:44.000000 cloudview-0.3.9/cloudview/gcp.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1419 2022-02-17 19:55:18.000000 cloudview-0.3.9/cloudview/html.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2977 2022-05-03 13:59:01.000000 cloudview-0.3.9/cloudview/openstack.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     3012 2022-02-17 19:55:18.000000 cloudview-0.3.9/cloudview/output.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      844 2022-02-17 19:55:18.000000 cloudview-0.3.9/cloudview/singleton.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1080 2022-02-18 14:14:53.000000 cloudview-0.3.9/cloudview/utils.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-05-25 15:00:53.340900 cloudview-0.3.9/cloudview.egg-info/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8640 2022-05-25 15:00:53.000000 cloudview-0.3.9/cloudview.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      483 2022-05-25 15:00:53.000000 cloudview-0.3.9/cloudview.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2022-05-25 15:00:53.000000 cloudview-0.3.9/cloudview.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2022-05-25 14:53:19.000000 cloudview-0.3.9/cloudview.egg-info/not-zip-safe
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1330 2022-05-25 15:00:53.000000 cloudview-0.3.9/cloudview.egg-info/requires.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       10 2022-05-25 15:00:53.000000 cloudview-0.3.9/cloudview.egg-info/top_level.txt
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2022-05-25 15:00:53.340900 cloudview-0.3.9/scripts/
+-rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)      289 2022-02-17 19:55:18.000000 cloudview-0.3.9/scripts/cloudview
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2022-05-25 15:00:53.340900 cloudview-0.3.9/setup.cfg
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1651 2022-02-17 19:55:18.000000 cloudview-0.3.9/setup.py
```

### Comparing `cloudview-0.3.8/PKG-INFO` & `cloudview-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,203 @@
 Metadata-Version: 2.1
 Name: cloudview
-Version: 0.3.8
+Version: 0.3.9
 Summary: View instance information on all supported cloud providers
 Home-page: https://github.com/ricardobranco777/cloudview
 Author: Ricardo Branco
 Author-email: rbranco@suse.de
 License: MIT License
-Description: # cloudview
-        View instance information on all supported cloud providers: Amazon Web Services, Azure, Google Compute Platform & OpenStack.
-        
-        [![Build Status](https://travis-ci.com/ricardobranco777/cloudview.svg?branch=master)](https://travis-ci.org/ricardobranco777/cloudview)
-        
-        ## Usage
-        
-        ```
-        Usage: cloudview [OPTIONS]
-        Options:
-            -h, --help                          show this help message and exit
-            -l, --log debug|info|warning|error|critical
-            -o, --output text|html|json|JSON    output type
-            -p, --port PORT                     run a web server on port PORT
-            -r, --reverse                       reverse sort
-            -s, --sort name|time|status         sort type
-            -S, --status stopped|running|all    filter by instance status
-            -T, --time TIME_FORMAT              time format as used by strftime(3)
-            -v, --verbose                       be verbose
-            -V, --version                       show version and exit
-        Filter options:
-            --filter-aws NAME VALUE             may be specified multiple times
-            --filter-azure FILTER               Filter for Azure
-            --filter-gcp FILTER                 Filter for GCP
-            --filter-openstack NAME VALUE       may be specified multiple times
-        ```
-        
-        **NOTES**:
-          - Use `--output JSON` to dump _all_ available information received from each provider.
-        
-        This script is best run with Docker to have all dependencies in just one package, but it may be run stand-alone on systems with Python 3.6+
-        
-        ## Environment variables
-        
-            - `AWS_ACCESS_KEY_ID`
-            - `AWS_DEFAULT_REGION`
-            - `AWS_SECRET_ACCESS_KEY`
-            - `AZURE_TENANT_ID`
-            - `AZURE_SUBSCRIPTION_ID`
-            - `AZURE_CLIENT_SECRET`
-            - `AZURE_CLIENT_ID`
-            - `GOOGLE_APPLICATION_CREDENTIALS`
-            - `OS_USERNAME`
-            - `OS_PASSWORD`
-            - `OS_PROJECT_ID`
-            - `OS_AUTH_URL`
-            - `OS_USER_DOMAIN_NAME`
-            - `OS_CACERT`
-        
-        **NOTES**:
-          - The `AWS_*` environment variables are optional.  If not set, the AWS SDK will grab the information from `~/.aws/credentials` and `~/.aws/config`.
-          - The `GOOGLE_APPLICATION_CREDENTIALS` environment variable must contain the path to the JSON file downloaded from the GCP web console after creating a personal key for the service account of your project.
-          - The `AZURE_*` environment variables are mandatory if you want Azure output.  For `AZURE_TENANT_ID` & `AZURE_SUBSCRIPTION_ID` check the output of `az account show --query "{subscriptionId:id, tenantId:tenantId}"`.  For the client id and secret, an Azure AD Service Principal is required and can be created, with the proper permissions, with this command: `az ad sp create-for-rbac --name MY-AD-SP --role=Contributor --scopes=/subscriptions/<SUBSCRIPTION ID>`.  These variables are the same as the `ARM_*` variables used by the Terraform Azure provider.  More information in the [official Microsoft documentation](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/terraform-install-configure)
-          - The `OS_*` variables are optional.  You may set them by sourcing the OpenStack RC v2.0 or v3 scripts that you may download from the web UI at [https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/](https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/).  Alternatively, you may use the `clouds.yaml` file described at the [OpenstackSDK documentation](https://docs.openstack.org/openstacksdk/latest/user/guides/connect_from_config.html)
-        
-        ## To run stand-alone:
-        
-        ```
-        pip3 install --user cloudview
-        ```
-        
-        ## To run with Docker (or Podman):
-        
-        If you want to use Podman instead of Docker:
-        ```
-        alias docker=podman
-        ```
-        
-        Build image with:
-        ```
-        docker build -t cloud --pull .
-        ```
-        
-        Export the variables listed in the [.dockerenv](.dockerenv) file and run with:
-        
-        ```
-        docker run --rm -v "$GOOGLE_APPLICATION_CREDENTIALS:$GOOGLE_APPLICATION_CREDENTIALS:ro" -v "$OS_CACERT:$OS_CACERT:ro" -v ~/.config/openstack:/etc/openstack:ro --env-file .dockerenv cloudview --status all
-        ```
-        
-        NOTES:
-          - To use `podman` in rootless mode, make sure to add your user to the /etc/subuid & /etc/subgid files as described in the [manual page](https://github.com/containers/libpod/blob/master/docs/podman.1.md#rootless-mode)
-        
-        ## Run the web server with [Docker Compose](https://docs.docker.com/compose/install/):
-        
-        If you have a TLS key pair, rename the certificate to `cert.pem`, the private key to `key.pem` and the file containing the passphrase to the private key to `key.txt`.  Then edit the [docker-compose.yml](docker-compose.yml) file to mount them to `/etc/nginx/ssl` in read-only mode like this: `- "/path/to/tls:/etc/nginx/ssl:ro"`.  Set and export the `NGINX_HOST` environment variable with the DNS of your host.
-        
-        If you don't have a TLS key pair, a self-signed certificate will be generated.  Be aware of the typical problems with time resolution related to TLS certificates.
-        
-        For HTTP Basic Authentication, create a file named `auth.htpasswd` in the same directory with the TLS certs.  Use the `htpasswd` utility for this.  This file is generated if a self-signed certificate is generated too.  In this case you must look up the generated password with `docker-compose logs`.  The user is `test`.
-        
-        This command creates 2 read-only containers for security, one with the Python app and another using Nginx as reverse-proxy:
-        
-        ```
-        docker-compose up -d
-        ```
-        
-        Now browse to [https://localhost:8443](https://localhost:8443)
-        
-        To stop the web server:
-        ```
-        docker-compose down
-        ```
-        
-        To rebuild the images:
-        ```
-        docker-compose build --pull
-        ```
-        
-        ### Filter options (AWS)
-        
-        Usage: `--filter-aws NAME VALUE`
-        
-        May be specified multiple times.
-        
-        Complete list of filters:
-        
-        [https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html)
-        
-        Example: `--filter-aws tag-key production`
-        
-        Note: If `instance-state-name` is present in the filter name, the `--status` option is ignored.
-        
-        ### Filter options (Azure)
-        
-        Usage: `--filter-azure FILTER`
-        
-        Note: This filtering is done in the client SDK using [JMESPath](http://jmespath.org/) to filter the JSON response.  You can view the JSON output using `--output JSON` or following the instance link in the HTML table.
-        
-        Complete list of filters:
-        
-        https://github.com/MicrosoftDocs/azure-docs-cli/blob/master/docs-ref-conceptual/query-azure-cli.md#filter-arrays
-        
-        Example: `--filter-azure "location == 'westeurope' && !(name == 'admin')"`
-        
-        Note: If `instance_view.statuses` is present in the filter, the `--status` option is ignored.
-        
-        ### Filter options (GCP)
-        
-        Usage: `--filter-gcp FILTER`
-        
-        Note: You may filter the resources listed in the API response.
-        
-        Complete list of resources:
-        
-        [https://cloud.google.com/compute/docs/reference/rest/v1/instances/list](https://cloud.google.com/compute/docs/reference/rest/v1/instances/list)
-        
-        Example: `--filter-gcp 'name: instance-1 AND canIpForward: false'`
-        
-        Note: If `status` is present in the filter, the `--status` option is ignored.
-        
-        ### Filter options (Openstack)
-        
-        Usage: `--filter-openstack NAME VALUE`
-        
-        May be specified multiple times.
-        
-        Complete list of filters:
-        
-        https://developer.openstack.org/api-ref/compute/?expanded=list-servers-detail#listServers
-        
-        Example: `--filter-openstack name admin`
-        
-        Note: If `status` is present in the filter, the `--status` option is ignored.
-        
-        ## TODO
-          - Search by tag (this can be done with the `filter-*` options)
-          - Sort by instance type (very tricky to get right ATM for all providers).
-          - Use apache-libcloud? (slow for some providers)
-        
-        ## Similar projects
-        
-          - [public cloud watch](https://github.com/cfconrad/pcw/)
-        
 Keywords: cloudview
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cloudview
+View instance information on all supported cloud providers: Amazon Web Services, Azure, Google Compute Platform & OpenStack.
+
+[![Build Status](https://travis-ci.com/ricardobranco777/cloudview.svg?branch=master)](https://travis-ci.org/ricardobranco777/cloudview)
+
+## Usage
+
+```
+Usage: cloudview [OPTIONS]
+Options:
+    -h, --help                          show this help message and exit
+    -l, --log debug|info|warning|error|critical
+    -o, --output text|html|json|JSON    output type
+    -p, --port PORT                     run a web server on port PORT
+    -r, --reverse                       reverse sort
+    -s, --sort name|time|status         sort type
+    -S, --status stopped|running|all    filter by instance status
+    -T, --time TIME_FORMAT              time format as used by strftime(3)
+    -v, --verbose                       be verbose
+    -V, --version                       show version and exit
+    --insecure                          do not validate TLS certificates
+Filter options:
+    --filter-aws NAME VALUE             may be specified multiple times
+    --filter-azure FILTER               Filter for Azure
+    --filter-gcp FILTER                 Filter for GCP
+    --filter-openstack NAME VALUE       may be specified multiple times
+```
+
+**NOTES**:
+  - Use `--output JSON` to dump _all_ available information received from each provider.
+
+This script is best run with Docker to have all dependencies in just one package, but it may be run stand-alone on systems with Python 3.6+
+
+## Environment variables
+
+    - `AWS_ACCESS_KEY_ID`
+    - `AWS_DEFAULT_REGION`
+    - `AWS_SECRET_ACCESS_KEY`
+    - `AZURE_TENANT_ID`
+    - `AZURE_SUBSCRIPTION_ID`
+    - `AZURE_CLIENT_SECRET`
+    - `AZURE_CLIENT_ID`
+    - `GOOGLE_APPLICATION_CREDENTIALS`
+    - `OS_USERNAME`
+    - `OS_PASSWORD`
+    - `OS_PROJECT_ID`
+    - `OS_AUTH_URL`
+    - `OS_USER_DOMAIN_NAME`
+    - `OS_CACERT`
+
+**NOTES**:
+  - The `AWS_*` environment variables are optional.  If not set, the AWS SDK will grab the information from `~/.aws/credentials` and `~/.aws/config`.
+  - The `GOOGLE_APPLICATION_CREDENTIALS` environment variable must contain the path to the JSON file downloaded from the GCP web console after creating a personal key for the service account of your project.
+  - The `AZURE_*` environment variables are mandatory if you want Azure output.  For `AZURE_TENANT_ID` & `AZURE_SUBSCRIPTION_ID` check the output of `az account show --query "{subscriptionId:id, tenantId:tenantId}"`.  For the client id and secret, an Azure AD Service Principal is required and can be created, with the proper permissions, with this command: `az ad sp create-for-rbac --name MY-AD-SP --role=Contributor --scopes=/subscriptions/<SUBSCRIPTION ID>`.  These variables are the same as the `ARM_*` variables used by the Terraform Azure provider.  More information in the [official Microsoft documentation](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/terraform-install-configure)
+  - The `OS_*` variables are optional.  You may set them by sourcing the OpenStack RC v2.0 or v3 scripts that you may download from the web UI at [https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/](https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/).  Alternatively, you may use the `clouds.yaml` file described at the [OpenstackSDK documentation](https://docs.openstack.org/openstacksdk/latest/user/guides/connect_from_config.html)
+
+## To run stand-alone:
+
+```
+pip3 install --user cloudview
+```
+
+## To run with Docker (or Podman):
+
+If you want to use Podman instead of Docker:
+```
+alias docker=podman
+```
+
+Build image with:
+```
+docker build -t cloud --pull .
+```
+
+Export the variables listed in the [.dockerenv](.dockerenv) file and run with:
+
+```
+docker run --rm -v "$GOOGLE_APPLICATION_CREDENTIALS:$GOOGLE_APPLICATION_CREDENTIALS:ro" -v "$OS_CACERT:$OS_CACERT:ro" -v ~/.config/openstack:/etc/openstack:ro --env-file .dockerenv cloudview --status all
+```
+
+NOTES:
+  - To use `podman` in rootless mode, make sure to add your user to the /etc/subuid & /etc/subgid files as described in the [manual page](https://github.com/containers/libpod/blob/master/docs/podman.1.md#rootless-mode)
+
+## Run the web server with [Docker Compose](https://docs.docker.com/compose/install/):
+
+If you have a TLS key pair, rename the certificate to `cert.pem`, the private key to `key.pem` and the file containing the passphrase to the private key to `key.txt`.  Then edit the [docker-compose.yml](docker-compose.yml) file to mount them to `/etc/nginx/ssl` in read-only mode like this: `- "/path/to/tls:/etc/nginx/ssl:ro"`.  Set and export the `NGINX_HOST` environment variable with the DNS of your host.
+
+If you don't have a TLS key pair, a self-signed certificate will be generated.  Be aware of the typical problems with time resolution related to TLS certificates.
+
+For HTTP Basic Authentication, create a file named `auth.htpasswd` in the same directory with the TLS certs.  Use the `htpasswd` utility for this.  This file is generated if a self-signed certificate is generated too.  In this case you must look up the generated password with `docker-compose logs`.  The user is `test`.
+
+This command creates 2 read-only containers for security, one with the Python app and another using Nginx as reverse-proxy:
+
+```
+docker-compose up -d
+```
+
+Now browse to [https://localhost:8443](https://localhost:8443)
+
+To stop the web server:
+```
+docker-compose down
+```
+
+To rebuild the images:
+```
+docker-compose build --pull
+```
+
+### Filter options (AWS)
+
+Usage: `--filter-aws NAME VALUE`
+
+May be specified multiple times.
+
+Complete list of filters:
+
+[https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html)
+
+Example: `--filter-aws tag-key production`
+
+Note: If `instance-state-name` is present in the filter name, the `--status` option is ignored.
+
+### Filter options (Azure)
+
+Usage: `--filter-azure FILTER`
+
+Note: This filtering is done in the client SDK using [JMESPath](http://jmespath.org/) to filter the JSON response.  You can view the JSON output using `--output JSON` or following the instance link in the HTML table.
+
+Complete list of filters:
+
+https://github.com/MicrosoftDocs/azure-docs-cli/blob/master/docs-ref-conceptual/query-azure-cli.md#filter-arrays
+
+Example: `--filter-azure "location == 'westeurope' && !(name == 'admin')"`
+
+Note: If `instance_view.statuses` is present in the filter, the `--status` option is ignored.
+
+### Filter options (GCP)
+
+Usage: `--filter-gcp FILTER`
+
+Note: You may filter the resources listed in the API response.
+
+Complete list of resources:
+
+[https://cloud.google.com/compute/docs/reference/rest/v1/instances/list](https://cloud.google.com/compute/docs/reference/rest/v1/instances/list)
+
+Example: `--filter-gcp 'name: instance-1 AND canIpForward: false'`
+
+Note: If `status` is present in the filter, the `--status` option is ignored.
+
+### Filter options (Openstack)
+
+Usage: `--filter-openstack NAME VALUE`
+
+May be specified multiple times.
+
+Complete list of filters:
+
+https://developer.openstack.org/api-ref/compute/?expanded=list-servers-detail#listServers
+
+Example: `--filter-openstack name admin`
+
+Note: If `status` is present in the filter, the `--status` option is ignored.
+
+## TODO
+  - Search by tag (this can be done with the `filter-*` options)
+  - Sort by instance type (very tricky to get right ATM for all providers).
+  - Use apache-libcloud? (slow for some providers)
+
+## Similar projects
+
+  - [public cloud watch](https://github.com/cfconrad/pcw/)
+
+
```

### Comparing `cloudview-0.3.8/README.md` & `cloudview-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     -p, --port PORT                     run a web server on port PORT
     -r, --reverse                       reverse sort
     -s, --sort name|time|status         sort type
     -S, --status stopped|running|all    filter by instance status
     -T, --time TIME_FORMAT              time format as used by strftime(3)
     -v, --verbose                       be verbose
     -V, --version                       show version and exit
+    --insecure                          do not validate TLS certificates
 Filter options:
     --filter-aws NAME VALUE             may be specified multiple times
     --filter-azure FILTER               Filter for Azure
     --filter-gcp FILTER                 Filter for GCP
     --filter-openstack NAME VALUE       may be specified multiple times
 ```
```

### Comparing `cloudview-0.3.8/_cloudview/amazon.py` & `cloudview-0.3.9/cloudview/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 Reference:
 https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_instances
 """
 
 from boto3 import client
 from botocore.exceptions import BotoCoreError, ClientError
 
-from _cloudview.exceptions import FatalError, WarningError
-from _cloudview.singleton import Singleton
+from cloudview.exceptions import FatalError, WarningError
+from cloudview.singleton import Singleton
 
 
 @Singleton
 class AWS:
     """
     Class for handling AWS stuff
     """
     def __init__(self):
         try:
             self._client = client('ec2')
         except (BotoCoreError, ClientError) as exc:
-            raise FatalError("AWS", exc)
+            raise FatalError("AWS", exc) from exc
         self._cache = None
 
     @staticmethod
     def get_tags(instance):
         """
         Return a dictionary of tags
         """
@@ -39,15 +39,15 @@
         """
         filters = filters or []
         instances = []
         try:
             pages = self._client.get_paginator('describe_instances').paginate(
                 Filters=filters)
         except (BotoCoreError, ClientError) as exc:
-            raise FatalError("AWS", exc)
+            raise FatalError("AWS", exc) from exc
         if jmespath_filter is not None:
             pages = pages.search(jmespath_filter)
         for page in pages:
             for item in page['Reservations']:
                 instances.extend(item['Instances'])
         self._cache = instances
         return instances
@@ -57,15 +57,15 @@
         Return specific instance
         """
         if self._cache is None:
             try:
                 return self._client.describe_instances(
                     InstanceIds=[instance_id])
             except (BotoCoreError, ClientError) as exc:
-                raise WarningError("AWS", exc)
+                raise WarningError("AWS", exc) from exc
         else:
             for instance in self._cache:
                 if instance['InstanceId'] == instance_id:
                     return instance
         return None
 
     @staticmethod
```

### Comparing `cloudview-0.3.8/_cloudview/az.py` & `cloudview-0.3.9/cloudview/az.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 from azure.identity import DefaultAzureCredential
 from azure.mgmt.compute import ComputeManagementClient
 from azure.core.exceptions import AzureError
 from msrestazure.azure_exceptions import CloudError
 from requests.exceptions import RequestException
 
-from _cloudview.exceptions import FatalError
-from _cloudview.singleton import Singleton
+from cloudview.exceptions import FatalError
+from cloudview.singleton import Singleton
 
 
 def get_credentials():
     """
     Get credentials for Azure
     """
     try:
```

### Comparing `cloudview-0.3.8/_cloudview/exceptions.py` & `cloudview-0.3.9/cloudview/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudview-0.3.8/_cloudview/gcp.py` & `cloudview-0.3.9/cloudview/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import json
 import os
 
 from googleapiclient.discovery import build
 from googleapiclient.errors import Error as GoogleError, HttpError
 from google.auth.exceptions import GoogleAuthError
 
-from _cloudview.exceptions import FatalError, WarningError
-from _cloudview.singleton import Singleton
+from cloudview.exceptions import FatalError, WarningError
+from cloudview.singleton import Singleton
 
 
 def get_project():
     """
     Get the project from the GCP credentials JSON file
     """
     try:
@@ -57,15 +57,15 @@
             except (GoogleAuthError, GoogleError) as exc:
                 FatalError("GCP", exc)
             if 'items' in response:
                 items.extend(_['name'] for _ in response['items'])
             request = self._compute.zones().list_next(request, response)
         return items
 
-    def get_instances(self, filters=None, orderBy=None):
+    def get_instances(self, filters=None, orderBy=None):  # pylint: disable=invalid-name
         """
         Get GCP instances
         Only sorting by "name" or "creationTimestamp desc" is supported
         Specifying both a list filter and sort order is not currently supported
         """
         if filters is not None and orderBy is not None:
             raise FatalError(
```

### Comparing `cloudview-0.3.8/_cloudview/openstack.py` & `cloudview-0.3.9/cloudview/openstack.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from concurrent.futures import ThreadPoolExecutor
 from functools import lru_cache
 
 import openstack
 from openstack.exceptions import OpenStackCloudException
 
-from _cloudview.exceptions import FatalError
-from _cloudview.singleton import Singleton2
+from cloudview.exceptions import FatalError
+from cloudview.singleton import Singleton2
 
 
 @Singleton2
 class Openstack:
     """
     Class for handling Openstack stuff
     """
@@ -27,55 +27,55 @@
             # https://urllib3.readthedocs.io/en/latest/advanced-usage.html#ssl-warnings
             import logging
             logging.captureWarnings(True)
         try:
             self._client = openstack.connect(
                 cloud=cloud, insecure=insecure)
         except OpenStackCloudException as exc:
-            raise FatalError("Openstack", exc)
+            raise FatalError("Openstack", exc) from exc
         self._cache = None
 
     def get_instances(self, filters=None):
         """
         Get Openstack instances
         """
         filters = filters or {}
         try:
             # https://developer.openstack.org/api-ref/compute/#list-servers
             instances = list(self._client.list_servers(filters=filters))
         except OpenStackCloudException as exc:
-            raise FatalError("Openstack", exc)
+            raise FatalError("Openstack", exc) from exc
         self._get_instance_types(instances)
         self._cache = instances
         return instances
 
     def get_instance(self, instance_id):
         """
         Return specific instance
         """
         if self._cache is None:
             try:
                 return self._client.get_server_by_id(instance_id)
             except OpenStackCloudException as exc:
-                raise FatalError("Openstack", exc)
+                raise FatalError("Openstack", exc) from exc
         else:
-            for instance in self._cache:
+            for instance in self._cache:  # pylint: disable=not-an-iterable
                 if instance['id'] == instance_id:
                     return instance
         return None
 
-    @lru_cache(maxsize=None)
+    @lru_cache(maxsize=1)
     def get_instance_type(self, flavor_id):
         """
         Return instance type
         """
         try:
             return self._client.get_flavor_by_id(flavor_id).name
         except OpenStackCloudException as exc:
-            raise FatalError("Openstack", exc)
+            raise FatalError("Openstack", exc) from exc
 
     def _get_instance_types(self, instances):
         """
         Threaded version to get all instance types using a pool of workers
         """
         with ThreadPoolExecutor() as executor:
             executor.map(
```

### Comparing `cloudview-0.3.8/_cloudview/output.py` & `cloudview-0.3.9/cloudview/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,32 @@
 # Copyright 2019 Ricardo Branco <rbranco@suse.de>
 # MIT License
 #
 """
 Handle tabular output in these formats: text, json & html
 """
 
-from functools import lru_cache
-from os.path import dirname
 from json import JSONEncoder
 
-from jinja2 import Template
+from cloudview.singleton import Singleton
+from cloudview.html import HEADER, FOOTER
 
-from _cloudview.singleton import Singleton
 
-
-@lru_cache(maxsize=1)
 def get_html_header(**kwargs):
     """
     Return the HTML header rendered from a Jinja2 template
     """
-    with open(dirname(__file__) + "/html/header.html", encoding="utf-8") as file:
-        template = Template(file.read())
-    return template.render(**kwargs)
+    return HEADER.render(**kwargs)
 
 
-@lru_cache(maxsize=1)
 def get_html_footer(**kwargs):
     """
     Return the HTML footer rendered from a Jinja2 template
     """
-    with open(dirname(__file__) + "/html/footer.html", encoding="utf-8") as file:
-        template = Template(file.read())
-    return template.render(**kwargs)
+    return FOOTER.render(**kwargs)
 
 
 @Singleton
 class Output:
     """
     Helper class to handle tabular output in text, json or html
     """
```

### Comparing `cloudview-0.3.8/_cloudview/singleton.py` & `cloudview-0.3.9/cloudview/singleton.py`

 * *Files identical despite different names*

### Comparing `cloudview-0.3.8/cloudview` & `cloudview-0.3.9/cloudview/cloudview.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,103 +9,66 @@
 
 import argparse
 import os
 import re
 import logging
 import sys
 
-from datetime import datetime
+import html
+from json import JSONEncoder
+
 from io import StringIO
-from itertools import groupby
 from operator import itemgetter
 from threading import Thread
 from wsgiref.simple_server import make_server
 
-import jmespath
-from jmespath.exceptions import JMESPathError
-
-import timeago
-
 from cachetools import cached, TTLCache
-from dateutil import parser
-from pytz import utc
 from pyramid.view import view_config
 from pyramid.config import Configurator
 from pyramid.response import Response
 
-from _cloudview.exceptions import FatalError
-from _cloudview.output import Output
-from _cloudview import __version__
+import openstack
+from .aws import AWS
+from .az import Azure
+from .gcp import GCP
+from .openstack import Openstack
+from .utils import fix_date
+from .output import Output
+from .filters import filters_aws, filters_azure, filters_gcp, filters_openstack
+from . import __version__
 
 
-USAGE = "Usage: " + os.path.basename(sys.argv[0]) + """ [OPTIONS]
+USAGE = f"""Usage: {os.path.basename(sys.argv[0])} [OPTIONS]
 Options:
     -h, --help                          show this help message and exit
     -l, --log debug|info|warning|error|critical
     -o, --output text|html|json|JSON    output type
     -p, --port PORT                     run a web server on port PORT
     -r, --reverse                       reverse sort
     -s, --sort name|time|status         sort type
     -S, --status stopped|running|all    filter by instance status
     -T, --time TIME_FORMAT              time format as used by strftime(3)
     -V, --version                       show version and exit
     -v, --verbose                       be verbose
+    --insecure                          do not validate TLS certificates
 Filter options:
     --filter-aws NAME VALUE             may be specified multiple times
     --filter-azure FILTER               Filter for Azure
     --filter-gcp FILTER                 Filter for GCP
     --filter-openstack NAME VALUE       may be specified multiple times
 """
 
-args = None
-
-
-def fix_date(date):
-    """
-    Converts datetime object or string to local time or the
-    timezone specified by the TZ environment variable
-    """
-    if isinstance(date, str):
-        # The parser returns datetime objects
-        date = parser.parse(date)
-    if isinstance(date, datetime):
-        # GCP doesn't return UTC dates
-        date = utc.normalize(date)
-        if args.verbose:
-            return date.astimezone().strftime(args.time)
-        return timeago.format(date, datetime.now(tz=utc))
-    return ""
+args = None  # pylint: disable=invalid-name
 
 
 def print_amazon_instances():
     """
     Print information about AWS EC2 instances
     """
-    filters = []
-    # https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-lifecycle.html
-    if args.status in ('running', 'stopped'):
-        # Consider an instance "running" if not stopped or terminated
-        # and "stopped" if not pending or running, hence the overlap
-        if args.status == "running":
-            statuses = 'pending running stopping shutting-down'.split()
-        else:
-            statuses = 'stopping stopped shutting-down terminated'.split()
-        filters = [['instance-state-name', _] for _ in statuses]
-    # If instance-state-name was specified in the filter, use it instead
-    if args.filter_aws:
-        if 'instance-state-name' in {_[0] for _ in args.filter_aws}:
-            filters = args.filter_aws
-        else:
-            filters.extend(args.filter_aws)
-    # Compile filter using 'Name' & 'Values'
-    filters = [
-        {'Name': name, 'Values': [v for _, v in values]}
-        for name, values in groupby(
-            sorted(filters, key=itemgetter(0)), itemgetter(0))
-    ]
+    filters = filters_aws(args.filter_aws, args.status)
     aws = AWS()
     instances = aws.get_instances(filters=filters)
     keys = {
         'name': lambda k: aws.get_tags(k).get('Name', k['InstanceId']),
         'time': itemgetter('LaunchTime', 'InstanceId'),
         'status': lambda k: (aws.get_status(k), k['InstanceId'])
     }
@@ -116,45 +79,23 @@
     for instance in instances:
         Output().info(
             provider="AWS",
             name=aws.get_tags(instance).get('Name', instance['InstanceId']),
             instance_id=instance['InstanceId'],
             size=instance['InstanceType'],
             status=aws.get_status(instance),
-            created=fix_date(instance['LaunchTime']),
+            created=fix_date(instance['LaunchTime'], args.time if args.verbose else None),
             location=instance['Placement']['AvailabilityZone'])
 
 
 def print_azure_instances():
     """
     Print information about Azure Compute instances
     """
-    filters = ""
-    # https://docs.microsoft.com/en-us/azure/virtual-machines/windows/states-lifecycle
-    if args.status in ('running', 'stopped'):
-        # Consider an instance "running" if not stopped / deallocated
-        # and "stopped" if not starting or running, hence the overlap
-        if args.status == "running":
-            statuses = 'starting running stopping'
-        else:
-            statuses = 'stopping stopped deallocating deallocated'
-        filters = " || ".join(
-            f"instance_view.statuses[1].code == 'PowerState/{status}'"
-            for status in statuses.split())
-    # If status was specified in the filter, use it instead
-    if args.filter_azure:
-        if "instance_view.statuses" in args.filter_azure or not filters:
-            filters = args.filter_azure
-        else:
-            filters += f" && ({args.filter_azure})"
-    if filters:
-        try:
-            filters = jmespath.compile(filters)
-        except JMESPathError as exc:
-            FatalError("Azure", exc)
+    filters = filters_azure(args.filter_azure, args.status)
     azure = Azure()
     instances = azure.get_instances(filters=filters if filters else None)
     keys = {
         'name': itemgetter('name'),
         'time': lambda k: (azure.get_date(k), k['name']),
         'status': lambda k: (azure.get_status(k), k['name'])
     }
@@ -169,42 +110,23 @@
     for instance in instances:
         Output().info(
             provider="Azure",
             name=instance['name'],
             instance_id=instance['vm_id'],
             size=instance['hardware_profile']['vm_size'],
             status=azure.get_status(instance),
-            created=fix_date(azure.get_date(instance)),
+            created=fix_date(azure.get_date(instance), args.time if args.verbose else None),
             location=instance['location'])
 
 
 def print_google_instances():
     """
     Print information about Google Compute instances
     """
-    filters = ""
-    # https://cloud.google.com/compute/docs/instances/instance-life-cycle
-    # NOTE: The above list is incomplete. The API returns more statuses
-    if args.status in ('running', 'stopped'):
-        # Consider an instance "running if not stopped / terminated
-        # and "stopped" if not starting, running, hence the overlap
-        if args.status == "running":
-            statuses = ('provisioning staging running'
-                        ' stopping suspending suspended')
-        else:
-            statuses = 'stopping stopped terminated'
-        filters = " OR ".join(
-            f"status: {status}"
-            for status in statuses.split())
-    # If status was specified in the filter, use it instead
-    if args.filter_gcp:
-        if "status" in args.filter_gcp or not filters:
-            filters = args.filter_gcp
-        else:
-            filters += f" AND ({args.filter_gcp})"
+    filters = filters_gcp(args.filter_gcp, args.status)
     gcp = GCP()
     instances = gcp.get_instances(filters=filters if filters else None)
     keys = {
         'name': itemgetter('name'),
         'time': itemgetter('creationTimestamp', 'name'),
         'status': itemgetter('status', 'name'),
     }
@@ -215,34 +137,24 @@
     for instance in instances:
         Output().info(
             provider="GCP",
             name=instance['name'],
             instance_id=instance['id'],
             size=instance['machineType'].rsplit('/', 1)[-1],
             status=gcp.get_status(instance),
-            created=fix_date(instance['creationTimestamp']),
+            created=fix_date(instance['creationTimestamp'], args.time if args.verbose else None),
             location=instance['zone'].rsplit('/', 1)[-1])
 
 
 def print_openstack_instances(cloud=None):
     """
     Print information about Openstack instances
     """
-    filters = {}
-    if args.status == 'running':
-        filters = {'status': 'ACTIVE'}
-    elif args.status == 'stopped':
-        filters = {'status': 'STOPPED'}
-    # If instance-state-name was specified in the filter, use it instead
-    if args.filter_openstack:
-        if 'status' in {_[0] for _ in args.filter_openstack}:
-            filters = {}
-        filters.update({_[0]: _[1] for _ in args.filter_openstack})
-    # https://docs.openstack.org/openstack/latest/reference/vm-states.html
-    ostack = Openstack(cloud=cloud)
+    filters = filters_openstack(args.filter_openstack, args.status)
+    ostack = Openstack(cloud=cloud, insecure=args.insecure)
     instances = ostack.get_instances(filters=filters)
     keys = {
         'name': itemgetter('name'),
         'time': itemgetter('created', 'name'),
         'status': lambda k: (ostack.get_status(k), k['name'])
     }
     instances.sort(key=keys[args.sort], reverse=args.reverse)
@@ -250,17 +162,17 @@
         Output().all(instances)
         return
     for instance in instances:
         Output().info(
             provider=cloud or "Openstack",
             name=instance['name'],
             instance_id=instance['id'],
-            size=ostack.get_instance_type(instance['flavor']['id']) if 'id' in instance['flavor'] else instance['flavor'],
+            size=ostack.get_instance_type(instance['flavor']['id']) if 'id' in instance['flavor'] else instance['flavor']['original_name'],
             status=ostack.get_status(instance),
-            created=fix_date(instance['created']),
+            created=fix_date(instance['created'], args.time if args.verbose else None),
             location=instance['OS-EXT-AZ:availability_zone'])
 
 
 @cached(cache=TTLCache(maxsize=2, ttl=120))
 def print_info():
     """
     Print information about instances
@@ -316,30 +228,27 @@
 
 
 @view_config(route_name='instance')
 def handle_instance(request):
     """
     Handle HTTP requests for instances
     """
-    import html
-    from json import JSONEncoder
-
     logging.info(request)
     provider = request.matchdict['provider']
     instance = request.matchdict['id']
     response = None
     if re.match("(i-)?[0-9a-f-]+$", instance):
         if provider == "aws":
             response = AWS().get_instance(instance)
         elif provider == "azure":
             response = Azure().get_instance(instance)
         elif provider == "gcp":
             response = GCP().get_instance(instance)
         else:
-            response = Openstack(cloud=provider).get_instance(instance)
+            response = Openstack(cloud=provider, insecure=args.insecure).get_instance(instance)
     if response is None:
         response = Response('Not found!')
         response.status_int = 404
         return response
     response = html.escape(
         JSONEncoder(default=str, indent=4, sort_keys=True).encode(response))
     header = '''<!DOCTYPE html><html><head><meta charset="utf-8">
@@ -403,21 +312,30 @@
     Check port argument
     """
     if port.isdigit() and 1 <= int(port) <= 65535:
         return int(port)
     raise argparse.ArgumentTypeError(f"{port} is an invalid port number")
 
 
+args = parse_args()
+check_aws = any([bool(args.filter_aws),
+                'AWS_ACCESS_KEY_ID' in os.environ,
+                 os.path.exists(os.getenv('AWS_SHARED_CREDENTIALS_FILE', os.path.expanduser("~/.aws/credentials")))])
+check_azure = bool(args.filter_azure) or any(v.startswith("AZURE_") for v in os.environ)
+check_gcp = bool(args.filter_gcp) or 'GOOGLE_APPLICATION_CREDENTIALS' in os.environ
+check_openstack = any([bool(args.filter_openstack),
+                      any(v.startswith("OS_") for v in os.environ),
+                      os.path.exists(os.path.expanduser("~/.config/openstack/clouds.yaml")),
+                      os.path.exists("/etc/openstack/clouds.yaml")])
+
+
 def main():
     """
     Main function
     """
-    global args  # pylint: disable=global-statement
-    args = parse_args()
-
     if args.help or args.version:
         print(USAGE if args.help else __version__)
         sys.exit(0)
 
     setup_logging()
 
     keys = "provider name size status created location"
@@ -432,31 +350,7 @@
     _ = Output(output_format=args.output.lower(), keys=keys, fmt=fmt)
 
     if args.port:
         web_server()
         sys.exit(1)
 
     print_info()
-
-
-if __name__ == "__main__":
-    args = parse_args()
-    check_aws = bool(args.filter_aws) or 'AWS_ACCESS_KEY_ID' in os.environ or \
-        os.path.exists(os.getenv('AWS_SHARED_CREDENTIALS_FILE', os.path.expanduser("~/.aws/credentials")))
-    check_azure = bool(args.filter_azure) or any(v.startswith("AZURE_") for v in os.environ)
-    check_gcp = bool(args.filter_gcp) or 'GOOGLE_APPLICATION_CREDENTIALS' in os.environ
-    check_openstack = bool(args.filter_openstack) or any(v.startswith("OS_") for v in os.environ) or \
-        os.path.exists(os.path.expanduser("~/.config/openstack/clouds.yaml")) or \
-        os.path.exists("/etc/openstack/clouds.yaml")
-    if check_aws:
-        from _cloudview.amazon import AWS
-    if check_azure:
-        from _cloudview.az import Azure
-    if check_gcp:
-        from _cloudview.gcp import GCP
-    if check_openstack:
-        import openstack
-        from _cloudview.openstack import Openstack  # pylint: disable=ungrouped-imports
-    try:
-        main()
-    except KeyboardInterrupt:
-        sys.exit(1)
```

### Comparing `cloudview-0.3.8/cloudview.egg-info/PKG-INFO` & `cloudview-0.3.9/cloudview.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,203 @@
 Metadata-Version: 2.1
 Name: cloudview
-Version: 0.3.8
+Version: 0.3.9
 Summary: View instance information on all supported cloud providers
 Home-page: https://github.com/ricardobranco777/cloudview
 Author: Ricardo Branco
 Author-email: rbranco@suse.de
 License: MIT License
-Description: # cloudview
-        View instance information on all supported cloud providers: Amazon Web Services, Azure, Google Compute Platform & OpenStack.
-        
-        [![Build Status](https://travis-ci.com/ricardobranco777/cloudview.svg?branch=master)](https://travis-ci.org/ricardobranco777/cloudview)
-        
-        ## Usage
-        
-        ```
-        Usage: cloudview [OPTIONS]
-        Options:
-            -h, --help                          show this help message and exit
-            -l, --log debug|info|warning|error|critical
-            -o, --output text|html|json|JSON    output type
-            -p, --port PORT                     run a web server on port PORT
-            -r, --reverse                       reverse sort
-            -s, --sort name|time|status         sort type
-            -S, --status stopped|running|all    filter by instance status
-            -T, --time TIME_FORMAT              time format as used by strftime(3)
-            -v, --verbose                       be verbose
-            -V, --version                       show version and exit
-        Filter options:
-            --filter-aws NAME VALUE             may be specified multiple times
-            --filter-azure FILTER               Filter for Azure
-            --filter-gcp FILTER                 Filter for GCP
-            --filter-openstack NAME VALUE       may be specified multiple times
-        ```
-        
-        **NOTES**:
-          - Use `--output JSON` to dump _all_ available information received from each provider.
-        
-        This script is best run with Docker to have all dependencies in just one package, but it may be run stand-alone on systems with Python 3.6+
-        
-        ## Environment variables
-        
-            - `AWS_ACCESS_KEY_ID`
-            - `AWS_DEFAULT_REGION`
-            - `AWS_SECRET_ACCESS_KEY`
-            - `AZURE_TENANT_ID`
-            - `AZURE_SUBSCRIPTION_ID`
-            - `AZURE_CLIENT_SECRET`
-            - `AZURE_CLIENT_ID`
-            - `GOOGLE_APPLICATION_CREDENTIALS`
-            - `OS_USERNAME`
-            - `OS_PASSWORD`
-            - `OS_PROJECT_ID`
-            - `OS_AUTH_URL`
-            - `OS_USER_DOMAIN_NAME`
-            - `OS_CACERT`
-        
-        **NOTES**:
-          - The `AWS_*` environment variables are optional.  If not set, the AWS SDK will grab the information from `~/.aws/credentials` and `~/.aws/config`.
-          - The `GOOGLE_APPLICATION_CREDENTIALS` environment variable must contain the path to the JSON file downloaded from the GCP web console after creating a personal key for the service account of your project.
-          - The `AZURE_*` environment variables are mandatory if you want Azure output.  For `AZURE_TENANT_ID` & `AZURE_SUBSCRIPTION_ID` check the output of `az account show --query "{subscriptionId:id, tenantId:tenantId}"`.  For the client id and secret, an Azure AD Service Principal is required and can be created, with the proper permissions, with this command: `az ad sp create-for-rbac --name MY-AD-SP --role=Contributor --scopes=/subscriptions/<SUBSCRIPTION ID>`.  These variables are the same as the `ARM_*` variables used by the Terraform Azure provider.  More information in the [official Microsoft documentation](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/terraform-install-configure)
-          - The `OS_*` variables are optional.  You may set them by sourcing the OpenStack RC v2.0 or v3 scripts that you may download from the web UI at [https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/](https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/).  Alternatively, you may use the `clouds.yaml` file described at the [OpenstackSDK documentation](https://docs.openstack.org/openstacksdk/latest/user/guides/connect_from_config.html)
-        
-        ## To run stand-alone:
-        
-        ```
-        pip3 install --user cloudview
-        ```
-        
-        ## To run with Docker (or Podman):
-        
-        If you want to use Podman instead of Docker:
-        ```
-        alias docker=podman
-        ```
-        
-        Build image with:
-        ```
-        docker build -t cloud --pull .
-        ```
-        
-        Export the variables listed in the [.dockerenv](.dockerenv) file and run with:
-        
-        ```
-        docker run --rm -v "$GOOGLE_APPLICATION_CREDENTIALS:$GOOGLE_APPLICATION_CREDENTIALS:ro" -v "$OS_CACERT:$OS_CACERT:ro" -v ~/.config/openstack:/etc/openstack:ro --env-file .dockerenv cloudview --status all
-        ```
-        
-        NOTES:
-          - To use `podman` in rootless mode, make sure to add your user to the /etc/subuid & /etc/subgid files as described in the [manual page](https://github.com/containers/libpod/blob/master/docs/podman.1.md#rootless-mode)
-        
-        ## Run the web server with [Docker Compose](https://docs.docker.com/compose/install/):
-        
-        If you have a TLS key pair, rename the certificate to `cert.pem`, the private key to `key.pem` and the file containing the passphrase to the private key to `key.txt`.  Then edit the [docker-compose.yml](docker-compose.yml) file to mount them to `/etc/nginx/ssl` in read-only mode like this: `- "/path/to/tls:/etc/nginx/ssl:ro"`.  Set and export the `NGINX_HOST` environment variable with the DNS of your host.
-        
-        If you don't have a TLS key pair, a self-signed certificate will be generated.  Be aware of the typical problems with time resolution related to TLS certificates.
-        
-        For HTTP Basic Authentication, create a file named `auth.htpasswd` in the same directory with the TLS certs.  Use the `htpasswd` utility for this.  This file is generated if a self-signed certificate is generated too.  In this case you must look up the generated password with `docker-compose logs`.  The user is `test`.
-        
-        This command creates 2 read-only containers for security, one with the Python app and another using Nginx as reverse-proxy:
-        
-        ```
-        docker-compose up -d
-        ```
-        
-        Now browse to [https://localhost:8443](https://localhost:8443)
-        
-        To stop the web server:
-        ```
-        docker-compose down
-        ```
-        
-        To rebuild the images:
-        ```
-        docker-compose build --pull
-        ```
-        
-        ### Filter options (AWS)
-        
-        Usage: `--filter-aws NAME VALUE`
-        
-        May be specified multiple times.
-        
-        Complete list of filters:
-        
-        [https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html)
-        
-        Example: `--filter-aws tag-key production`
-        
-        Note: If `instance-state-name` is present in the filter name, the `--status` option is ignored.
-        
-        ### Filter options (Azure)
-        
-        Usage: `--filter-azure FILTER`
-        
-        Note: This filtering is done in the client SDK using [JMESPath](http://jmespath.org/) to filter the JSON response.  You can view the JSON output using `--output JSON` or following the instance link in the HTML table.
-        
-        Complete list of filters:
-        
-        https://github.com/MicrosoftDocs/azure-docs-cli/blob/master/docs-ref-conceptual/query-azure-cli.md#filter-arrays
-        
-        Example: `--filter-azure "location == 'westeurope' && !(name == 'admin')"`
-        
-        Note: If `instance_view.statuses` is present in the filter, the `--status` option is ignored.
-        
-        ### Filter options (GCP)
-        
-        Usage: `--filter-gcp FILTER`
-        
-        Note: You may filter the resources listed in the API response.
-        
-        Complete list of resources:
-        
-        [https://cloud.google.com/compute/docs/reference/rest/v1/instances/list](https://cloud.google.com/compute/docs/reference/rest/v1/instances/list)
-        
-        Example: `--filter-gcp 'name: instance-1 AND canIpForward: false'`
-        
-        Note: If `status` is present in the filter, the `--status` option is ignored.
-        
-        ### Filter options (Openstack)
-        
-        Usage: `--filter-openstack NAME VALUE`
-        
-        May be specified multiple times.
-        
-        Complete list of filters:
-        
-        https://developer.openstack.org/api-ref/compute/?expanded=list-servers-detail#listServers
-        
-        Example: `--filter-openstack name admin`
-        
-        Note: If `status` is present in the filter, the `--status` option is ignored.
-        
-        ## TODO
-          - Search by tag (this can be done with the `filter-*` options)
-          - Sort by instance type (very tricky to get right ATM for all providers).
-          - Use apache-libcloud? (slow for some providers)
-        
-        ## Similar projects
-        
-          - [public cloud watch](https://github.com/cfconrad/pcw/)
-        
 Keywords: cloudview
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cloudview
+View instance information on all supported cloud providers: Amazon Web Services, Azure, Google Compute Platform & OpenStack.
+
+[![Build Status](https://travis-ci.com/ricardobranco777/cloudview.svg?branch=master)](https://travis-ci.org/ricardobranco777/cloudview)
+
+## Usage
+
+```
+Usage: cloudview [OPTIONS]
+Options:
+    -h, --help                          show this help message and exit
+    -l, --log debug|info|warning|error|critical
+    -o, --output text|html|json|JSON    output type
+    -p, --port PORT                     run a web server on port PORT
+    -r, --reverse                       reverse sort
+    -s, --sort name|time|status         sort type
+    -S, --status stopped|running|all    filter by instance status
+    -T, --time TIME_FORMAT              time format as used by strftime(3)
+    -v, --verbose                       be verbose
+    -V, --version                       show version and exit
+    --insecure                          do not validate TLS certificates
+Filter options:
+    --filter-aws NAME VALUE             may be specified multiple times
+    --filter-azure FILTER               Filter for Azure
+    --filter-gcp FILTER                 Filter for GCP
+    --filter-openstack NAME VALUE       may be specified multiple times
+```
+
+**NOTES**:
+  - Use `--output JSON` to dump _all_ available information received from each provider.
+
+This script is best run with Docker to have all dependencies in just one package, but it may be run stand-alone on systems with Python 3.6+
+
+## Environment variables
+
+    - `AWS_ACCESS_KEY_ID`
+    - `AWS_DEFAULT_REGION`
+    - `AWS_SECRET_ACCESS_KEY`
+    - `AZURE_TENANT_ID`
+    - `AZURE_SUBSCRIPTION_ID`
+    - `AZURE_CLIENT_SECRET`
+    - `AZURE_CLIENT_ID`
+    - `GOOGLE_APPLICATION_CREDENTIALS`
+    - `OS_USERNAME`
+    - `OS_PASSWORD`
+    - `OS_PROJECT_ID`
+    - `OS_AUTH_URL`
+    - `OS_USER_DOMAIN_NAME`
+    - `OS_CACERT`
+
+**NOTES**:
+  - The `AWS_*` environment variables are optional.  If not set, the AWS SDK will grab the information from `~/.aws/credentials` and `~/.aws/config`.
+  - The `GOOGLE_APPLICATION_CREDENTIALS` environment variable must contain the path to the JSON file downloaded from the GCP web console after creating a personal key for the service account of your project.
+  - The `AZURE_*` environment variables are mandatory if you want Azure output.  For `AZURE_TENANT_ID` & `AZURE_SUBSCRIPTION_ID` check the output of `az account show --query "{subscriptionId:id, tenantId:tenantId}"`.  For the client id and secret, an Azure AD Service Principal is required and can be created, with the proper permissions, with this command: `az ad sp create-for-rbac --name MY-AD-SP --role=Contributor --scopes=/subscriptions/<SUBSCRIPTION ID>`.  These variables are the same as the `ARM_*` variables used by the Terraform Azure provider.  More information in the [official Microsoft documentation](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/terraform-install-configure)
+  - The `OS_*` variables are optional.  You may set them by sourcing the OpenStack RC v2.0 or v3 scripts that you may download from the web UI at [https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/](https://OPENSTACK_SERVER/project/access_and_security/api_access/openrc/).  Alternatively, you may use the `clouds.yaml` file described at the [OpenstackSDK documentation](https://docs.openstack.org/openstacksdk/latest/user/guides/connect_from_config.html)
+
+## To run stand-alone:
+
+```
+pip3 install --user cloudview
+```
+
+## To run with Docker (or Podman):
+
+If you want to use Podman instead of Docker:
+```
+alias docker=podman
+```
+
+Build image with:
+```
+docker build -t cloud --pull .
+```
+
+Export the variables listed in the [.dockerenv](.dockerenv) file and run with:
+
+```
+docker run --rm -v "$GOOGLE_APPLICATION_CREDENTIALS:$GOOGLE_APPLICATION_CREDENTIALS:ro" -v "$OS_CACERT:$OS_CACERT:ro" -v ~/.config/openstack:/etc/openstack:ro --env-file .dockerenv cloudview --status all
+```
+
+NOTES:
+  - To use `podman` in rootless mode, make sure to add your user to the /etc/subuid & /etc/subgid files as described in the [manual page](https://github.com/containers/libpod/blob/master/docs/podman.1.md#rootless-mode)
+
+## Run the web server with [Docker Compose](https://docs.docker.com/compose/install/):
+
+If you have a TLS key pair, rename the certificate to `cert.pem`, the private key to `key.pem` and the file containing the passphrase to the private key to `key.txt`.  Then edit the [docker-compose.yml](docker-compose.yml) file to mount them to `/etc/nginx/ssl` in read-only mode like this: `- "/path/to/tls:/etc/nginx/ssl:ro"`.  Set and export the `NGINX_HOST` environment variable with the DNS of your host.
+
+If you don't have a TLS key pair, a self-signed certificate will be generated.  Be aware of the typical problems with time resolution related to TLS certificates.
+
+For HTTP Basic Authentication, create a file named `auth.htpasswd` in the same directory with the TLS certs.  Use the `htpasswd` utility for this.  This file is generated if a self-signed certificate is generated too.  In this case you must look up the generated password with `docker-compose logs`.  The user is `test`.
+
+This command creates 2 read-only containers for security, one with the Python app and another using Nginx as reverse-proxy:
+
+```
+docker-compose up -d
+```
+
+Now browse to [https://localhost:8443](https://localhost:8443)
+
+To stop the web server:
+```
+docker-compose down
+```
+
+To rebuild the images:
+```
+docker-compose build --pull
+```
+
+### Filter options (AWS)
+
+Usage: `--filter-aws NAME VALUE`
+
+May be specified multiple times.
+
+Complete list of filters:
+
+[https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html)
+
+Example: `--filter-aws tag-key production`
+
+Note: If `instance-state-name` is present in the filter name, the `--status` option is ignored.
+
+### Filter options (Azure)
+
+Usage: `--filter-azure FILTER`
+
+Note: This filtering is done in the client SDK using [JMESPath](http://jmespath.org/) to filter the JSON response.  You can view the JSON output using `--output JSON` or following the instance link in the HTML table.
+
+Complete list of filters:
+
+https://github.com/MicrosoftDocs/azure-docs-cli/blob/master/docs-ref-conceptual/query-azure-cli.md#filter-arrays
+
+Example: `--filter-azure "location == 'westeurope' && !(name == 'admin')"`
+
+Note: If `instance_view.statuses` is present in the filter, the `--status` option is ignored.
+
+### Filter options (GCP)
+
+Usage: `--filter-gcp FILTER`
+
+Note: You may filter the resources listed in the API response.
+
+Complete list of resources:
+
+[https://cloud.google.com/compute/docs/reference/rest/v1/instances/list](https://cloud.google.com/compute/docs/reference/rest/v1/instances/list)
+
+Example: `--filter-gcp 'name: instance-1 AND canIpForward: false'`
+
+Note: If `status` is present in the filter, the `--status` option is ignored.
+
+### Filter options (Openstack)
+
+Usage: `--filter-openstack NAME VALUE`
+
+May be specified multiple times.
+
+Complete list of filters:
+
+https://developer.openstack.org/api-ref/compute/?expanded=list-servers-detail#listServers
+
+Example: `--filter-openstack name admin`
+
+Note: If `status` is present in the filter, the `--status` option is ignored.
+
+## TODO
+  - Search by tag (this can be done with the `filter-*` options)
+  - Sort by instance type (very tricky to get right ATM for all providers).
+  - Use apache-libcloud? (slow for some providers)
+
+## Similar projects
+
+  - [public cloud watch](https://github.com/cfconrad/pcw/)
+
+
```

### Comparing `cloudview-0.3.8/cloudview.egg-info/requires.txt` & `cloudview-0.3.9/cloudview.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,72 @@
+Jinja2==3.1.2
+MarkupSafe==2.1.1
+PasteDeploy==2.1.1
+PyJWT==2.4.0
+PyYAML==6.0
+WebOb==1.8.7
 adal==1.2.7
 appdirs==1.4.4
 azure-common==1.1.28
-azure-core==1.22.1
-azure-identity==1.7.1
-azure-mgmt-compute==25.0.0
+azure-core==1.24.0
+azure-identity==1.10.0
+azure-mgmt-compute==27.0.0
 azure-mgmt-core==1.3.0
-boto3==1.20.52
-botocore==1.23.52
-cachetools==5.0.0
-certifi==2021.10.8
+boto3==1.23.7
+botocore==1.26.7
+cachetools==5.1.0
+certifi==2022.5.18.1
 cffi==1.15.0
-charset-normalizer==2.0.11
-cryptography==36.0.1
+charset-normalizer==2.0.12
+cryptography==37.0.2
 decorator==5.1.1
 dogpile.cache==1.1.5
-google-api-core==2.5.0
-google-api-python-client==2.37.0
-google-auth==2.6.0
+google-api-core==2.8.0
+google-api-python-client==2.48.0
 google-auth-httplib2==0.1.0
-googleapis-common-protos==1.54.0
+google-auth==2.6.6
+googleapis-common-protos==1.56.1
 httplib2==0.20.4
 hupper==1.10.3
 idna==3.3
 iso8601==1.0.2
 isodate==0.6.1
-Jinja2==3.0.3
-jmespath==0.10.0
+jmespath==1.0.0
 jsonpatch==1.32
-jsonpointer==2.2
-keystoneauth1==4.4.0
-MarkupSafe==2.0.1
-msal==1.16.0
-msal-extensions==0.3.1
+jsonpointer==2.3
+keystoneauth1==4.6.0
+msal-extensions==1.0.0
+msal==1.17.0
 msrest==0.6.21
 msrestazure==0.6.4
 munch==2.5.0
 netifaces==0.11.0
 oauth2client==4.1.3
 oauthlib==3.2.0
-openstacksdk==0.61.0
+openstacksdk==0.99.0
 os-service-types==1.7.0
-PasteDeploy==2.1.1
-pbr==5.8.1
-plaster==1.0
+pbr==5.9.0
 plaster-pastedeploy==0.7
-portalocker==2.3.2
-protobuf==3.19.4
-pyasn1==0.4.8
+plaster==1.0
+portalocker==2.4.0
+protobuf==3.20.1
 pyasn1-modules==0.2.8
+pyasn1==0.4.8
 pycparser==2.21
-PyJWT==2.3.0
-pyparsing==3.0.7
+pyparsing==3.0.9
 pyramid==2.0
 python-dateutil==2.8.2
-pytz==2021.3
-PyYAML==6.0
-requests==2.27.1
+pytz==2022.1
 requests-oauthlib==1.3.1
+requests==2.27.1
 requestsexceptions==1.4.0
 rsa==4.8
-s3transfer==0.5.1
+s3transfer==0.5.2
 six==1.16.0
 stevedore==3.5.0
-timeago==1.0.15
 translationstring==1.4
+typing_extensions==4.2.0
 uritemplate==4.1.1
-urllib3==1.26.8
+urllib3==1.26.9
 venusian==3.0.0
-WebOb==1.8.7
 zope.deprecation==4.4.0
 zope.interface==5.4.0
```

### Comparing `cloudview-0.3.8/setup.py` & `cloudview-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,46 +14,47 @@
         return file_.read()
 
 
 def grep_version():
     """
     Get __version__
     """
-    from _cloudview import __version__
+    from cloudview import __version__
     return __version__
 
 
 setup(
     name='cloudview',
     version=grep_version(),
     description="View instance information on all supported cloud providers",
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     author="Ricardo Branco",
     author_email='rbranco@suse.de',
     url='https://github.com/ricardobranco777/cloudview',
-    package_dir={'cloudview': '_cloudview'},
+    package_dir={'cloudview': 'cloudview'},
     packages=find_packages(),
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=read('requirements.txt'),
     license='MIT License',
     zip_safe=False,
     keywords='cloudview',
-    scripts=['cloudview'],
+    scripts=['scripts/cloudview'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Topic :: System :: Monitoring',
         'License :: OSI Approved :: '
         'MIT License',
         'Natural Language :: English',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
     ],
 )
```

