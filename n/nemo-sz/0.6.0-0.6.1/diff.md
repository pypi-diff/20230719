# Comparing `tmp/nemo-sz-0.6.0.tar.gz` & `tmp/nemo-sz-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo-sz-0.6.0.tar", last modified: Fri Jul 14 12:08:04 2023, max compression
+gzip compressed data, was "nemo-sz-0.6.1.tar", last modified: Wed Jul 19 10:22:57 2023, max compression
```

## Comparing `nemo-sz-0.6.0.tar` & `nemo-sz-0.6.1.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1694 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/INSTALL.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     1531 2020-11-05 07:18:13.000000 nemo-sz-0.6.0/LICENSE
--rw-rw-r--   0 matty     (1000) matty     (1000)      343 2021-11-17 08:09:46.000000 nemo-sz-0.6.0/MANIFEST.in
--rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/PKG-INFO
--rw-rw-r--   0 matty     (1000) matty     (1000)     2132 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/README.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/bin/
--rw-rw-r--   0 matty     (1000) matty     (1000)     8401 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemo
--rw-rw-r--   0 matty     (1000) matty     (1000)     5336 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/bin/nemoCatalogCheck
--rw-rw-r--   0 matty     (1000) matty     (1000)    23560 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemoMass
--rw-rw-r--   0 matty     (1000) matty     (1000)     4274 2022-08-24 09:10:58.000000 nemo-sz-0.6.0/bin/nemoMock
--rw-rw-r--   0 matty     (1000) matty     (1000)    18345 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemoModel
--rw-rw-r--   0 matty     (1000) matty     (1000)     6385 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/bin/nemoSpec
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/docs/
--rw-rw-r--   0 matty     (1000) matty     (1000)      580 2019-02-24 16:16:40.000000 nemo-sz-0.6.0/docs/Makefile
--rw-rw-r--   0 matty     (1000) matty     (1000)     3317 2021-03-04 16:41:54.000000 nemo-sz-0.6.0/docs/advanced.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2310 2022-08-26 03:53:41.000000 nemo-sz-0.6.0/docs/commands.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     5731 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/docs/conf.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    38946 2022-01-11 13:00:45.000000 nemo-sz-0.6.0/docs/config.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2874 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/docs/development.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      261 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/dr3_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      225 2021-03-08 15:45:50.000000 nemo-sz-0.6.0/docs/dr5_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      634 2021-10-01 12:20:40.000000 nemo-sz-0.6.0/docs/index.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)       89 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/install.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     6167 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/docs/outputs.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      194 2021-02-17 16:06:52.000000 nemo-sz-0.6.0/docs/quickstart.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      976 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/docs/reference.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      253 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/sosims_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)       79 2020-11-11 10:23:57.000000 nemo-sz-0.6.0/docs/testing.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      123 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/tutorials.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/examples/
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR3-clusters/
--rw-rw-r--   0 matty     (1000) matty     (1000)  8743680 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)  9696960 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)    74880 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/E-D56Clusters.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)     8262 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     7063 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     3816 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56_quick.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)   412359 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/
--rw-rw-r--   0 matty     (1000) matty     (1000)   240000 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     4656 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/selFnExample.py
--rw-rw-r--   0 matty     (1000) matty     (1000)   138534 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/surveyMask.fits.gz
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR5-clusters/
--rw-rw-r--   0 matty     (1000) matty     (1000)      220 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.slurm
--rw-rw-r--   0 matty     (1000) matty     (1000)     6184 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      712 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     3429 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/README.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/SOSims/
--rw-rw-r--   0 matty     (1000) matty     (1000)      824 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/HEALPIX_TO_CAR.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      224 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_BEAMS.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_MOCKS_SMALL.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_MOCKS_TILES.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     6258 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_small.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6618 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     3132 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/NzCheck.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     9122 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      583 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1475 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/combineComponentMaps.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1457 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/createSurveyMask.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     3443 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/healpix2CAR.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      876 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/makeGaussianBeam.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1429 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/makeRedshiftsCatalog.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     2081 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/readWebSkyInputCatalog.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     4554 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/selFnExample.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      203 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_cosmo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      205 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_mass.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      273 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_nemo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      292 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_small_cosmo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     1255 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/surveyMask.reg
--rw-rw-r--   0 matty     (1000) matty     (1000)     1237 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_AdvACT.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_E-D56.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_small.txt
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/SOSims/validationScripts/
--rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     5366 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     5188 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6703 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6787 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/TILe-C/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1030 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/TILe-C/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     4238 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/TILe-C/y_f090beam.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/clustercal/
--rw-rw-r--   0 matty     (1000) matty     (1000)       22 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     9692 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/clustercal.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6420 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/makeConfigs.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     5375 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/template_singlefreq.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/quickstart/
--rw-rw-r--   0 matty     (1000) matty     (1000)     2900 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     4966 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/quickstart-clusters.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1823 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/quickstart-sources.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/sources/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1410 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_E-D56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1385 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_deep56_s15_f090.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1541 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_deep8.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8852 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S16_f090_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8870 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S16_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2813 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f090_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f150_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      168 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     7784 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     7960 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_f150_act+planck_day+night.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8901 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_f220_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      183 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)      172 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/RUN_PS.sh
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/nemo/
--rw-rw-r--   0 matty     (1000) matty     (1000)    31319 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/MockSurvey.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      499 2020-01-29 14:51:01.000000 nemo-sz-0.6.0/nemo/__init__.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      497 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/nemo/_version.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    39014 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/catalogs.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    88877 2023-07-14 12:02:44.000000 nemo-sz-0.6.0/nemo/completeness.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/nemo/data/
--rw-rw-r--   0 matty     (1000) matty     (1000)   140701 2019-03-11 10:14:35.000000 nemo-sz-0.6.0/nemo/data/planck_lensedCls.dat
--rw-rw-r--   0 matty     (1000) matty     (1000)    67692 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/filters.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     4464 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/nemo/gnfw.py
--rw-rw-r--   0 matty     (1000) matty     (1000)   127604 2023-07-14 12:05:05.000000 nemo-sz-0.6.0/nemo/maps.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    26084 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/photometry.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    55311 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/pipelines.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1576 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/plotSettings.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    72242 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/signals.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    40957 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/startUp.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/nemo_sz.egg-info/
--rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/PKG-INFO
--rw-rw-r--   0 matty     (1000) matty     (1000)     4198 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/SOURCES.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)        1 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/dependency_links.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)      121 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/requires.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)        5 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/top_level.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)       81 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/pyproject.toml
--rw-rw-r--   0 matty     (1000) matty     (1000)      192 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/setup.cfg
--rw-rw-r--   0 matty     (1000) matty     (1000)     2019 2023-07-13 15:43:22.000000 nemo-sz-0.6.0/setup.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/tests/
--rw-rw-r--   0 matty     (1000) matty     (1000)      977 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2157 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/clusters.robot
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/tests/configs/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/configs/MPITestSurveyMaskHeader.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1324 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_E-D56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1430 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_south2008.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1233 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_south2008_fourier.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      255 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     3442 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/equD56_quick_fourier.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6660 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/quickstart-multipass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2022-11-15 08:06:49.000000 nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     5732 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_B12_MFMF_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6038 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_MFMF.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6107 2022-11-15 08:07:19.000000 nemo-sz-0.6.0/tests/configs/sim_cl_MFMF_pass2.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1365 2022-01-11 13:00:45.000000 nemo-sz-0.6.0/tests/configs/sim_ptsrc_f090.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/smallTestSurveyMaskHeader.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1227 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/debug.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/tests/lib/
--rw-rw-r--   0 matty     (1000) matty     (1000)    17643 2022-01-21 15:05:26.000000 nemo-sz-0.6.0/tests/lib/NemoTests.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     2422 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/point_sources.robot
--rw-rw-r--   0 matty     (1000) matty     (1000)     5896 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/quick.robot
--rw-rw-r--   0 matty     (1000) matty     (1000)    70144 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/versioneer.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1694 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/INSTALL.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1531 2020-11-05 07:18:13.000000 nemo-sz-0.6.1/LICENSE
+-rw-rw-r--   0 matty     (1000) matty     (1000)      343 2021-11-17 08:09:46.000000 nemo-sz-0.6.1/MANIFEST.in
+-rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/PKG-INFO
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2132 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/README.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.587916 nemo-sz-0.6.1/bin/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8401 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/bin/nemo
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5336 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/bin/nemoCatalogCheck
+-rw-rw-r--   0 matty     (1000) matty     (1000)    23591 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/bin/nemoMass
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4274 2022-08-24 09:10:58.000000 nemo-sz-0.6.1/bin/nemoMock
+-rw-rw-r--   0 matty     (1000) matty     (1000)    18345 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/bin/nemoModel
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6385 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/bin/nemoSpec
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.587916 nemo-sz-0.6.1/docs/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      580 2019-02-24 16:16:40.000000 nemo-sz-0.6.1/docs/Makefile
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3317 2021-03-04 16:41:54.000000 nemo-sz-0.6.1/docs/advanced.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2310 2022-08-26 03:53:41.000000 nemo-sz-0.6.1/docs/commands.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5731 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/docs/conf.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    38946 2022-01-11 13:00:45.000000 nemo-sz-0.6.1/docs/config.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2874 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/docs/development.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      261 2021-02-17 13:10:21.000000 nemo-sz-0.6.1/docs/dr3_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      225 2021-03-08 15:45:50.000000 nemo-sz-0.6.1/docs/dr5_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      634 2021-10-01 12:20:40.000000 nemo-sz-0.6.1/docs/index.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)       89 2021-02-17 13:10:21.000000 nemo-sz-0.6.1/docs/install.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6167 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/docs/outputs.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      194 2021-02-17 16:06:52.000000 nemo-sz-0.6.1/docs/quickstart.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      976 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/docs/reference.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      253 2021-02-17 13:10:21.000000 nemo-sz-0.6.1/docs/sosims_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)       79 2020-11-11 10:23:57.000000 nemo-sz-0.6.1/docs/testing.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      123 2021-02-17 13:10:21.000000 nemo-sz-0.6.1/docs/tutorials.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.583916 nemo-sz-0.6.1/examples/
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.607915 nemo-sz-0.6.1/examples/ACT-DR3-clusters/
+-rw-rw-r--   0 matty     (1000) matty     (1000)  8743680 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/ACTPol_clusters.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)  9696960 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/ACTPol_redshifts.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)    74880 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/E-D56Clusters.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8262 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7063 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/equD56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3816 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/equD56_quick.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)   412359 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/pointSourceMask.fits.gz
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.607915 nemo-sz-0.6.1/examples/ACT-DR3-clusters/profiles_ACT/
+-rw-rw-r--   0 matty     (1000) matty     (1000)   240000 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4656 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/selFnExample.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)   138534 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR3-clusters/surveyMask.fits.gz
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.607915 nemo-sz-0.6.1/examples/ACT-DR5-clusters/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      220 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR5-clusters/DR5ClusterSearch.slurm
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6184 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR5-clusters/DR5ClusterSearch.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      712 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR5-clusters/FETCH_MAPS.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3429 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/ACT-DR5-clusters/README.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.611915 nemo-sz-0.6.1/examples/SOSims/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      824 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/HEALPIX_TO_CAR.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      224 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/MAKE_BEAMS.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/MAKE_MOCKS_SMALL.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/MAKE_MOCKS_TILES.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6258 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/MFMF_SOSim_3freq_small.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6618 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/MFMF_SOSim_3freq_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3132 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/NzCheck.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     9122 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      583 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1475 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/combineComponentMaps.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1457 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/createSurveyMask.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3443 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/healpix2CAR.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      876 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/makeGaussianBeam.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1429 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/makeRedshiftsCatalog.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2081 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/readWebSkyInputCatalog.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4554 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/selFnExample.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      203 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/slurm_cosmo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      205 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/slurm_mass.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      273 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/slurm_nemo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      292 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/slurm_small_cosmo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1255 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/surveyMask.reg
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1237 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/template_AdvACT.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/template_E-D56.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/template_small.txt
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.615915 nemo-sz-0.6.1/examples/SOSims/validationScripts/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/validationScripts/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5366 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/validationScripts/checkMassRecovery.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5188 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/validationScripts/checkMassRecovery_M200m.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6703 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6787 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.615915 nemo-sz-0.6.1/examples/TILe-C/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1030 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/TILe-C/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4238 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/TILe-C/y_f090beam.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.615915 nemo-sz-0.6.1/examples/clustercal/
+-rw-rw-r--   0 matty     (1000) matty     (1000)       22 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/clustercal/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     9692 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/clustercal/clustercal.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6420 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/clustercal/makeConfigs.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5375 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/clustercal/template_singlefreq.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.615915 nemo-sz-0.6.1/examples/quickstart/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2900 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/quickstart/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4966 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/quickstart/quickstart-clusters.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1823 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/quickstart/quickstart-sources.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.619915 nemo-sz-0.6.1/examples/sources/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1410 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PSExample_E-D56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1385 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PSExample_deep56_s15_f090.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1541 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PSExample_deep8.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8852 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S16_f090_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8870 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S16_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2813 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S18d_f090_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S18d_f150_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      168 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S18d_f220_202006.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7784 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S18d_f220_202006.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_S18d_f220_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7960 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_f150_act+planck_day+night.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8901 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/PS_f220_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      183 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)      172 2023-07-14 10:39:55.000000 nemo-sz-0.6.1/examples/sources/RUN_PS.sh
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/nemo/
+-rw-rw-r--   0 matty     (1000) matty     (1000)    31319 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/nemo/MockSurvey.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      499 2020-01-29 14:51:01.000000 nemo-sz-0.6.1/nemo/__init__.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      497 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/nemo/_version.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    39014 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/nemo/catalogs.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    88877 2023-07-14 12:02:44.000000 nemo-sz-0.6.1/nemo/completeness.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.619915 nemo-sz-0.6.1/nemo/data/
+-rw-rw-r--   0 matty     (1000) matty     (1000)   140701 2019-03-11 10:14:35.000000 nemo-sz-0.6.1/nemo/data/planck_lensedCls.dat
+-rw-rw-r--   0 matty     (1000) matty     (1000)    67684 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/nemo/filters.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4464 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/nemo/gnfw.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)   127595 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/nemo/maps.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    26085 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/nemo/photometry.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    57345 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/nemo/pipelines.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1576 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/nemo/plotSettings.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    72242 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/nemo/signals.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    40957 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/nemo/startUp.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.619915 nemo-sz-0.6.1/nemo_sz.egg-info/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-19 10:22:57.000000 nemo-sz-0.6.1/nemo_sz.egg-info/PKG-INFO
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4238 2023-07-19 10:22:57.000000 nemo-sz-0.6.1/nemo_sz.egg-info/SOURCES.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)        1 2023-07-19 10:22:57.000000 nemo-sz-0.6.1/nemo_sz.egg-info/dependency_links.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)      121 2023-07-19 10:22:57.000000 nemo-sz-0.6.1/nemo_sz.egg-info/requires.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)        5 2023-07-19 10:22:57.000000 nemo-sz-0.6.1/nemo_sz.egg-info/top_level.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)       81 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/pyproject.toml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      192 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/setup.cfg
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2019 2023-07-13 15:43:22.000000 nemo-sz-0.6.1/setup.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.619915 nemo-sz-0.6.1/tests/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      977 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/tests/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2157 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/clusters.robot
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/tests/configs/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/tests/configs/MPITestSurveyMaskHeader.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1324 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/PSTest_E-D56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1430 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/PSTest_south2008.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1233 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/PSTest_south2008_fourier.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      255 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3442 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/equD56_quick_fourier.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4969 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/tests/configs/quickstart-clusters-Q.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6660 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/tests/configs/quickstart-multipass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/tests/configs/sim_cl_A10_MFMF_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2022-11-15 08:06:49.000000 nemo-sz-0.6.1/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5732 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/tests/configs/sim_cl_B12_MFMF_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6038 2023-07-13 13:29:55.000000 nemo-sz-0.6.1/tests/configs/sim_cl_MFMF.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6107 2022-11-15 08:07:19.000000 nemo-sz-0.6.1/tests/configs/sim_cl_MFMF_pass2.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1365 2022-01-11 13:00:45.000000 nemo-sz-0.6.1/tests/configs/sim_ptsrc_f090.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/configs/smallTestSurveyMaskHeader.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1227 2021-11-17 06:29:36.000000 nemo-sz-0.6.1/tests/debug.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-19 10:22:57.623915 nemo-sz-0.6.1/tests/lib/
+-rw-rw-r--   0 matty     (1000) matty     (1000)    17984 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/tests/lib/NemoTests.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2422 2021-09-07 15:31:52.000000 nemo-sz-0.6.1/tests/point_sources.robot
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6537 2023-07-19 10:18:33.000000 nemo-sz-0.6.1/tests/quick.robot
+-rw-rw-r--   0 matty     (1000) matty     (1000)    70144 2021-02-17 13:10:21.000000 nemo-sz-0.6.1/versioneer.py
```

### Comparing `nemo-sz-0.6.0/INSTALL.rst` & `nemo-sz-0.6.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/LICENSE` & `nemo-sz-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/PKG-INFO` & `nemo-sz-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-sz
-Version: 0.6.0
+Version: 0.6.1
 Summary: Millimeter-wave galaxy cluster and source detection package.
 Home-page: https://nemo-sz.readthedocs.io
 Author: Matt Hilton + Nemo Contributors
 Author-email: hiltonm@ukzn.ac.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nemo-sz-0.6.0/README.rst` & `nemo-sz-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/bin/nemo` & `nemo-sz-0.6.1/bin/nemo`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/bin/nemoCatalogCheck` & `nemo-sz-0.6.1/bin/nemoCatalogCheck`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/bin/nemoMass` & `nemo-sz-0.6.1/bin/nemoMass`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     
     # Trim all filters except the reference one, then make catalog
     trimmedList=[]
     for mapFilter in config.parDict['mapFilters']:
         if mapFilter['label'] == config.parDict['photFilter']:
             trimmedList.append(mapFilter)
     config.parDict['mapFilters']=trimmedList
-    forcedTab=pipelines.filterMapsAndMakeCatalogs(config)
+    forcedTab=pipelines.filterMapsAndMakeCatalogs(config, useCachedFilteredMaps = True)
 
     # Need to graft the redshifts back on
     zMatched, forcedMatched, rDeg=catalogs.crossMatch(zTab, forcedTab)
     tab=forcedMatched
     tab.add_column(zMatched['redshift'])
     tab.add_column(zMatched['redshiftErr'])
     
@@ -318,15 +318,15 @@
         # Enter forced photometry mode if we can't find the columns we need
         # If we're doing forced photometry, we're going to need to set-up so we can find the filtered maps
         keysNeeded=['fixed_y_c', 'fixed_err_y_c']
         for key in keysNeeded:
             if key not in tab.keys():
                 forcedPhotometry=True
         config=startUp.NemoConfig(parDictFileName, MPIEnabled = args.MPIEnabled, divideTilesByProcesses = False,
-                                  setUpMaps = forcedPhotometry, writeTileDir = False, verbose = False,
+                                  setUpMaps = forcedPhotometry, writeTileInfo = False, verbose = False,
                                   strictMPIExceptions = strictMPIExceptions)
     
     # Remaining set-up
     massOptions=config.parDict['massOptions']
     Q=signals.QFit(QSource, selFnDir = config.selFnDir)
     fRelWeightsDict=signals.getFRelWeights(config)
```

