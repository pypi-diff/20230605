# Comparing `tmp/CheckSSLCert-0.1.0.tar.gz` & `tmp/CheckSSLCert-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheckSSLCert-0.1.0.tar", last modified: Sat Jun  3 08:39:23 2023, max compression
+gzip compressed data, was "CheckSSLCert-0.1.1.tar", last modified: Mon Jun  5 07:34:16 2023, max compression
```

## Comparing `CheckSSLCert-0.1.0.tar` & `CheckSSLCert-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.324526 CheckSSLCert-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-06-01 13:49:19.000000 CheckSSLCert-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4763 2023-06-03 08:39:23.277628 CheckSSLCert-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4074 2023-06-03 07:51:20.000000 CheckSSLCert-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-02 05:24:56.000000 CheckSSLCert-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 08:39:23.324526 CheckSSLCert-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-06-03 08:38:48.000000 CheckSSLCert-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.262007 CheckSSLCert-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.262007 CheckSSLCert-0.1.0/src/CheckSSLCert/
--rw-rw-rw-   0        0        0       35 2023-06-01 08:02:33.000000 CheckSSLCert-0.1.0/src/CheckSSLCert/__init__.py
--rw-rw-rw-   0        0        0    11419 2023-06-02 13:55:06.000000 CheckSSLCert-0.1.0/src/CheckSSLCert/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.277628 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/
--rw-rw-rw-   0        0        0     4763 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:16.828329 CheckSSLCert-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 13:49:19.000000 CheckSSLCert-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7048 2023-06-05 07:34:16.828329 CheckSSLCert-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6359 2023-06-05 07:29:08.000000 CheckSSLCert-0.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-02 05:24:56.000000 CheckSSLCert-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:34:16.828329 CheckSSLCert-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-06-05 07:33:21.000000 CheckSSLCert-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:16.797088 CheckSSLCert-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:16.812710 CheckSSLCert-0.1.1/src/CheckSSLCert/
+-rw-rw-rw-   0        0        0       35 2023-06-01 08:02:33.000000 CheckSSLCert-0.1.1/src/CheckSSLCert/__init__.py
+-rw-rw-rw-   0        0        0    13379 2023-06-05 07:24:30.000000 CheckSSLCert-0.1.1/src/CheckSSLCert/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:16.828329 CheckSSLCert-0.1.1/src/CheckSSLCert.egg-info/
+-rw-rw-rw-   0        0        0     7048 2023-06-05 07:34:16.000000 CheckSSLCert-0.1.1/src/CheckSSLCert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-05 07:34:16.000000 CheckSSLCert-0.1.1/src/CheckSSLCert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:34:16.000000 CheckSSLCert-0.1.1/src/CheckSSLCert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 07:34:16.000000 CheckSSLCert-0.1.1/src/CheckSSLCert.egg-info/top_level.txt
```

### Comparing `CheckSSLCert-0.1.0/LICENSE` & `CheckSSLCert-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CheckSSLCert-0.1.0/PKG-INFO` & `CheckSSLCert-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,44 @@
-Metadata-Version: 2.1
-Name: CheckSSLCert
-Version: 0.1.0
-Summary: CheckSSLCert is a Python library that allows you to check the SSL certificate status.
-Home-page: https://github.com/Huntroid-India/CheckSSLCert
-Author: Srimath
-Author-email: srimath8@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/Huntroid-India/CheckSSLCert/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CheckSSLCert
-[![Made with Python](https://img.shields.io/badge/Python->=3.6-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 
+[![Made with Python](https://img.shields.io/badge/Python->=3.6-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 
 [![Huntroid-India - SSLCheckerr](https://img.shields.io/static/v1?label=Huntroid-India&message=CheckSSLCert&color=blue&logo=github)](https://github.com/Huntroid-India/CheckSSLCert "Go to GitHub repo")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 [![stars - SSLChecker](https://img.shields.io/github/stars/Huntroid-India/CheckSSLCert?style=social)](https://github.com/Huntroid-India/CheckSSLCert)
 [![forks - SSLChecker](https://img.shields.io/github/forks/Huntroid-India/CheckSSLCert?style=social)](https://github.com/Huntroid-India/CheckSSLCert)
-[![GitHub release](https://img.shields.io/github/release/Huntroid-India/CheckSSLCert?include_prereleases=&sort=semver&color=blue)](https://github.com/Huntroid-India/CheckSSLCert/releases/)
 [![issues - SSLCheckerr](https://img.shields.io/github/issues/Huntroid-India/CheckSSLCert)](https://github.com/Huntroid-India/CheckSSLCert/issues)
+<!-- [![GitHub release](https://img.shields.io/github/release/Huntroid-India/CheckSSLCert?include_prereleases=&sort=semver&color=blue)](https://github.com/Huntroid-India/CheckSSLCert/releases/)
+-->
+
 
-CheckSSLCert is a Python library that allows you to check the SSL certificate status for single or multiple domains. It provides an easy way to determine if an SSL certificate is active, the number of days left until it expires, and additional certificate information. 
+CheckSSLCert is a Python library that allows you to check the SSL certificate status for single or multiple domains. It
+provides an easy way to determine if an SSL certificate is active, the number of days left until it expires, and
+additional certificate information.
 
 ## Installation
+
 You can install CheckSSLCert using pip:
+
 ```
 pip install CheckSSLCert
 ```
 
 ## Usage
+
 ### SSL Validation (Single Domain)
-To check the SSL certificate status for a single domain, you can use the from_link function from validate class. Here's a sample code demonstrating the usage:
+
+To check the SSL certificate status for a single domain, you can use the ``from_link`` function from ``validate`` class.
+
+_Here's a sample code demonstrating the usage:_
+
 ```
 from CheckSSLCert import validate
 
-# Create an sslchecker object for the domain
+# Create an from_link object for the domain
 checker = validate.from_link("example.com")
 
 # Check the SSL certificate status
 status = checker.IsActive()
 days_left = checker.getDayLeft()
 info = checker.getInfo()
 
@@ -54,55 +47,125 @@
 print("Days Left:", days_left)
 print("Certificate Info:", info)
 
 # Print the SSL certificate Report
 print(checker)
 ```
 
-### Bulk SSL Validation (Multiple Domains - CSV File)
-To check the SSL certificate status for multiple domains, you can use the from_file function from validate class. Here's a sample code demonstrating the usage:
+## Bulk SSL Validation (Multiple Domains - CSV File)
+
+To check the SSL certificate status for multiple domains, you can use the ``from_file`` function from ``validate``
+class.
+
+### Print the SSL certificate status report to the console
+
+_Here's a sample code demonstrating the usage:_
+
 ```
 from CheckSSLCert import validate
 
-# Create a bulksslchecker object with the path to the domain list file (CSV format)
+# Create a from_file object with the path to the domain list file (CSV format)
 checker = validate.from_file("domain_list.csv")
 
-# Print the SSL certificate status report to the console
+# Print the SSL certificate status report to the console (Full Report)
 checker.print_report()
 
-# Send the SSL certificate status report to an email address
-checker.send_report("sender_address", "sender_password", "receiver_address", "Subject")
-# Note: It is recommended to use an app password for the sender password. It only works with Gmail(Sender).
+# Print the SSL certificate status report to the console (Partial Report)
+checker.print_report(IsAll=False)
+
+```
+
+**Note:**
+
++ If you want to print the complete report, set ``IsAll`` to ``True``. By default, the full report is printed.
++ If you want to print the report only for the domains with expired or expiring in 14 days, set ``IsAll`` to ``False``.
+
+---
+
+### Send the SSL certificate status report via email
+
+_Here's a sample code demonstrating the usage:_
+
+```
+from CheckSSLCert import validate
+
+# Create a from_file object with the path to the domain list file (CSV format)
+checker = validate.from_file("domain_list.csv")
+
+# Configure the Mail Server
+mail_config = {'sender': "example@gmail.com",
+               'password': "passward",
+               'receiver': ["example2@gmail.com", "example3@gmail.com"],
+               'subject': "SSL Checker Report",
+               'smtp_server': "smtp.gmail.com",
+               'port': 587}
+
+# Send the SSL certificate status report to an email address (Full Report)
+checker.send_report(mail_config, IsAll=True)
+
+# Send the SSL certificate status report to an email address (Partial Report)
+checker.send_report(mail_config, IsAll=False)
+
+```
+
+**Note:**
+
++ If you want to you a different mail server, set ``smtp_server`` to the SMTP server address in ``mail_config``.
++ If you want to use TLS, set ``port`` to ``587`` in ``mail_config``.
++ If you want to use SSL, set ``port`` to ``465`` in ``mail_config``.
++ If you want to send the complete report, set ``IsAll`` to ``True``. By default, the full report is sent.
++ If you want to send the report only for the domains with expired or expiring in 14 days, set ``IsAll`` to ``False``.
+
+---
+
+### Save the SSL certificate status report to a file
+
+_Here's a sample code demonstrating the usage:_
+
+```
+from CheckSSLCert import validate
+
+# Create a from_file object with the path to the domain list file (CSV format)
+checker = validate.from_file("domain_list.csv")
 
 # Save the SSL certificate status report to a file (HTML format)
-checker.save_report("C:\Users\YourUsername\Desktop") # By default HTML is selected
-checker.save_report("C:\Users\YourUsername\Desktop", "html")
+
+# By default, the report is saved in HTML format
+checker.save_report("C:\Users\YourUsername\Desktop") 
 
 # Save the SSL certificate status report to a file (CSV format)
-checker.save_report("C:\Users\YourUsername\Desktop", "csv")
+checker.save_report("C:\Users\YourUsername\Desktop", file_type="csv")
 ```
-### Domain List File Format
-The domain list file should be in CSV format. The first row should contain the column names. Here's a sample domain list file:
+
+**Note:**
+
++ If you want to save the complete report, set ``IsAll`` to ``True``. By default, the full report is saved.
++ If you want to save the report only for the domains with expired or expiring in 14 days, set ``IsAll`` to ``False``.
++ By default, the report is saved in HTML format. If you want to save the report in CSV format, set ``file_type``
+  to ``csv``.
+
+## Domain List File Format
+
+The domain list file should be in CSV format. The first row should contain the column names. Here's a sample domain list
+file:
+
+Click the Download button and Save it as ``domain_list.csv``.
 
 [![CSV - Documentation](https://img.shields.io/badge/Download-CSV-blue?style=for-the-badge)](https://raw.githubusercontent.com/Huntroid-India/CheckSSLCert/main/domain_list.csv "Go to project documentation")
 
 #### File Format
 
-
 | S.No | Website_Name      | Website_URL        |
 |------|-------------------|--------------------|
 | 1 | Google            | https://google.com |
 | 2 | Facebook - Mobile | https://m.facebook.com     |
 | 3 | Twitter           | www.twitter.com    |
 
-
-
-
-
 ## Contribution
+
 Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please submit a pull request.
 
 ## License
 
 Released under [MIT](/LICENSE) by [@Huntroid-India](https://github.com/Huntroid-India).
```

### Comparing `CheckSSLCert-0.1.0/setup.py` & `CheckSSLCert-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='CheckSSLCert',
-    version='0.1.0',
+    version='0.1.1',
     url='https://github.com/Huntroid-India/CheckSSLCert',
     project_urls={
         "Bug Tracker": "https://github.com/Huntroid-India/CheckSSLCert/issues",
     },
     license='MIT',
     author='Srimath',
     author_email='srimath8@gmail.com',
```

### Comparing `CheckSSLCert-0.1.0/src/CheckSSLCert/validate.py` & `CheckSSLCert-0.1.1/src/CheckSSLCert/validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class from_file:
 
     def __init__(self, path):
         import datetime
         self.__path = path
-        self.__subject = "SSL Certificate Status Report on " + datetime.datetime.now().strftime("%d-%m-%Y %H:%M:%S %p %z")
+        self.__subject = "SSL Certificate Status Report on " + datetime.datetime.now().strftime(
+            "%d-%m-%Y %H:%M:%S %p %z")
         self.__d_sno = []
         self.__d_name = []
         self.__d_link = []
         self.__d_status = []
         self.__d_days = []
         self.__d_info = []
         self.__m_row = [["S.NO", "Site Name", "Domain", "Status", "Days Left", "Error Info"]]
@@ -108,51 +109,89 @@
                               ['<td>{}</td>'.format(cell) for cell in row]
                           )) for row in table_data[1:]
                       ])
                       )
         print("Content Composed")
         return email_body
 
-    def send_report(self, sender, pwd, receiver, subject):
+    def send_report(self, mail_config, IsAll=True):
         import smtplib, ssl
         from email.mime.text import MIMEText
         from email.mime.multipart import MIMEMultipart
+        try:
+            smtp_server = mail_config['smtp_server']
+            port = mail_config['port']
+            sender = mail_config['sender']
+            pwd = mail_config['password']
+            receiver = mail_config['receiver']
+            subject = mail_config['subject']
+        except KeyError:
+            print("Error : Invalid Mail Config")
+            return
 
         try:
-            self.__mail_data = self.__compose_email_with_table(self.__getrawdata())
-            context = ssl.create_default_context()
-            with smtplib.SMTP('smtp.gmail.com', 587) as server:
-                print("Sending Email")
-                server.ehlo()
-                server.starttls(context=context)
-                server.ehlo()
-                server.ehlo()
-                server.login(sender, pwd, initial_response_ok=True)
-                message = MIMEMultipart()
-                message['From'] = sender
-                message['To'] = receiver
-                message['Subject'] = subject
-                message.attach(MIMEText(self.__getmaildata(), 'html'))
-                text = message.as_string()
-                server.ehlo()
-                server.sendmail(sender, receiver, text)
-                server.quit()
-                print("Email Sent")
+            self.__mail_data = self.__compose_email_with_table(self.__getrawdata(IsAll))
+            if port == 465:
+                context = ssl.create_default_context()
+                with smtplib.SMTP_SSL(smtp_server, port, context=context) as server:
+                    print("Sending Email")
+                    server.login(sender, pwd, initial_response_ok=True)
+                    message = MIMEMultipart()
+                    message['From'] = sender
+                    message['To'] = receiver if isinstance(receiver, str) else ','.join(receiver)
+                    message['Subject'] = subject
+                    message.attach(MIMEText(self.__getmaildata(), 'html'))
+                    text = message.as_string()
+                    server.sendmail(sender, receiver, text)
+                    server.quit()
+                    print("Email Sent Successfully")
+            elif port == 587:
+                context = ssl.create_default_context()
+                with smtplib.SMTP(smtp_server, port) as server:
+                    print("Sending Email")
+                    server.ehlo()
+                    server.starttls(context=context)
+                    server.ehlo()
+                    server.ehlo()
+                    server.login(sender, pwd, initial_response_ok=True)
+                    message = MIMEMultipart()
+                    message['From'] = sender
+                    message['To'] = receiver if isinstance(receiver, str) else ','.join(receiver)
+                    message['Subject'] = subject
+                    message.attach(MIMEText(self.__getmaildata(), 'html'))
+                    text = message.as_string()
+                    server.ehlo()
+                    server.sendmail(sender, receiver, text)
+                    server.quit()
+                    print("Email Sent Successfully")
         except Exception as e:
             print("Error: ", e)
 
     def __getmaildata(self):
         return self.__mail_data
 
-    def __getrawdata(self):
-        return self.__m_row
+    def __getrawdata(self, IsAll=True):
+        if IsAll:
+            return self.__m_row
+        else:
+            import csv
+            mycsv = self.__m_row[1:]
+            # filter the data based on the condition
+            # skip the header row
+            filtered = [row for row in mycsv if row[3] == 'Inactive' or int(row[4]) in range(0, 14)]
+            # reset the s.no column
+            for i in range(len(filtered)):
+                filtered[i][0] = i + 1
+            # add the header row
+            filtered.insert(0, self.__m_row[0])
+            return filtered
 
-    def print_report(self):
+    def print_report(self, IsAll=True):
         headers = self.__getrawdata()[0]
-        data = self.__getrawdata()[1:]
+        data = self.__getrawdata(IsAll)[1:]
         if not data:
             print("No data to display.")
             return
 
         column_widths = self.__get_column_widths(data, headers)
         print("\n")
         width = self.__print_separator(column_widths)
@@ -193,26 +232,26 @@
 
         for row in data:
             for i, item in enumerate(row):
                 column_widths[i] = max(column_widths[i], len(str(item)))
 
         return column_widths
 
-    def save_report(self, path, ftype='html'):
+    def save_report(self, path, file_type='html', IsAll=True):
 
-        path = path + "\\" + "report." + ftype
+        path = path + "\\" + "report." + file_type
 
-        if ftype == 'html':
+        if file_type == 'html':
             with open(path, 'w') as f:
-                f.write(self.__compose_email_with_table(self.__getrawdata()))
+                f.write(self.__compose_email_with_table(self.__getrawdata(IsAll)))
         else:
             import csv
             with open(path, 'w', newline='') as f:
                 writer = csv.writer(f)
-                writer.writerows(self.__m_row)
+                writer.writerows(self.__getrawdata(IsAll))
         print("Report Saved to {}".format(path))
 
 
 class from_link:
     def __init__(self, domain):
         self.__domain = self.__domain_finder(domain)
         self.__verified = self.__IsInternetAvailable()
```

