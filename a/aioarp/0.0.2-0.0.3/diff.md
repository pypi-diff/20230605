# Comparing `tmp/aioarp-0.0.2.tar.gz` & `tmp/aioarp-0.0.3.tar.gz`

## Comparing `aioarp-0.0.2.tar` & `aioarp-0.0.3.tar`

### file list

```diff
@@ -1,76 +1,209 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 aioarp-0.0.2/unasync.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/17946c0e3734f56
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/18bd9323e775c06
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/1cf748db3edf4393
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/1d813f87eae436dc
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/20360c87813708ee
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/20e8c6fb6ec65fba
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/22273ee756d2aeab
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/22eb75e2705cd7cb
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/27380b38303cddd4
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/2894d2afe73e6dee
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/28bfffee8af0f637
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/29a3dfb41b2e153e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/2b17b1ab21ba1879
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/3546886ec7b89ca2
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/44618acc04af2a98
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/464ea8dcb036f50b
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/48dc01dafed313cb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/53922c565bc4cfdf
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/608e0f7e2331dfd0
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/64f9f289e0610564
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/65bac7c6a4c4cb5e
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/6857c9063a540073
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/6ba798af16bd34e5
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/75d5cb975af2bc07
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/7753615b71d6a36e
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/869f865c9f14daf7
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/936f955f01285847
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/967dc6947ad8c113
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/a12cec0addd27620
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/a64cd85354e281c5
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/b3202a665cec273b
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/bdd7c44b4f88bf5b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c0d92e761aa72a56
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c24cf3b955d01f58
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c2e7f8eb8bfe8525
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c78c3248c370d9f2
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c7a507ee84d3e2ab
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/dc53fc214ceea0dd
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/de93c4dfa993ec19
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e11920c476dc4f59
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e12d636458d129da
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e305b1c5b826225
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e512a2b647437caa
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f3ac79af6cdde497
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f3d289f55f0ad6bd
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f45e36470415dca1
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f58c3d661899d706
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/ffe7d79671eca8f
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/__about__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/__init__.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_arp.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_client.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_mock.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/defaults.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_async/__init__.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_sync/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/backends/_async.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/backends/_sync.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/lint
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/test
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_proto.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 aioarp-0.0.2/README.md
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 aioarp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aioarp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aioarp-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.3/unasync.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/120fd5a3e305da5b
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/12101680e8031881
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/16b1a595f0c0b695
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/17946c0e3734f56
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/18bd9323e775c06
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1911b721541a132
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1a43e2fa66cc521
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1bfc7af844c09624
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1c4766f25c290393
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1cf748db3edf4393
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1d813f87eae436dc
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20360c87813708ee
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20b471ae4ae2c716
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20cf28b4a08829e
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20e8c6fb6ec65fba
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/22273ee756d2aeab
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/22eb75e2705cd7cb
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/258218bd1af61054
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/259f2d45c9b5e8f8
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/259f7be1f71aae17
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/27380b38303cddd4
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/277c58fd0e92dc6f
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2894d2afe73e6dee
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/28bfffee8af0f637
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/29a3dfb41b2e153e
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/29ec5304bead68a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2b17b1ab21ba1879
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2b74d3f1efd79c7b
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2f2908e30cbaaf6f
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3546886ec7b89ca2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3a9f29e79b12106b
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3c82c38fdeb726f5
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3cf42c96bb03e8e
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/40ec6c4657092d14
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/42d47131a22f033d
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/44618acc04af2a98
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/464ea8dcb036f50b
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/48dc01dafed313cb
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4bfeb322489be7b2
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4c18fbd43c6124d9
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4c7aefddb4afaa07
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4ce11f41c925600e
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4d80d8cbd7abb331
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4dcc3bf9688e8634
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4e4abc9127fe2106
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/522c23633820a258
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5259c25c40a66c52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/53480da31b2357be
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/536385ed3a8bbf59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/53922c565bc4cfdf
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/54ca2556c07eb0e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/57ee6e97f4833ae1
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5845e4d7f49b3f6b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/590fd00a0401d086
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5e5e4a02dc426617
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/608e0f7e2331dfd0
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6190d891377c8571
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6269535ee79a68b3
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6390cd3a2155b002
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/64f9f289e0610564
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6572fa7cae8df134
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/65bac7c6a4c4cb5e
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/65d6dc214750c212
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6857c9063a540073
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/68e278cd0a30d24c
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6aa5b22c44c81236
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6aee26157f3848b9
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6b926a7206e2e0f5
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6ba798af16bd34e5
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6dbcf7ab6c32f876
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6de1f164718890ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6ec79cb0a99a4ffa
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/70ee6f5e2e8b7d90
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/75d5cb975af2bc07
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7753615b71d6a36e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/78dc31b63dbd1e69
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/79da2ffd4120460
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7d0a3cccefcd7db3
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7f23f9f7d375f4fd
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/80b8f04bc59d958c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/82b9ee56f8fed787
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8362e113a849836
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/841d7ee35702e48e
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/85532fbdb4ec8100
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/859b9d135acd891b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/85a7bda1ebac02be
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/869f865c9f14daf7
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/879246cf978566b8
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/89ad75a37b7215d3
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8af090de0021767
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8ba2e035b666505
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8caa6ea7d00a8ef9
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8e5085aaf38947dd
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8e9682f1b99c3026
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/93389fd7b221ce32
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/936f955f01285847
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/94a86b805b8c04e2
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/9600ec5b79137dcc
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/967dc6947ad8c113
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/990e2b74e6a14435
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/9db40d9bd33cc32a
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a0edd6b97fbe3e68
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a12cec0addd27620
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a22627f4ad982518
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a41b182cef331aa5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a42de4efa897ae1e
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a5253384caf62eef
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a62236fd623ff7ad
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a64cd85354e281c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a7b52a5c13a67fed
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aabe170d14233a1f
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aac73f953da24b03
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/ac1d91a6ebb4bed9
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aced40484cbf3132
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/adb7c2d2342ef983
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b27cd0e5108544e0
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b3202a665cec273b
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b74ab4e72907ed4b
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b752bc22791212b3
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b874aac73807837a
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bb3a8375be948e99
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bb98194f279aef4d
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bc9d2b60dadbf05e
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bd0ea26a717d1380
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bd3e6a97ee360bd7
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bdd7c44b4f88bf5b
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bffaaf1ee55da212
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c0cc1810bd812c85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c0d92e761aa72a56
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c12c935be2da0714
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c24cf3b955d01f58
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c2e7f8eb8bfe8525
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c370f17718b5228b
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c3b1cc9370bb49b5
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c54b124e74d7c29a
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c64725c588d56756
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c6c7c5bdc9a58d71
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c78c3248c370d9f2
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c7a507ee84d3e2ab
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c908c9d3ee0eb43c
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cc374f0497dbc539
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cc5595ab776e807c
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cd40078ccedf2012
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cd84fa1ee95c780c
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cdc31ad9b3ea9979
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d08cf74ff5eeb16e
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d3d46de068ceaf65
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d4ed3103ad57bd80
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d8259ee38b03fc0e
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/dc53fc214ceea0dd
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/de93c4dfa993ec19
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e11920c476dc4f59
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e12d636458d129da
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e25cfbd84c59869
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e2a8017124da7733
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e305b1c5b826225
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e512a2b647437caa
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e84bd53ae32ad4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e8f0ea35cc3b448a
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e9d1ab2b1a8c3cca
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/eb250aff0edc4ecb
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/eee42766c50b6490
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f0ff9ca6cba080b9
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f2ebd390a47aa1cd
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f3ac79af6cdde497
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f3d289f55f0ad6bd
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f45e36470415dca1
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f56e6b11a3d4a68b
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f58c3d661899d706
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f96d453d0b6b9c85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/fb10e8087c484390
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/fd508bd27e156044
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/ffe7d79671eca8f
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/__init__.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_arp.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_async.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_mock.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_sync.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_sync.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/lint
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/test
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_async.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_proto.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_sync.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 aioarp-0.0.3/README.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aioarp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 aioarp-0.0.3/PKG-INFO
```