### Comparing `nemo-sz-0.6.0/bin/nemoMock` & `nemo-sz-0.6.1/bin/nemoMock`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/bin/nemoModel` & `nemo-sz-0.6.1/bin/nemoModel`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/bin/nemoSpec` & `nemo-sz-0.6.1/bin/nemoSpec`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/Makefile` & `nemo-sz-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/advanced.rst` & `nemo-sz-0.6.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/commands.rst` & `nemo-sz-0.6.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/conf.py` & `nemo-sz-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/config.rst` & `nemo-sz-0.6.1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/development.rst` & `nemo-sz-0.6.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/index.rst` & `nemo-sz-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/outputs.rst` & `nemo-sz-0.6.1/docs/outputs.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/docs/reference.rst` & `nemo-sz-0.6.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/ACTPol_clusters.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/ACTPol_redshifts.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/E-D56Clusters.fits` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/E-D56Clusters.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/README.rst` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56.yml` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/equD56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56_quick.yml` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/equD56_quick.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/pointSourceMask.fits.gz`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/selFnExample.py` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/selFnExample.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR3-clusters/surveyMask.fits.gz` & `nemo-sz-0.6.1/examples/ACT-DR3-clusters/surveyMask.fits.gz`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml` & `nemo-sz-0.6.1/examples/ACT-DR5-clusters/DR5ClusterSearch.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh` & `nemo-sz-0.6.1/examples/ACT-DR5-clusters/FETCH_MAPS.sh`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/ACT-DR5-clusters/README.rst` & `nemo-sz-0.6.1/examples/ACT-DR5-clusters/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/HEALPIX_TO_CAR.sh` & `nemo-sz-0.6.1/examples/SOSims/HEALPIX_TO_CAR.sh`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_small.yml` & `nemo-sz-0.6.1/examples/SOSims/MFMF_SOSim_3freq_small.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml` & `nemo-sz-0.6.1/examples/SOSims/MFMF_SOSim_3freq_tiles.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/NzCheck.py` & `nemo-sz-0.6.1/examples/SOSims/NzCheck.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/README.rst` & `nemo-sz-0.6.1/examples/SOSims/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml` & `nemo-sz-0.6.1/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/combineComponentMaps.py` & `nemo-sz-0.6.1/examples/SOSims/combineComponentMaps.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/createSurveyMask.py` & `nemo-sz-0.6.1/examples/SOSims/createSurveyMask.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/healpix2CAR.py` & `nemo-sz-0.6.1/examples/SOSims/healpix2CAR.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/makeGaussianBeam.py` & `nemo-sz-0.6.1/examples/SOSims/makeGaussianBeam.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/makeRedshiftsCatalog.py` & `nemo-sz-0.6.1/examples/SOSims/makeRedshiftsCatalog.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/readWebSkyInputCatalog.py` & `nemo-sz-0.6.1/examples/SOSims/readWebSkyInputCatalog.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/selFnExample.py` & `nemo-sz-0.6.1/examples/SOSims/selFnExample.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/surveyMask.reg` & `nemo-sz-0.6.1/examples/SOSims/surveyMask.reg`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/template_AdvACT.txt` & `nemo-sz-0.6.1/examples/SOSims/template_AdvACT.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/template_E-D56.txt` & `nemo-sz-0.6.1/examples/SOSims/template_E-D56.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/template_small.txt` & `nemo-sz-0.6.1/examples/SOSims/template_small.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/validationScripts/README.md` & `nemo-sz-0.6.1/examples/SOSims/validationScripts/README.md`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery.py` & `nemo-sz-0.6.1/examples/SOSims/validationScripts/checkMassRecovery.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py` & `nemo-sz-0.6.1/examples/SOSims/validationScripts/checkMassRecovery_M200m.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py` & `nemo-sz-0.6.1/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py` & `nemo-sz-0.6.1/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/TILe-C/README.md` & `nemo-sz-0.6.1/examples/TILe-C/README.md`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/TILe-C/y_f090beam.yml` & `nemo-sz-0.6.1/examples/TILe-C/y_f090beam.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/clustercal/clustercal.py` & `nemo-sz-0.6.1/examples/clustercal/clustercal.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/clustercal/makeConfigs.py` & `nemo-sz-0.6.1/examples/clustercal/makeConfigs.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/clustercal/template_singlefreq.yml` & `nemo-sz-0.6.1/examples/clustercal/template_singlefreq.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/quickstart/README.rst` & `nemo-sz-0.6.1/examples/quickstart/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/quickstart/quickstart-clusters.yml` & `nemo-sz-0.6.1/examples/quickstart/quickstart-clusters.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/quickstart/quickstart-sources.yml` & `nemo-sz-0.6.1/examples/quickstart/quickstart-sources.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PSExample_E-D56.yml` & `nemo-sz-0.6.1/examples/sources/PSExample_E-D56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PSExample_deep56_s15_f090.yml` & `nemo-sz-0.6.1/examples/sources/PSExample_deep56_s15_f090.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PSExample_deep8.yml` & `nemo-sz-0.6.1/examples/sources/PSExample_deep8.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S16_f090_nightOnly.yml` & `nemo-sz-0.6.1/examples/sources/PS_S16_f090_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S16_nightOnly.yml` & `nemo-sz-0.6.1/examples/sources/PS_S16_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S18d_f090_202006_2pass.yml` & `nemo-sz-0.6.1/examples/sources/PS_S18d_f090_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S18d_f150_202006_2pass.yml` & `nemo-sz-0.6.1/examples/sources/PS_S18d_f150_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.yml` & `nemo-sz-0.6.1/examples/sources/PS_S18d_f220_202006.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006_2pass.yml` & `nemo-sz-0.6.1/examples/sources/PS_S18d_f220_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_f150_act+planck_day+night.yml` & `nemo-sz-0.6.1/examples/sources/PS_f150_act+planck_day+night.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/examples/sources/PS_f220_nightOnly.yml` & `nemo-sz-0.6.1/examples/sources/PS_f220_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/MockSurvey.py` & `nemo-sz-0.6.1/nemo/MockSurvey.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/catalogs.py` & `nemo-sz-0.6.1/nemo/catalogs.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/completeness.py` & `nemo-sz-0.6.1/nemo/completeness.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/data/planck_lensedCls.dat` & `nemo-sz-0.6.1/nemo/data/planck_lensedCls.dat`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/filters.py` & `nemo-sz-0.6.1/nemo/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         A dictionary containing the filtered map in signal units, a signal-to-noise-map, area mask, WCS, and
         a label (for housekeeping).
     
     """
         
     f=filterParams
     label=f['label']+"#"+tileName
-        
+
     print("... making filtered map %s" % (label))
     filterClass=eval('%s' % (f['class']))
     filterObj=filterClass(f['label'], unfilteredMapsDictList, f['params'], tileName = tileName,
                             diagnosticsDir = diagnosticsDir, selFnDir = selFnDir)
     filteredMapDict=filterObj.buildAndApply(useCachedFilter = useCachedFilter)
 
     # Keywords we need for photometry later
```

### Comparing `nemo-sz-0.6.0/nemo/gnfw.py` & `nemo-sz-0.6.1/nemo/gnfw.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/maps.py` & `nemo-sz-0.6.1/nemo/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import math
 import time
 import shutil
 import copy
 import yaml
 import pickle
 from pixell import enmap, curvedsky, utils, powspec
-import sharp
 import nemo
 try:
     import reproject
 except:
     pass
 from . import catalogs
 from . import signals
@@ -1319,15 +1318,15 @@
             ivarMap=enmap.enmap(ivarMap, wcs.AWCS)
         else:
             ivarMap=enmap.enmap(np.ones(shape)*(1/noiseLevel**2), wcs.AWCS)
 
         def _mod_noise_map(ivar, Nl):
             map1 = enmap.rand_gauss(ivar.shape, ivar.wcs)
             lmax = len(Nl)-1
-            ainfo = sharp.alm_info(lmax)
+            ainfo = curvedsky.alm_info(lmax)
             alm = curvedsky.map2alm(map1, ainfo=ainfo)
             map2 = curvedsky.alm2map(alm, np.zeros_like(map1))
             map1 -= map2
             ainfo.lmul(alm, Nl**0.5, alm)
             map2 = curvedsky.alm2map(alm, np.zeros_like(map1))
             map1 += map2
             map1 *= ivar**-0.5
```

### Comparing `nemo-sz-0.6.0/nemo/photometry.py` & `nemo-sz-0.6.1/nemo/photometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                 obj[prefix+'deltaT_c']=deltaTc
                 obj[prefix+'err_deltaT_c']=deltaTc/obj[prefix+'SNR']                        
                 if reportJyFluxes == True:
                     obj[prefix+"fluxJy"]=deltaTToJyPerSr(obj[prefix+'deltaT_c'], obsFreqGHz)*beamSolidAngle_nsr*1.e-9
                     obj[prefix+"err_fluxJy"]=deltaTToJyPerSr(obj[prefix+'err_deltaT_c'], obsFreqGHz)*beamSolidAngle_nsr*1.e-9
 
 #------------------------------------------------------------------------------------------------------------
-def makeForcedPhotometryCatalog(filteredMapDict, inputCatalog, useInterpolator = True,
+def makeForcedPhotometryCatalog(filteredMapDict, inputCatalog, useInterpolator = True,\
                                 DS9RegionsPath = None):
     """Make a catalog on which we can do forced photometry at the locations of objects in it.
     
     inputCatalog is either a path or a table object.
         
     """
```

### Comparing `nemo-sz-0.6.0/nemo/pipelines.py` & `nemo-sz-0.6.1/nemo/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,29 @@
 from . import maps
 from . import signals
 from . import completeness
 from . import MockSurvey
 
 #------------------------------------------------------------------------------------------------------------
 def filterMapsAndMakeCatalogs(config, rootOutDir = None, useCachedFilters = False, useCachedRMSMap = False,\
-                              measureFluxes = True, invertMap = False, verbose = True, writeAreaMask = False,\
-                              writeFlagMask = False):
+                              useCachedFilteredMaps = False, measureFluxes = True, invertMap = False, \
+                              verbose = True, writeAreaMask = False, writeFlagMask = False):
     """Runs the map filtering and catalog construction steps according to the given configuration.
     
     Args:
         config (:obj: 'startup.NemoConfig'): Nemo configuration object.
         rootOutDir (str): If None, use the default given by config. Otherwise, use this to override where the
             output filtered maps and catalogs are written.
         useCachedFilters (:obj:`bool`, optional): If True, and previously made filters are found, they will be
             read from disk, rather than re-calculated (used by source injection simulations).
         useCachedRMSMap (:obj:`bool`, optional): If True, use the previously estimated noise map, which has
             been saved to disk. This is only useful for source injection simulations.
