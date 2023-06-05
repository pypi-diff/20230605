# Comparing `tmp/pypipr-0.1.94.tar.gz` & `tmp/pypipr-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.94.tar", max compression
+gzip compressed data, was "pypipr-0.1.95.tar", max compression
```

## Comparing `pypipr-0.1.94.tar` & `pypipr-0.1.95.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.94/pypipr/__init__.py
--rw-r--r--   0        0        0    34991 2023-05-18 03:26:00.742616 pypipr-0.1.94/pypipr/pypipr.py
--rw-r--r--   0        0        0      615 2023-05-18 03:26:50.438771 pypipr-0.1.94/pyproject.toml
--rw-r--r--   0        0        0    15380 2023-05-18 03:26:04.004382 pypipr-0.1.94/README.md
--rw-r--r--   0        0        0    16296 1970-01-01 00:00:00.000000 pypipr-0.1.94/setup.py
--rw-r--r--   0        0        0    15172 1970-01-01 00:00:00.000000 pypipr-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.95/pypipr/__init__.py
+-rw-r--r--   0        0        0    35790 2023-05-18 05:33:43.263472 pypipr-0.1.95/pypipr/pypipr.py
+-rw-r--r--   0        0        0      631 2023-05-18 07:58:10.393265 pypipr-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0    15948 2023-05-18 07:55:46.464798 pypipr-0.1.95/README.md
+-rw-r--r--   0        0        0    16885 1970-01-01 00:00:00.000000 pypipr-0.1.95/setup.py
+-rw-r--r--   0        0        0    15743 1970-01-01 00:00:00.000000 pypipr-0.1.95/PKG-INFO
```

### Comparing `pypipr-0.1.94/pypipr/pypipr.py` & `pypipr-0.1.95/pypipr/pypipr.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 
 """PYPI Module"""
 import colorama
 import lxml.html
 import requests
 import yaml
+import pint
 
 if LINUX:
     import getch as _getch
 
 
 colorama.init()
 
@@ -76,14 +77,17 @@
 # is_empty()
 __is_empty__empty_list__ = [None, False, 0, -0]
 __is_empty__empty_list__ += ["0", "", "-0", "\n", "\t"]
 __is_empty__empty_list__ += [set(), dict(), list(), tuple()]
 # batchmaker()
 __batchmaker__regex_pattern__ = r"\{([0-9a-zA-Z]+)\-([0-9a-zA-Z]+)(?:\-(\d+))?\}"
 __batchmaker__regex_compile__ = re.compile(__batchmaker__regex_pattern__)
+# calculate()
+__calculate__ureg__ = pint.UnitRegistry()
+__calculate__Quantity__ = __calculate__ureg__.Quantity
 
 
 class generator:
     """
     Class ini menyediakan beberapa fungsi yang bisa mengembalikan generator.
     Digunakan untuk mengoptimalkan program.
 
@@ -1264,15 +1268,18 @@
         return value
     if isinstance(value, (int, float)):
         return str(value)
     if isinstance(value, bool):
         return "1" if value else "0"
     if is_empty(value):
         return ""
-    raise Exception(f"Tipe data {value} tidak diketahui")
+    try:
+        return str(value)
+    except:
+        raise Exception(f"Tipe data {value} tidak diketahui")
 
 
 def is_empty(variable, empty=__is_empty__empty_list__):
     """
     Mengecek apakah variable setara dengan nilai kosong pada empty.
 
     Pengecekan nilai yang setara menggunakan simbol '==', sedangkan untuk
