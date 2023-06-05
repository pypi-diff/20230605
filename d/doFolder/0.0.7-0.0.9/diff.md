# Comparing `tmp/doFolder-0.0.7.tar.gz` & `tmp/doFolder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.7.tar", last modified: Sun Jun  4 18:50:58 2023, max compression
+gzip compressed data, was "doFolder-0.0.9.tar", last modified: Mon Jun  5 04:37:22 2023, max compression
```

## Comparing `doFolder-0.0.7.tar` & `doFolder-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.707246 doFolder-0.0.7/
--rw-rw-rw-   0        0        0     3351 2023-06-04 18:50:58.707246 doFolder-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.698248 doFolder-0.0.7/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.7/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.7/doFolder/compare.py
--rw-rw-rw-   0        0        0    28190 2023-06-04 18:48:56.000000 doFolder-0.0.7/doFolder/main.py
--rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.7/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.706247 doFolder-0.0.7/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3351 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:50:58.708245 doFolder-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-06-04 18:50:47.000000 doFolder-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.826742 doFolder-0.0.9/
+-rw-rw-rw-   0        0        0     3351 2023-06-05 04:37:22.825742 doFolder-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.793743 doFolder-0.0.9/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.9/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.9/doFolder/compare.py
+-rw-rw-rw-   0        0        0    29519 2023-06-05 04:36:08.000000 doFolder-0.0.9/doFolder/main.py
+-rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.9/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.824742 doFolder-0.0.9/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3351 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 04:37:22.826742 doFolder-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-06-05 04:37:16.000000 doFolder-0.0.9/setup.py
```

### Comparing `doFolder-0.0.7/PKG-INFO` & `doFolder-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.7
+Version: 0.0.9
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.0.7/README.rst` & `doFolder-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.7/doFolder/__init__.py` & `doFolder-0.0.9/doFolder/__init__.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.7/doFolder/compare.py` & `doFolder-0.0.9/doFolder/compare.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.7/doFolder/main.py` & `doFolder-0.0.9/doFolder/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,15 +198,22 @@
         for i in other.partition:
             if not len(retsult) or retsult[0]!=i:
                 if error=="strict":
                     raise ValueError(f"\"{other}\" is not the ancestor folder of {self}")
                 return retsult
             del retsult[0]
         return retsult
-    
+    def getAbsolutePath(self,path)->"Path":
+        """
+        Returns the absolute path of a given file or directory by joining it with the current working directory.
+        :param path: A string representing the relative path to be joined with the current working directory.
+        :return: An object of type "Path" representing the absolute path obtained after joining.
+        :raise ValueError: If input argument 'path' is not a valid string.
+        """
+        return Path(os.path.join(self, path))
 class File(_HasName):
     """
     Represents a file on disk.
     ## Attributes:
         - path (Path): The path of the file.
         - parent (Folder or None): The parent folder of the file.
         - mode (int): The mode of the file.
@@ -351,43 +358,59 @@
         - search(self,condition:List[UnformattedMatching],aim:Literal["file","folder","both"]="both",threaded:bool=False,threads:Union[None,int]=None)
         Searches for files/folders in the current directory that match certain criteria.
         - createFile(self,path:Union[str,Path],content:bytes=b"")->Path
         Creates a new file at the specified location with optional content.
         - createFolder(self,path:Union[str,Path])->Path
         Creates a new sub-folder at the specified location.
     """
-    def __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None,scan:bool=False):
+    def __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None,scan:bool=False,ignores:Iterable[Union[str,Path]]=[],gitignore:bool=False):
         if type(path)!=Path:
             path=Path(path)
         self.onlisten=onlisten
         self.path=path
         self.parent=parent
         self.scaned=scan
         self.scan=scan
         self.logger=logging.getLogger(self.name)
         if self.onlisten:
             self.event_handler = _FolderUpdateHeader(self)
             self.observer = Observer()
             self.observer.schedule(self.event_handler, path=path, recursive=True)
             self.observer.start()
+        gitignores=[]
+        self.gitignore=gitignore
+        if gitignore:
+            try:
+                with open(path.add(".gitignore"),encoding="utf-8") as f:
+                    gitignores=[i[:-1] for i in set(f.readlines())]
+                    
+            except:
+                gitignores=[]
+        self.ignores:List[Path]=[]
+        for i in set(gitignores+list(ignores)):
+            if type(i)!=Path:
+                i=Path(path.getAbsolutePath(i))
+            self.ignores.append(i)
         if scan:
             self.refresh()
     def refresh(self):
         self.logger.debug("refresh folder contents")
         """Rebuild all of this folder object"""
         self.scaned=True
         self.dir:List[str]=os.listdir(self.path)
         self.files:FileList = FileList([])
         self.subfolder:FolderList=FolderList([])
         for i in self.dir:
             newPath=self.path.add(i)