+        useCachedFilteredMaps (:obj:`bool`, optional): If True, and previously written maps are found, these
+            will be read from disk, rather than re-made. This is useful for performing forced photometry using
+            external catalogs without having to run nemo again. Otherwise, this should be set to False.
         measureFluxes (bool, optional): If True, measure fluxes. If False, just extract S/N values for 
             detected objects.
         invertMap (bool, optional): If True, multiply all maps by -1; needed by 
             :meth:maps.estimateContaminationFromInvertedMaps).
     
     Returns:
         Optimal catalog (keeps the highest S/N detection when filtering at multiple scales).
@@ -65,14 +68,15 @@
             print(">>> Filter set: %d" % (setNum))
             config.setFilterSet(setNum)
             if setNum == config.filterSets[-1]:
                 writeAreaMask=True
                 writeFlagMask=True
             config.filterSetOptions[setNum]['catalog']=_filterMapsAndMakeCatalogs(config, verbose = True,
                                                                                   useCachedFilters = False,
+                                                                                  useCachedFilteredMaps = False,
                                                                                   writeAreaMask = writeAreaMask,
                                                                                   writeFlagMask = writeFlagMask)
 
             if config.filterSetOptions[setNum]['addSiphonedFromSets'] is not None:
                 toStack=[config.filterSetOptions[setNum]['catalog']]
                 for siphonSetNum in config.filterSetOptions[setNum]['addSiphonedFromSets']:
                     toStack.append(config.filterSetOptions[siphonSetNum]['catalog'])