### Comparing `aioarp-0.0.2/unasync.py` & `aioarp-0.0.3/unasync.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
 import re
 
 SUBS = [
     ('async def async_send_arp', 'def sync_send_arp'),
     ('async def', 'def'),
-    ('from ..backends._async import AsyncSocket', 'from ..backends._sync import Socket'),
-    ('AsyncSocket', 'Socket'),
+    ('from .backends._async import AsyncStream', 'from .backends._sync import Stream'),
+    ('AsyncStream', 'Stream'),
     ('await ', ''),
-    ('async_send_arp', 'sync_send_arp')
+    ('async_send_arp', 'sync_send_arp'),
+    ('aioarp.arequest', 'aioarp.request')
 ]
 
 COMPILED_SUBS = [
     (re.compile(r'(^|\b)' + regex + r'($|\b)'), replaced)
     for regex, replaced in SUBS
 ]
 
@@ -25,18 +25,9 @@
 def unasync_file(async_path, sync_path):
     with (open(async_path, "r") as in_file, \
           open(sync_path, "w", newline="") as sync_file):
             for line in in_file.readlines():
                 line = unasync_line(line)
                 sync_file.write(line)
 
-def unasync(async_dir, sync_dir):
-    for dirpath, _dirnames, filenames in os.walk(async_dir):
-        for filename in filenames:
-            if filename.endswith('.py'):
-                rel_dir = os.path.relpath(dirpath, async_dir)
-                async_path = os.path.normpath(os.path.join(async_dir, rel_dir, filename))
-                sync_path = os.path.normpath(os.path.join(sync_dir, rel_dir, filename))
-                unasync_file(async_path, sync_path)
-
-
-unasync("aioarp/_async", "aioarp/_sync")
+unasync_file("aioarp/_async.py", "aioarp/_sync.py")
+unasync_file("tests/test_async.py", "tests/test_sync.py")
```

### Comparing `aioarp-0.0.2/.ruff_cache/content/18bd9323e775c06` & `aioarp-0.0.3/.ruff_cache/content/18bd9323e775c06`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/1cf748db3edf4393` & `aioarp-0.0.3/.ruff_cache/content/1cf748db3edf4393`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/1d813f87eae436dc` & `aioarp-0.0.3/.ruff_cache/content/1d813f87eae436dc`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/22273ee756d2aeab` & `aioarp-0.0.3/.ruff_cache/content/22273ee756d2aeab`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/2894d2afe73e6dee` & `aioarp-0.0.3/.ruff_cache/content/2894d2afe73e6dee`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/28bfffee8af0f637` & `aioarp-0.0.3/.ruff_cache/content/28bfffee8af0f637`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/29a3dfb41b2e153e` & `aioarp-0.0.3/.ruff_cache/content/29a3dfb41b2e153e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/44618acc04af2a98` & `aioarp-0.0.3/.ruff_cache/content/44618acc04af2a98`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/464ea8dcb036f50b` & `aioarp-0.0.3/.ruff_cache/content/464ea8dcb036f50b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/48dc01dafed313cb` & `aioarp-0.0.3/.ruff_cache/content/48dc01dafed313cb`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/608e0f7e2331dfd0` & `aioarp-0.0.3/.ruff_cache/content/608e0f7e2331dfd0`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/64f9f289e0610564` & `aioarp-0.0.3/.ruff_cache/content/64f9f289e0610564`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/6ba798af16bd34e5` & `aioarp-0.0.3/.ruff_cache/content/6ba798af16bd34e5`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/936f955f01285847` & `aioarp-0.0.3/.ruff_cache/content/936f955f01285847`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/a12cec0addd27620` & `aioarp-0.0.3/.ruff_cache/content/a12cec0addd27620`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/bdd7c44b4f88bf5b` & `aioarp-0.0.3/.ruff_cache/content/bdd7c44b4f88bf5b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/c78c3248c370d9f2` & `aioarp-0.0.3/.ruff_cache/content/c78c3248c370d9f2`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/e12d636458d129da` & `aioarp-0.0.3/.ruff_cache/content/e12d636458d129da`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/f45e36470415dca1` & `aioarp-0.0.3/.ruff_cache/content/f45e36470415dca1`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.ruff_cache/content/f58c3d661899d706` & `aioarp-0.0.3/.ruff_cache/content/f58c3d661899d706`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/aioarp/_arp.py` & `aioarp-0.0.3/aioarp/_arp.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,8 +169,8 @@
 
 def size_of(type: typing.Union[HardwareType, Protocol]) -> int:
     if type is Protocol.ip:
         return 4
     elif type is HardwareType.ethernet:
         return 6
     else:
-        raise Exception
+        raise NotImplementedError()
```

