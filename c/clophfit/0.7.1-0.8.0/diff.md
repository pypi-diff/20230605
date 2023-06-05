# Comparing `tmp/clophfit-0.7.1.tar.gz` & `tmp/clophfit-0.8.0.tar.gz`

## Comparing `clophfit-0.7.1.tar` & `clophfit-0.8.0.tar`

### file list

```diff
@@ -1,228 +1,235 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.1/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.7.1/.darglint
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.7.1/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.7.1/.readthedocs.yml
--rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 clophfit-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.7.1/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.7.1/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/Makefile
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/click.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/conf.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/api.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/binding.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/prenspire.rst
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/prtecan.rst
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/contributing.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/description.rst
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/development.rst
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/older.rst
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prenspire.rst
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prenspire.uml.rst
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prtecan.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prtecan.uml.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/references.rst
--rw-r--r--   0        0        0   172988 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    18269 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    54541 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_binding.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_oldscripts.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_prenspire.py
--rw-r--r--   0        0        0    26719 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.7.1/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 clophfit-0.7.1/README.md
--rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 clophfit-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 clophfit-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.0/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.8.0/.darglint
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 clophfit-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.8.0/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.8.0/.readthedocs.yml
+-rw-r--r--   0        0        0    16409 2020-02-02 00:00:00.000000 clophfit-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 clophfit-0.8.0/TODO.org
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.8.0/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.8.0/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/click.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/api.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/binding.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/prenspire.rst
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/prtecan.rst
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/contributing.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/description.rst
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/development.rst
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/older.rst
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prenspire.rst
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prenspire.uml.rst
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prtecan.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prtecan.uml.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/references.rst
+-rw-r--r--   0        0        0  1158929 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/__init__.py
+-rw-r--r--   0        0        0    12856 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0    22246 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/binding/fitting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/__init__.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    22071 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    54541 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_binding.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_prenspire.py
+-rw-r--r--   0        0        0    26719 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0   679291 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/G10.csv
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/NTT-G10_note.csv
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota.csv
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/H04.dat
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0   530592 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/tmp/A04 Cl.csv
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/tmp/NTT-A04-Cl_note.csv
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 clophfit-0.8.0/README.md
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 clophfit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 clophfit-0.8.0/PKG-INFO
```

### Comparing `clophfit-0.7.1/.pre-commit-config.yaml` & `clophfit-0.8.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,26 @@
       - id: mixed-line-ending
         exclude: "^tests/EnSpire/"
       - id: name-tests-test
         args: [--pytest-test-first]
       - id: requirements-txt-fixer
       - id: detect-private-key
       - id: trailing-whitespace # hyper
-        exclude: "^tests/EnSpire/"
+        exclude: "^tests/EnSpire/|^tests/data/tmp/"
 
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
     rev: v2.9.0
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+    rev: v0.0.270
     hooks:
       - id: ruff
         # args: [--exclude, "src/clophfit/prenspire/*"]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
@@ -64,17 +64,17 @@
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
-      - id: python-check-blanket-noqa
+      # - id: python-check-blanket-noqa
       # - id: python-check-blanket-type-ignore # same as ruff PGH
