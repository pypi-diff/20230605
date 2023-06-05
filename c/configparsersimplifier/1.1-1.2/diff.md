# Comparing `tmp/configparsersimplifier-1.1.tar.gz` & `tmp/configparsersimplifier-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configparsersimplifier-1.1.tar", last modified: Mon Jun  5 13:03:36 2023, max compression
+gzip compressed data, was "configparsersimplifier-1.2.tar", last modified: Mon Jun  5 14:01:32 2023, max compression
```

## Comparing `configparsersimplifier-1.1.tar` & `configparsersimplifier-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.561881 configparsersimplifier-1.1/
--rw-rw-rw-   0        0        0      173 2023-06-05 13:03:36.561881 configparsersimplifier-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.552888 configparsersimplifier-1.1/configparsersimplifier/
--rw-rw-rw-   0        0        0       54 2023-06-03 16:45:07.000000 configparsersimplifier-1.1/configparsersimplifier/__init__.py
--rw-rw-rw-   0        0        0     1946 2023-06-05 13:02:59.000000 configparsersimplifier-1.1/configparsersimplifier/configparsersimplifier.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.560882 configparsersimplifier-1.1/configparsersimplifier.egg-info/
--rw-rw-rw-   0        0        0      173 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:03:36.563881 configparsersimplifier-1.1/setup.cfg
--rw-rw-rw-   0        0        0      224 2023-06-05 13:03:24.000000 configparsersimplifier-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:01:32.190632 configparsersimplifier-1.2/
+-rw-rw-rw-   0        0        0      173 2023-06-05 14:01:32.190632 configparsersimplifier-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 14:01:32.182638 configparsersimplifier-1.2/configparsersimplifier/
+-rw-rw-rw-   0        0        0       54 2023-06-03 16:45:07.000000 configparsersimplifier-1.2/configparsersimplifier/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-06-05 14:01:09.000000 configparsersimplifier-1.2/configparsersimplifier/configparsersimplifier.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:01:32.189632 configparsersimplifier-1.2/configparsersimplifier.egg-info/
+-rw-rw-rw-   0        0        0      173 2023-06-05 14:01:31.000000 configparsersimplifier-1.2/configparsersimplifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-06-05 14:01:31.000000 configparsersimplifier-1.2/configparsersimplifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:01:31.000000 configparsersimplifier-1.2/configparsersimplifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-05 14:01:31.000000 configparsersimplifier-1.2/configparsersimplifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:01:32.191631 configparsersimplifier-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      224 2023-06-05 14:01:17.000000 configparsersimplifier-1.2/setup.py
```

### Comparing `configparsersimplifier-1.1/configparsersimplifier/configparsersimplifier.py` & `configparsersimplifier-1.2/configparsersimplifier/configparsersimplifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from configparser import ConfigParser
 
 class ConfigParserSimple:
     def __init__(self, config_path):
         self.cpath = r'{}'.format(config_path)
         self.config = ConfigParser()
     
+    def reread(self):
+        self.config.read(self.cpath)
+    
     def add_section(self, section: str):
         '''
         Добавляет секцию в файл.
         '''
         self.config.add_section(section)
     
     def set_keys(self, section: str, **pairs):
@@ -21,37 +24,41 @@
         with open(self.cpath, 'w') as config_file:
             self.config.write(config_file)
     
     def get_keys(self, section: str, keys: list):
         '''
         Позволяет получить из файла сразу несколько пар ключ=значение.
         '''
+        self.reread()
         values = list()
         for key in keys:
             values.append(f'{self.config.get(section, key)}')
 
         return values
     
     def get_sections(self):
         '''
         Возвращает список существующих секций.
         '''
+        self.reread()
         return self.config.sections()
     
     def delete_keys(self, section: str, keys: list):
         '''
         Позволяет удалить из файла сразу несколько пар ключ=значение.
         '''
+        self.reread()
         for key in keys:
             self.config.remove_option(section, key)
         
         with open(self.cpath, 'w') as config_file:
             self.config.write(config_file)
     
     def delete_section(self, section: str):
         '''
         Удаляет секцию.
         '''
+        self.reread()
         self.config.remove_section(section)
         
         with open(self.cpath, 'w') as config_file:
             self.config.write(config_file)
```

