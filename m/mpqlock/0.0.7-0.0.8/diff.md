# Comparing `tmp/mpqlock-0.0.7.tar.gz` & `tmp/mpqlock-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqlock-0.0.7.tar", last modified: Tue Mar 14 07:23:51 2023, max compression
+gzip compressed data, was "mpqlock-0.0.8.tar", last modified: Mon Jun  5 01:27:00 2023, max compression
```

## Comparing `mpqlock-0.0.7.tar` & `mpqlock-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 07:23:51.903700 mpqlock-0.0.7/
--rw-rw-rw-   0        0        0      219 2023-03-14 07:23:51.902721 mpqlock-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-14 07:23:51.892063 mpqlock-0.0.7/mpqlock/
--rw-rw-rw-   0        0        0    31232 2023-03-14 07:18:24.000000 mpqlock-0.0.7/mpqlock/My_code_lock_2024.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0      146 2023-03-14 07:23:12.000000 mpqlock-0.0.7/mpqlock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 07:23:51.902243 mpqlock-0.0.7/mpqlock.egg-info/
--rw-rw-rw-   0        0        0      219 2023-03-14 07:23:51.000000 mpqlock-0.0.7/mpqlock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-03-14 07:23:51.000000 mpqlock-0.0.7/mpqlock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 07:23:51.000000 mpqlock-0.0.7/mpqlock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-14 07:23:51.000000 mpqlock-0.0.7/mpqlock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 07:23:51.903700 mpqlock-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-03-14 07:22:30.000000 mpqlock-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:27:00.139514 mpqlock-0.0.8/
+-rw-rw-rw-   0        0        0      219 2023-06-05 01:27:00.138243 mpqlock-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 01:27:00.134218 mpqlock-0.0.8/mpqlock/
+-rw-rw-rw-   0        0        0    31232 2023-06-05 01:25:30.000000 mpqlock-0.0.8/mpqlock/My_code_lock_2024.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0      146 2023-03-14 07:23:12.000000 mpqlock-0.0.8/mpqlock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:27:00.138243 mpqlock-0.0.8/mpqlock.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-06-05 01:27:00.000000 mpqlock-0.0.8/mpqlock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-05 01:27:00.000000 mpqlock-0.0.8/mpqlock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:27:00.000000 mpqlock-0.0.8/mpqlock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 01:27:00.000000 mpqlock-0.0.8/mpqlock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:27:00.139514 mpqlock-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-06-05 01:21:50.000000 mpqlock-0.0.8/setup.py
```