### Comparing `aioarp-0.0.2/aioarp/_utils.py` & `aioarp-0.0.3/aioarp/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     try:
         ipaddress.IPv4Address(ip)
         return True
     except ipaddress.AddressValueError:
         return False
 
 
-def get_mac(interface: str) -> str:
+def get_mac(interface: str) -> str:  # pragma: no cover
     global OUR_MAC
     if OUR_MAC:
         return OUR_MAC
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         info = fcntl.ioctl(s.fileno(), 0x8927, struct.pack('256s', bytes(interface, 'utf-8')[:15]))
         mac = ':'.join('%02x' % b for b in info[18:24])
         OUR_MAC = mac
         return OUR_MAC
 
 
-def get_ip() -> str:
+def get_ip() -> str:  # pragma: no cover
     global OUR_IP
     if OUR_IP:
         return OUR_IP
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         s.connect(("1.1.1.1", 80))
         ip = typing.cast(str, s.getsockname()[0])
         OUR_IP = ip
```

### Comparing `aioarp-0.0.2/aioarp/_async/__init__.py` & `aioarp-0.0.3/aioarp/_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 import time
+import typing
 
 from aioarp import _exceptions as exc
 from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
 from aioarp._utils import is_valid_ipv4
 from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
 
-from ..backends._async import AsyncSocket
+from ._backends._async import AsyncStream
 
 __all__ = (
     'async_send_arp',
 )
 
-async def receive_arp(sock: AsyncSocket, timeout: float) -> ArpPacket:
+
+async def receive_arp(sock: AsyncStream, timeout: float) -> ArpPacket:
     start_time = time.time()
     while True:
 
         # Check if timeout was expired
         if time.time() - start_time > timeout:
             raise exc.NotFoundError()
 
         # Try to read frame
         try:
             frame = await sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
             raise exc.NotFoundError() from e
 
         # Extract the ethernet header
         eth_header = frame[:ETHERNET_HEADER_SIZE]
 
         try:
             eth_packet = EthPacket.parse(eth_header)
             if eth_packet.proto != Protocol.arp:
                 continue
 
             arp_response = ArpPacket.parse(
                 frame[ETHERNET_HEADER_SIZE: ETHERNET_HEADER_SIZE + ARP_HEADER_SIZE])
             if is_valid_ipv4(arp_response.sender_ip):
                 return arp_response