@@ -89,35 +93,39 @@
                     catalogs.catalog2DS9(config.filterSetOptions[setNum]['catalog'], outFileName.replace(".fits", ".reg"))
 
         catalog=config.filterSetOptions[config.filterSets[-1]]['catalog']
 
     else:
         # Default single pass behaviour (also used by source injection tests)
         catalog=_filterMapsAndMakeCatalogs(config, rootOutDir = rootOutDir, useCachedFilters = useCachedFilters,
+                                           useCachedFilteredMaps = useCachedFilteredMaps,
                                            useCachedRMSMap = useCachedRMSMap, measureFluxes = measureFluxes,
                                            invertMap = invertMap, verbose = verbose,
                                            writeAreaMask = writeAreaMask, writeFlagMask = writeFlagMask)
 
     if verbose == True and config.rank == 0:
         print("... after map filtering and making catalogs: time since start = %.3f sec" % (time.time()-config._timeStarted))
 
     return catalog
 
 #------------------------------------------------------------------------------------------------------------
 def _filterMapsAndMakeCatalogs(config, rootOutDir = None, useCachedFilters = False, useCachedRMSMap = False,\
-                               measureFluxes = True, invertMap = False, verbose = True, writeAreaMask = False,\
-                               writeFlagMask = False):
+                               useCachedFilteredMaps = False, measureFluxes = True, invertMap = False, \
+                               verbose = True, writeAreaMask = False, writeFlagMask = False):
     """Runs the map filtering and catalog construction steps according to the given configuration.
     
     Args:
         config (:obj: 'startup.NemoConfig'): Nemo configuration object.
         rootOutDir (str): If None, use the default given by config. Otherwise, use this to override where the
             output filtered maps and catalogs are written.
         useCachedFilters (:obj:`bool`, optional): If True, and previously made filters are found, they will be
             read from disk, rather than re-calculated (used by source injection simulations).
+        useCachedFilteredMaps (:obj:`bool`, optional): If True, and previously written maps are found, these
+            will be read from disk, rather than re-made. This is useful for performing forced photometry using
+            external catalogs without having to run nemo again. Otherwise, this should be set to False.
         measureFluxes (bool, optional): If True, measure fluxes. If False, just extract S/N values for 
             detected objects.
         invertMap (bool, optional): If True, multiply all maps by -1; needed by 
             :meth:maps.estimateContaminationFromInvertedMaps).
     
     Returns:
         Optimal catalog (keeps the highest S/N detection when filtering at multiple scales).
@@ -177,18 +185,36 @@
             label=f['label']+"#"+tileName            
             catalogDict[label]={}
             if 'saveDS9Regions' in f['params'] and f['params']['saveDS9Regions'] == True:
                 DS9RegionsPath=config.filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_filteredMap.reg"  % (label)
             else:
                 DS9RegionsPath=None
 
-            filteredMapDict=filters.filterMaps(config.unfilteredMapsDictList, f, tileName, 
-                                               diagnosticsDir = config.diagnosticsDir, selFnDir = config.selFnDir,
-                                               verbose = True, undoPixelWindow = undoPixelWindow,
-                                               useCachedFilter = useCachedFilters)
+            filteredMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_filteredMap.fits"  % (label)
+            SNMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_SNMap.fits" % (label)
+            if useCachedFilteredMaps == True and os.path.exists(filteredMapFileName):
+                print("... loading cached filtered map %s ..." % (filteredMapFileName))
+                filteredMapDict={}
+                with pyfits.open(filteredMapFileName) as img:
+                    filteredMapDict['data']=img[0].data
+                    filteredMapDict['wcs']=astWCS.WCS(img[0].header, mode = 'pyfits')
+                    filteredMapDict['mapUnits']=filteredMapDict['wcs'].header['BUNIT']
+                    if 'BEAMNSR' in filteredMapDict['wcs'].header.keys():
+                        filteredMapDict['beamSolidAngle_nsr']=filteredMapDict['wcs'].header['BEAMNSR']
+                        filteredMapDict['obsFreqGHz']=filteredMapDict['wcs'].header['FREQGHZ']
+                with pyfits.open(SNMapFileName) as img:
+                    filteredMapDict['SNMap']=img[0].data
+                filteredMapDict['surveyMask'], wcs=completeness.loadAreaMask(tileName, config.selFnDir)
+                filteredMapDict['label']=f['label']
+                filteredMapDict['tileName']=tileName
+            else:
+                filteredMapDict=filters.filterMaps(config.unfilteredMapsDictList, f, tileName,
+                                                   diagnosticsDir = config.diagnosticsDir, selFnDir = config.selFnDir,
+                                                   verbose = True, undoPixelWindow = undoPixelWindow,
+                                                   useCachedFilter = useCachedFilters)
 
             if useCachedRMSMap == True and photFilter is not None: # i.e., only an option for cluster insertion sims
                 # This is messy:
                 # 1. the saved RMS map doesn't have pixel window correction undone
                 # 2. we make the S/N map before doing the pixel window correction (it would cancel)
                 # 3. but if we're running a source injection sim using the cached RMS map, we'd make a new SN map
                 #    here that has the pixel window correction undone for S, but not for N
@@ -201,16 +227,14 @@
                 SNMap[validMask]=SNMap[validMask]/RMSMap[validMask]
                 filteredMapDict['SNMap']=SNMap
                 mask=np.equal(filteredMapDict['data'], 0)
                 filteredMapDict['data']=enmap.apply_window(filteredMapDict['data'], pow=-1.0)
                 filteredMapDict['data'][mask]=0 # just in case we rely elsewhere on zero == no data
 
             if 'saveFilteredMaps' in f['params'] and f['params']['saveFilteredMaps'] == True:
-                filteredMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_filteredMap.fits"  % (label)
-                SNMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_SNMap.fits" % (label)
                 maps.saveFITS(filteredMapFileName, filteredMapDict['data'], filteredMapDict['wcs'])
                 maps.saveFITS(SNMapFileName, filteredMapDict['SNMap'], filteredMapDict['wcs'])
 
             if f['label'] == photFilter:
                 photFilteredMapDict={}
                 photFilteredMapDict['SNMap']=filteredMapDict['SNMap']
                 photFilteredMapDict['data']=filteredMapDict['data']
```

### Comparing `nemo-sz-0.6.0/nemo/plotSettings.py` & `nemo-sz-0.6.1/nemo/plotSettings.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/signals.py` & `nemo-sz-0.6.1/nemo/signals.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo/startUp.py` & `nemo-sz-0.6.1/nemo/startUp.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/nemo_sz.egg-info/PKG-INFO` & `nemo-sz-0.6.1/nemo_sz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-sz
-Version: 0.6.0
+Version: 0.6.1
 Summary: Millimeter-wave galaxy cluster and source detection package.
 Home-page: https://nemo-sz.readthedocs.io
 Author: Matt Hilton + Nemo Contributors
 Author-email: hiltonm@ukzn.ac.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nemo-sz-0.6.0/nemo_sz.egg-info/SOURCES.txt` & `nemo-sz-0.6.1/nemo_sz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 tests/quick.robot
 tests/configs/MPITestSurveyMaskHeader.txt
 tests/configs/PSTest_E-D56.yml
 tests/configs/PSTest_south2008.yml
 tests/configs/PSTest_south2008_fourier.yml
 tests/configs/README.rst
 tests/configs/equD56_quick_fourier.yml
+tests/configs/quickstart-clusters-Q.yml
 tests/configs/quickstart-multipass.yml
 tests/configs/sim_cl_A10_MFMF_tiles.yml
 tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml
 tests/configs/sim_cl_B12_MFMF_tiles.yml
 tests/configs/sim_cl_MFMF.yml
 tests/configs/sim_cl_MFMF_pass2.yml
 tests/configs/sim_ptsrc_f090.yml
```

### Comparing `nemo-sz-0.6.0/setup.py` & `nemo-sz-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/README.rst` & `nemo-sz-0.6.1/tests/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/clusters.robot` & `nemo-sz-0.6.1/tests/clusters.robot`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/MPITestSurveyMaskHeader.txt` & `nemo-sz-0.6.1/tests/configs/MPITestSurveyMaskHeader.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/PSTest_E-D56.yml` & `nemo-sz-0.6.1/tests/configs/PSTest_E-D56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/PSTest_south2008.yml` & `nemo-sz-0.6.1/tests/configs/PSTest_south2008.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/PSTest_south2008_fourier.yml` & `nemo-sz-0.6.1/tests/configs/PSTest_south2008_fourier.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/equD56_quick_fourier.yml` & `nemo-sz-0.6.1/tests/configs/equD56_quick_fourier.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/quickstart-multipass.yml` & `nemo-sz-0.6.1/tests/configs/quickstart-multipass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles.yml` & `nemo-sz-0.6.1/tests/configs/sim_cl_A10_MFMF_tiles.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml` & `nemo-sz-0.6.1/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_cl_B12_MFMF_tiles.yml` & `nemo-sz-0.6.1/tests/configs/sim_cl_B12_MFMF_tiles.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_cl_MFMF.yml` & `nemo-sz-0.6.1/tests/configs/sim_cl_MFMF.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_cl_MFMF_pass2.yml` & `nemo-sz-0.6.1/tests/configs/sim_cl_MFMF_pass2.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/sim_ptsrc_f090.yml` & `nemo-sz-0.6.1/tests/configs/sim_ptsrc_f090.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/configs/smallTestSurveyMaskHeader.txt` & `nemo-sz-0.6.1/tests/configs/smallTestSurveyMaskHeader.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/debug.py` & `nemo-sz-0.6.1/tests/debug.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/lib/NemoTests.py` & `nemo-sz-0.6.1/tests/lib/NemoTests.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     
         # Maps and beams
         thisDir=os.getcwd()        
         self.inMapFileName=self.cacheDir+os.path.sep+"maps"+os.path.sep+"f150_1_10_8_map.fits"
         if os.path.exists(self.inMapFileName) == False:
             print(">>> Downloading quickstart files ...")
             os.chdir(self.cacheDir)
-            os.system("wget https://astro.ukzn.ac.za/~mjh/nemo-quickstart-maps.tar.gz")
+            os.system("wget 'https://www.dropbox.com/scl/fi/5sjapfshk8g3kxgy4zc56/nemo-quickstart-maps.tar.gz?rlkey=swpdttpgvkffbgr9pcmebslw2&dl=0' -O nemo-quickstart-maps.tar.gz")
             os.system("tar -zxvf nemo-quickstart-maps.tar.gz")
             os.remove("nemo-quickstart-maps.tar.gz")
             os.chdir(thisDir)
         
         # DR5 release catalog for comparing signals
         comparisonCatalog=self.cacheDir+os.path.sep+"DR5_cluster-catalog_v1.1.fits"
         if os.path.exists(comparisonCatalog) == False:
@@ -159,30 +159,35 @@
         
         """
         self.configFileName=os.path.abspath(configFileName)
         self.selFnDir=configFileName.replace(".yml", "")+os.path.sep+"selFn"
         self.mocksDir=configFileName.replace(".yml", "")+os.path.sep+"mocks"
         
         
