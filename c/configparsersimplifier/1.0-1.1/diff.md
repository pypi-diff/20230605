# Comparing `tmp/configparsersimplifier-1.0.tar.gz` & `tmp/configparsersimplifier-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configparsersimplifier-1.0.tar", last modified: Sat Jun  3 16:45:33 2023, max compression
+gzip compressed data, was "configparsersimplifier-1.1.tar", last modified: Mon Jun  5 13:03:36 2023, max compression
```

## Comparing `configparsersimplifier-1.0.tar` & `configparsersimplifier-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 16:45:33.292458 configparsersimplifier-1.0/
--rw-rw-rw-   0        0        0      173 2023-06-03 16:45:33.292458 configparsersimplifier-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 16:45:33.283464 configparsersimplifier-1.0/configparsersimplifier/
--rw-rw-rw-   0        0        0       54 2023-06-03 16:45:07.000000 configparsersimplifier-1.0/configparsersimplifier/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-06-03 16:37:59.000000 configparsersimplifier-1.0/configparsersimplifier/configparsersimplifier.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:45:33.290459 configparsersimplifier-1.0/configparsersimplifier.egg-info/
--rw-rw-rw-   0        0        0      173 2023-06-03 16:45:33.000000 configparsersimplifier-1.0/configparsersimplifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-06-03 16:45:33.000000 configparsersimplifier-1.0/configparsersimplifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 16:45:33.000000 configparsersimplifier-1.0/configparsersimplifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-03 16:45:33.000000 configparsersimplifier-1.0/configparsersimplifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 16:45:33.293457 configparsersimplifier-1.0/setup.cfg
--rw-rw-rw-   0        0        0      224 2023-06-03 16:43:47.000000 configparsersimplifier-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.561881 configparsersimplifier-1.1/
+-rw-rw-rw-   0        0        0      173 2023-06-05 13:03:36.561881 configparsersimplifier-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.552888 configparsersimplifier-1.1/configparsersimplifier/
+-rw-rw-rw-   0        0        0       54 2023-06-03 16:45:07.000000 configparsersimplifier-1.1/configparsersimplifier/__init__.py
+-rw-rw-rw-   0        0        0     1946 2023-06-05 13:02:59.000000 configparsersimplifier-1.1/configparsersimplifier/configparsersimplifier.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:03:36.560882 configparsersimplifier-1.1/configparsersimplifier.egg-info/
+-rw-rw-rw-   0        0        0      173 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-05 13:03:36.000000 configparsersimplifier-1.1/configparsersimplifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 13:03:36.563881 configparsersimplifier-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      224 2023-06-05 13:03:24.000000 configparsersimplifier-1.1/setup.py
```

### Comparing `configparsersimplifier-1.0/configparsersimplifier/configparsersimplifier.py` & `configparsersimplifier-1.1/configparsersimplifier/configparsersimplifier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,57 @@
 from configparser import ConfigParser
 
 class ConfigParserSimple:
     def __init__(self, config_path):
-        self.cpath = config_path
+        self.cpath = r'{}'.format(config_path)
         self.config = ConfigParser()
     
-    def apply_changes(self):
+    def add_section(self, section: str):
         '''
-        Записывает изменения в файл.
+        Добавляет секцию в файл.
         '''
-        with open(r'{}'.format(self.cpath), 'w') as config_file:
-            self.config.write(config_file)
+        self.config.add_section(section)
     
-    def create_config(self, section: str, **pairs):
+    def set_keys(self, section: str, **pairs):
         '''
-        Создает .ini файл.
+        Позволяет записать в файл сразу несколько пар ключ=значение.
         '''
-        self.config.add_section(section)
         for k, v in pairs.items():
-            self.config.set(section, k, v)
+            self.config.set(section, str(k), str(v))
         
-        self.apply_changes()
-    
-    def read_dict(self, settings: dict):
-        '''
-        Читает настройки из файла.
-        '''
-        self.config.read_dict(settings)
+        with open(self.cpath, 'w') as config_file:
+            self.config.write(config_file)
     
     def get_keys(self, section: str, keys: list):
         '''
-        Возвращает список значений ключей
+        Позволяет получить из файла сразу несколько пар ключ=значение.
         '''
         values = list()
-        self.config.read(self.cpath)
         for key in keys:
             values.append(f'{self.config.get(section, key)}')
 
         return values
     
     def get_sections(self):
         '''
         Возвращает список существующих секций.
         '''
-        self.config.read(self.cpath)
         return self.config.sections()
     
-    
-    def set_keys(self, section: str, **pairs):
-        '''
-        Устанавливает значение ключам.
-        '''
-        self.config.read(self.cpath)
-        for k, v in pairs.items():
-            self.config.set(section, k, v)
-        
-        self.apply_changes()
-    
     def delete_keys(self, section: str, keys: list):
         '''
-        Удаляет ключи.
+        Позволяет удалить из файла сразу несколько пар ключ=значение.
         '''
-        self.config.read(self.cpath)
         for key in keys:
             self.config.remove_option(section, key)
+        
+        with open(self.cpath, 'w') as config_file:
+            self.config.write(config_file)
     
     def delete_section(self, section: str):
         '''
         Удаляет секцию.
         '''
-        self.config.read(self.cpath)
-        self.config.remove_section(section)
+        self.config.remove_section(section)
+        
+        with open(self.cpath, 'w') as config_file:
+            self.config.write(config_file)
```

