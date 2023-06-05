# Comparing `tmp/remindmail-2023.5.8.1.tar.gz` & `tmp/remindmail-2023.6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.5.8.1.tar", last modified: Mon May  8 18:42:02 2023, max compression
+gzip compressed data, was "remindmail-2023.6.4.1.tar", last modified: Mon Jun  5 04:52:30 2023, max compression
```

## Comparing `remindmail-2023.5.8.1.tar` & `remindmail-2023.6.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.5.8.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.5.8.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.5.8.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.048849 remindmail-2023.5.8.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25030 2023-05-03 20:03:29.000000 remindmail-2023.5.8.1/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     8342 2023-05-08 18:33:48.000000 remindmail-2023.5.8.1/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.6.4.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13624 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13275 2023-06-05 04:37:46.000000 remindmail-2023.6.4.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.6.4.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.6.4.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4199 2023-06-05 04:48:55.000000 remindmail-2023.6.4.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.6.4.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    25417 2023-06-05 03:58:58.000000 remindmail-2023.6.4.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11473 2023-06-05 04:33:46.000000 remindmail-2023.6.4.1/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:52:30.779745 remindmail-2023.6.4.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13624 2023-06-05 04:52:30.000000 remindmail-2023.6.4.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-06-05 04:52:30.000000 remindmail-2023.6.4.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-05 04:52:30.000000 remindmail-2023.6.4.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-06-05 04:52:30.000000 remindmail-2023.6.4.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-06-05 04:52:30.000000 remindmail-2023.6.4.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.5.8.1/LICENSE.md` & `remindmail-2023.6.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.8.1/PKG-INFO` & `remindmail-2023.6.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-Metadata-Version: 2.1
-Name: remindmail
-Version: 2023.5.8.1
-Summary: Easily schedule reminders to be emailed
-Home-page: https://github.com/tylerjwoodfin/remindmail
-Author: Tyler Woodfin
-Author-email: feedback@tyler.cloud
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
 - schedule one-time or recurring reminders