-    def run_nemo(self):
-        self._run_command(["nemo", self.configFileName])
+    def run_nemo(self, forcedPhotometryCatalog = None):
+        args=['nemo', self.configFileName]
+        if forcedPhotometryCatalog is not None:
+            args=args+['-f', forcedPhotometryCatalog]
+        self._run_command(args)
 
 
     def run_nemo_injection_test(self):
         self._run_command(["nemo", self.configFileName, "-I"])
 
 
     def run_parallel_nemo(self):
         self._run_command(["mpiexec", "-np", "4", "nemo", self.configFileName, "-M"])
 
 
-    def run_nemo_mass(self, catalogFileName = None):
+    def run_nemo_mass(self, catalogFileName = None, forcedPhotometry = False):
         args=['nemoMass', self.configFileName]
-        if catalogFileName != None:
+        if catalogFileName is not None:
             args=args+['-c', catalogFileName]
+        if forcedPhotometry == True:
+            args=args+['-F']
         self._run_command(args)
 
 
     def make_sim(self, catalogFileName = None, noiseLevel = None, seed = None, band = None, size = None):
         args=['nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'], 
               "sim_%s.fits" % (band), '-f', self.bandsDict[band]['freq'], 
               '-C', '-N', noiseLevel, '-S', seed]
```

### Comparing `nemo-sz-0.6.0/tests/point_sources.robot` & `nemo-sz-0.6.1/tests/point_sources.robot`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.6.0/tests/quick.robot` & `nemo-sz-0.6.1/tests/quick.robot`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,26 @@
     Cross match             testsCache/quickstart-clusters/quickstart-clusters_optimalCatalog.fits      testsCache/DR5_cluster-catalog_v1.1.fits
     Check recovered ratio   fixed_y_c    fixed_y_c    toleranceSigma=3.0    expectedRatio=0.94  errInKey=fixed_err_y_c  errOutKey=fixed_err_y_c  SNRKey=fixed_SNR  SNRCut=5.0  plotLabel=quickstart-clusters
     Status should be        SUCCESS
 
 Quickstart sources tutorial runs
     Run quickstart sources
 