-        except BaseException:
+        except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
-async def async_send_arp(arp_packet: ArpPacket, interface: str) -> ArpPacket:
-    sock = AsyncSocket(interface)
+async def async_send_arp(arp_packet: ArpPacket,
+                         stream: AsyncStream,
+                         timeout: typing.Optional[float] = None) -> ArpPacket:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
 
     try:
         frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
-        await sock.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
-    except exc.WriteTimeoutError as e:
+        await stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
+    except exc.WriteTimeoutError as e:  # pragma: no cover
         raise exc.NotFoundError from e
 
-    return await receive_arp(sock, DEFAULT_REPLY_MISSING_TIME)
+    return await receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
```

### Comparing `aioarp-0.0.2/aioarp/_sync/__init__.py` & `aioarp-0.0.3/aioarp/_sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import time
+import typing
 
-from aioarp import _exceptions as exc
+from aioarp import Stream, _exceptions as exc
 from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
 from aioarp._utils import is_valid_ipv4
 from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
 
-from ..backends._sync import Socket
-
 __all__ = (
     'sync_send_arp',
 )
 
-def receive_arp(sock: Socket, timeout: float) -> ArpPacket:
+
+def receive_arp(sock: Stream, timeout: float) -> ArpPacket:
     start_time = time.time()
     while True:
 
         # Check if timeout was expired
         if time.time() - start_time > timeout:
             raise exc.NotFoundError()
 
         # Try to read frame
         try:
             frame = sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
             raise exc.NotFoundError() from e
 
         # Extract the ethernet header
         eth_header = frame[:ETHERNET_HEADER_SIZE]
 
         try:
             eth_packet = EthPacket.parse(eth_header)
             if eth_packet.proto != Protocol.arp:
                 continue
 
             arp_response = ArpPacket.parse(
                 frame[ETHERNET_HEADER_SIZE: ETHERNET_HEADER_SIZE + ARP_HEADER_SIZE])
             if is_valid_ipv4(arp_response.sender_ip):
                 return arp_response
-        except BaseException:
+        except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
-def sync_send_arp(arp_packet: ArpPacket, interface: str) -> ArpPacket:
-    sock = Socket(interface)
+def sync_send_arp(arp_packet: ArpPacket,
+                         stream: Stream,
+                         timeout: typing.Optional[float] = None) -> ArpPacket:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
 
     try:
         frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
-        sock.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
-    except exc.WriteTimeoutError as e:
+        stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
+    except exc.WriteTimeoutError as e:  # pragma: no cover
         raise exc.NotFoundError from e
 