+            if newPath in self.ignores:
+                continue
             if os.path.isfile(newPath):
-                self.files.append(File(newPath))
+                self.files.append(File(newPath,parent=self))
             elif os.path.isdir(newPath):
-                self.subfolder.append(Folder(newPath,parent=self,scan=self.scan))
+                self.subfolder.append(Folder(newPath,parent=self,scan=self.scan,ignores=self.ignores,gitignore=self.gitignore))
     @property
     def name(self)->str:
         return self.path.name
     def __str__(self)->str:
         return f"<Folder \"{self.name}\">"
     def __repr__(self) -> str:
         return self.__str__()
@@ -412,30 +435,30 @@
         if not self.scaned:
             return
         if len(path)>1:
             nextFolder=self[path[0]]
             if type(nextFolder)==Folder:
                 nextFolder._update(path[1:],eventType,eventTarget,isDirectory)
                 return
-            else:
+            elif self.path.add(path[0]) not in self.ignores:
                 raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain folder \"{path[0]}\"")
         self.logger.debug(f"file content update.{eventType}")
         name=path[0]
         if eventType==EVENT_TYPE_CREATED:
             if isDirectory:self.subfolder.append(Folder(eventTarget,parent=self))
             else:self.files.append(File(eventTarget,parent=self))
         if eventType==EVENT_TYPE_DELETED:
             target=self[name]
             if type(target)==Folder:self.subfolder.remove(target)
             elif type(target)==File:self.files.remove(target)
-            else:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain item \"{name}\"")
+            elif self.path.add(name) not in self.ignores:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain item \"{name}\"")
         if eventType==EVENT_TYPE_MODIFIED:
             target=self[name]
             if type(target)==File:target.refresh()
-            else:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contains file \"{name}\"")
+            elif self.path.add(name) not in self.ignores:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contains file \"{name}\"")
     def __getattribute__(self, name: str) -> Any:
         if not super().__getattribute__("scaned") and name in ["dir","files","subfolder"]:
             self.refresh()
         try:
             return super().__getattribute__(name)
         except AttributeError:
             target=self[name]
@@ -534,15 +557,15 @@
         :param condition: search conditions which is formatted
         :param aim: search type
         """
         for i in range(len(condition)):
             if aim!="folder":
                 for j in self.files:
                     if not condition[i][0](j):continue
-                    restCondition=copy.deepcopy(condition)
+                    restCondition=copy.deepcopy(condition[i:])
                     restCondition[0]=(restCondition[0][0],max(restCondition[0][1]-1,0),None if restCondition[0][2]==None else max(restCondition[0][2]-1,0))
                     k=i
                     while k<len(restCondition):
                         if restCondition[k][1]!=0:
                             break
                         k+=1
                     if (k==len(restCondition)):
@@ -568,29 +591,29 @@
         """
         Create a new file at the specified path with the given content.
         :param path: The path where the file will be created. Can be either a string or a Path object.
         :param content: The bytes to write into the newly created file. Default is an empty byte string.
         :return: A Path object representing the newly created file.
         :raise FileOrFolderAlreadyExists: If there is already a file or folder at the specified path.
         """
-        path=Path(os.path.join(self.path, path))
+        path=self.path.getAbsolutePath(path)
         if os.path.exists(path):
             raise FileOrFolderAlreadyExists(f"Can't create file {path} because it already exists")
         with open(path,"wb") as f:
             f.write(content)
         return path
     def createFolder(self,path:Union[str,Path],content:bytes=b"")->Path:
         """
         Create a new folder at the specified path.
         :param path: The path where the new folder will be created. Can be either a string or a Path object.
         :param content: Optional parameter specifying the initial content of the folder. Default is an empty bytes object.
         :return: Returns a Path object representing the newly created folder.
         :raise FileOrFolderAlreadyExists: If there is already a file or folder with the same name as `path`.
         """
-        path=Path(os.path.join(self.path, path))
+        path=self.path.getAbsolutePath(path)
         if os.path.exists(path):
             raise FileOrFolderAlreadyExists(f"Can't create folder {path} because it already exists")
         os.makedirs(path)
         return path
     def add(self,aim:Union["File","Folder"],move:bool=False):
         "add a file or folder to this folder"
         if move:
```

### Comparing `doFolder-0.0.7/doFolder/terminal.py` & `doFolder-0.0.9/doFolder/terminal.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.7/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.9/doFolder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.7
+Version: 0.0.9
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.0.7/setup.py` & `doFolder-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.7',
+    version = '0.0.9',
     keywords = ['file',"foler","path","filesystem"],
     description = 'Manage files more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

