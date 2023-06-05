# Comparing `tmp/cgpmgr-1.2.tar.gz` & `tmp/cgpmgr-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpmgr-1.2.tar", last modified: Sat Jul  2 12:22:18 2022, max compression
+gzip compressed data, was "cgpmgr-1.3.tar", last modified: Sat Jun  3 09:46:41 2023, max compression
```

## Comparing `cgpmgr-1.2.tar` & `cgpmgr-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-02 12:22:18.941439 cgpmgr-1.2/
--rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.2/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2022-07-02 12:22:18.941439 cgpmgr-1.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3085 2021-11-01 12:43:53.000000 cgpmgr-1.2/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-02 12:22:18.941439 cgpmgr-1.2/cgpmgr/
--rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.2/cgpmgr/__init__.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    30100 2022-07-02 12:20:46.000000 cgpmgr-1.2/cgpmgr/cli.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-02 12:22:18.941439 cgpmgr-1.2/cgpmgr.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2022-07-02 12:22:14.000000 cgpmgr-1.2/cgpmgr.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2022-07-02 12:22:18.000000 cgpmgr-1.2/cgpmgr.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-07-02 12:22:14.000000 cgpmgr-1.2/cgpmgr.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-07-02 12:22:16.000000 cgpmgr-1.2/cgpmgr.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       16 2022-07-02 12:22:17.000000 cgpmgr-1.2/cgpmgr.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2022-07-02 12:22:17.000000 cgpmgr-1.2/cgpmgr.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-07-02 12:22:18.941439 cgpmgr-1.2/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)      480 2022-07-02 12:20:46.000000 cgpmgr-1.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.556194 cgpmgr-1.3/
+-rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.3/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-03 09:46:41.546194 cgpmgr-1.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     3085 2021-11-01 12:43:53.000000 cgpmgr-1.3/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.516194 cgpmgr-1.3/cgpmgr/
+-rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.3/cgpmgr/__init__.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    30353 2023-06-03 09:42:53.000000 cgpmgr-1.3/cgpmgr/cli.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.546194 cgpmgr-1.3/cgpmgr.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-03 09:46:41.556194 cgpmgr-1.3/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-03 09:42:53.000000 cgpmgr-1.3/setup.py
```

### Comparing `cgpmgr-1.2/LICENSE` & `cgpmgr-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.2/README.md` & `cgpmgr-1.3/README.md`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.2/cgpmgr/cli.py` & `cgpmgr-1.3/cgpmgr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
-Raspberry Pi電源管理 拡張基板 RPZ-PowerMGR用コントロールツール
+Raspberry Pi/Jetson Nano電源管理 拡張基板 RPZ-PowerMGR用コントロールツール
 Indoor Corgi, https://www.indoorcorgielec.com
 GitHub: https://github.com/IndoorCorgi/cgpmgr
-Version 1.2
+Version 1.3
 
 必要環境:
-1) Raspberry Pi OS, Python3
+1) Raspberry Pi OS / Jetson Linux, Python3
 2) I2Cインターフェース
-  Raspberry PiでI2Cを有効にして下さい
+  Raspberry PiでI2Cを有効にする方法
   https://www.indoorcorgielec.com/resources/raspberry-pi/raspberry-pi-i2c/
 3) 電源管理 拡張基板 RPZ-PowerMGR
   製品ページ https://www.indoorcorgielec.com/products/rpz-powermgr/
 
 Usage:
   cgpmgr cf [-a] [-u <sec>] [-d <sec>] [-r <num>] [-c <num>] [-z <num>] [-p <num>] [-w <num>]
   cgpmgr sc [-a] [-o] [-D <date>] <time> (on | off)
@@ -38,29 +38,28 @@
   -w <num>   USB Type-AモバイルバッテリーWake up. 1で有効. 0で無効. 
 
   sc         電源ON/OFFスケジュールに関するサブコマンド. 
              オプションを何も指定しないと現在登録済みのスケジュールを表示する. 
   -o         指定すると, 登録するスケジュールがOneTime(1回のみ)になる. 
              省略するとRepeat(繰り返し). 
   -D <date>  登録するスケジュールの月/日を指定. *か**で全てに一致. 
-             日はSun, Mon, Tue, Wed, Thu, Fri, Satで曜日も指定可能. 
-             日は必ず指定する. 省略すると*/*. 例)5/10, , 9/Sun, */15. 
+             日はSun, Mon, Tue, Wed, Thu, Fri, Satで曜日も指定可能. 例)5/10, , 9/Sun, */15. 
   <time>     登録するスケジュールの時:分を指定. *か**で全てに一致. 
-             時を*にしたら月日も必ず*になる(-D 指定不可). 分は*指定不可. 例)21:30, *:45
+             分は*指定不可. 例)21:30, *:45
   on         電源をONするスケジュールを登録する. 
   off        電源をOFFするスケジュールを登録する. 
   -l <min>   現在からmin分後にスケジュールを登録. 秒は切り上げになる. 1-999の範囲で指定. 
              このオプションで登録するとOneTime(1回のみ)になる. 
   -R <num>   指定すると登録済みスケジュールから指定番号のものを削除. 255を指定すると全て削除. 
   -i         スケジュールをcsvファイルから読み出して追加する. 
              省略すると登録済みスケジュールをcsvファイルに保存する.
 
-  me         Raspberry Piの消費電流測定, 結果ログを行うサブコマンド. 
+  me         Raspberry Pi/Jetson Nanoの消費電流測定, 結果ログを行うサブコマンド. 
              オプションを指定しないと直近の電流測定値を表示. 
-  -L         記録されているRaspberry Piの消費電流値を読み出す. 
+  -L         記録されている消費電流値を読み出す. 
              電源ONから1秒ごとに最大1時間まで記録可能.  
   -s         消費電流の記録をリセットして再スタート. 1秒ごと最大1時間まで記録可能.
 
   fw         ファームウェアを-fで指定したものに書き換える.
 
   共通オプション
   -a         I2Cセカンダリアドレス0x22を使用. 
@@ -73,34 +72,36 @@
 import os
 import time
 import datetime
 import re
 import struct
 import subprocess
 import hashlib
-import smbus
+import smbus2
 import RPi.GPIO as GPIO
 
 i2c_adr = 0x20
-compatible_fw = {1: 4, 2: 1}
+compatible_fw = {1: 5, 2: 2}
 sig2gpio = [0, 16, 17, 26, 27]  # SIG番号とGPIO番号の対応
 dow2str = ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat']  # スケジュールデータは日曜が1, 土曜が7
 gpio_rst = 7
 gpio_boot = 25
 fw_ver = []
 
 # ファームウェアハッシュ値
 known_hash = [
     'cf0d1818ade696bc5b7af150ff4a085266fdc829f196f26ed2ed127b7ba12eb3',  # Ver1.0
     '1a6fdf815b5b23a6e39c79d6b734bfd3bd51ddf59b803912425bfc07504f0d1b',  # Ver1.1
     '5764c3cc8442930997fefcc048e35a8242df9bdcdf5f302ed4fb43f1a4fd8c24',  # Ver1.2
     'a37fe6f36a4e99bab07e3106cb99306d13f88d4c72c68b309a4fd9eb8e4c44e8',  # Ver1.3
     '36313403baab9d50183f17d0f9cea991455baf7b1b0478e1ef8773cee0ea91cc',  # Ver1.4
+    'c3f465e5c8e2e004b23d85a6f5846931e106fd8a06715d48e54750c875cfe882',  # Ver1.5
     '0bdb41e819fcd8380a9bf1f551a6a7692bd22bcdb3734580413e4401fa613490',  # Ver2.0
     'f5aa9ab42affd8004238bf1f747d93095b5138602473660eb7965a24d03b167b',  # Ver2.1
+    'a49c1fa3c1f540fcbb77d69be4d599791d3a5a88508e7519aaab2c5426f0fb0c',  # Ver2.2
 ]
 
 
 def cli():
   """
   コマンドラインツールを実行
   """
@@ -113,15 +114,15 @@
   except ImportError:
     print('docoptのインポートに失敗しました. sudo python3 -m pip install docopt コマンドでインストールして下さい. ')
     return
 
   args = docopt(__doc__)
 
   try:
-    i2c = smbus.SMBus(1)
+    i2c = smbus2.SMBus(1)
   except FileNotFoundError:
     print('I2Cバスが開けませんでした. I2Cが有効になっているか確認して下さい. ')
     return
 
   # セカンダリI2Cアドレスを使用
   if args['-a']:
     i2c_adr = 0x22
@@ -155,15 +156,16 @@
       i2c_write(0x16, [int(args['-u'])])
       print('スタートアップタイマーを{}秒に設定しました. '.format(args['-u']))
 
     if args['-d'] != None:
       if not check_digit('-d', args['-d'], 0, 250):
         return
       i2c_write(0x17, [int(args['-d'])])
-      print('シャットダウンタイマーを' + ('無効にしました.' if 0 == int(args['-d']) else '{}秒に設定しました. '.format(args['-d'])))
+      print('シャットダウンタイマーを' +
+            ('無効にしました.' if 0 == int(args['-d']) else '{}秒に設定しました. '.format(args['-d'])))
 
     r = i2c_read(0x18, 1)[0]
     c = i2c_read(0x19, 1)[0]
     if args['-r'] != None:
       if not check_digit_list('-r', args['-r'], sig2gpio):
         return
       r = sig2gpio.index(int(args['-r']))
@@ -177,19 +179,21 @@
       print('シャットダウン要求と完了信号を同じ番号に割り付けることはできません. ')
       return
 
     if args['-r'] != None:
       if args['-c'] != None:
         i2c_write(0x19, [0])  # 番号が重なる可能性があるので一度無効化
       i2c_write(0x18, [r])
-      print('シャットダウン要求信号を' + ('無効にしました.' if 0 == int(args['-r']) else 'GPIO{} に設定しました. '.format(args['-r'])))
+      print('シャットダウン要求信号を' +
+            ('無効にしました.' if 0 == int(args['-r']) else 'GPIO{} に設定しました. '.format(args['-r'])))
 
     if args['-c'] != None:
       i2c_write(0x19, [c])
-      print('シャットダウン完了信号を' + ('無効にしました.' if 0 == int(args['-c']) else 'GPIO{} に設定しました. '.format(args['-c'])))
+      print('シャットダウン完了信号を' +
+            ('無効にしました.' if 0 == int(args['-c']) else 'GPIO{} に設定しました. '.format(args['-c'])))
 
     if args['-z'] != None:
       if not check_digit('-z', args['-z'], -720, 840):
         return
       i2c_write(0x1A, list(struct.pack("h", int(args['-z']))))
 
     if args['-p'] != None:
@@ -216,16 +220,18 @@
     sig_sd_request = i2c_read(0x18, 1)[0]
     sig_sd_complete = i2c_read(0x19, 1)[0]
     time_zone_min = i2c_read(0x1A, 2)
     print('コンフィグ情報')
     print('  ファームウェアバージョン: {}.{}'.format(fw_ver[1], fw_ver[0]))
     print('  スタートアップタイマー: {}秒'.format(rpi_startup_timer))
     print('  シャットダウンタイマー: ' + ('無効' if rpi_sd_timer == 0 else '{}秒'.format(rpi_sd_timer)))
-    print('  シャットダウン要求信号: ' + ('無効' if sig_sd_request == 0 else 'GPIO{}'.format(sig2gpio[sig_sd_request])))
-    print('  シャットダウン完了信号: ' + ('無効' if sig_sd_complete == 0 else 'GPIO{}'.format(sig2gpio[sig_sd_complete])))
+    print('  シャットダウン要求信号: ' +
+          ('無効' if sig_sd_request == 0 else 'GPIO{}'.format(sig2gpio[sig_sd_request])))
+    print('  シャットダウン完了信号: ' +
+          ('無効' if sig_sd_complete == 0 else 'GPIO{}'.format(sig2gpio[sig_sd_complete])))
     print('  タイムゾーン設定: ' + ('{}'.format(struct.unpack("h", bytes(time_zone_min))[0])))
 
     # ファームウェアVersion1.4 / 2.1以降で追加されたオプション
     if (1 == fw_ver[1] and 4 <= fw_ver[0]) or (2 == fw_ver[1] and 1 <= fw_ver[0]):
       auto_run = i2c_read(0x1C, 1)[0]
       usba_wake_up = i2c_read(0x1D, 1)[0]
       print('  電源自動リカバリー: ' + ('無効' if auto_run == 0 else '有効'))
@@ -436,25 +442,28 @@
         for i in range(count):
           i2c_write(0x24, [i & 0xFF, i >> 8])
           curr = i2c_read(0x26, 2)
           print('{}, {}'.format(i, (curr[1] << 8) + curr[0]))
 
     elif args['-s']:
       i2c_write(0x24, [0xFF, 0xFF])
-      print('Raspberry Pi電流値のログをリセットしました. 現在から毎秒, 最大1時間まで記録します. ')
+      print('電流値のログをリセットしました. 現在から毎秒, 最大1時間まで記録します. ')
 
     else:
       curr = i2c_read(0x20, 2)
-      print('Raspberry Pi電流値 {}[mA]'.format((curr[1] << 8) + curr[0]))
+      print('電流値 {}[mA]'.format((curr[1] << 8) + curr[0]))
 
   #----------------------------
   # ファームウェア書き換え
   if args['fw']:
     try:
-      res = subprocess.run(['stm32flash'], encoding='utf-8', stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+      res = subprocess.run(['stm32flash'],
+                           encoding='utf-8',
+                           stdout=subprocess.PIPE,
+                           stderr=subprocess.STDOUT)
     except:
       print('stm32flashが見つかりませんでした. sudo apt install stm32flash コマンドでインストールして下さい. ')
       return
 
     try:
       with open(args['-f'], 'rb') as f:
         hash = hashlib.sha256(f.read()).hexdigest()
@@ -492,15 +501,16 @@
     if re.search(r'Fail', res.stdout):
       print('ファームウェアの書き換え中にエラーが発生しました')
       GPIO.cleanup(gpio_rst)
       GPIO.cleanup(gpio_boot)
       return
 
     boot_loader()
-    res = subprocess.run(['stm32flash', '/dev/i2c-1', '-a', '0x42', '-e 0', '-w', args['-f'], '-v', '-R'])
+    res = subprocess.run(
+        ['stm32flash', '/dev/i2c-1', '-a', '0x42', '-e 0', '-w', args['-f'], '-v', '-R'])
     if res.returncode != 0:
       print('ファームウェアの書き換え中にエラーが発生しました')
       GPIO.cleanup(gpio_rst)
       GPIO.cleanup(gpio_boot)
       return
 
     GPIO.cleanup(gpio_rst)
@@ -601,15 +611,16 @@
   bcd[4]: 日
   bcd[5]: 月
   bcd[6]: 年
   
   Args:
     bcd: BCDフォーマットの7バイトデータのリスト
   """
-  print('20{}{}/{}{}/{}{} '.format(bcd[6] >> 4, bcd[6] & 0xF, bcd[5] >> 4, bcd[5] & 0xF, bcd[4] >> 4, bcd[4] & 0xF),
+  print('20{}{}/{}{}/{}{} '.format(bcd[6] >> 4, bcd[6] & 0xF, bcd[5] >> 4, bcd[5] & 0xF,
+                                   bcd[4] >> 4, bcd[4] & 0xF),
         end='')
   if bcd[3] == 1:
     print('日 ', end='')
   elif bcd[3] == 2:
     print('月 ', end='')
   elif bcd[3] == 3:
     print('火 ', end='')
@@ -617,15 +628,16 @@
     print('水 ', end='')
   elif bcd[3] == 5:
     print('木 ', end='')
   elif bcd[3] == 6:
     print('金 ', end='')
   elif bcd[3] == 7:
     print('土 ', end='')
-  print('{}{}:{}{}:{}{}'.format(bcd[2] >> 4, bcd[2] & 0xF, bcd[1] >> 4, bcd[1] & 0xF, bcd[0] >> 4, bcd[0] & 0xF))
+  print('{}{}:{}{}:{}{}'.format(bcd[2] >> 4, bcd[2] & 0xF, bcd[1] >> 4, bcd[1] & 0xF, bcd[0] >> 4,
+                                bcd[0] & 0xF))
 
 
 def make_bcd(year, month, date, dow, hour, minute, second):
   """
   指定日時から, BCDフォーマットの7バイトのデータを生成
 
   Args:
```