-    return receive_arp(sock, DEFAULT_REPLY_MISSING_TIME)
+    return receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
```

### Comparing `aioarp-0.0.2/aioarp/backends/_async.py` & `aioarp-0.0.3/.ruff_cache/content/16b1a595f0c0b695`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-00000000: 696d 706f 7274 2073 656c 6563 740a 696d  import select.im
-00000010: 706f 7274 2073 6f63 6b65 740a 696d 706f  port socket.impo
-00000020: 7274 2074 7970 696e 670a 0a69 6d70 6f72  rt typing..impor
-00000030: 7420 616e 7969 6f0a 6672 6f6d 2061 6e79  t anyio.from any
-00000040: 696f 2e61 6263 2069 6d70 6f72 7420 4173  io.abc import As
-00000050: 796e 6352 6573 6f75 7263 650a 0a66 726f  yncResource..fro
-00000060: 6d20 6169 6f61 7270 2069 6d70 6f72 7420  m aioarp import 
-00000070: 5f65 7863 6570 7469 6f6e 7320 6173 2065  _exceptions as e
-00000080: 7863 0a0a 2320 544f 444f 3a20 6164 6420  xc..# TODO: add 
-00000090: 6572 726f 7220 6d61 700a 0a63 6c61 7373  error map..class
-000000a0: 2041 7379 6e63 536f 636b 6574 2841 7379   AsyncSocket(Asy
-000000b0: 6e63 5265 736f 7572 6365 293a 0a0a 2020  ncResource):..  
-000000c0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-000000d0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000000e0: 2020 2020 2020 696e 7465 7266 6163 653a        interface:
-000000f0: 2073 7472 293a 0a20 2020 2020 2020 2073   str):.        s
-00000100: 6f63 6b20 3d20 736f 636b 6574 2e73 6f63  ock = socket.soc
-00000110: 6b65 7428 736f 636b 6574 2e50 465f 5041  ket(socket.PF_PA
-00000120: 434b 4554 2c20 736f 636b 6574 2e53 4f43  CKET, socket.SOC
-00000130: 4b5f 5241 572c 2073 6f63 6b65 742e 6e74  K_RAW, socket.nt
-00000140: 6f68 7328 3078 3030 3033 2929 0a20 2020  ohs(0x0003)).   
-00000150: 2020 2020 2073 6f63 6b2e 6269 6e64 2828       sock.bind((
-00000160: 696e 7465 7266 6163 652c 2030 2929 0a20  interface, 0)). 
-00000170: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
-00000180: 203d 2073 6f63 6b0a 0a20 2020 2061 7379   = sock..    asy
-00000190: 6e63 2064 6566 2072 6563 6569 7665 5f66  nc def receive_f
-000001a0: 7261 6d65 2873 656c 662c 2074 696d 656f  rame(self, timeo
-000001b0: 7574 3a20 666c 6f61 7429 202d 3e20 6279  ut: float) -> by
-000001c0: 7465 733a 0a20 2020 2020 2020 2066 7261  tes:.        fra
-000001d0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
-000001e0: 6e61 6c5b 6279 7465 735d 0a20 2020 2020  nal[bytes].     
-000001f0: 2020 2077 6974 6820 616e 7969 6f2e 6d6f     with anyio.mo
-00000200: 7665 5f6f 6e5f 6166 7465 7228 7469 6d65  ve_on_after(time
-00000210: 6f75 7429 3a0a 2020 2020 2020 2020 2020  out):.          
-00000220: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
-00000230: 2020 2020 2020 2020 2020 2020 2020 722c                r,
-00000240: 205f 2c20 5f20 3d20 7365 6c65 6374 2e73   _, _ = select.s
-00000250: 656c 6563 7428 5b73 656c 662e 736f 636b  elect([self.sock
-00000260: 5d2c 205b 5d2c 205b 5d2c 2030 2e30 3030  ], [], [], 0.000
-00000270: 3031 290a 2020 2020 2020 2020 2020 2020  01).            
-00000280: 2020 2020 6966 2072 3a0a 2020 2020 2020      if r:.      
-00000290: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-000002a0: 616d 6520 3d20 7365 6c66 2e73 6f63 6b2e  ame = self.sock.
-000002b0: 7265 6376 2831 3132 3331 3233 290a 2020  recv(1123123).  
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-000002e0: 2020 2020 2020 2020 6177 6169 7420 616e          await an
-000002f0: 7969 6f2e 736c 6565 7028 3029 0a20 2020  yio.sleep(0).   
-00000300: 2020 2020 2069 6620 6e6f 7420 6672 616d       if not fram
-00000310: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00000320: 6169 7365 2065 7863 2e52 6561 6454 696d  aise exc.ReadTim
-00000330: 656f 7574 4572 726f 7228 290a 2020 2020  eoutError().    
-00000340: 2020 2020 7265 7475 726e 2066 7261 6d65      return frame
-00000350: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00000360: 7772 6974 655f 6672 616d 6528 7365 6c66  write_frame(self
-00000370: 2c20 6672 616d 653a 2062 7974 6573 2c20  , frame: bytes, 
-00000380: 7469 6d65 6f75 743a 2066 6c6f 6174 2920  timeout: float) 
-00000390: 2d3e 204e 6f6e 653a 0a0a 2020 2020 2020  -> None:..      
-000003a0: 2020 7769 7468 2061 6e79 696f 2e6d 6f76    with anyio.mov
-000003b0: 655f 6f6e 5f61 6674 6572 2874 696d 656f  e_on_after(timeo
-000003c0: 7574 293a 0a20 2020 2020 2020 2020 2020  ut):.           
-000003d0: 2077 6869 6c65 2066 7261 6d65 3a0a 2020   while frame:.  
-000003e0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
-000003f0: 2077 2c20 5f20 3d20 7365 6c65 6374 2e73   w, _ = select.s
-00000400: 656c 6563 7428 5b5d 2c20 5b73 656c 662e  elect([], [self.
-00000410: 736f 636b 5d2c 205b 5d2c 2030 2e30 3030  sock], [], 0.000
-00000420: 3031 290a 0a20 2020 2020 2020 2020 2020  01)..           
-00000430: 2020 2020 206e 7365 6e74 203d 2073 656c       nsent = sel
-00000440: 662e 736f 636b 2e73 656e 6428 6672 616d  f.sock.send(fram
-00000450: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00000460: 2020 2066 7261 6d65 203d 2066 7261 6d65     frame = frame
-00000470: 5b6e 7365 6e74 3a5d 0a20 2020 2020 2020  [nsent:].       
-00000480: 2020 2020 2020 2020 2061 7761 6974 2061           await a
-00000490: 6e79 696f 2e73 6c65 6570 2830 290a 2020  nyio.sleep(0).  
-000004a0: 2020 2020 2020 6966 2066 7261 6d65 3a0a        if frame:.
-000004b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000004c0: 6520 6578 632e 5772 6974 6554 696d 656f  e exc.WriteTimeo
-000004d0: 7574 4572 726f 7228 290a 0a20 2020 2061  utError()..    a
-000004e0: 7379 6e63 2064 6566 2061 636c 6f73 6528  sync def aclose(
-000004f0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00000500: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
-00000510: 2e63 6c6f 7365 2829 0a                   .close().
+00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000010: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
+00000020: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
+00000030: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
+00000040: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
+00000050: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
+00000060: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
+00000070: 7300 0000 0045 0000 0001 0100 0000 0000  s....E..........
+00000080: 0000 0000 0000 4500 0000 0144 0000 0000  ......E....D....
+00000090: 0000 0069 6d70 6f72 7420 736f 636b 6574  ...import socket
+000000a0: 0a69 6d70 6f72 7420 7479 7069 6e67 0a0a  .import typing..
+000000b0: 6672 6f6d 2061 696f 6172 7020 696d 706f  from aioarp impo
+000000c0: 7274 205f 6578 6365 7074 696f 6e73 2061  rt _exceptions a
+000000d0: 7320 6578 630a 0a03 0000 0000 0000 0000  s exc...........
+000000e0: 0000 0000 0000 0001 0000 0000 0000 0032  ...............2
+000000f0: 0000 0000 0000 002f 686f 6d65 2f74 6573  ......./home/tes
+00000100: 742f 4465 736b 746f 702f 6169 6f61 7270  t/Desktop/aioarp
+00000110: 2f61 696f 6172 702f 6261 636b 656e 6473  /aioarp/backends
+00000120: 2f5f 7379 6e63 2e70 79bf 0300 0000 0000  /_sync.py.......
+00000130: 0069 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
+00000140: 6d70 6f72 7420 7479 7069 6e67 0a0a 6672  mport typing..fr
+00000150: 6f6d 2061 696f 6172 7020 696d 706f 7274  om aioarp import
+00000160: 205f 6578 6365 7074 696f 6e73 2061 7320   _exceptions as 
+00000170: 6578 630a 0a0a 2320 544f 444f 3a20 6164  exc...# TODO: ad
+00000180: 6420 6572 726f 7220 6d61 700a 0a63 6c61  d error map..cla
+00000190: 7373 2053 7472 6561 6d3a 0a0a 2020 2020  ss Stream:..    
+000001a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000001b0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+000001c0: 2020 2020 696e 7465 7266 6163 653a 2073      interface: s
+000001d0: 7472 293a 0a20 2020 2020 2020 2073 6f63  tr):.        soc
+000001e0: 6b20 3d20 736f 636b 6574 2e73 6f63 6b65  k = socket.socke
+000001f0: 7428 736f 636b 6574 2e50 465f 5041 434b  t(socket.PF_PACK
+00000200: 4554 2c20 736f 636b 6574 2e53 4f43 4b5f  ET, socket.SOCK_
+00000210: 5241 572c 2073 6f63 6b65 742e 6e74 6f68  RAW, socket.ntoh
+00000220: 7328 3078 3030 3033 2929 0a20 2020 2020  s(0x0003)).     
+00000230: 2020 2073 6f63 6b2e 6269 6e64 2828 696e     sock.bind((in
+00000240: 7465 7266 6163 652c 2030 2929 0a20 2020  terface, 0)).   
+00000250: 2020 2020 2073 656c 662e 736f 636b 203d       self.sock =
+00000260: 2073 6f63 6b0a 0a20 2020 2064 6566 2072   sock..    def r
+00000270: 6563 6569 7665 5f66 7261 6d65 2873 656c  eceive_frame(sel
+00000280: 662c 2074 696d 656f 7574 3a20 666c 6f61  f, timeout: floa
+00000290: 7429 202d 3e20 6279 7465 733a 0a20 2020  t) -> bytes:.   
+000002a0: 2020 2020 2073 656c 662e 736f 636b 2e73       self.sock.s
+000002b0: 6574 7469 6d65 6f75 7428 7469 6d65 6f75  ettimeout(timeou
+000002c0: 7429 0a20 2020 2020 2020 2074 7279 3a0a  t).        try:.
+000002d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000002e0: 6520 3d20 7365 6c66 2e73 6f63 6b2e 7265  e = self.sock.re
+000002f0: 6376 2831 3132 3331 3233 290a 2020 2020  cv(1123123).    
+00000300: 2020 2020 6578 6365 7074 2073 6f63 6b65      except socke
+00000310: 742e 7469 6d65 6f75 743a 0a20 2020 2020  t.timeout:.     
+00000320: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
+00000330: 2e52 6561 6454 696d 656f 7574 4572 726f  .ReadTimeoutErro
+00000340: 7228 290a 2020 2020 2020 2020 7265 7475  r().        retu
+00000350: 726e 2066 7261 6d65 0a0a 2020 2020 6465  rn frame..    de
+00000360: 6620 7772 6974 655f 6672 616d 6528 7365  f write_frame(se
+00000370: 6c66 2c20 6672 616d 653a 2062 7974 6573  lf, frame: bytes
+00000380: 2c20 7469 6d65 6f75 743a 2066 6c6f 6174  , timeout: float
+00000390: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000003a0: 2020 2073 656c 662e 736f 636b 2e73 6574     self.sock.set
+000003b0: 7469 6d65 6f75 7428 7469 6d65 6f75 7429  timeout(timeout)
+000003c0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+000003d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000003e0: 6f63 6b2e 7365 6e64 616c 6c28 6672 616d  ock.sendall(fram
+000003f0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
+00000400: 7420 736f 636b 6574 2e74 696d 656f 7574  t socket.timeout
+00000410: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00000420: 6973 6520 6578 632e 5772 6974 6554 696d  ise exc.WriteTim
+00000430: 656f 7574 4572 726f 7228 290a 0a20 2020  eoutError()..   
+00000440: 2064 6566 205f 5f65 6e74 6572 5f5f 2873   def __enter__(s
+00000450: 656c 6629 202d 3e20 2753 7472 6561 6d27  elf) -> 'Stream'
+00000460: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00000470: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
+00000480: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
+00000490: 635f 7479 7065 3a20 7479 7069 6e67 2e41  c_type: typing.A
+000004a0: 6e79 2c20 6578 635f 7661 6c3a 2074 7970  ny, exc_val: typ
+000004b0: 696e 672e 416e 792c 2065 7863 5f74 623a  ing.Any, exc_tb:
+000004c0: 2074 7970 696e 672e 416e 7929 202d 3e20   typing.Any) -> 
+000004d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+000004e0: 6c66 2e73 6f63 6b2e 636c 6f73 6528 290a  lf.sock.close().
```