-      - id: python-no-eval
+      # - id: python-no-eval
       - id: python-use-type-annotations
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5 # Update me!
```

### Comparing `clophfit-0.7.1/CHANGELOG.md` & `clophfit-0.8.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,53 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.8.0 (2023-06-05)
+
+### Feat
+
+- **prenspire**: build and fit single-and-global SVD-or-band titrations
+- **clop**: fit_titration for old note
+- **clop**: `fit titration global old` and `fit titration old` as cli command
+- add \_\_version\_\_ for output into "Meas-{version}"
+
+### Test
+
+- **clop**: add test for new fit_titration cli
+
+### Docs
+
+- Add instruction to install auto completion
+
+### Build
+
+- remove pygrep-hook: python-check-blanket-noqa and python-no-eval
+- update coverage[toml] requirement from <7.2.7 to <7.2.8 (#272)
+- update pandas requirement from <2.0.2 to <2.0.3 (#271)
+- bump nbsphinx from 0.9.1 to 0.9.2 (#269)
+- bump ruff from 0.0.269 to 0.0.270 (#268)
+- update coverage[toml] requirement from <7.2.6 to <7.2.7 (#267)
+- update rpy2 requirement from <3.5.12 to <3.5.13 (#265)
+- bump ruff from 0.0.267 to 0.0.269 (#264)
+
+### Refactor
+
+- **prenspire**: new Note (titration build) and fit_titration cmd; keep the old
+  ExpNote for compatibility with old note files.
+- **prenspire**: analyze_spectra_glob for SVD or multiple bands
+- **prenspire**: SVD spectra expand (with helpers functions) on old
+  `fit_titration` script
+
+### chore
+
+- update pre-commit hooks (#270)
+- update pre-commit hooks (#266)
+
 ## v0.7.1 (2023-05-18)
 
 ### Fix
 
 - **docs**: README links to pages
 
 ### Docs
```

### Comparing `clophfit-0.7.1/cz_customize_info.txt` & `clophfit-0.8.0/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/.github/workflows/ci.yml` & `clophfit-0.8.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
           ver=`echo ${{ github.event.head_commit.message }} | awk '{ print $NF }'`
           echo "ver=${ver}" >> $GITHUB_OUTPUT
           echo "ver=${ver}" >> $GITHUB_ENV
       - name: Run clop
         run: |
           python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ clophfit==${{ env.ver }}
           clop --version
-          clop prtecan tests/Tecan/list.pH
+          clop pr.tecan tests/Tecan/list.pH
           cat out2/metadata-labels.txt
 
   release:
     name: Release to github
     needs: testpypi
     runs-on: ubuntu-latest
     steps:
```

### Comparing `clophfit-0.7.1/.github/workflows/docs.yml` & `clophfit-0.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/Makefile` & `clophfit-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/conf.py` & `clophfit-0.8.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2023, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
-release = "0.7.1"
+release = "0.8.0"
 html_title = "ClopHfit"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `clophfit-0.7.1/docs/index.rst` & `clophfit-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/make.bat` & `clophfit-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f1.png` & `clophfit-0.8.0/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f2.png` & `clophfit-0.8.0/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f3.png` & `clophfit-0.8.0/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f4.png` & `clophfit-0.8.0/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f5.png` & `clophfit-0.8.0/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f6.png` & `clophfit-0.8.0/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/bs_pd_f7.png` & `clophfit-0.8.0/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/csvtable.png` & `clophfit-0.8.0/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/emcee-01.png` & `clophfit-0.8.0/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/emcee-02.png` & `clophfit-0.8.0/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/emcee-11.png` & `clophfit-0.8.0/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/emcee-12.png` & `clophfit-0.8.0/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/f01.png` & `clophfit-0.8.0/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/file.png` & `clophfit-0.8.0/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit1.png` & `clophfit-0.8.0/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit2.png` & `clophfit-0.8.0/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit3.png` & `clophfit-0.8.0/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit4.png` & `clophfit-0.8.0/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit5.png` & `clophfit-0.8.0/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit6.png` & `clophfit-0.8.0/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/gR_fit7.png` & `clophfit-0.8.0/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/glmfit0.png` & `clophfit-0.8.0/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/glmfit1.png` & `clophfit-0.8.0/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/glmfit2.png` & `clophfit-0.8.0/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/glmfit3.png` & `clophfit-0.8.0/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/glmfit_np.r_.png` & `clophfit-0.8.0/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmfit1.png` & `clophfit-0.8.0/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmfit2.png` & `clophfit-0.8.0/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmfit3.png` & `clophfit-0.8.0/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmfit4.png` & `clophfit-0.8.0/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmfit5.png` & `clophfit-0.8.0/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel1.png` & `clophfit-0.8.0/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel2.png` & `clophfit-0.8.0/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel3.png` & `clophfit-0.8.0/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel4.png` & `clophfit-0.8.0/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel5.png` & `clophfit-0.8.0/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel6.png` & `clophfit-0.8.0/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/lmodel_H04.png` & `clophfit-0.8.0/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/note_file.png` & `clophfit-0.8.0/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/r_bs.png` & `clophfit-0.8.0/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.8.0/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.8.0/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R1.png` & `clophfit-0.8.0/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R2.png` & `clophfit-0.8.0/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R3.png` & `clophfit-0.8.0/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R4.png` & `clophfit-0.8.0/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R5.png` & `clophfit-0.8.0/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/ratio2P_R6.png` & `clophfit-0.8.0/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/_static/rpy_bs.png` & `clophfit-0.8.0/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/contributing.rst` & `clophfit-0.8.0/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/development.rst` & `clophfit-0.8.0/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/older.rst` & `clophfit-0.8.0/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/prenspire.uml.rst` & `clophfit-0.8.0/docs/references/prenspire.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/prtecan.rst` & `clophfit-0.8.0/docs/references/prtecan.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/references/prtecan.uml.rst` & `clophfit-0.8.0/docs/references/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/tutorials/prtecan.ipynb` & `clophfit-0.8.0/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/tutorials/usage.org` & `clophfit-0.8.0/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/tutorials/usage.rst` & `clophfit-0.8.0/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/tutorials/usage2.org` & `clophfit-0.8.0/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/docs/tutorials/usage2.rst` & `clophfit-0.8.0/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/dil_buffer.py` & `clophfit-0.8.0/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/dil_correction.py` & `clophfit-0.8.0/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/fit_rpy.py` & `clophfit-0.8.0/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/fit_titration.py` & `clophfit-0.8.0/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/fit_titration_global.py` & `clophfit-0.8.0/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/merge.py` & `clophfit-0.8.0/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/plot_tecan.py` & `clophfit-0.8.0/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.8.0/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/prenspire/__init__.py` & `clophfit-0.8.0/src/clophfit/prenspire/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/prenspire/prenspire.py` & `clophfit-0.8.0/src/clophfit/prenspire/prenspire.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Parses EnSpire data files."""
 from __future__ import annotations
 
+import collections
 import csv
+import datetime
 import typing
 import warnings
-from collections import Counter
-from collections import namedtuple
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 
 import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
 import pandas as pd
 import pyparsing
 
+from clophfit import __default_enspire_out_dir__
+from clophfit.prtecan import lookup_listoflines
+
 # TODO: kd1.csv kd2.csv kd3.csv kd1-nota kd2-nota kd3-nota --> Titration
 # TODO: Titration.data ['A' 'B' 'C'] -- global fit
-from clophfit.prtecan import lookup_listoflines
 
 
 def verbose_print(verbose: int) -> typing.Callable[..., typing.Any]:
     """Return print function when verbose output is True."""
     if verbose:
         return print
     else:
@@ -55,15 +57,16 @@
     ------
     Exception
         If unexpected format is found.
 
     Examples
     --------
     >>> from clophfit.prenspire import EnspireFile
-    >>> ef = EnspireFile("tests/EnSpire/h148g-spettroC.csv", verbose=0)
+    >>> from pathlib import Path
+    >>> ef = EnspireFile(Path("tests/EnSpire/h148g-spettroC.csv"), verbose=0)
     >>> ef.measurements['A']['lambda'][2]
     274.0
     """
 
     file: Path
     verbose: int = 0
     #: General metadata.
@@ -72,44 +75,50 @@
     measurements: dict[str, typing.Any] = field(default_factory=dict, init=False)
     #: List of exported wells.
     wells: list[str] = field(default_factory=list, init=False)
 
     def __post_init__(self) -> None:
         """Complete initialization."""
         verboseprint = verbose_print(self.verbose)
-        csvl = self._read_csv_file(Path(self.file), verboseprint)
+        csvl = self._read_csv_file(self.file, verboseprint)
         ini, fin = self._find_data_indices(csvl, verboseprint)
         self._ini, self._fin = ini, fin
         self._check_csvl_format(csvl, ini, fin, verboseprint)
         self._wells_platemap, self._platemap = self._extract_platemap(
             csvl[fin + 1 :], verboseprint
         )
         self.metadata = self._create_metadata(csvl[0 : ini - 2], csvl[fin + 1 :])
         self.wells, self.measurements = self._extract_measurements(
             csvl[ini - 1 : fin], csvl[fin + 1 :], verboseprint
         )
 
-    def export_measurements(self, output_dir: Path = Path("Meas")) -> None:
-        """Create table as DataFrame and plot; save into Meas folder."""
-        output_dir.mkdir(parents=True, exist_ok=True)
+    def export_measurements(self, out_dir: Path = __default_enspire_out_dir__) -> None:
+        """Save measurements, metadata and plots into out_dir."""
+        out_dir.mkdir(parents=True, exist_ok=True)
         for m in self.measurements:
-            data_dict = {"lambda": list(map(float, self.measurements[m]["lambda"]))}
-            data_dict.update(
-                {w: list(map(float, self.measurements[m][w])) for w in self.wells}
-            )
+            # Prepare data dictionary and construct DataFrame
+            data_dict = {"lambda": self.measurements[m]["lambda"]}
+            data_dict.update({w: self.measurements[m][w] for w in self.wells})
             dfdata = pd.DataFrame(data=data_dict).set_index("lambda")
-            # Create plot
-            dfdata.plot(title=m, legend=False)
-            # Save files
-            file = output_dir / (self.file.stem + "_" + m + ".csv")
-            while file.exists():
-                # because with_stem was introduced in py3.9
-                file = file.with_name(file.stem + "-b" + file.suffix)
-            dfdata.to_csv(str(file))
-            plt.savefig(str(file.with_suffix(".png")))
+            basename = f"{self.file.stem}_{m}"
+            if (out_dir / f"{basename}.csv").exists():
+                timestamp = datetime.datetime.now(datetime.timezone.utc).strftime(
+                    "%Y%m%d%H%M%S"
+                )  # e.g. '20230518093055'
+                basename = f"{self.file.stem}_{m}_{timestamp}"
+            csv_file = out_dir / f"{basename}.csv"
+            md_file = out_dir / f"{basename}.json"
+            png_file = out_dir / f"{basename}.png"
+            dfdata.to_csv(csv_file)
+            pd.DataFrame([self.measurements[m]["metadata"]]).to_json(md_file, indent=4)
+            # Create and save plot
+            fig, ax = plt.subplots()
+            dfdata.plot(title=m, legend=False, ax=ax)
+            plt.savefig(png_file)
+            plt.close(fig)
 
     # Helpers
     def _read_csv_file(
         self, file: Path, verboseprint: typing.Callable[..., typing.Any]
     ) -> list[list[str]]:
         """Read EnSpire exported file into csvl."""
         csvl = list(csv.reader(file.open(encoding="iso-8859-1"), dialect="excel-tab"))
@@ -252,35 +261,35 @@
         if wells != self._wells_platemap:
             msg = "well_list from data_list and platemap differ. It might be that you did not export data for all acquired wells"
             warnings.warn(msg, stacklevel=2)
 
         # Monochromator is expected to be either Exc or Ems
         for k, measurement in measurements.items():
             label = f"Meas{k}"
-            heading = namedtuple("heading", "ex em res")
+            heading = collections.namedtuple("heading", "ex em res")
             head = heading(
                 f"{label}WavelengthExc", f"{label}WavelengthEms", f"{label}Result"
             )
             # excitation spectra must have only one emission wavelength
             if measurement["metadata"]["Monochromator"] == "Excitation":
                 x = [r for r in dfdata[head.em] if r]
-                c = Counter(x)
+                c = collections.Counter(x)
                 if (
                     len(c) != 1
                     or list(c.keys())[0] != measurement["metadata"]["Wavelength"]
                 ):
                     msg = f"Excitation spectra with unexpected emission in {label}"
                     raise CsvLineError(msg)
                 measurement["lambda"] = [
                     float(r) for r in dfdata[head.ex][dfdata.Well == wells[0]] if r
                 ]
             # emission spectra must have only one excitation wavelength
             elif measurement["metadata"]["Monochromator"] == "Emission":
                 x = [r for r in dfdata[head.ex] if r]
-                c = Counter(x)
+                c = collections.Counter(x)
                 if (
                     len(c) != 1
                     or list(c.keys())[0] != measurement["metadata"]["Wavelength"]
                 ):
                     msg = f"Emission spectra with unexpected excitation in {label}"
                     raise CsvLineError(msg)
                 measurement["lambda"] = [
@@ -357,15 +366,15 @@
         headerdata: list[str],
         measurements: dict[str, typing.Any],
         verboseprint: typing.Callable[..., typing.Any],
     ) -> bool:
         """Check header and measurements.keys()."""
         counter_constant = 3  # Not sure, maybe for md with units. <Exc, Ems, F>
         meas = [line.split(":")[0].replace("Meas", "") for line in headerdata]
-        b = {k for k, v in Counter(meas).items() if v == counter_constant}
+        b = {k for k, v in collections.Counter(meas).items() if v == counter_constant}
         a = set(measurements.keys())
         verboseprint("check header and measurements.keys()", a == b, a, b)
         return a == b
 
 
 @dataclass
 class ExpNote:
@@ -454,14 +463,79 @@
                     ),
                 )
             self.titrations.append(Titration(conc, data, ph=ph))
 
         # TODO: BUFFER
 
 
+@dataclass
+class Note:
+    """Read and processes an Experimental Note file."""
+
+    fpath: Path
+    verbose: int = 0
+    #: A list of wells generated from the note file.
+    wells: list[str] = field(init=False, default_factory=list)
+    # A list of lines extracted from the note file.
+    _note: pd.DataFrame = field(init=False, default_factory=pd.DataFrame)
+    #: A list of titrations extracted from the note file.
+    titrations: dict[typing.Any, typing.Any] = field(init=False, default_factory=dict)
+
+    def __post_init__(self) -> None:
+        """Complete the initialization generating wells and _note_list."""
+        verboseprint = verbose_print(self.verbose)
+        with self.fpath.open("r", newline="") as file:
+            sample_data = file.read(1024)  # Read a sample of the CSV data
+        dialect = typing.cast(csv.Dialect, csv.Sniffer().sniff(sample_data))
+        self._note = pd.read_csv(self.fpath, dialect=dialect)
+        self.wells: list[str] = np.array(self._note)[1:, 0].tolist()
+        verboseprint(f"Wells {self.wells[:2]}...{self.wells[-2:]} generated.")
+
+    def build_titrations(self, ef: EnspireFile) -> None:
+        """Extract titrations from the given ef (_note file like: <well, pH, Cl>)."""
+        df_no_buffer = self._note.query('Name != "buffer"')
+        threshold = 3
+        grouped0 = df_no_buffer.groupby("Name")
+        titrations: dict[typing.Any, typing.Any] = {}
+        for name0, group0 in grouped0:
+            grouped1 = group0.groupby("Temp")
+            titrations[name0] = {}
+            for name1, group1 in grouped1:
+                titrations[name0][name1] = {}
+                # Group by 'pH' and 'Cl' and keep only groups with more than 'threshold' rows.
+                for grouping in ["pH", "Cl"]:
+                    grouped2 = group1.groupby(grouping)
+                    for name2, group2 in grouped2:
+                        if len(group2) > threshold:
+                            grouped3 = group2.groupby("Labels")
+                            for name3, group3 in grouped3:
+                                wells = group3["Well"].to_list()
+                                meas_dict = {}
+                                for label in str(name3).split():
+                                    d = {w: ef.measurements[label][w] for w in wells}
+                                    value_df = pd.DataFrame(
+                                        d,
+                                        index=ef.measurements[label]["lambda"],
+                                        columns=wells,
+                                    )
+                                    if group3["pH"].nunique() > group3["Cl"].nunique():
+                                        value_df.columns = pd.Index(
+                                            group3["pH"].to_list()
+                                        )
+                                    else:
+                                        value_df.columns = pd.Index(
+                                            group3["Cl"].to_list()
+                                        )
+                                    meas_dict[label] = value_df
+                                titrations[name0][name1][
+                                    f"{grouping}_{name2}"
+                                ] = meas_dict
+        self.titrations = titrations
+
+
 class Titration:
     """Store titration data and fit results."""
 
     def __init__(
         self,
         conc: typing.Sequence[float],
         data: dict[str, pd.DataFrame],
```

### Comparing `clophfit-0.7.1/src/clophfit/prtecan/__init__.py` & `clophfit-0.8.0/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/src/clophfit/prtecan/prtecan.py` & `clophfit-0.8.0/src/clophfit/prtecan/prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/test_cli.py` & `clophfit-0.8.0/tests/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     expected = tpath / "EnSpire" / "cli" / "output"
     input_csv = tpath / "EnSpire" / "cli" / "NTT_37C_pKa.csv"
     out = tmp_path / "E"
     out.mkdir()
     runner = CliRunner()
     result = runner.invoke(
         clop,
-        ["prenspire", str(input_csv), "--out", str(out)],
+        ["pr.enspire", str(input_csv), "--out", str(out)],
     )
     assert result.exit_code == 0
     # validate output files
     assert (out / "NTT_37C_pKa_A.csv").exists()
     assert (out / "NTT_37C_pKa_B.csv").exists()
     assert (out / "NTT_37C_pKa_A.png").exists()
     assert (out / "NTT_37C_pKa_B.png").exists()
@@ -56,10 +56,45 @@
     lfile = str(tpath / "Tecan" / "140220" / "list.pH")
     sfile = str(tpath / "Tecan" / "140220" / "scheme.txt")
     out = tmp_path / "out3"
     out.mkdir()
     runner = CliRunner()
     result = runner.invoke(
         clop,
-        ["prtecan", lfile, "--out", str(out), "--fit", "--scheme", sfile, "--bg"],
+        ["pr.tecan", lfile, "--out", str(out), "--fit", "--scheme", sfile, "--bg"],
     )
     assert result.exit_code == 0
+
+
+@pytest.mark.parametrize(
+    ("csv_file", "expected_output", "additional_params"),
+    [
+        ("A04 Cl_A.csv", " K :  13.64  14.28  14.86  15.44  16.04  16.71  17.51", None),
+        ("A04 Cl_A.csv", " K :  13.52  14.11  14.66  15.20", ["-b", "480", "530"]),
+        ("A04 Cl_B.csv", " K :  12.73  13.46  14.14  14.82  15.54  16.35  17.32", None),
+        ("A04 Cl_B.csv", " K :  12.93  13.66  14.34  15.02", ["-b", "480", "530"]),
+    ],
+)
+def test_fit_titration(
+    csv_file: str, expected_output: str, additional_params: list[str], tmp_path: Path
+) -> None:
+    """Test the old ``fit_titration.py`` script with actual data and validate output."""
+    note_fp = tpath / "data" / "NTT-A04-Cl_note"
+    csv_fp = tpath / "data" / "Meas" / csv_file
+    out = tmp_path / "tit_fit"
+    out.mkdir()
+    runner = CliRunner()
+    base_args = ["fit_titration", str(csv_fp), str(note_fp)]
+    base_args.extend(["-t", "cl", "-d", str(out)])
+    if additional_params:
+        base_args.extend(additional_params)
+        sbands = f"({additional_params[1]}, {additional_params[2]})"
+    else:
+        sbands = "None"
+    result = runner.invoke(clop, base_args)
+    print(result.exc_info)
+    print(result.output)
+    assert result.exit_code == 0
+    assert expected_output in result.output
+    # Asserting that PDF is created
+    expected_pdf_filename = out / f"{csv_fp.stem}_{sbands}_{note_fp.stem}.pdf"
+    assert expected_pdf_filename.exists()
```

### Comparing `clophfit-0.7.1/tests/test_oldscripts.py` & `clophfit-0.8.0/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/test_prenspire.py` & `clophfit-0.8.0/tests/test_prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/test_prtecan.py` & `clophfit-0.8.0/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.8.0/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.8.0/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/h148g-spettroC.csv` & `clophfit-0.8.0/tests/EnSpire/h148g-spettroC.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/cli/NTT_37C_pKa.csv` & `clophfit-0.8.0/tests/EnSpire/cli/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv` & `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png` & `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv` & `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png` & `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv` & `clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv` & `clophfit-0.8.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_100.xls` & `clophfit-0.8.0/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_150.xls` & `clophfit-0.8.0/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_20.xls` & `clophfit-0.8.0/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_5.78.xls` & `clophfit-0.8.0/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_50.xls` & `clophfit-0.8.0/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_6.38.xls` & `clophfit-0.8.0/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_6.83.xls` & `clophfit-0.8.0/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_7.24.xls` & `clophfit-0.8.0/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_7.67.xls` & `clophfit-0.8.0/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_8.23.xls` & `clophfit-0.8.0/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_8.82.xls` & `clophfit-0.8.0/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290212_9.31.xls` & `clophfit-0.8.0/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290513_5.5.xls` & `clophfit-0.8.0/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.8.0/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290513_7.2.xls` & `clophfit-0.8.0/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/290513_8.8.xls` & `clophfit-0.8.0/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.8.0/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.8.0/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/fit0.csv` & `clophfit-0.8.0/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.8.0/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/fit1.csv` & `clophfit-0.8.0/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.8.0/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.8.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.8.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.8.0/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.8.0/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/A01-20140311a.dat` & `clophfit-0.8.0/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/A01.dat` & `clophfit-0.8.0/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/NTT-A04-Cl_note` & `clophfit-0.8.0/tests/data/NTT-A04-Cl_note`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 well	pH	Cl	mutant
 E01	5.2	0	NTT-A04
-E02	5.2	5	NTT-A04
+E02	5.2	5.0	NTT-A04
 E03	5.2	10	NTT-A04
 E04	5.2	20	NTT-A04
 E05	5.2	40	NTT-A04
 E06	5.2	80	NTT-A04
 E07	5.2	200	NTT-A04
 E08	5.2	500	NTT-A04
 E09	5.2	1000	NTT-A04
```

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.8.0/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/k/D05.dat-bs.png` & `clophfit-0.8.0/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/k/D05.dat.png` & `clophfit-0.8.0/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.8.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.8.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.8.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.8.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.8.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.8.0/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/.gitignore` & `clophfit-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/LICENSE.txt` & `clophfit-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.1/README.md` & `clophfit-0.8.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,27 +6,38 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.7.1"
+- Version: "0.8.0"
 
 ## Installation
 
-You can get the library directly from
-[PyPI](https://pypi.org/project/ClopHfit/):
+You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
+using `pip`:
 
     pip install clophfit
 
-or with [pipx](https://pypa.github.io/pipx/):
+Alternatively, you can use [pipx](https://pypa.github.io/pipx/) to install it in
+an isolated environment:
 
     pipx install clophfit
 
+To enable auto completion for the `clop` command, follow these steps:
+
+1.  Generate the completion script by running the following command:
+
+        _CLOP_COMPLETE=bash_source clop > ~/.local/bin/clop-complete.bash
+
+2.  Source the generated completion script to enable auto completion:
+
+        source ~/.local/bin/clop-complete.bash
+
 ## Usage
 
 You can check out the documentation on <https://darosio.github.io/ClopHfit> for
 up to date usage information and examples.
 
 ### CLI
```

### Comparing `clophfit-0.7.1/pyproject.toml` & `clophfit-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   'click < 8.1.4',
   'corner < 2.2.3',
   'emcee < 3.1.5',
   'lmfit < 1.2.2',
   'matplotlib < 3.7.2',
   'numpy < 1.24.4',
   'openpyxl < 3.1.3',
-  'pandas < 2.0.2',
-  'rpy2 < 3.5.12',
+  'pandas < 2.0.3',
+  'rpy2 < 3.5.13',
   'scipy < 1.10.2',
   'seaborn < 0.12.3',
   'sympy < 1.13.0',
   'tqdm < 4.65.1',
   'xlrd < 2.0.2'
 ]
 description = "Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra."
@@ -44,47 +44,49 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.7.1"
+version = "0.8.0"
 
 [project.optional-dependencies]
 dev = [
   "commitizen < 3.2.3",
   "ipykernel",
   "jupyter",
-  "ruff == 0.0.267",
+  "ruff == 0.0.270",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
   "autodocsumm == 0.2.11",
   # "myst-parser == 1.0.0",
-  "nbsphinx == 0.9.1",
+  "nbsphinx == 0.9.2",
   "pydata-sphinx-theme == 0.13.3",
   "Sphinx == 7.0.1",
   "sphinx-click == 4.4.0",
   "sphinx_autodoc_typehints == 1.23.0",
   "sphinxcontrib-plantuml == 0.25"
 ]
 tests = [
-  "coverage[toml] < 7.2.6",
+  "coverage[toml] < 7.2.8",
   "mypy < 1.4",
   "pandas-stubs == 2.0.1.230501",
   "Pygments < 2.15.2",
   "pytest < 7.3.2",
   "typeguard == 4.0.0",
   "xdoctest < 1.1.2"
 ]
 
 [project.scripts]
 "clop" = "clophfit.__main__:clop"
+"fit_titration_global_old" = "clophfit.old.fit_titration_global:main"
+"fit_titration_old" = "clophfit.old.fit_titration:main"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/darosio/ClopHfit/issues"
 Changelog = "https://darosio.github.io/ClopHfit/misc/CHANGELOG.html"
 Discussions = "https://github.com/darosio/ClopHfit/discussions"
 Documentation = "https://clophfit.readthedocs.io"
 "Github releases" = "https://github.com/darosio/ClopHfit/releases"
@@ -106,15 +108,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.7.1"
+version = "0.8.0"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
@@ -175,15 +177,15 @@
 exclude_lines = [
   "pragma: no cover"
 ]
 show_missing = true
 
 [tool.coverage.run]
 branch = true
-omit = ["*__init__.py"]
+omit = ["*__init__.py", "*/old/*"]
 source = ["clophfit", "tests"]
 
 [tool.hatch.envs.coverage]
 dependencies = ["coverage[toml]>=7.1.0"]  # XXX:
 detached = true
 
 [tool.hatch.envs.coverage.scripts]
```

### Comparing `clophfit-0.7.1/PKG-INFO` & `clophfit-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.7.1
+Version: 0.8.0
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -27,38 +27,38 @@
 Requires-Dist: click<8.1.4
 Requires-Dist: corner<2.2.3
 Requires-Dist: emcee<3.1.5
 Requires-Dist: lmfit<1.2.2
 Requires-Dist: matplotlib<3.7.2
 Requires-Dist: numpy<1.24.4
 Requires-Dist: openpyxl<3.1.3
-Requires-Dist: pandas<2.0.2
-Requires-Dist: rpy2<3.5.12
+Requires-Dist: pandas<2.0.3
+Requires-Dist: rpy2<3.5.13
 Requires-Dist: scipy<1.10.2
 Requires-Dist: seaborn<0.12.3
 Requires-Dist: sympy<1.13.0
 Requires-Dist: tqdm<4.65.1
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
 Requires-Dist: commitizen<3.2.3; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff==0.0.267; extra == 'dev'
+Requires-Dist: ruff==0.0.270; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
-Requires-Dist: nbsphinx==0.9.1; extra == 'docs'
+Requires-Dist: nbsphinx==0.9.2; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints==1.23.0; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
 Requires-Dist: sphinx==7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-plantuml==0.25; extra == 'docs'
 Provides-Extra: tests
-Requires-Dist: coverage[toml]<7.2.6; extra == 'tests'
+Requires-Dist: coverage[toml]<7.2.8; extra == 'tests'
 Requires-Dist: mypy<1.4; extra == 'tests'
 Requires-Dist: pandas-stubs==2.0.1.230501; extra == 'tests'
 Requires-Dist: pygments<2.15.2; extra == 'tests'
 Requires-Dist: pytest<7.3.2; extra == 'tests'
 Requires-Dist: typeguard==4.0.0; extra == 'tests'
 Requires-Dist: xdoctest<1.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
@@ -71,27 +71,38 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.7.1"
+- Version: "0.8.0"
 
 ## Installation
 
-You can get the library directly from
-[PyPI](https://pypi.org/project/ClopHfit/):
+You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
+using `pip`:
 
     pip install clophfit
 
-or with [pipx](https://pypa.github.io/pipx/):
+Alternatively, you can use [pipx](https://pypa.github.io/pipx/) to install it in
+an isolated environment:
 
     pipx install clophfit
 
+To enable auto completion for the `clop` command, follow these steps:
+
+1.  Generate the completion script by running the following command:
+
+        _CLOP_COMPLETE=bash_source clop > ~/.local/bin/clop-complete.bash
+
+2.  Source the generated completion script to enable auto completion:
+
+        source ~/.local/bin/clop-complete.bash
+
 ## Usage
 
 You can check out the documentation on <https://darosio.github.io/ClopHfit> for
 up to date usage information and examples.
 
 ### CLI
```