@@ -1304,7 +1311,32 @@
     """
     if include_separator:
         separator = f"({separator})"
 
     result = re.split(separator, text, flags=re.IGNORECASE | re.MULTILINE)
 
     return result
+
+
+def calculate(teks):
+    """
+    Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
+    Mendukung perhitungan matematika dasar dengan satuan.
+
+    Return value:
+    - Berupa class Quantity dari modul pint
+
+    Format:
+    - f"{fx:~P}"            -> pretty
+    - f"{fx:~H}"            -> html
+    - fx.to_base_units()    -> SI
+    - fx.to_compact()       -> human readable
+
+    ```python
+    fx = "3 meter * 10 cm * 3 km"
+    res = calculate(fx)
+    print(res)
+    print(res.to_base_units())
+    print(res.to_compact())
+    ```
+    """
+    return __calculate__Quantity__(teks)
```

### Comparing `pypipr-0.1.94/pyproject.toml` & `pypipr-0.1.95/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "pypipr"
-version = "0.1.94"
+version = "0.1.95"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
 colorama = "*"
 lxml = "*"
 cssselect = "*"
 tzdata = "*"
 requests = "^2.30.0"
 pyyaml = "^6.0"
+pint = "^0.21"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^22.12.0", allow-prereleases = true}
```

### Comparing `pypipr-0.1.94/README.md` & `pypipr-0.1.95/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,40 @@
 ```python
 s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
 print(generator.batchmaker(s))
 print(batchmaker(s))
 ```
 
 
+## calculate
+
+`calculate`
+
+
+Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
+Mendukung perhitungan matematika dasar dengan satuan.
+
+Return value:
+- Berupa class Quantity dari modul pint
+
+Format:
+- f"{fx:~P}"            -> pretty
+- f"{fx:~H}"            -> html
+- fx.to_base_units()    -> SI
+- fx.to_compact()       -> human readable
+
+```python
+fx = "3 meter * 10 cm * 3 km"
+res = calculate(fx)
+print(res)
+print(res.to_base_units())
+print(res.to_compact())
+```
+
+
 ## chunck_array
 
 `chunck_array`
 
 
 Membagi array menjadi potongan-potongan dengan besaran yg diinginkan
 
@@ -814,14 +840,20 @@
 if __name__ == "__main__":
     print(ExampleRunParallel().run_asyncio())
     print(ExampleRunParallel().run_multi_threading())
     print(ExampleRunParallel().run_multi_processing())
 ```
 
 
+## __calculate__Quantity__
+
+`__calculate__Quantity__`
+
+
+
 ## generator
 
 `generator`
 
 
 Class ini menyediakan beberapa fungsi yang bisa mengembalikan generator.
 Digunakan untuk mengoptimalkan program.
```

### Comparing `pypipr-0.1.94/setup.py` & `pypipr-0.1.95/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['colorama',
  'cssselect',
  'lxml',
+ 'pint>=0.21,<0.22',
  'pyyaml>=6.0,<7.0',
  'requests>=2.30.0,<3.0.0',
  'tzdata']
 
 extras_require = \
 {':platform_system == "Linux"': ['getch']}
 
 setup_kwargs = {
     'name': 'pypipr',
-    'version': '0.1.94',
+    'version': '0.1.95',
     'description': 'The Python Package Index Project',
-    'long_description': '\n# About\nThe Python Package Index Project (pypipr)\n\npypi : https://pypi.org/project/pypipr\n\n\n# Setup\nInstall with pip\n```\npython -m pip install pypipr\n```\n\nImport with * for fastest access\n```python\nfrom pypipr.pypipr import *\n```\n\n# CONSTANT\n\n`LINUX`\n\n`WINDOWS`\n\n# FUNCTION\n\n## avg\n\n`avg`\n\n\nSimple Average Function karena tidak disediakan oleh python\n\n```python\nn = [1, 22, 2, 3, 13, 2, 123, 12, 31, 2, 2, 12, 2, 1]\nprint(avg(n))\n```\n\n\n## basename\n\n`basename`\n\n\nMengembalikan nama file dari path\n\n```python\nprint(basename("/ini/nama/folder/ke/file.py"))\n```\n\n\n## batchmaker\n\n`batchmaker`\n\n\nAlat Bantu untuk membuat teks yang berulang.\nGunakan {[start]-[finish][-[step]]}.\n```\n[start] dan [finish]    -> bisa berupa huruf maupun angka\n[-[step]]               -> bersifat optional\n```\n\n```python\ns = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."\nprint(generator.batchmaker(s))\nprint(batchmaker(s))\n```\n\n\n## chunck_array\n\n`chunck_array`\n\n\nMembagi array menjadi potongan-potongan dengan besaran yg diinginkan\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.chunck_array(array, 5))\nprint(chunck_array(array, 5))\n```\n\n\n## console_run\n\n`console_run`\n\n\nMenjalankan command seperti menjalankan command di Command Terminal\n\n```python\nconsole_run(\'dir\')\nconsole_run(\'ls\')\n```\n\n\n## create_folder\n\n`create_folder`\n\n\nMembuat folder.\nMembuat folder secara recursive dengan permission.\n\n```py\ncreate_folder("contoh_membuat_folder")\ncreate_folder("contoh/membuat/folder/recursive")\ncreate_folder("./contoh_membuat_folder/secara/recursive")\n```\n\n\n## datetime_from_string\n\n`datetime_from_string`\n\n\nParse iso_string menjadi datetime object\n\n```python\nprint(datetime_from_string("2022-12-12 15:40:13").isoformat())\nprint(datetime_from_string("2022-12-12 15:40:13", timezone="Asia/Jakarta").isoformat())\n```\n\n\n## datetime_now\n\n`datetime_now`\n\n\nMemudahkan dalam membuat Datetime untuk suatu timezone tertentu\n\n```python\nprint(datetime_now("Asia/Jakarta"))\nprint(datetime_now("GMT"))\nprint(datetime_now("Etc/GMT+7"))\n```\n\n\n## dict_first\n\n`dict_first`\n\n\nMengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple\n\n```python\nd = {\n    "key1": "value1",\n    "key2": "value2",\n    "key3": "value3",\n}\nprint(dict_first(d))\n```\n\n\n## dirname\n\n`dirname`\n\n\nMengembalikan nama folder dari path.\nTanpa trailing slash di akhir.\n\n```python\nprint(dirname("/ini/nama/folder/ke/file.py"))\n```\n\n\n## exit_if_empty\n\n`exit_if_empty`\n\n\nKeluar dari program apabila seluruh variabel\nsetara dengan empty\n\n```python\nvar1 = None\nvar2 = \'0\'\nexit_if_empty(var1, var2)\n```\n\n\n## explode\n\n`explode`\n\n\nMemecah text menjadi list berdasarkan separator.\n\n```python\nt = \'/ini/contoh/path/\'\nprint(explode(t, separator=\'/\'))\n```\n\n\n## file_get_contents\n\n`file_get_contents`\n\n\nMembaca seluruh isi file ke memory.\nApabila file tidak ada maka akan return None.\nApabila file ada tetapi kosong, maka akan return empty string\n\n```py\nprint(file_get_contents("ifile_test.txt"))\n```\n\n\n## file_put_contents\n\n`file_put_contents`\n\n\nMenuliskan content ke file.\nApabila file tidak ada maka file akan dibuat.\nApabila file sudah memiliki content maka akan di overwrite.\n\n```py\nfile_put_contents("ifile_test.txt", "Contoh menulis content")\n```\n\n\n## filter_empty\n\n`filter_empty`\n\n\n\n## get_class_method\n\n`get_class_method`\n\n\nMengembalikan berupa tuple yg berisi list dari method dalam class\n\n```python\nclass ExampleGetClassMethod:\n    def a():\n        return [x for x in range(10)]\n\n    def b():\n        return [x for x in range(10)]\n\n    def c():\n        return [x for x in range(10)]\n\n    def d():\n        return [x for x in range(10)]\n\nif __name__ == "__main__":\n    print(get_class_method(ExampleGetClassMethod))\n```\n\n\n## get_filemtime\n\n`get_filemtime`\n\n\nMengambil informasi last modification time file dalam nano seconds\n\n```python\nprint(get_filemtime(__file__))\n```\n\n\n## get_filesize\n\n`get_filesize`\n\n\nMengambil informasi file size dalam bytes\n\n```python\nprint(get_filesize(__file__))\n```\n\n\n## github_pull\n\n`github_pull`\n\n\nMenjalankan command `git pull`\n\n```py\ngithub_pull()\n```\n\n\n## github_push\n\n`github_push`\n\n\nMenjalankan command status, add, commit dan push\n\n```py\ngithub_push(\'Commit Message\')\n```\n\n\n## html_get_contents\n\n`html_get_contents`\n\n\nMengambil content html dari url.\n\nRETURN:\n- String: Apabila hanya url saja yg diberikan\n- List of etree: Apabila xpath diberikan\n- False: Apabila terjadi error\n\n```py\nprint(html_get_contents("https://arbadzukhron.deta.dev/"))\n```\n```python\n# Using XPATH\na = html_get_contents("https://www.google.com/", xpath="//a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get(\'href\'))\n\n# Using REGEX\na = html_get_contents("https://www.google.com/", regex=r"(<a.[^>]+>(?:(?:\\s+)?(.[^<]+)(?:\\s+)?)<\\/a>)")\nfor i in a:\n    print(i)\n\n# Using cssselect\na = html_get_contents("https://www.google.com/", css_select="a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get("href"))\n```\n\n\n## html_put_contents\n\n`html_put_contents`\n\n\nFungsi untuk mengirim data ke URL dengan method POST dan mengembalikan\nrespon dari server sebagai string.\n\nParameters:\n    url (str): URL tujuan.\n    data (dict): Data yang akan dikirim.\n\nReturns:\n- str: Respon dari server dalam bentuk string.\n\n```python\ndata = dict(pengirim="saya", penerima="kamu")\nprint(html_put_contents("https://arbadzukhron.deta.dev/", data))\n```\n\n\n## implode\n\n`implode`\n\n\nSimplify Python join functions like PHP function.\nIterable bisa berupa sets, tuple, list, dictionary.\n\n```python\narr = {\'asd\',\'dfs\',\'weq\',\'qweqw\'}\nprint(implode(arr, \', \'))\n\narr = \'/ini/path/seperti/url/\'.split(\'/\')\nprint(implode(arr, \',\'))\nprint(implode(arr, \',\', remove_empty=True))\n\narr = {\'a\':\'satu\', \'b\':(12, 34, 56), \'c\':\'tiga\', \'d\':\'empat\'}\nprint(implode(arr, separator=\'</li>\\n<li>\', start=\'<li>\', end=\'</li>\', recursive_flat=True))\nprint(implode(arr, separator=\'</div>\\n<div>\', start=\'<div>\', end=\'</div>\'))\nprint(implode(10, \' \'))\n```\n\n\n## input_char\n\n`input_char`\n\n\nMeminta masukan satu huruf tanpa menekan Enter.\n\n```py\ninput_char("Input char : ")\ninput_char("Input char : ", default=\'Y\')\ninput_char("Input Char without print : ", echo_char=False)\n```\n\n\n## irange\n\n`irange`\n\n\nImprove python range() function untuk pengulangan menggunakan huruf\n\n```python\nprint(generator.irange(\'a\', \'z\'))\nprint(irange(\'H\', \'a\'))\nprint(irange(\'1\', \'5\', 3))\nprint(irange(\'1\', 5, 3))\n# print(irange(\'a\', 5, 3))\nprint(irange(-10, 4, 3))\nprint(irange(1, 5))\n```\n\n\n## is_empty\n\n`is_empty`\n\n\nMengecek apakah variable setara dengan nilai kosong pada empty.\n\nPengecekan nilai yang setara menggunakan simbol \'==\', sedangkan untuk\npengecekan lokasi memory yang sama menggunakan keyword \'is\'\n\n```python\nprint(is_empty("teks"))\nprint(is_empty(True))\nprint(is_empty(False))\nprint(is_empty(None))\nprint(is_empty(0))\nprint(is_empty([]))\n```\n\n\n## is_iterable\n\n`is_iterable`\n\n\nMengecek apakah suatu variabel bisa dilakukan forloop atau tidak\n\n```python\ns = \'ini string\'\nprint(is_iterable(s))\n\nl = [12,21,2,1]\nprint(is_iterable(l))\n\nr = range(100)\nprint(is_iterable(r))\n\nd = {\'a\':1, \'b\':2}\nprint(is_iterable(d.values()))\n```\n\n\n## iscandir\n\n`iscandir`\n\n\nMempermudah scandir untuk mengumpulkan folder, subfolder dan file\n\n```py\nfor i in generator.iscandir():\n    print(i)\n\nfor i in iscandir():\n    print(i)\n```\n\n\n## log\n\n`log`\n\n\nDecorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.\nMelakukan print ke console untuk menginformasikan proses yg sedang berjalan didalam program.\n\n```python\n@log\ndef some_function():\n    pass\n\n@log()\ndef some_function_again():\n    pass\n\n@log("Calling some function")\ndef some_function_more():\n    pass\n\nif __name__ == "__main__":\n    some_function()\n    some_function_again()\n    some_function_more()\n```\n\n\n## print_colorize\n\n`print_colorize`\n\n\nPrint text dengan warna untuk menunjukan text penting\n\n```python\nprint_colorize("Print some text")\nprint_colorize("Print some text", color=colorama.Fore.RED)\n```\n\n\n## print_dir\n\n`print_dir`\n\n\nPrint property dan method yang tersedia pada variabel\n\n```python\np = pathlib.Path("c:/arba/dzukhron.dz")\nprint_dir(p)\n```\n\n\n## print_log\n\n`print_log`\n\n\nAkan melakukan print ke console.\nBerguna untuk memberikan informasi proses program yg sedang berjalan.\n\n```python\nprint_log("Standalone Log")\n```\n\n\n## random_bool\n\n`random_bool`\n\n\nMenghasilkan nilai random True atau False.\nFungsi ini merupakan fungsi tercepat untuk mendapatkan random bool.\n\n```python\nprint(random_bool())\n```\n\n\n## scan_file\n\n`scan_file`\n\n\nMengumpulkan nama-nama file dalam folder dan subfolder.\n\n```py\nfor i in generator.scan_file():\n    print(i)\n\nfor i in scan_file():\n    print(i)\n```\n\n\n## scan_folder\n\n`scan_folder`\n\n\nMengumpulkan nama-nama folder dan subfolder.\nTidak termasuk [".", ".."] dan file.\n\n```python\nfor i in generator.scan_folder(recursive=False):\n    print(i)\n\nfor i in scan_folder(recursive=False):\n    print(i)\n```\n\n\n## serialize\n\n`serialize`\n\n\nMengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.\nString yang dihasilkan berbentuk syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\nprint(serialize(data))\n```\n\n\n## set_timeout\n\n`set_timeout`\n\n\nMenjalankan fungsi ketika sudah sekian detik.\nApabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka\nprogram tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,\nkemudian program dihentikan.\n\n```python\nset_timeout(3, lambda: print("Timeout 3"))\nx = set_timeout(7, lambda: print("Timeout 7"))\nprint(x)\nprint("menghentikan timeout 7")\nx.cancel()\n```\n\n\n## sets_ordered\n\n`sets_ordered`\n\n\nHanya mengambil nilai unik dari suatu list\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.sets_ordered(array))\nprint(sets_ordered(array))\n```\n\n\n## strtr\n\n`strtr`\n\n\nSTRing TRanslate, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku disini mau kemana saja\'\nreplacements = {\n    "disini": "disitu",\n    "kemana": "kesini",\n}\nprint(strtr(text, replacements))\n```\n\n\n## strtr_regex\n\n`strtr_regex`\n\n\nSTRing TRanslate metode Regex, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku {{ ini }} mau ke {{ sini }} mau kemana saja\'\nreplacements = {\n    r"\\{\\{\\s*(ini)\\s*\\}\\}": r"itu dan \\1",\n    r"\\{\\{\\s*sini\\s*\\}\\}": r"situ",\n}\nprint(strtr_regex(text, replacements))\n```\n\n\n## to_str\n\n`to_str`\n\n\nMengubah value menjadi string literal\n\n```python\nprint(to_str(5))\nprint(to_str([]))\nprint(to_str(False))\nprint(to_str(True))\nprint(to_str(None))\n```\n\n\n## unserialize\n\n`unserialize`\n\n\nMengubah string data hasil dari serialize menjadi variabel.\nString data adalah berupa syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\ns = serialize(data)\nprint(unserialize(s))\n```\n\n\n# CLASS\n\n## ComparePerformance\n\n`ComparePerformance`\n\n\nMenjalankan seluruh method dalam class,\nkemudian membandingkan waktu yg diperlukan.\n\n```python\nclass ExampleComparePerformance(ComparePerformance):\n    # number = 1\n    z = 10\n\n    def a(self):\n        return (x for x in range(self.z))\n\n    def b(self):\n        return tuple(x for x in range(self.z))\n\n    def c(self):\n        return [x for x in range(self.z)]\n\n    def d(self):\n        return list(x for x in range(self.z))\n\nif __name__ == "__main__":\n    print(ExampleComparePerformance().compare_result())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n```\n\n\n## RunParallel\n\n`RunParallel`\n\n\nMenjalankan program secara bersamaan.\n\nStructure:\n- Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`\n- Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunaan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.\n- Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.\n- Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi\n\nNote:\n- `class RunParallel` didesain hanya untuk pemrosesan data saja.\n- Penggunaannya `class RunParallel` dengan cara membuat instance sub class beserta data yg akan diproses, kemudian panggil fungsi yg dipilih `run_asyncio / run_multi_threading / run_multi_processing`, kemudian dapatkan hasilnya.\n- `class RunParallel` tidak didesain untuk menyimpan data, karena setiap module terutama module `multiprocessing` tidak dapat mengakses data kelas dari proses yg berbeda.\n\n```python\nclass ExampleRunParallel(RunParallel):\n    z = "ini"\n\n    def __init__(self) -> None:\n        self.pop = random.randint(0, 100)\n\n    def _set_property_here(self, v):\n        self.prop = v\n\n    def a(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["a"] = "a"\n        q.put("from a 1")\n        q.put("from a 2")\n\n    def b(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["b"] = "b"\n        result["q_get"] = q.get()\n\n    def c(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["c"] = "c"\n        result["q_get"] = q.get()\n\n    async def d(self):\n        print("hello")\n        await asyncio.sleep(0)\n        print("hello")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["d"] = "d"\n        return result\n\n    async def e(self):\n        print("world")\n        await asyncio.sleep(0)\n        print("world")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["e"] = "e"\n        return result\n\nif __name__ == "__main__":\n    print(ExampleRunParallel().run_asyncio())\n    print(ExampleRunParallel().run_multi_threading())\n    print(ExampleRunParallel().run_multi_processing())\n```\n\n\n## generator\n\n`generator`\n\n\nClass ini menyediakan beberapa fungsi yang bisa mengembalikan generator.\nDigunakan untuk mengoptimalkan program.\n\nClass ini dibuat karena python generator yang disimpan dalam variabel\nhanya dapat diakses satu kali.\n\n',
+    'long_description': '\n# About\nThe Python Package Index Project (pypipr)\n\npypi : https://pypi.org/project/pypipr\n\n\n# Setup\nInstall with pip\n```\npython -m pip install pypipr\n```\n\nImport with * for fastest access\n```python\nfrom pypipr.pypipr import *\n```\n\n# CONSTANT\n\n`LINUX`\n\n`WINDOWS`\n\n# FUNCTION\n\n## avg\n\n`avg`\n\n\nSimple Average Function karena tidak disediakan oleh python\n\n```python\nn = [1, 22, 2, 3, 13, 2, 123, 12, 31, 2, 2, 12, 2, 1]\nprint(avg(n))\n```\n\n\n## basename\n\n`basename`\n\n\nMengembalikan nama file dari path\n\n```python\nprint(basename("/ini/nama/folder/ke/file.py"))\n```\n\n\n## batchmaker\n\n`batchmaker`\n\n\nAlat Bantu untuk membuat teks yang berulang.\nGunakan {[start]-[finish][-[step]]}.\n```\n[start] dan [finish]    -> bisa berupa huruf maupun angka\n[-[step]]               -> bersifat optional\n```\n\n```python\ns = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."\nprint(generator.batchmaker(s))\nprint(batchmaker(s))\n```\n\n\n## calculate\n\n`calculate`\n\n\nMengembalikan hasil dari perhitungan teks menggunakan modul pint.\nMendukung perhitungan matematika dasar dengan satuan.\n\nReturn value:\n- Berupa class Quantity dari modul pint\n\nFormat:\n- f"{fx:~P}"            -> pretty\n- f"{fx:~H}"            -> html\n- fx.to_base_units()    -> SI\n- fx.to_compact()       -> human readable\n\n```python\nfx = "3 meter * 10 cm * 3 km"\nres = calculate(fx)\nprint(res)\nprint(res.to_base_units())\nprint(res.to_compact())\n```\n\n\n## chunck_array\n\n`chunck_array`\n\n\nMembagi array menjadi potongan-potongan dengan besaran yg diinginkan\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.chunck_array(array, 5))\nprint(chunck_array(array, 5))\n```\n\n\n## console_run\n\n`console_run`\n\n\nMenjalankan command seperti menjalankan command di Command Terminal\n\n```python\nconsole_run(\'dir\')\nconsole_run(\'ls\')\n```\n\n\n## create_folder\n\n`create_folder`\n\n\nMembuat folder.\nMembuat folder secara recursive dengan permission.\n\n```py\ncreate_folder("contoh_membuat_folder")\ncreate_folder("contoh/membuat/folder/recursive")\ncreate_folder("./contoh_membuat_folder/secara/recursive")\n```\n\n\n## datetime_from_string\n\n`datetime_from_string`\n\n\nParse iso_string menjadi datetime object\n\n```python\nprint(datetime_from_string("2022-12-12 15:40:13").isoformat())\nprint(datetime_from_string("2022-12-12 15:40:13", timezone="Asia/Jakarta").isoformat())\n```\n\n\n## datetime_now\n\n`datetime_now`\n\n\nMemudahkan dalam membuat Datetime untuk suatu timezone tertentu\n\n```python\nprint(datetime_now("Asia/Jakarta"))\nprint(datetime_now("GMT"))\nprint(datetime_now("Etc/GMT+7"))\n```\n\n\n## dict_first\n\n`dict_first`\n\n\nMengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple\n\n```python\nd = {\n    "key1": "value1",\n    "key2": "value2",\n    "key3": "value3",\n}\nprint(dict_first(d))\n```\n\n\n## dirname\n\n`dirname`\n\n\nMengembalikan nama folder dari path.\nTanpa trailing slash di akhir.\n\n```python\nprint(dirname("/ini/nama/folder/ke/file.py"))\n```\n\n\n## exit_if_empty\n\n`exit_if_empty`\n\n\nKeluar dari program apabila seluruh variabel\nsetara dengan empty\n\n```python\nvar1 = None\nvar2 = \'0\'\nexit_if_empty(var1, var2)\n```\n\n\n## explode\n\n`explode`\n\n\nMemecah text menjadi list berdasarkan separator.\n\n```python\nt = \'/ini/contoh/path/\'\nprint(explode(t, separator=\'/\'))\n```\n\n\n## file_get_contents\n\n`file_get_contents`\n\n\nMembaca seluruh isi file ke memory.\nApabila file tidak ada maka akan return None.\nApabila file ada tetapi kosong, maka akan return empty string\n\n```py\nprint(file_get_contents("ifile_test.txt"))\n```\n\n\n## file_put_contents\n\n`file_put_contents`\n\n\nMenuliskan content ke file.\nApabila file tidak ada maka file akan dibuat.\nApabila file sudah memiliki content maka akan di overwrite.\n\n```py\nfile_put_contents("ifile_test.txt", "Contoh menulis content")\n```\n\n\n## filter_empty\n\n`filter_empty`\n\n\n\n## get_class_method\n\n`get_class_method`\n\n\nMengembalikan berupa tuple yg berisi list dari method dalam class\n\n```python\nclass ExampleGetClassMethod:\n    def a():\n        return [x for x in range(10)]\n\n    def b():\n        return [x for x in range(10)]\n\n    def c():\n        return [x for x in range(10)]\n\n    def d():\n        return [x for x in range(10)]\n\nif __name__ == "__main__":\n    print(get_class_method(ExampleGetClassMethod))\n```\n\n\n## get_filemtime\n\n`get_filemtime`\n\n\nMengambil informasi last modification time file dalam nano seconds\n\n```python\nprint(get_filemtime(__file__))\n```\n\n\n## get_filesize\n\n`get_filesize`\n\n\nMengambil informasi file size dalam bytes\n\n```python\nprint(get_filesize(__file__))\n```\n\n\n## github_pull\n\n`github_pull`\n\n\nMenjalankan command `git pull`\n\n```py\ngithub_pull()\n```\n\n\n## github_push\n\n`github_push`\n\n\nMenjalankan command status, add, commit dan push\n\n```py\ngithub_push(\'Commit Message\')\n```\n\n\n## html_get_contents\n\n`html_get_contents`\n\n\nMengambil content html dari url.\n\nRETURN:\n- String: Apabila hanya url saja yg diberikan\n- List of etree: Apabila xpath diberikan\n- False: Apabila terjadi error\n\n```py\nprint(html_get_contents("https://arbadzukhron.deta.dev/"))\n```\n```python\n# Using XPATH\na = html_get_contents("https://www.google.com/", xpath="//a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get(\'href\'))\n\n# Using REGEX\na = html_get_contents("https://www.google.com/", regex=r"(<a.[^>]+>(?:(?:\\s+)?(.[^<]+)(?:\\s+)?)<\\/a>)")\nfor i in a:\n    print(i)\n\n# Using cssselect\na = html_get_contents("https://www.google.com/", css_select="a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get("href"))\n```\n\n\n## html_put_contents\n\n`html_put_contents`\n\n\nFungsi untuk mengirim data ke URL dengan method POST dan mengembalikan\nrespon dari server sebagai string.\n\nParameters:\n    url (str): URL tujuan.\n    data (dict): Data yang akan dikirim.\n\nReturns:\n- str: Respon dari server dalam bentuk string.\n\n```python\ndata = dict(pengirim="saya", penerima="kamu")\nprint(html_put_contents("https://arbadzukhron.deta.dev/", data))\n```\n\n\n## implode\n\n`implode`\n\n\nSimplify Python join functions like PHP function.\nIterable bisa berupa sets, tuple, list, dictionary.\n\n```python\narr = {\'asd\',\'dfs\',\'weq\',\'qweqw\'}\nprint(implode(arr, \', \'))\n\narr = \'/ini/path/seperti/url/\'.split(\'/\')\nprint(implode(arr, \',\'))\nprint(implode(arr, \',\', remove_empty=True))\n\narr = {\'a\':\'satu\', \'b\':(12, 34, 56), \'c\':\'tiga\', \'d\':\'empat\'}\nprint(implode(arr, separator=\'</li>\\n<li>\', start=\'<li>\', end=\'</li>\', recursive_flat=True))\nprint(implode(arr, separator=\'</div>\\n<div>\', start=\'<div>\', end=\'</div>\'))\nprint(implode(10, \' \'))\n```\n\n\n## input_char\n\n`input_char`\n\n\nMeminta masukan satu huruf tanpa menekan Enter.\n\n```py\ninput_char("Input char : ")\ninput_char("Input char : ", default=\'Y\')\ninput_char("Input Char without print : ", echo_char=False)\n```\n\n\n## irange\n\n`irange`\n\n\nImprove python range() function untuk pengulangan menggunakan huruf\n\n```python\nprint(generator.irange(\'a\', \'z\'))\nprint(irange(\'H\', \'a\'))\nprint(irange(\'1\', \'5\', 3))\nprint(irange(\'1\', 5, 3))\n# print(irange(\'a\', 5, 3))\nprint(irange(-10, 4, 3))\nprint(irange(1, 5))\n```\n\n\n## is_empty\n\n`is_empty`\n\n\nMengecek apakah variable setara dengan nilai kosong pada empty.\n\nPengecekan nilai yang setara menggunakan simbol \'==\', sedangkan untuk\npengecekan lokasi memory yang sama menggunakan keyword \'is\'\n\n```python\nprint(is_empty("teks"))\nprint(is_empty(True))\nprint(is_empty(False))\nprint(is_empty(None))\nprint(is_empty(0))\nprint(is_empty([]))\n```\n\n\n## is_iterable\n\n`is_iterable`\n\n\nMengecek apakah suatu variabel bisa dilakukan forloop atau tidak\n\n```python\ns = \'ini string\'\nprint(is_iterable(s))\n\nl = [12,21,2,1]\nprint(is_iterable(l))\n\nr = range(100)\nprint(is_iterable(r))\n\nd = {\'a\':1, \'b\':2}\nprint(is_iterable(d.values()))\n```\n\n\n## iscandir\n\n`iscandir`\n\n\nMempermudah scandir untuk mengumpulkan folder, subfolder dan file\n\n```py\nfor i in generator.iscandir():\n    print(i)\n\nfor i in iscandir():\n    print(i)\n```\n\n\n## log\n\n`log`\n\n\nDecorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.\nMelakukan print ke console untuk menginformasikan proses yg sedang berjalan didalam program.\n\n```python\n@log\ndef some_function():\n    pass\n\n@log()\ndef some_function_again():\n    pass\n\n@log("Calling some function")\ndef some_function_more():\n    pass\n\nif __name__ == "__main__":\n    some_function()\n    some_function_again()\n    some_function_more()\n```\n\n\n## print_colorize\n\n`print_colorize`\n\n\nPrint text dengan warna untuk menunjukan text penting\n\n```python\nprint_colorize("Print some text")\nprint_colorize("Print some text", color=colorama.Fore.RED)\n```\n\n\n## print_dir\n\n`print_dir`\n\n\nPrint property dan method yang tersedia pada variabel\n\n```python\np = pathlib.Path("c:/arba/dzukhron.dz")\nprint_dir(p)\n```\n\n\n## print_log\n\n`print_log`\n\n\nAkan melakukan print ke console.\nBerguna untuk memberikan informasi proses program yg sedang berjalan.\n\n```python\nprint_log("Standalone Log")\n```\n\n\n## random_bool\n\n`random_bool`\n\n\nMenghasilkan nilai random True atau False.\nFungsi ini merupakan fungsi tercepat untuk mendapatkan random bool.\n\n```python\nprint(random_bool())\n```\n\n\n## scan_file\n\n`scan_file`\n\n\nMengumpulkan nama-nama file dalam folder dan subfolder.\n\n```py\nfor i in generator.scan_file():\n    print(i)\n\nfor i in scan_file():\n    print(i)\n```\n\n\n## scan_folder\n\n`scan_folder`\n\n\nMengumpulkan nama-nama folder dan subfolder.\nTidak termasuk [".", ".."] dan file.\n\n```python\nfor i in generator.scan_folder(recursive=False):\n    print(i)\n\nfor i in scan_folder(recursive=False):\n    print(i)\n```\n\n\n## serialize\n\n`serialize`\n\n\nMengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.\nString yang dihasilkan berbentuk syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\nprint(serialize(data))\n```\n\n\n## set_timeout\n\n`set_timeout`\n\n\nMenjalankan fungsi ketika sudah sekian detik.\nApabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka\nprogram tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,\nkemudian program dihentikan.\n\n```python\nset_timeout(3, lambda: print("Timeout 3"))\nx = set_timeout(7, lambda: print("Timeout 7"))\nprint(x)\nprint("menghentikan timeout 7")\nx.cancel()\n```\n\n\n## sets_ordered\n\n`sets_ordered`\n\n\nHanya mengambil nilai unik dari suatu list\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.sets_ordered(array))\nprint(sets_ordered(array))\n```\n\n\n## strtr\n\n`strtr`\n\n\nSTRing TRanslate, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku disini mau kemana saja\'\nreplacements = {\n    "disini": "disitu",\n    "kemana": "kesini",\n}\nprint(strtr(text, replacements))\n```\n\n\n## strtr_regex\n\n`strtr_regex`\n\n\nSTRing TRanslate metode Regex, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku {{ ini }} mau ke {{ sini }} mau kemana saja\'\nreplacements = {\n    r"\\{\\{\\s*(ini)\\s*\\}\\}": r"itu dan \\1",\n    r"\\{\\{\\s*sini\\s*\\}\\}": r"situ",\n}\nprint(strtr_regex(text, replacements))\n```\n\n\n## to_str\n\n`to_str`\n\n\nMengubah value menjadi string literal\n\n```python\nprint(to_str(5))\nprint(to_str([]))\nprint(to_str(False))\nprint(to_str(True))\nprint(to_str(None))\n```\n\n\n## unserialize\n\n`unserialize`\n\n\nMengubah string data hasil dari serialize menjadi variabel.\nString data adalah berupa syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\ns = serialize(data)\nprint(unserialize(s))\n```\n\n\n# CLASS\n\n## ComparePerformance\n\n`ComparePerformance`\n\n\nMenjalankan seluruh method dalam class,\nkemudian membandingkan waktu yg diperlukan.\n\n```python\nclass ExampleComparePerformance(ComparePerformance):\n    # number = 1\n    z = 10\n\n    def a(self):\n        return (x for x in range(self.z))\n\n    def b(self):\n        return tuple(x for x in range(self.z))\n\n    def c(self):\n        return [x for x in range(self.z)]\n\n    def d(self):\n        return list(x for x in range(self.z))\n\nif __name__ == "__main__":\n    print(ExampleComparePerformance().compare_result())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n```\n\n\n## RunParallel\n\n`RunParallel`\n\n\nMenjalankan program secara bersamaan.\n\nStructure:\n- Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`\n- Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunaan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.\n- Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.\n- Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi\n\nNote:\n- `class RunParallel` didesain hanya untuk pemrosesan data saja.\n- Penggunaannya `class RunParallel` dengan cara membuat instance sub class beserta data yg akan diproses, kemudian panggil fungsi yg dipilih `run_asyncio / run_multi_threading / run_multi_processing`, kemudian dapatkan hasilnya.\n- `class RunParallel` tidak didesain untuk menyimpan data, karena setiap module terutama module `multiprocessing` tidak dapat mengakses data kelas dari proses yg berbeda.\n\n```python\nclass ExampleRunParallel(RunParallel):\n    z = "ini"\n\n    def __init__(self) -> None:\n        self.pop = random.randint(0, 100)\n\n    def _set_property_here(self, v):\n        self.prop = v\n\n    def a(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["a"] = "a"\n        q.put("from a 1")\n        q.put("from a 2")\n\n    def b(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["b"] = "b"\n        result["q_get"] = q.get()\n\n    def c(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["c"] = "c"\n        result["q_get"] = q.get()\n\n    async def d(self):\n        print("hello")\n        await asyncio.sleep(0)\n        print("hello")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["d"] = "d"\n        return result\n\n    async def e(self):\n        print("world")\n        await asyncio.sleep(0)\n        print("world")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["e"] = "e"\n        return result\n\nif __name__ == "__main__":\n    print(ExampleRunParallel().run_asyncio())\n    print(ExampleRunParallel().run_multi_threading())\n    print(ExampleRunParallel().run_multi_processing())\n```\n\n\n## __calculate__Quantity__\n\n`__calculate__Quantity__`\n\n\n\n## generator\n\n`generator`\n\n\nClass ini menyediakan beberapa fungsi yang bisa mengembalikan generator.\nDigunakan untuk mengoptimalkan program.\n\nClass ini dibuat karena python generator yang disimpan dalam variabel\nhanya dapat diakses satu kali.\n\n',
     'author': 'ufiapjj',
     'author_email': 'ufiapjj@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pypipr-0.1.94/PKG-INFO` & `pypipr-0.1.95/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 0.1.94
+Version: 0.1.95
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama
 Requires-Dist: cssselect
 Requires-Dist: getch; platform_system == "Linux"
 Requires-Dist: lxml
+Requires-Dist: pint (>=0.21,<0.22)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: tzdata
 Description-Content-Type: text/markdown
 
 
 # About
@@ -84,14 +85,40 @@
 ```python
 s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
 print(generator.batchmaker(s))
 print(batchmaker(s))
 ```
 
 
+## calculate
+
+`calculate`
+
+
+Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
+Mendukung perhitungan matematika dasar dengan satuan.
+
+Return value:
+- Berupa class Quantity dari modul pint
+
+Format:
+- f"{fx:~P}"            -> pretty
+- f"{fx:~H}"            -> html
+- fx.to_base_units()    -> SI
+- fx.to_compact()       -> human readable
+
+```python
+fx = "3 meter * 10 cm * 3 km"
+res = calculate(fx)
+print(res)
+print(res.to_base_units())
+print(res.to_compact())
+```
+
+
 ## chunck_array
 
 `chunck_array`
 
 
 Membagi array menjadi potongan-potongan dengan besaran yg diinginkan
 
@@ -834,14 +861,20 @@
 if __name__ == "__main__":
     print(ExampleRunParallel().run_asyncio())
     print(ExampleRunParallel().run_multi_threading())
     print(ExampleRunParallel().run_multi_processing())
 ```
 
 
+## __calculate__Quantity__
+
+`__calculate__Quantity__`
+
+
+
 ## generator
 
 `generator`
 
 
 Class ini menyediakan beberapa fungsi yang bisa mengembalikan generator.
 Digunakan untuk mengoptimalkan program.
```