### Comparing `aioarp-0.0.2/aioarp/backends/_sync.py` & `aioarp-0.0.3/aioarp/_backends/_sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import socket
 import typing
 
 from aioarp import _exceptions as exc
+from aioarp._backends._base import SocketInterface
 
-# TODO: add error map
-
-class Socket:
+__all__ = (
+    'Stream',
+)
+class Stream:
 
     def __init__(self,
-                 interface: str):
-        sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
-        sock.bind((interface, 0))
-        self.sock = sock
+                 interface: str,
+                 sock: typing.Optional[SocketInterface] = None
+                 ):
+        self.sock: SocketInterface
+        if not sock:  # pragma: no cover
+            self.sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
+        else:
+            self.sock = sock
+        self.sock.bind((interface, 0))
 
     def receive_frame(self, timeout: float) -> bytes:
         self.sock.settimeout(timeout)
         try:
             frame = self.sock.recv(1123123)
-        except socket.timeout:
+        except socket.timeout:  # pragma: no cover
             raise exc.ReadTimeoutError()
         return frame
 
     def write_frame(self, frame: bytes, timeout: float) -> None:
         self.sock.settimeout(timeout)
         try:
             self.sock.sendall(frame)
-        except socket.timeout:
+        except socket.timeout:  # pragma: no cover
             raise exc.WriteTimeoutError()
 