+- create issues for your Jira board
 - schedule commands (your crontab can't run every 2 weeks as easily!)
 
 # notable dependencies
 
 - use `pip install -r requirements.md` to install all dependencies
 - Linux (Raspberry Pis work great!)
 - [cabinet](https://pypi.org/project/cabinet/)
@@ -82,16 +71,19 @@
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
+- `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
+- `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
+- `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
@@ -288,7 +280,42 @@
 
 - see [offset](##offset)
 
 ## using "d" to set one-time reminders
 
 - an item with `]d`, such as `[D%5]d`, will add the reminder and remove it from remind.md, meaning it will only generate once until you add it again.
   - this is useful for scheduling a reminder in the future that you don't need to repeat.
+
+# Jira Integration
+
+RemindMail provides a barebones integration with Jira to create issues directly from the application. To enable this integration, you need to configure the required Jira settings in the Cabinet configuration file.
+
+## configuration
+
+Before using the Jira integration, ensure that you have the following information available:
+
+- Jira project URL: The base URL of your Jira project.
+- Jira email: The email associated with your Jira account.
+- Jira API token: The API token generated for your Jira account.
+  - obtain through [these instructions](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/)
+- Jira project key: The key of the Jira project where you want to create issues.
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the values by running:
+
+```
+cabinet --put jira email <your Jira email>
+cabinet --put jira project-url <your project url, e.g. https://username.atlassian.net>
+cabinet --put jira project-key <your project key prefix that all issues have, e.g. USR>
+cabinet --put keys jira <your Jira API token>
+```
+
+Make sure to replace values in brackets with your own values.
+
+## Usage
+
+```
+# creates a ticket directly with no confirmation
+remind -m this is a new ticket --jira
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```

### Comparing `remindmail-2023.5.8.1/README.md` & `remindmail-2023.6.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,28 @@
+Metadata-Version: 2.1
+Name: remindmail
+Version: 2023.6.4.1
+Summary: Easily schedule reminders to be emailed
+Home-page: https://github.com/tylerjwoodfin/remindmail
+Author: Tyler Woodfin
+Author-email: feedback@tyler.cloud
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
 - schedule one-time or recurring reminders
+- create issues for your Jira board
 - schedule commands (your crontab can't run every 2 weeks as easily!)
 
 # notable dependencies
 
 - use `pip install -r requirements.md` to install all dependencies
 - Linux (Raspberry Pis work great!)
 - [cabinet](https://pypi.org/project/cabinet/)
@@ -70,16 +83,19 @@
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
+- `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
+- `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
+- `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
@@ -276,7 +292,42 @@
 
 - see [offset](##offset)
 
 ## using "d" to set one-time reminders
 
 - an item with `]d`, such as `[D%5]d`, will add the reminder and remove it from remind.md, meaning it will only generate once until you add it again.
   - this is useful for scheduling a reminder in the future that you don't need to repeat.
+
+# Jira Integration
+
+RemindMail provides a barebones integration with Jira to create issues directly from the application. To enable this integration, you need to configure the required Jira settings in the Cabinet configuration file.
+
+## configuration
+
+Before using the Jira integration, ensure that you have the following information available:
+
+- Jira project URL: The base URL of your Jira project.
+- Jira email: The email associated with your Jira account.
+- Jira API token: The API token generated for your Jira account.
+  - obtain through [these instructions](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/)
+- Jira project key: The key of the Jira project where you want to create issues.
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the values by running:
+
+```
+cabinet --put jira email <your Jira email>
+cabinet --put jira project-url <your project url, e.g. https://username.atlassian.net>
+cabinet --put jira project-key <your project key prefix that all issues have, e.g. USR>
+cabinet --put keys jira <your Jira API token>
+```
+
+Make sure to replace values in brackets with your own values.
+
+## Usage
+
+```
+# creates a ticket directly with no confirmation
+remind -m this is a new ticket --jira
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```

### Comparing `remindmail-2023.5.8.1/setup.cfg` & `remindmail-2023.6.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.05.08.1
+version = 2023.06.04.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.5.8.1/src/remind/__main__.py` & `remindmail-2023.6.4.1/src/remind/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 The main entrypoint
 """
 
 from pathlib import Path
 import sys
 import argparse
+from remind.remindmail_utils import RemindMailUtils  # pylint: disable=wrong-import-position
+from remind.remindmail import RemindMail  # pylint: disable=wrong-import-position
 sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from remind.remindmail import RemindMail #pylint: disable=wrong-import-position
-from remind.remindmail_utils import RemindMailUtils #pylint: disable=wrong-import-position
+
 
 def main():
     """
     Parses command line arguments and performs the appropriate action based on the arguments passed.
     """
 
     help_offset = """Calculates the offset for a certain date (today by default)
@@ -26,48 +27,63 @@
 
     parser = argparse.ArgumentParser()
 
     parser.add_argument('-m', '--message', nargs='?',
                         const='', help='Specify reminder message')
     parser.add_argument('-d', '--date', nargs='?', const='',
                         help='Specify reminder date')
+    parser.add_argument('-n', '--notes', action='store_true',
+                        help='Notes for the body of the email (or description of Jira task)')
     parser.add_argument('-ls', '-l', '--list', action='store_true',
                         help='List all reminders')
     parser.add_argument('-g', '--generate', action='store_true',
                         help='Generate reminders. By default, only generates every 12 hours.')
     parser.add_argument('--force', action='store_true',
                         help='Force reminders to be generated. Only used with -g.')
     parser.add_argument('--noconfirm', action='store_true',
                         help='Skip the confirmation before a reminder is scheduled/sent.')
     parser.add_argument('--dry-run', action='store_true',
                         help='Print generated reminders without sending them. Only used with -g.')
     parser.add_argument('--later', action='store_true',
                         help='Mail reminders for later')
+    parser.add_argument('--stats', action='store_true',
+                        help='Prints RemindMail usage statistics')
     parser.add_argument('-o', '--offset', nargs='?',
                         help=help_offset)
     parser.add_argument('-e', '--edit', action='store_true',
                         help='Edits remind.md through the terminal')
     parser.add_argument('--show-tomorrow', action='store_true',
                         help='Shows a list of reminders scheduled for tomorrow')
+    parser.add_argument('--sent-today', action='store_true',
+                        help='Prints the sum of reminders sent today (yesterday, if before 4AM)')
     parser.add_argument('manual_reminder_args', nargs='*')
+    parser.add_argument('-j', '--jira', action='store_true',
+                        help='Creates an issue through Jira rather than using email.')
 
     args = parser.parse_args()
 
     if args.list:
         RemindMailUtils().print_reminders_file()
     elif args.generate:
         RemindMail().generate(force=args.force, dry_run=args.dry_run)
     elif args.later:
         RemindMailUtils().mail_reminders_for_later()
+    elif args.stats:
+        RemindMailUtils().print_stats()
     elif args.offset is not None:
         RemindMailUtils().offset(args.offset.split(" "))
     elif args.edit:
         RemindMailUtils().edit_reminders_file()
     elif args.show_tomorrow:
         RemindMail().show_tomorrow()
+    elif args.sent_today:
+        print(RemindMailUtils().get_sent_today())
+    elif args.jira:
+        RemindMailUtils().create_jira_issue(
+            args.message or ' '.join(args.manual_reminder_args), args.notes or '')
     elif args.manual_reminder_args:
         RemindMail().parse_query(query=' '.join(args.manual_reminder_args),
                                  noconfirm=args.noconfirm)
     else:
         RemindMail().manual_reminder(manual_message=args.message or '',
                                      manual_date=args.date or '', noconfirm=args.noconfirm)
```

### Comparing `remindmail-2023.5.8.1/src/remind/reminder.py` & `remindmail-2023.6.4.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.8.1/src/remind/remindmail.py` & `remindmail-2023.6.4.1/src/remind/remindmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,16 +511,25 @@
 
         response = ''
         query = strip_to(query.strip())
 
         if manual_message:
             query = manual_message
 
-        while response not in ['y', 'n', 'r', 'l', 'm']:
-            options = "(y)es\n(n)o\n(p)arse entire query\n(r)eport\n(l)ater\n(t)omorrow\n(m)anual"
+        while response not in ['y', 'n', 'r', 'l', 't', 'j', 'm']:
+            options = (
+                "(y)es\n"
+                "(n)o\n"
+                "(p)arse entire query\n"
+                "(r)eport\n"
+                "(l)ater\n"
+                "(t)omorrow\n"
+                "(j)ira\n"
+                "(m)anual"
+            )
 
             query_time_formatted = query_time_formatted or 'right now'
 
             if not noconfirm:
                 prompt = (f"""\nYour reminder for {query_time_formatted}:"""
                           f"\n{query}\n{query_notes_formatted or ''}\nOK?\n\n{options}\n\n")
                 RemindMailUtils.query_trace.append(prompt)
@@ -551,14 +560,19 @@
             elif response == 't':
                 days = ["Monday", "Tuesday", "Wednesday",
                         "Thursday", "Friday", "Saturday", "Sunday"]
                 weekday = days[(datetime.now() + timedelta(days=1)).weekday()]
                 RemindMail().manual_reminder(query, weekday)
                 return
 
+            elif response == 'j':
+                print("Creating Jira issue...")
+                RemindMailUtils().create_jira_issue(summary=query, description=query_notes or '')
+                return
+
         # send immediate reminders
         if query_time_formatted == 'right now' and response == 'y':
             RemindMailUtils().send_email(query.strip(), query_notes, False, is_quiet=True)
             return
 
         # scheduled reminders
         if query_time_token:
```

### Comparing `remindmail-2023.5.8.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.6.4.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.5.8.1
+Version: 2023.6.4.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
 - schedule one-time or recurring reminders
+- create issues for your Jira board
 - schedule commands (your crontab can't run every 2 weeks as easily!)
 
 # notable dependencies
 
 - use `pip install -r requirements.md` to install all dependencies
 - Linux (Raspberry Pis work great!)
 - [cabinet](https://pypi.org/project/cabinet/)
@@ -82,16 +83,19 @@
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
+- `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
+- `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
+- `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
@@ -288,7 +292,42 @@
 
 - see [offset](##offset)
 
 ## using "d" to set one-time reminders
 
 - an item with `]d`, such as `[D%5]d`, will add the reminder and remove it from remind.md, meaning it will only generate once until you add it again.
   - this is useful for scheduling a reminder in the future that you don't need to repeat.
+
+# Jira Integration
+
+RemindMail provides a barebones integration with Jira to create issues directly from the application. To enable this integration, you need to configure the required Jira settings in the Cabinet configuration file.
+
+## configuration
+
+Before using the Jira integration, ensure that you have the following information available:
+
+- Jira project URL: The base URL of your Jira project.
+- Jira email: The email associated with your Jira account.
+- Jira API token: The API token generated for your Jira account.
+  - obtain through [these instructions](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/)
+- Jira project key: The key of the Jira project where you want to create issues.
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the values by running:
+
+```
+cabinet --put jira email <your Jira email>
+cabinet --put jira project-url <your project url, e.g. https://username.atlassian.net>
+cabinet --put jira project-key <your project key prefix that all issues have, e.g. USR>
+cabinet --put keys jira <your Jira API token>
+```
+
+Make sure to replace values in brackets with your own values.
+
+## Usage
+
+```
+# creates a ticket directly with no confirmation
+remind -m this is a new ticket --jira
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```