+Mass estimation works
+    Run quickstart clusters with Q
+    Run nemo mass
+
+Forced photometry using nemo works
+    Set config              configs/quickstart-clusters-Q.yml
+    Run nemo    DR5_cluster-catalog_v1.1.fits
+
+Forced photometry using nemoMass works
+    Run quickstart clusters with Q
+    Run nemo mass   DR5_cluster-catalog_v1.1.fits   True
+
 Source injection test runs
     Generate simulated source maps
     Set config      configs/sim_ptsrc_f090.yml
     Run nemo injection test
 
 Quickstart multipass config runs
     Run quickstart multipass
@@ -53,14 +65,18 @@
     
 *** Keywords ***
 
 Run quickstart clusters
     Set config              ../examples/quickstart/quickstart-clusters.yml
     Run nemo
 
+Run quickstart clusters with Q
+    Set config              configs/quickstart-clusters-Q.yml
+    Run nemo
+
 Run quickstart sources
     Set config              ../examples/quickstart/quickstart-sources.yml
     Run nemo
 
 Run quickstart multipass
     Set config              configs/quickstart-multipass.yml
     Run nemo
@@ -111,15 +127,17 @@
 
 Clean up
     Remove directory        testsCache/sim_cl_MFMF                      True
     Remove directory        testsCache/sim_ptsrc_f090                   True
     Remove directory        testsCache/quickstart-clusters              True
     Remove directory        testsCache/quickstart-sources               True
     Remove directory        testsCache/quickstart-multipass             True
-
+    Remove directory        testsCache/quickstart-multipass-Q           True
+    Remove file             testsCache/*forcedCatalog*
+    Remove file             testsCache/*_mass.fits
 
 *** Settings ***
 #Documentation              To be added here
 Library                     OperatingSystem
 Library                     lib/NemoTests.py
 Suite Setup                 Setup quickstart
 Suite Teardown              Clean up
```

### Comparing `nemo-sz-0.6.0/versioneer.py` & `nemo-sz-0.6.1/versioneer.py`

 * *Files identical despite different names*