-    def __enter__(self) -> 'Socket':
+    def __enter__(self) -> 'Stream':
         return self
 
     def __exit__(self, exc_type: typing.Any, exc_val: typing.Any, exc_tb: typing.Any) -> None:
         self.sock.close()
```

### Comparing `aioarp-0.0.2/tests/test_proto.py` & `aioarp-0.0.3/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/.gitignore` & `aioarp-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/LICENSE.txt` & `aioarp-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.2/README.md` & `aioarp-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aioarp.svg)](https://pypi.org/project/aioarp)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [ARP request](#sending-arp-requests)
+- [ARP response](#arp-response)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install aioarp
 ```
 
-## License
-
-`aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-## Sending ARP requests
+## How to send ARP requests
 
 ### Sync
 ```python
 >>> import aioarp
 >>> response = aioarp.request('enp0s3', '10.0.2.2')
 >>> print(response.sender_mac)
 ee:xx:aa:mm:pp:le  # mac address
@@ -63,22 +61,22 @@
 
 If you want, you can explicitly set all of the **ARP** headers. To do so, create the `ArpPacket` instance yourself and then ask `aioarp` to send that request.
 
 ```python
 >>> import aioarp
 >>>
 >>> arp_packet = aioarp.ArpPacket(
-... hardware_type=aioarp.HardwareType.ethernet,
-... protocol_type=aioarp.Protocol.ip,
-... sender_mac='11:11:11:11:11:11',
-... sender_ip='127.0.0.1',
-... target_mac='11:11:11:11:11:11',
-... target_ip='127.0.0.1',)
+...     hardware_type=aioarp.HardwareType.ethernet,
+...     protocol_type=aioarp.Protocol.ip,
+...     sender_mac='11:11:11:11:11:11',
+...     sender_ip='127.0.0.1',
+...     target_mac='11:11:11:11:11:11',
+...     target_ip='127.0.0.1')
 >>>
->>> response = aioarp.sync_send_arp(arp_packet, 'enp0s3')
+>>> response = aioarp.sync_send_arp(arp_packet, aioarp.Stream('enp0s3'))
 ```
 
 This is the packet that was sent over the network.
 
 ```
 Ethernet II, Src: Private_11:11:11 (11:11:11:11:11:11), Dst: Private_11:11:11 (11:11:11:11:11:11)
     Destination: Private_11:11:11 (11:11:11:11:11:11)
@@ -126,19 +124,29 @@
 ```
 Each one has a distinct meaning, which can be found in https://en.wikipedia.org/wiki/Address_Resolution_Protocol.
 
 ## Failed Responses
 
 If the response is not received, aioarp should throw a `aioarp.NotFoundError` exception. 
 
-This occurs when the default arp request `timeout expires`. The timeout is set to 5 by default; in future releases, we will add a parameter to allow you to change that value.
+This occurs when the default arp request `timeout expires`. The timeout is set to 5 by default, but it can be changed by passing the `timeout` argument to the `request` function.
 
+Without timeout
 ```python
 >>> import aioarp
 >>>
 >>> try:
 ...     response = aioarp.request('enp0s3', '10.0.2.25')
 ...     print(response.opcode)
 ... except aioarp.NotFoundError:
 ...     print('10.0.2.25 was not found :(')
+
 ```
+With timeout
+```python
+response = aioarp.request('enp0s3', '10.0.2.25', timeout=0.5)
+```
+
+## License
+
+`aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `aioarp-0.0.2/pyproject.toml` & `aioarp-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,16 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "anyio"
+  "anyio==3.6.2",
+  "typing_extensions==4.6.3"
 ]
 
 [project.urls]
 Documentation = "https://github.com/karosis88/aioarp#readme"
 Issues = "https://github.com/karosis88/aioarp/issues"
 Source = "https://github.com/karosis88/aioarp"
 
@@ -48,8 +49,15 @@
 ignore_missing_imports = true
 strict = true
 exclude = ["unasync.py", "_mock.py"]
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
-check_untyped_defs = true
+check_untyped_defs = true
+
+[tool.coverage.report]
+
+exclude_also = [
+  '__repr__',
+  'raise NotImplementedError()'
+]
```

### Comparing `aioarp-0.0.2/PKG-INFO` & `aioarp-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
 Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Project-URL: Source, https://github.com/karosis88/aioarp
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,40 +13,39 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: anyio
+Requires-Dist: anyio==3.6.2
+Requires-Dist: typing-extensions==4.6.3
 Description-Content-Type: text/markdown
 
 # aioarp
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aioarp.svg)](https://pypi.org/project/aioarp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aioarp.svg)](https://pypi.org/project/aioarp)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [ARP request](#sending-arp-requests)
+- [ARP response](#arp-response)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install aioarp
 ```
 
-## License
-
-`aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-## Sending ARP requests
+## How to send ARP requests
 
 ### Sync
 ```python
 >>> import aioarp
 >>> response = aioarp.request('enp0s3', '10.0.2.2')
 >>> print(response.sender_mac)
 ee:xx:aa:mm:pp:le  # mac address
@@ -85,22 +84,22 @@
 
 If you want, you can explicitly set all of the **ARP** headers. To do so, create the `ArpPacket` instance yourself and then ask `aioarp` to send that request.
 
 ```python
 >>> import aioarp
 >>>
 >>> arp_packet = aioarp.ArpPacket(
-... hardware_type=aioarp.HardwareType.ethernet,
-... protocol_type=aioarp.Protocol.ip,
-... sender_mac='11:11:11:11:11:11',
-... sender_ip='127.0.0.1',
-... target_mac='11:11:11:11:11:11',
-... target_ip='127.0.0.1',)
+...     hardware_type=aioarp.HardwareType.ethernet,
+...     protocol_type=aioarp.Protocol.ip,
+...     sender_mac='11:11:11:11:11:11',
+...     sender_ip='127.0.0.1',
+...     target_mac='11:11:11:11:11:11',
+...     target_ip='127.0.0.1')
 >>>
->>> response = aioarp.sync_send_arp(arp_packet, 'enp0s3')
+>>> response = aioarp.sync_send_arp(arp_packet, aioarp.Stream('enp0s3'))
 ```
 
 This is the packet that was sent over the network.
 
 ```
 Ethernet II, Src: Private_11:11:11 (11:11:11:11:11:11), Dst: Private_11:11:11 (11:11:11:11:11:11)
     Destination: Private_11:11:11 (11:11:11:11:11:11)
@@ -148,19 +147,29 @@
 ```
 Each one has a distinct meaning, which can be found in https://en.wikipedia.org/wiki/Address_Resolution_Protocol.
 
 ## Failed Responses
 
 If the response is not received, aioarp should throw a `aioarp.NotFoundError` exception. 
 
-This occurs when the default arp request `timeout expires`. The timeout is set to 5 by default; in future releases, we will add a parameter to allow you to change that value.
+This occurs when the default arp request `timeout expires`. The timeout is set to 5 by default, but it can be changed by passing the `timeout` argument to the `request` function.
 
+Without timeout
 ```python
 >>> import aioarp
 >>>
 >>> try:
 ...     response = aioarp.request('enp0s3', '10.0.2.25')
 ...     print(response.opcode)
 ... except aioarp.NotFoundError:
 ...     print('10.0.2.25 was not found :(')
+
 ```
+With timeout
+```python
+response = aioarp.request('enp0s3', '10.0.2.25', timeout=0.5)
+```
+
+## License
+
+`aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

