# Comparing `tmp/dramkit-0.5.45.tar.gz` & `tmp/dramkit-0.5.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.45.tar", last modified: Fri Jun 30 07:52:53 2023, max compression
+gzip compressed data, was "dramkit-0.5.46.tar", last modified: Wed Jul 19 15:18:21 2023, max compression
```

## Comparing `dramkit-0.5.45.tar` & `dramkit-0.5.46.tar`

### file list

```diff
@@ -1,192 +1,209 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.262866 dramkit-0.5.45/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.45/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-06-30 07:52:53.261866 dramkit-0.5.45/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.45/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.764881 dramkit-0.5.45/dramkit/
--rw-rw-rw-   0        0        0     1052 2023-06-16 10:22:54.000000 dramkit-0.5.45/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-06-30 07:52:04.000000 dramkit-0.5.45/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.897867 dramkit-0.5.45/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.45/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.45/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0    41819 2023-06-06 08:45:33.000000 dramkit-0.5.45/dramkit/_tmp/feature_selection.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.45/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.45/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0    26310 2023-06-14 06:03:36.000000 dramkit-0.5.45/dramkit/_tmp/step_reg.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.45/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.45/dramkit/_tmp/test_await_timeout.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.45/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.45/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.45/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.45/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.45/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.45/dramkit/_tmp/test_multiprocessing.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.45/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.45/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.45/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.45/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.45/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.45/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.45/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.45/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.45/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.906870 dramkit-0.5.45/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.45/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.45/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.954883 dramkit-0.5.45/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21188 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3978799 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.45/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    35391 2023-06-26 02:06:52.000000 dramkit-0.5.45/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.027951 dramkit-0.5.45/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.45/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     8115 2023-06-08 02:59:55.000000 dramkit-0.5.45/dramkit/datsci/_rl_mab.py
--rw-rw-rw-   0        0        0    42723 2023-06-29 15:51:40.000000 dramkit-0.5.45/dramkit/datsci/_rl_markov.py
--rw-rw-rw-   0        0        0    13956 2023-06-29 16:36:06.000000 dramkit-0.5.45/dramkit/datsci/_rl_mcdp.py
--rw-rw-rw-   0        0        0     2865 2023-06-09 04:28:19.000000 dramkit-0.5.45/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.45/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.45/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.45/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.45/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.45/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.45/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.45/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.45/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.45/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.45/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     7362 2023-06-13 05:23:22.000000 dramkit-0.5.45/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    20428 2023-06-20 07:06:30.000000 dramkit-0.5.45/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0      790 2023-06-14 12:02:47.000000 dramkit-0.5.45/dramkit/datsci/rl_markov_new.py
--rw-rw-rw-   0        0        0    44419 2023-06-26 08:21:38.000000 dramkit-0.5.45/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    18111 2023-06-26 07:18:32.000000 dramkit-0.5.45/dramkit/datsci/stepreg.py
--rw-rw-rw-   0        0        0    36092 2023-06-20 06:09:25.000000 dramkit-0.5.45/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.45/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.45/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6869 2023-06-20 06:49:38.000000 dramkit-0.5.45/dramkit/datsci/utils_ml.py
--rw-rw-rw-   0        0        0    21136 2023-05-21 10:05:57.000000 dramkit-0.5.45/dramkit/datsci/zigzag.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.048868 dramkit-0.5.45/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   130403 2023-06-28 08:59:48.000000 dramkit-0.5.45/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.45/dramkit/install_check.py
--rw-rw-rw-   0        0        0    67711 2023-06-29 15:42:42.000000 dramkit-0.5.45/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.065881 dramkit-0.5.45/dramkit/logtools/
--rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.45/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.45/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.45/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.45/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4494 2023-06-18 01:41:28.000000 dramkit-0.5.45/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.078867 dramkit-0.5.45/dramkit/openai/
--rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.45/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.45/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.45/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.45/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.119869 dramkit-0.5.45/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.45/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.45/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.45/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.45/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.45/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.45/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.45/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.45/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.45/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.45/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.45/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.45/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.148866 dramkit-0.5.45/dramkit/other/
--rw-rw-rw-   0        0        0      831 2023-05-21 07:44:53.000000 dramkit-0.5.45/dramkit/other/_Git_notes.py
--rw-rw-rw-   0        0        0     3983 2023-06-13 02:44:22.000000 dramkit-0.5.45/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.45/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.45/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.45/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     6453 2023-06-15 12:19:25.000000 dramkit-0.5.45/dramkit/other/debt_cal.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.45/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8829 2023-06-29 09:50:52.000000 dramkit-0.5.45/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.45/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.45/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.171866 dramkit-0.5.45/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.45/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.45/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.45/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.45/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.45/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     4789 2023-06-12 03:17:06.000000 dramkit-0.5.45/dramkit/plottools/twinx_align.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.45/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.178887 dramkit-0.5.45/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.45/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.45/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.196917 dramkit-0.5.45/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.45/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.45/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.45/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.45/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.45/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.219868 dramkit-0.5.45/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.45/dramkit/speedup/_mp_test1.py
--rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.45/dramkit/speedup/_mp_test2.py
--rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.45/dramkit/speedup/_mp_test3.py
--rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.45/dramkit/speedup/iotools_tmp.py
--rw-rw-rw-   0        0        0      858 2023-06-12 06:03:15.000000 dramkit-0.5.45/dramkit/speedup/job_lib.py
--rw-rw-rw-   0        0        0     3796 2023-06-15 08:12:44.000000 dramkit-0.5.45/dramkit/speedup/multi_process_concurrent.py
--rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.45/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.243882 dramkit-0.5.45/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.45/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.45/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6985 2023-06-09 08:58:07.000000 dramkit-0.5.45/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.45/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.45/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.45/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.45/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.45/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.251944 dramkit-0.5.45/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5427 2023-05-31 05:22:42.000000 dramkit-0.5.45/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.258869 dramkit-0.5.45/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.45/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.45/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.779894 dramkit-0.5.45/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5009 2023-06-30 07:52:51.000000 dramkit-0.5.45/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:52:53.263869 dramkit-0.5.45/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.244255 dramkit-0.5.46/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 18:45:20.000000 dramkit-0.5.46/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-07-19 15:18:21.244255 dramkit-0.5.46/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 22:18:54.000000 dramkit-0.5.46/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.114602 dramkit-0.5.46/dramkit/
+-rw-rw-rw-   0        0        0     1052 2023-06-16 18:22:56.000000 dramkit-0.5.46/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-07-19 15:17:49.000000 dramkit-0.5.46/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.148512 dramkit-0.5.46/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 17:50:34.000000 dramkit-0.5.46/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 17:11:36.000000 dramkit-0.5.46/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     9239 2023-07-14 23:02:42.000000 dramkit-0.5.46/dramkit/_tmp/_dijkstra.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0    41819 2023-06-06 16:45:34.000000 dramkit-0.5.46/dramkit/_tmp/feature_selection.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0     5056 2023-07-07 22:21:00.000000 dramkit-0.5.46/dramkit/_tmp/important_sample.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 19:02:40.000000 dramkit-0.5.46/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2621 2023-07-04 13:46:02.000000 dramkit-0.5.46/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1085 2023-07-06 15:41:16.000000 dramkit-0.5.46/dramkit/_tmp/test_Wrapper.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 11:20:48.000000 dramkit-0.5.46/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 09:16:24.000000 dramkit-0.5.46/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 17:04:48.000000 dramkit-0.5.46/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 22:32:42.000000 dramkit-0.5.46/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 17:46:44.000000 dramkit-0.5.46/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 14:15:30.000000 dramkit-0.5.46/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 17:21:00.000000 dramkit-0.5.46/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 15:48:44.000000 dramkit-0.5.46/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 21:43:16.000000 dramkit-0.5.46/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 22:45:06.000000 dramkit-0.5.46/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 18:04:36.000000 dramkit-0.5.46/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 16:28:24.000000 dramkit-0.5.46/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 21:36:20.000000 dramkit-0.5.46/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 17:21:12.000000 dramkit-0.5.46/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 14:13:40.000000 dramkit-0.5.46/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 18:45:30.000000 dramkit-0.5.46/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 18:38:50.000000 dramkit-0.5.46/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.150506 dramkit-0.5.46/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 21:07:38.000000 dramkit-0.5.46/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 21:50:24.000000 dramkit-0.5.46/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.168458 dramkit-0.5.46/dramkit/chncal/
+-rw-rw-rw-   0        0        0     1413 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3983334 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-07-10 23:43:50.000000 dramkit-0.5.46/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 14:40:30.000000 dramkit-0.5.46/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    35391 2023-06-26 10:06:54.000000 dramkit-0.5.46/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.183418 dramkit-0.5.46/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 10:08:56.000000 dramkit-0.5.46/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-06-09 12:28:20.000000 dramkit-0.5.46/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 22:04:36.000000 dramkit-0.5.46/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 15:56:58.000000 dramkit-0.5.46/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 15:58:06.000000 dramkit-0.5.46/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 14:37:14.000000 dramkit-0.5.46/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 14:17:26.000000 dramkit-0.5.46/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 16:00:00.000000 dramkit-0.5.46/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 16:00:48.000000 dramkit-0.5.46/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-26 02:21:16.000000 dramkit-0.5.46/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50084 2023-05-10 10:47:38.000000 dramkit-0.5.46/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 16:06:28.000000 dramkit-0.5.46/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     2340 2023-07-15 13:20:06.000000 dramkit-0.5.46/dramkit/datsci/level_score.py
+-rw-rw-rw-   0        0        0     7373 2023-07-04 10:42:54.000000 dramkit-0.5.46/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    20428 2023-06-20 15:06:32.000000 dramkit-0.5.46/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    48434 2023-07-12 12:31:12.000000 dramkit-0.5.46/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    18137 2023-07-19 15:17:02.000000 dramkit-0.5.46/dramkit/datsci/stepreg.py
+-rw-rw-rw-   0        0        0    36092 2023-06-20 14:09:26.000000 dramkit-0.5.46/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-26 02:24:50.000000 dramkit-0.5.46/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 14:00:48.000000 dramkit-0.5.46/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6869 2023-06-20 14:49:40.000000 dramkit-0.5.46/dramkit/datsci/utils_ml.py
+-rw-rw-rw-   0        0        0    21136 2023-05-21 18:05:58.000000 dramkit-0.5.46/dramkit/datsci/zigzag.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.189402 dramkit-0.5.46/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 16:18:36.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 16:15:24.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 16:17:40.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 16:17:08.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 16:16:02.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-05-01 00:29:20.000000 dramkit-0.5.46/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   137766 2023-07-19 08:44:58.000000 dramkit-0.5.46/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 14:40:12.000000 dramkit-0.5.46/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    68840 2023-07-19 05:14:39.000000 dramkit-0.5.46/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.192398 dramkit-0.5.46/dramkit/logtools/
+-rw-rw-rw-   0        0        0      139 2023-05-01 15:34:22.000000 dramkit-0.5.46/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 12:11:48.000000 dramkit-0.5.46/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 11:04:58.000000 dramkit-0.5.46/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 11:04:40.000000 dramkit-0.5.46/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4494 2023-06-18 09:41:30.000000 dramkit-0.5.46/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.194389 dramkit-0.5.46/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 10:54:38.000000 dramkit-0.5.46/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-26 00:34:12.000000 dramkit-0.5.46/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    17000 2023-07-04 10:10:08.000000 dramkit-0.5.46/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 10:00:26.000000 dramkit-0.5.46/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.203365 dramkit-0.5.46/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 16:26:34.000000 dramkit-0.5.46/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 10:31:46.000000 dramkit-0.5.46/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 16:35:02.000000 dramkit-0.5.46/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 16:34:32.000000 dramkit-0.5.46/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 16:33:52.000000 dramkit-0.5.46/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 16:33:18.000000 dramkit-0.5.46/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 16:32:12.000000 dramkit-0.5.46/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 16:31:28.000000 dramkit-0.5.46/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 16:30:40.000000 dramkit-0.5.46/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 16:29:44.000000 dramkit-0.5.46/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 10:18:30.000000 dramkit-0.5.46/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 16:27:36.000000 dramkit-0.5.46/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.209349 dramkit-0.5.46/dramkit/other/
+-rw-rw-rw-   0        0        0      831 2023-05-21 15:44:54.000000 dramkit-0.5.46/dramkit/other/_Git_notes.py
+-rw-rw-rw-   0        0        0     5068 2023-07-18 15:48:56.000000 dramkit-0.5.46/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     3325 2023-07-19 09:07:32.000000 dramkit-0.5.46/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     5275 2023-07-19 06:34:34.000000 dramkit-0.5.46/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 09:46:28.000000 dramkit-0.5.46/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     6453 2023-06-15 20:19:26.000000 dramkit-0.5.46/dramkit/other/debt_cal.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 14:38:46.000000 dramkit-0.5.46/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8829 2023-06-29 17:50:54.000000 dramkit-0.5.46/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 16:36:52.000000 dramkit-0.5.46/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 09:37:22.000000 dramkit-0.5.46/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.214335 dramkit-0.5.46/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 22:50:06.000000 dramkit-0.5.46/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-07-19 02:11:27.000000 dramkit-0.5.46/dramkit/plottools/_plot_bar.py
+-rw-rw-rw-   0        0        0      712 2023-07-18 12:31:22.000000 dramkit-0.5.46/dramkit/plottools/_plot_heatmap.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 15:36:24.000000 dramkit-0.5.46/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 21:09:28.000000 dramkit-0.5.46/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-26 02:36:50.000000 dramkit-0.5.46/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 21:10:36.000000 dramkit-0.5.46/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     4789 2023-06-12 11:17:08.000000 dramkit-0.5.46/dramkit/plottools/twinx_align.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 22:27:14.000000 dramkit-0.5.46/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.217328 dramkit-0.5.46/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-26 00:04:08.000000 dramkit-0.5.46/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 21:24:38.000000 dramkit-0.5.46/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.226303 dramkit-0.5.46/dramkit/rl/
+-rw-rw-rw-   0        0        0       25 2023-07-05 13:21:22.000000 dramkit-0.5.46/dramkit/rl/__init__.py
+-rw-rw-rw-   0        0        0      815 2023-07-17 14:52:14.000000 dramkit-0.5.46/dramkit/rl/_approx.py
+-rw-rw-rw-   0        0        0     8115 2023-06-08 10:59:56.000000 dramkit-0.5.46/dramkit/rl/_mab.py
+-rw-rw-rw-   0        0        0    46293 2023-07-11 23:03:06.000000 dramkit-0.5.46/dramkit/rl/_markov.py
+-rw-rw-rw-   0        0        0      790 2023-06-14 20:02:48.000000 dramkit-0.5.46/dramkit/rl/_markov_new.py
+-rw-rw-rw-   0        0        0    28122 2023-07-15 20:06:14.000000 dramkit-0.5.46/dramkit/rl/_mc.py
+-rw-rw-rw-   0        0        0     2922 2023-07-12 20:45:36.000000 dramkit-0.5.46/dramkit/rl/_notes.py
+-rw-rw-rw-   0        0        0    30562 2023-07-18 21:48:16.000000 dramkit-0.5.46/dramkit/rl/_td.py
+-rw-rw-rw-   0        0        0    25811 2023-07-15 20:41:50.000000 dramkit-0.5.46/dramkit/rl/_td_dict.py
+-rw-rw-rw-   0        0        0    14911 2023-07-17 14:32:10.000000 dramkit-0.5.46/dramkit/rl/_tmpMountainCar-v0_tf.py
+-rw-rw-rw-   0        0        0     4009 2022-11-22 14:16:46.000000 dramkit-0.5.46/dramkit/rl/_tmprl_utils.py
+-rw-rw-rw-   0        0        0     8336 2023-07-19 07:24:18.000000 dramkit-0.5.46/dramkit/rl/_tmp第7章-DQN算法.py
+-rw-rw-rw-   0        0        0     1860 2023-07-19 07:56:49.000000 dramkit-0.5.46/dramkit/rl/env_hungrygame.py
+-rw-rw-rw-   0        0        0     2018 2023-07-12 11:22:58.000000 dramkit-0.5.46/dramkit/rl/gym_best_pi.py
+-rw-rw-rw-   0        0        0     5292 2023-07-15 20:45:10.000000 dramkit-0.5.46/dramkit/rl/utils_gym.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.229295 dramkit-0.5.46/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 16:45:30.000000 dramkit-0.5.46/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 16:51:56.000000 dramkit-0.5.46/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 16:10:58.000000 dramkit-0.5.46/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 17:23:32.000000 dramkit-0.5.46/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 16:55:16.000000 dramkit-0.5.46/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.236277 dramkit-0.5.46/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 21:02:48.000000 dramkit-0.5.46/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 21:17:46.000000 dramkit-0.5.46/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 21:14:46.000000 dramkit-0.5.46/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 21:25:52.000000 dramkit-0.5.46/dramkit/speedup/_tmp_iotools.py
+-rw-rw-rw-   0        0        0     2142 2023-07-19 10:52:53.000000 dramkit-0.5.46/dramkit/speedup/job_lib.py
+-rw-rw-rw-   0        0        0     3791 2023-07-19 10:57:14.000000 dramkit-0.5.46/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 16:59:36.000000 dramkit-0.5.46/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.241268 dramkit-0.5.46/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 13:15:10.000000 dramkit-0.5.46/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 09:33:30.000000 dramkit-0.5.46/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6985 2023-06-09 16:58:08.000000 dramkit-0.5.46/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0      160 2023-05-01 20:57:20.000000 dramkit-0.5.46/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    20285 2023-05-06 21:49:08.000000 dramkit-0.5.46/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 19:31:14.000000 dramkit-0.5.46/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50966 2023-05-06 21:23:22.000000 dramkit-0.5.46/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 10:56:26.000000 dramkit-0.5.46/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.242261 dramkit-0.5.46/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 17:25:24.000000 dramkit-0.5.46/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5423 2023-07-04 09:51:50.000000 dramkit-0.5.46/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.243258 dramkit-0.5.46/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 22:04:58.000000 dramkit-0.5.46/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 11:03:38.000000 dramkit-0.5.46/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:18:21.117594 dramkit-0.5.46/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-07-19 15:18:20.000000 dramkit-0.5.46/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5425 2023-07-19 15:18:21.000000 dramkit-0.5.46/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:18:20.000000 dramkit-0.5.46/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-19 15:18:20.000000 dramkit-0.5.46/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 15:18:20.000000 dramkit-0.5.46/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 15:18:21.245253 dramkit-0.5.46/setup.cfg
+-rw-rw-rw-   0        0        0     1974 2023-07-18 13:54:32.000000 dramkit-0.5.46/setup.py
```

### Comparing `dramkit-0.5.45/LICENSE` & `dramkit-0.5.46/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/PKG-INFO` & `dramkit-0.5.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.45
+Version: 0.5.46
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.45/README.md` & `dramkit-0.5.46/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/__init__.py` & `dramkit-0.5.46/dramkit/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_pkg_info.py` & `dramkit-0.5.46/dramkit/_pkg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.45',
+    '__version__': '0.5.46',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.45/dramkit/_tmp/CRR.py` & `dramkit-0.5.46/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.46/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.46/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.46/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.46/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/VMD.py` & `dramkit-0.5.46/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/cca_test.py` & `dramkit-0.5.46/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.46/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/explore.py` & `dramkit-0.5.46/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/feature_selection.py` & `dramkit-0.5.46/dramkit/_tmp/feature_selection.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/gini.py` & `dramkit-0.5.46/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.46/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.46/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.46/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.46/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/plot_test.py` & `dramkit-0.5.46/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.46/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.46/dramkit/_tmp/simple_smooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     return series
 
 
 if __name__ == '__main__':
     from dramkit import load_csv, plot_series
     
     # 上证50分钟行情------------------------------------------------------------
-    fpath = '../../../FinFactory/data/archives/index/joinquant/000016.XSHG_1min.csv'
+    fpath = '../../../FinFactory/findata/archives/index/joinquant/000016.XSHG_1min.csv'
     his_data = load_csv(fpath).iloc[:-240, :]
     his_data['time'] = his_data['time'].apply(lambda x: x[11:])
     his_data.set_index('time', drop=False, inplace=True)
 
     df = his_data.iloc[-60:, :].copy()
     # plot_series(df, {'close': '.-b'})
```

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.46/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_await_timeout.py` & `dramkit-0.5.46/dramkit/_tmp/test_await_timeout.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.46/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.46/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_code.py` & `dramkit-0.5.46/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.46/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.46/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_grading.py` & `dramkit-0.5.46/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_lr.py` & `dramkit-0.5.46/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.46/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.46/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_tree.py` & `dramkit-0.5.46/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.46/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.46/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.46/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/tmp.py` & `dramkit-0.5.46/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.46/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.46/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.46/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.46/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.46/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.46/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.46/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.46/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/apis.py` & `dramkit-0.5.46/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/constants.py` & `dramkit-0.5.46/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/constants_fate.py` & `dramkit-0.5.46/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/constants_hko.py` & `dramkit-0.5.46/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.46/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6142,14 +6142,25 @@
     ("CFFEX", datetime.date(year=2023, month=6, day=23)): 0,
     ("CFFEX", datetime.date(year=2023, month=6, day=24)): 0,
     ("CFFEX", datetime.date(year=2023, month=6, day=25)): 0,
     ("CFFEX", datetime.date(year=2023, month=6, day=26)): 1,
     ("CFFEX", datetime.date(year=2023, month=6, day=27)): 1,
     ("CFFEX", datetime.date(year=2023, month=6, day=28)): 1,
     ("CFFEX", datetime.date(year=2023, month=6, day=29)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=30)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=1)): 0,
+    ("CFFEX", datetime.date(year=2023, month=7, day=2)): 0,
+    ("CFFEX", datetime.date(year=2023, month=7, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=5)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=7, day=8)): 0,
+    ("CFFEX", datetime.date(year=2023, month=7, day=9)): 0,
+    ("CFFEX", datetime.date(year=2023, month=7, day=10)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -18090,14 +18101,25 @@
     ("CZCE", datetime.date(year=2023, month=6, day=23)): 0,
     ("CZCE", datetime.date(year=2023, month=6, day=24)): 0,
     ("CZCE", datetime.date(year=2023, month=6, day=25)): 0,
     ("CZCE", datetime.date(year=2023, month=6, day=26)): 1,
     ("CZCE", datetime.date(year=2023, month=6, day=27)): 1,
     ("CZCE", datetime.date(year=2023, month=6, day=28)): 1,
     ("CZCE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("CZCE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("CZCE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("CZCE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("CZCE", datetime.date(year=2023, month=7, day=10)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -29167,14 +29189,25 @@
     ("DCE", datetime.date(year=2023, month=6, day=23)): 0,
     ("DCE", datetime.date(year=2023, month=6, day=24)): 0,
     ("DCE", datetime.date(year=2023, month=6, day=25)): 0,
     ("DCE", datetime.date(year=2023, month=6, day=26)): 1,
     ("DCE", datetime.date(year=2023, month=6, day=27)): 1,
     ("DCE", datetime.date(year=2023, month=6, day=28)): 1,
     ("DCE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("DCE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("DCE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("DCE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("DCE", datetime.date(year=2023, month=7, day=10)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31395,14 +31428,25 @@
     ("INE", datetime.date(year=2023, month=6, day=23)): 0,
     ("INE", datetime.date(year=2023, month=6, day=24)): 0,
     ("INE", datetime.date(year=2023, month=6, day=25)): 0,
     ("INE", datetime.date(year=2023, month=6, day=26)): 1,
     ("INE", datetime.date(year=2023, month=6, day=27)): 1,
     ("INE", datetime.date(year=2023, month=6, day=28)): 1,
     ("INE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("INE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("INE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("INE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("INE", datetime.date(year=2023, month=7, day=10)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -43115,14 +43159,25 @@
     ("SHFE", datetime.date(year=2023, month=6, day=23)): 0,
     ("SHFE", datetime.date(year=2023, month=6, day=24)): 0,
     ("SHFE", datetime.date(year=2023, month=6, day=25)): 0,
     ("SHFE", datetime.date(year=2023, month=6, day=26)): 1,
     ("SHFE", datetime.date(year=2023, month=6, day=27)): 1,
     ("SHFE", datetime.date(year=2023, month=6, day=28)): 1,
     ("SHFE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("SHFE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("SHFE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("SHFE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("SHFE", datetime.date(year=2023, month=7, day=10)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54996,14 +55051,25 @@
     ("SSE", datetime.date(year=2023, month=6, day=23)): 0,
     ("SSE", datetime.date(year=2023, month=6, day=24)): 0,
     ("SSE", datetime.date(year=2023, month=6, day=25)): 0,
     ("SSE", datetime.date(year=2023, month=6, day=26)): 1,
     ("SSE", datetime.date(year=2023, month=6, day=27)): 1,
     ("SSE", datetime.date(year=2023, month=6, day=28)): 1,
     ("SSE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("SSE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("SSE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("SSE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("SSE", datetime.date(year=2023, month=7, day=10)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66681,8 +66747,19 @@
     ("SZSE", datetime.date(year=2023, month=6, day=23)): 0,
     ("SZSE", datetime.date(year=2023, month=6, day=24)): 0,
     ("SZSE", datetime.date(year=2023, month=6, day=25)): 0,
     ("SZSE", datetime.date(year=2023, month=6, day=26)): 1,
     ("SZSE", datetime.date(year=2023, month=6, day=27)): 1,
     ("SZSE", datetime.date(year=2023, month=6, day=28)): 1,
     ("SZSE", datetime.date(year=2023, month=6, day=29)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=30)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=1)): 0,
+    ("SZSE", datetime.date(year=2023, month=7, day=2)): 0,
+    ("SZSE", datetime.date(year=2023, month=7, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=5)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=7, day=8)): 0,
+    ("SZSE", datetime.date(year=2023, month=7, day=9)): 0,
+    ("SZSE", datetime.date(year=2023, month=7, day=10)): 1,
 }
```

### Comparing `dramkit-0.5.45/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.46/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.46/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/chncal/solar_terms.py` & `dramkit-0.5.46/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/cryptotools.py` & `dramkit-0.5.46/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datetimetools.py` & `dramkit-0.5.46/dramkit/datetimetools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/_rl_mab.py` & `dramkit-0.5.46/dramkit/rl/_mab.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/_rl_markov.py` & `dramkit-0.5.46/dramkit/rl/_markov.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from tqdm import tqdm
 from itertools import product
 from scipy.linalg import block_diag
 
 from dramkit.gentools import (link_lists,
                               isnull,
                               capture_print,
-                              rand_sum)
+                              rand_sum,
+                              raise_error)
 
 #%%
 def get_matrixs_by_sasr(pi_s2a,
                         p_sa2sr,
                         rewards,
                         s_names=None,
                         a_names=None):
@@ -354,14 +355,16 @@
     a_ub = gamma * p_sa2s - np.repeat(np.eye(n_s), n_a, axis=0)
     b_ub = -np.array(r_e_sa)
     if isnull(bounds):
         bounds = [(None, None),] * n_s
     v_s = scipy.optimize.linprog(weights, a_ub, b_ub, bounds=bounds,
                                  method='highs')
     v_s = v_s.x
+    if isnull(v_s):
+        raise_error('LingProError', '线性规划求解失败！')
     v_sa = get_sav_from_sv(v_s, p_sa2s, r_e_sa, gamma)
     return v_s, v_sa
 
 #%%
 def get_sv_mc(pi_s2a, p_sa2s, r_sa2s, gamma,
               max_step, n=1000,
               s_names=None, a_names=None, s_stop=None,
@@ -385,62 +388,62 @@
         s = np.random.choice(s_) # 随机选择初始状态
         while s != s_stop and n_step < max_step:
             n_step += 1
             rand, tmp = np.random.rand(), 0
             # 根据策略选择动作
             for _a in a_names:
                 tmp += pi_s2a.loc[s, _a]
-                if tmp > rand:
+                if rand < tmp:
                     a = _a
                     r = r_e_sa.loc[[(s, a)], 'r'][(s, a)]
                     break
             rand, tmp = np.random.rand(), 0
             # 根据转移概率获取下一个状态
             for _s in s_names:
                 tmp += p_sa2s.loc[[(s, a)], _s][(s, a)]
-                if tmp > rand:
+                if rand < tmp:
                     s_new = _s
                     break
-            route.append((s, a, r, s_new))
+            route.append((s, a, r, s_new, s_new == s_stop))
             s = s_new
         routes.append(route)
         
     # 状态价值估计
     if not first_visit:
         # 一条路径上从后往前计算状态价值
         s_n = {s: 0 for s in s_names}
         s_v = {s: 0 for s in s_names}
         for route in routes:
             k_r = 0
             for k in range(len(route)-1, -1, -1):
-                (s, a, r, s_new) = route[k]
+                (s, a, r, s_new, stop) = route[k]
                 k_r = r + gamma * k_r # 步骤(时间)k的奖励
                 s_n[s] = s_n[s] + 1
                 s_v[s] = s_v[s] + (k_r-s_v[s]) / s_n[s]
         # # 一条路径上从前往后计算状态价值
         # s_n = {s: 0 for s in s_names}
         # s_v = {s: 0 for s in s_names}
         # for route in routes:
         #     n_ = len(route)
         #     # 从前往后计算须先取出每个步骤(时间)的奖励
         #     r_route = [x[2] for x in route]
         #     for k in range(n_):
-        #         (s, a, r, s_new) = route[k]
+        #         (s, a, r, s_new, stop) = route[k]
         #         # 步骤(时间)k的奖励
         #         k_r = sum([r_route[_]*gamma**(_-k) for _ in range(k, n_)])
         #         s_n[s] = s_n[s] + 1
         #         s_v[s] = s_v[s] + (k_r-s_v[s]) / s_n[s]
     else:
         s_n = {s: 0 for s in s_names}
         s_v = {s: 0 for s in s_names}
         for route in routes:
             k_r = 0
             route_r = []
             for k in range(len(route)-1, -1, -1):
-                (s, a, r, s_new) = route[k]
+                (s, a, r, s_new, stop) = route[k]
                 k_r = r + gamma * k_r
                 route_r.append((s, k_r))
             visited = {s: 0 for s in s_names}
             for s, k_r in route_r[::-1]:
                 # 仅考虑首次访问
                 if visited[s]:
                     break
@@ -454,15 +457,15 @@
 def get_occupancy(routes, s, a, max_step, gamma):
     '''计算状态动作对(s, a)出现的频率, 以此来估算策略的占用度量'''
     rho = 0
     n_all = np.zeros(max_step) # 记录每个时间步t被经历的次数
     n_sa = np.zeros(max_step) # 记录(s_t, a_t)=(s, a)的次数
     for route in routes:
         for k in range(len(route)):
-            (_s, _a, r, s_new) = route[k]
+            (_s, _a, r, s_new, stop) = route[k]
             n_all[k] += 1
             if s == _s and a == _a:
                 n_sa[k] += 1
     for i in range(max_step):
     # for i in reversed(range(max_step)):
         if n_all[i]:
             # n_sa[i] / n_all[i]为第i步中(s, a)出现的比例
@@ -611,15 +614,16 @@
               [      0,      1]]
     # 状态&动作-状态奖励表
     r_sa2s = [[-2, 0],
               [-3, 1],
               [-2, 2],
               [ 0, 1]]
     
-    alpha_, beta_, gamma_ = 2/3, 3/4, 4/5
+    # alpha_, beta_, gamma_ = 2/3, 3/4, 4/5
+    alpha_, beta_, gamma_ = 1, 1, 4/5
     # '''
     
     '''
     # 1. 使用带奖励的状态&动作-状态&奖励转移矩阵-----------------
     res1, sys1 = bellman_sasr(
                     pi_s2a, p_sa2sr, rewards, gamma,
                     s_names=s_names, a_names=a_names,
@@ -938,44 +942,39 @@
         import gymnasium as gym
     except:
         import gym
     env = gym.make('CliffWalking-v0')
     p_sa2s = np.zeros((env.nS*env.nA, env.nS))
     r_sa2s = np.zeros((env.nS*env.nA, env.nS))
     k = 0
-    index = []
     for s in env.P:
         if s != 47: # 47是终点
             for a in env.P[s]:
                 p_sa2s[k, env.P[s][a][0][1]] = env.P[s][a][0][0]
                 r_sa2s[k, env.P[s][a][0][1]] = env.P[s][a][0][2]
-                index.append([k, s, a])
                 k += 1
     
     s_names = ['loc_%s'%x for x in range(env.nS)]
     a_names = ['^', '>', 'v', '<']
     n_s, n_a = len(s_names), len(a_names)
     gamma = 0.9
     
     def show_pi(pi_s2a, N=5, max_step=np.inf):
         # gym悬崖寻路可视化
         env = gym.make('CliffWalking-v0', render_mode='human')
-        observation, info = env.reset()
-        n, n_step = 0, 0
-        while True:
-            action = np.argmax(pi_s2a[observation])
-            observation, reward, terminated, truncated, info = env.step(action)
-            n_step += 1
-            if n_step > max_step:
-                break
-            if terminated or truncated:
-                n += 1
-                if n < N:
-                    observation, info = env.reset()
-                else:
+        for n in range(N):
+            observation, info = env.reset()
+            n_step = 0
+            while True:
+                action = np.argmax(pi_s2a[observation])
+                observation, reward, terminated, truncated, info = env.step(action)
+                n_step += 1
+                if n_step > max_step:
+                    break
+                if terminated or truncated:
                     break
         env.close()
     # '''
     
     '''
     # 随机策略
     for _ in range(10):
@@ -999,15 +998,15 @@
     bests_a = np.array(v_sa).reshape(-1, n_a).argmax(axis=1)
     pi_s2a = np.eye(n_a)[bests_a]
     show_pi(pi_s2a, N=2)
     # '''
     
     '''
     # 动态规划求解（策略迭代）
-    #  随机策略
+    # 随机策略
     pi_s2a_rand = [rand_sum(1, env.nA, 0.0, 1.0) for _ in range(env.nS)]
     # 最优策略
     pi_s2a_best = np.eye(4)[v_sa.reshape(-1, env.nA).argmax(axis=1)]
     p_s2a = pi_s2a_rand
     # p_s2a = pi_s2a_best
     # 策略评估
     v_s, v_sa = get_sv_dp(p_s2a, p_sa2s, r_sa2s, gamma, max_iter=3000)
@@ -1159,11 +1158,115 @@
     rhos = []
     for s, a in product(s_names, a_names):
         rho = get_occupancy(routes2, s, a, max_step, gamma)
         rhos.append([s, a, rho])
     rhos = pd.DataFrame(rhos, columns=['s', 'a', 'rho'])
     print(rhos['rho'].sum())
     # '''
+
+    #%%
+    '''
+    # 冰湖游戏----------------------------------------------
+    try:
+        import gymnasium as gym
+    except:
+        import gym
+    env = gym.make('FrozenLake-v1')
+    n_s = env.observation_space.n
+    n_a = env.action_space.n
+    p_sa2s = np.zeros((n_s*n_a, n_s))
+    r_sa2s = np.zeros((n_s*n_a, n_s))
+    k = 0
+    for s in env.P:
+        for a in env.P[s]:
+            for s_ in env.P[s][a]:
+                p_sa2s[k, s_[1]] = s_[0]
+                r_sa2s[k, s_[1]] = s_[2]
+            k += 1
+
+    s_names = ['loc_%s'%x for x in range(n_s)]
+    a_names = ['<', 'v', '>', '^']
+    gamma = 1.0
+
+    def show_pi(pi_s2a, N=5, max_step=np.inf):
+        # gym冰湖游戏可视化
+        env = gym.make('FrozenLake-v1', render_mode='human')
+        n_win = 0
+        for n in range(N):
+            observation, info = env.reset()
+            n_step = 0
+            while True:
+                action = np.argmax(pi_s2a[observation])
+                observation, reward, terminated, truncated, info = env.step(action)
+                n_step += 1
+                if n_step > max_step:
+                    break
+                if terminated or truncated:
+                    if reward > 0:
+                        n_win += 1
+                    break
+        print('n_win: {}/{}'.format(n_win, N))
+        env.close()
+    # '''
+
+    '''
+    # 随机策略
+    for _ in range(10):
+        pi_s2a = np.random.rand(n_s, n_a)
+        show_pi(pi_s2a, N=1, max_step=5)
+    # '''
+
+    '''
+    # 动态规划求解（策略迭代）
+    # 随机策略
+    pi_s2a_rand = [rand_sum(1, n_a, 0.0, 1.0) for _ in range(n_s)]
+    p_s2a = pi_s2a_rand
+    # 策略评估
+    v_s, v_sa = get_sv_dp(p_s2a, p_sa2s, r_sa2s, gamma, max_iter=3000)
+    # 策略优化提升（单步）
+    best_pi_s2a, optimal = dp_improve_pi(p_s2a, v_sa)
+    # 策略迭代提升求解
+    pi_s2a, v_s, v_sa = dp_pi(
+        p_sa2s, r_sa2s, gamma, pi_s2a=p_s2a, tol=1e-6,
+        max_iter_est=2000, max_iter_impr=1000,
+        s_names=None, a_names=None, show_step_est=1000,
+        show_step=1000)
+    print(np.array(v_s).reshape(4, -1).round(2))
+    print(np.array(v_sa).reshape(-1, n_a))
+    print('dp优化最佳策略: ')
+    best_acts = [a_names[x] for x in pi_s2a.argmax(axis=1)]
+    best_acts = np.array(best_acts).reshape(4, -1)
+    print(best_acts)
+    # show_pi(pi_s2a)
+    # '''
+
+    '''
+    # 动态规划求解（价值迭代）
+    pi_s2a, v_s, v_sa = dp_val(
+        p_sa2s, r_sa2s, gamma, pi_s2a=p_s2a,
+        s_names=None, a_names=None,
+        tol=1e-6, max_iter=2000, show_step=1000)
+    print(np.array(v_s).reshape(4, -1).round(2))
+    print(np.array(v_sa).reshape(-1, n_a))
+    print('dp优化最佳策略: ')
+    best_acts = [a_names[x] for x in pi_s2a.argmax(axis=1)]
+    best_acts = np.array(best_acts).reshape(4, -1)
+    print(best_acts)
+    show_pi(pi_s2a)
+    # '''
+    
+    '''
+    # 线性规划求解，会失败（因为本身就没有唯一最优解？）
+    v_s, v_sa = get_best_bellman_linprog(p_sa2s, r_sa2s,
+                                          gamma=gamma,
+                                          weights=None)
+    print(np.array(v_s).reshape(4, -1).round(2))
+    print(v_sa.reshape(-1, n_a))
+    # 生成最优策略
+    bests_a = np.array(v_sa).reshape(-1, n_a).argmax(axis=1)
+    pi_s2a = np.eye(n_a)[bests_a]
+    show_pi(pi_s2a, N=2)
+    # '''
     
     #%%
     tr.used()
```

### Comparing `dramkit-0.5.45/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.46/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.46/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/ahp.py` & `dramkit-0.5.46/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.46/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/apriori.py` & `dramkit-0.5.46/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/curvature.py` & `dramkit-0.5.46/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/elm_cls.py` & `dramkit-0.5.46/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/elm_reg.py` & `dramkit-0.5.46/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.46/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.46/dramkit/datsci/find_maxmin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.46/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/lr.py` & `dramkit-0.5.46/dramkit/datsci/lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 
 @beartype
 def lr_smf_df(df : pd.DataFrame,
               ycol: str,
               xcols : Union[list, tuple, set] = None,
               intercept : bool = True):
     '''
-    statsmodels.formula拟合线性回归
-    
+    用 `statsmodels.formula` 拟合线性回归
+
     Examples
     --------
     >>> df = pd.DataFrame({'x': [1, 2, 3, 4, 5],
     >>>                    'y': [2, 3, 4, 5, 6],
-    # >>>                    'y': [2, 4, 6, 8, 10]
+    >>>                    #'y': [2, 4, 6, 8, 10]
     >>>                   })
     >>> xcols = ['x']
     >>> ycol = 'y'
     >>> mdl1 = lr_smf_df(df, ycol, xcols, intercept=True)
     >>> mdl2 = lr_smf_df(df, ycol, xcols, intercept=False)
-    >>> print(mdl1.params, '\n', mdl2.params)
+    >>> print(mdl1.params)
+    >>> print(mdl2.params)
     '''
     if isnull(xcols):
         xcols = [x for x in df.columns if x != ycol]
     if intercept: # 是否有截距
         formula = '{} ~ {} + 1'.format(ycol, ' + '.join(xcols))
     else:
         formula = '{} ~ {} - 1'.format(ycol, ' + '.join(xcols))
```

### Comparing `dramkit-0.5.45/dramkit/datsci/preprocess.py` & `dramkit-0.5.46/dramkit/datsci/preprocess.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/rl_markov_new.py` & `dramkit-0.5.46/dramkit/rl/_markov_new.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/stats.py` & `dramkit-0.5.46/dramkit/datsci/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import math
+from beartype.typing import Callable
+
 import numpy as np
 import pandas as pd
 
 from scipy.stats import norm, lognorm, weibull_min, kstest
 from scipy.stats import t, f, chi2
 
 from statsmodels.tools.tools import add_constant
@@ -375,14 +377,104 @@
     Stat, P = kstest(np.log(series), 'weibull_min', args=(c, loc, scale))
     if plot:
         from dramkit.plottools.plot_histdist import plot_histdist
         plot_histdist(series, dists={'weibull': ('-r', None)}, **kwargs_plot)
     return (Stat, P), (k, lmd)
 
 
+def mc_important_sample(smp_gener: Callable,
+                        gener_pdf: Callable,
+                        tgt_func: Callable,
+                        tgt_pdf: Callable = None,
+                        n_mc: int = 100000,
+                        cumsum: bool = False):
+    '''
+    | 重要性采样
+    | https://zhuanlan.zhihu.com/p/250282313
+    | https://zhuanlan.zhihu.com/p/629016302
+    | https://zhuanlan.zhihu.com/p/258384070
+    | https://zhuanlan.zhihu.com/p/259389498
+    | https://blog.csdn.net/bigheadyushan/article/details/80623249
+    | https://zhuanlan.zhihu.com/p/41217212
+    | https://www.jianshu.com/p/5648c7321868
+    
+    TODO
+    ----
+    加权重要性采样？
+    
+    Parameters
+    ----------
+    smp_gener : Callable
+        采样器，用于根据给定的概率分布生成样本，调用方式为smps = smp_gener(n_mc)
+    gener_pdf : Callable
+        采样器采样用的分布的概率密度函数，必须保证在采样范围内该函数积分为1（符合概率分布函数特征）
+    tgt_func : Callable
+        目标函数，调用方式为tgts = tgt_func(smps)
+    tgt_pdf : Callable
+        目标变量真实分布的概率密度函数，若是已知的，可以设置
+    n_mc : int
+        采样数量 
+    cumsum : bool
+        若为True, 则对采样样本累计进行蒙特卡洛估计，即返回收敛过程
+        
+    Returns
+    --------
+    mc_res : np.ndarray
+        蒙特卡洛估计结果
+    smps : np.ndarray
+        采样取得的样本
+        
+    Examples
+    --------
+    >>> # 估计y=4-x^2在[-2, 2]区间上的面积（真实值为32/3=10.6666...）
+    >>> # 用均匀分布采样:
+    >>> n_mc = 10000
+    >>> smp_gener = lambda n: np.random.uniform(-2, 2, n)
+    >>> gener_pdf = lambda x: 1 / 4
+    >>> tgt_func = lambda x: 4 - x**2
+    >>> print(mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc))
+    10.672217965691754
+    >>> from dramkit import plot_series
+    >>> df = pd.DataFrame({'v_u': mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc, cumsum=True)})
+    >>> plot_series(df, {'v_u': None}, figsize=(8, 5))
+    >>> # 用标准正态分布采样：
+    >>> smp_gener = lambda n: np.clip(np.random.randn(n), -2, 2)
+    >>> gener_pdf = lambda x: normpdf(0, 1, x)
+    >>> print(mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc))
+    10.667448905107554
+    >>> df['v_n'] = mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc, cumsum=True)
+    >>> plot_series(df, {'v_u': ('-b', None), 'v_n': '-r'}, figsize=(8, 5))
+    >>> # 用概率密度函数为f=(4-x^2)/(32/3)的分布（即使将tgt_func按概率积分为1进行了缩放）进行采样:
+    >>> C = 32/3
+    >>> # C = 16/3
+    >>> # 均匀分布和其他分布转化，参考：
+    >>> # https://blog.csdn.net/Hoooo_233/article/details/107010480
+    >>> # Python求反函数，参考：https://blog.csdn.net/jacke121/article/details/120493603
+    >>> tgt_cdf = lambda x: (4*x - (x**3)/3) / C
+    >>> from pynverse import inversefunc
+    >>> invtrans_func = lambda p: inversefunc(tgt_cdf, y_values=p, domain=[-2, 2])
+    >>> smp_gener = lambda n: invtrans_func(np.random.uniform(-0.5, 0.5, n))
+    >>> gener_pdf = lambda x: (4-x**2) / C
+    >>> print(mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc))
+    10.666666666666664
+    >>> df['v_self'] = mc_important_sample(smp_gener, gener_pdf, tgt_func, n_mc=n_mc, cumsum=True)
+    >>> plot_series(df, {'v_u': '-b', 'v_n': '-r', 'v_self': '-g'}, figsize=(8, 5))
+    '''
+    smps = smp_gener(n_mc)
+    gen_pdf = gener_pdf(smps)
+    tgt_pdf = tgt_pdf(smps) if not isnull(tgt_pdf) else 1.0
+    weights = tgt_pdf / gen_pdf
+    tgts = tgt_func(smps) * weights
+    if not cumsum:
+        mc_res = np.sum(tgts) / float(n_mc)
+    else:
+        mc_res = np.cumsum(tgts) / np.arange(1, n_mc+1)
+    return mc_res
+
+
 def get_at_range_prob_norm(mu, sigma, low, high):
     '''获取正态分布N(mu,sigma)取值范围在low和high之间的概率'''
     # 计算标准化的z_score值
     z_low = (low - mu) / sigma
     z_high = (high - mu) / sigma
     # 计算在z-score范围内的概率
     prob = norm.cdf(z_high) - norm.cdf(z_low)
@@ -1270,23 +1362,23 @@
     #                     get_pct_loc(value, values, isnew=True, method=method)
     df['PctLoc'] = df['v'].rolling(lag).apply(lambda x:
               get_pct_loc(x.iloc[-1], x.iloc[:-1], isnew=True, method=method))
     df.index = ori_idx
     return df['PctLoc']
 
 
-def mean_update_inrc(v, mean, n):
+def cal_mean_update_inrc(v, mean, n):
     '''均值增量更新算法(根据新值v和已知均值mean，已知技术n计算新的均值)'''
     res = (mean * n + v) / (n+1)
     # res = mean + (v - mean) / (n+1)
     return res
 
 
-def robbins_morno(vals, alphas=None, mean_init=0):
-    '''Robbins-Monro算法'''
+def cal_mean_robbins_morno(vals, alphas=None, mean_init=0):
+    '''Robbins-Monro算法计算均值'''
     n = len(vals)
     if isnull(alphas):
         alphas = [1/k for k in range(1, n+1)]
     m = mean_init
     for k in range(n):
         m += alphas[k] * (vals[k] - m)
     return m
```

### Comparing `dramkit-0.5.45/dramkit/datsci/stepreg.py` & `dramkit-0.5.46/dramkit/datsci/stepreg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 
-from typing import Literal, NewType, Union
+from beartype.typing import Literal, NewType, Union
 
 import numpy as np
 import pandas as pd
 from beartype import beartype
 from beartype.typing import List
 from joblib import Parallel, delayed
 
 from dramkit.datsci.lr import lr_smf_df
-from dramkit.gentools import check_list_arg, isna
-from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
+from dramkit.gentools import check_list_arg, isna, raise_warn
 
 
 def _get_new_literal_type(name, l):
     return NewType(name, eval('Literal[{}]'.format(', '.join(["'%s'"%x for x in l]))))
 
-
 # 允许的模型评价指标
 CRITERIA = ['bic', 'aic', 'r2', 'r2_adj', 'fvalue', 'mse']
-CriterionType = _get_new_literal_type('CriterionType', CRITERIA)
 CRI_ALIAS = {'r2': 'rsquared', 'r2_adj': 'rsquared_adj', 'mse': 'mse_resid'}
+CriterionType = _get_new_literal_type('CriterionType',
+                                      CRITERIA+list(CRI_ALIAS.values()))
 SMALL_BETTER = ['bic', 'aic', 'mse_resid']
 LARGE_BETTER = ['rsquared', 'rsquared_adj', 'fvalue']
 
 # 允许的变量筛选方法
 METHODS = ['backward', 'forward', 'both']
 MethodType = _get_new_literal_type('MethodType', METHODS)
 
@@ -32,38 +31,27 @@
 def joblib_parl(func, args_list, n_jobs, backend='loky',
                 **kw_jb):
     jb = Parallel(n_jobs=n_jobs, backend=backend, **kw_jb)
     res = jb(delayed(func)(*args) for args in args_list)
     return res
 
 
-def joblib_parl_(func, args_list, n_jobs, backend='loky',
-                **kw_jb):
-    jb = Parallel(n_jobs=n_jobs, backend=backend, **kw_jb)
-    res = jb(delayed(func)(args) for args in args_list)
-    return res
-
-
 def _fit_new(df, ycol, x_olds, x_new, intercept,
              criterion, add_or_del):
     '''增加或减少单个自变量，模型拟合'''
     assert add_or_del in ['add', 'del'], '`add_or_del`必须为`add`或`del`！'
     if add_or_del == 'add':
         x_mdl = list(x_olds) + [x_new]
     elif add_or_del == 'del':
         x_mdl = set(x_olds) - set([x_new])
     mdl = lr_smf_df(df, ycol, xcols=x_mdl, intercept=intercept)
     score = eval('mdl.'+criterion)
     return score, x_new, mdl
 
 
-def _fit_new_(args):
-    return _fit_new(*args)
-
-
 @beartype
 def stepreg(df: pd.DataFrame,
             ycol: str,
             xcols: Union[List[str], None] = None,
             xcols_fixed: Union[List[str], str, None] = None,
             intercept: bool = True,
             criterion: CriterionType = 'bic',
@@ -73,15 +61,14 @@
             cri_abs_out: Union[float, int, None] = None,
             x_pvalue_out: float = 0.05,
             nx_min: Union[int, None] = None,
             nx_max: Union[int, None] = None,
             method: MethodType = 'both',
             max_iter: Union[int, None] = None,
             n_jobs: int = 1,
-            # jb_backend: str = 'loky',
             jb_backend: str = 'threading',
             kw_jb: dict = {},
             **kwargs):
 
     '''
     逐步回归
 
@@ -90,19 +77,19 @@
     df : pd.Dataframe
         回归用数据
     ycol : str
         回归分析因变量列名
     xcols : list, None
         指定自变量X的列名范围，不指定则默认为除ycol之外的所有列
     xcols_fixed : list, None
-        必须包含的自变量列名
+        回归模型中必须包含的自变量列名
     intercept : bool
         模型是否有截距项，默认有
     criterion : str
-        模型优化评价标准指标
+        模型优化评价标准指标，可选'bic', 'aic', 'r2', 'r2_adj', 'fvalue', 'mse'
     cri_tol_in : float
         | 准入时模型评价指标变化量阈值（应大于等于0）
         | 对于越小越好的指标，旧值-新值>cri_tol_in，则准入
         | 对于越大越好的指标，新值-旧值>cir_tol_in，则准入
     cri_tol_out : float
         | 准出时模型评价指标变化量阈值（应大于等于0）
         | 对于越小越好的指标，旧值-新值>cri_tol_out，则准出
@@ -118,35 +105,47 @@
     x_pvalue_out : float
         当设置`method`=`both`时，移除变量的pvalue阈值
     nx_min : int, None
         纳入模型的自变量个数下限，默认0
     nx_max : int, None
         纳入模型的自变量个数上限，默认等于xcols的个数
     method : str
-        逐步回归筛选变量过程方法        
+        逐步回归筛选变量过程方法，可选'backward', 'forward', 'both'
     max_iter : int, None
         最大迭代轮数
     n_jobs : int
         | joblib参数n_jobs，若为0则不适用joblib，直接用循环
         | 在自变量不是很多的情况下，不使用并行反而更快
     jb_backend : str
         | joblib参数backend
         | 除非要筛选的自变量特别多，否则不要用multiprocessing
     kw_jb: dict
-        joblib关键字参数
+        joblib接收的关键字参数
         
+    Returns
+    -------
+    picks : list
+        最终筛选保留的变量
+    final_mdl : statsmodels.regression.linear_model
+        最终线性回归模型
+    step_data : pd.DataFrame
+        迭代过程数据
+    
     Note
     ----
     准入准出条件判断优先顺序：自变量个数限制 > 评价指标阈值条件&评价指标变化量阈值条件
 
     References
     ----------
     - https://www.cnblogs.com/lantingg/p/9535010.html
     - https://www.jianshu.com/p/bb1c6c319d9b
     '''
+    
+    if df.shape[0] < 2:
+        raise ValueError('样本数量少于两条！')
         
     # 模型评价指标名称统一
     if criterion in CRI_ALIAS:
         criterion = CRI_ALIAS[criterion]
         
     # 模型评价指标准入准出阈值控制
     if isna(cri_abs_in):
@@ -182,14 +181,24 @@
             else:
                 return cur_cri >= cri_abs_out
     
     # 自变量可选范围
     xcols = check_list_arg(xcols, allow_none=True)
     xcols = [c for c in df.columns if c != ycol] if isna(xcols) else xcols
     
+    # 最小有效样本检查
+    notna = (~df[xcols+[ycol]].isna()).sum(axis=1)
+    notna = notna[notna == len(xcols+[ycol])]
+    if len(notna) < 2:
+        raise ValueError('数据完整的样本数量小于2！')
+        
+    # 无效值检查
+    if df[xcols+[ycol]].isna().sum().sum() > 0:
+        raise_warn('DataNaNWarning', '数据中存在无效值。')
+    
     # 最大迭代轮数
     if isna(max_iter):
         max_iter = sum(range(1, len(xcols)+1))
     
     # 必选自变量
     xcols_fixed = check_list_arg(xcols_fixed, allow_none=True)
     xcols_fixed = [] if isna(xcols_fixed) else xcols_fixed
@@ -199,187 +208,191 @@
     nx_max = len(xcols) if isna(nx_max) else nx_max
     
     # 若必须全选，则直接返回全部变量回归模型
     if nx_min >= len(xcols):
         final_mdl = lr_smf_df(df, ycol, xcols=xcols, intercept=intercept)
         final_cri = eval('final_mdl.'+criterion)
         pvalues = final_mdl.pvalues.to_dict()
+        params = final_mdl.params.to_dict()
         step_data = [(final_cri, # 评价指标值
                       xcols, # 保留的变量列表
+                      params, # 保留的变量系数
                       pvalues, # 变量P值
                       ('add', xcols)) # 变量筛选动作
                      ]
         step_data = pd.DataFrame(
                         step_data,
-                        columns=[criterion, 'picks', 'pvalue', 'change'])
+                        columns=[criterion, 'picks', 'param', 'pvalue', 'change'])
         return xcols, final_mdl, step_data
     
     if method in ['forward', 'both']:
         picks = xcols_fixed.copy()
         lefts = [x for x in xcols if x not in picks+[ycol]]
     else:
         picks = [x for x in xcols if x != ycol]
-        lefts = [x for x in picks if picks if x not in xcols_fixed]
+        lefts = [x for x in picks if x not in xcols_fixed]
       
     # 初始化评价指标值
     if picks:
         final_mdl = lr_smf_df(df, ycol, xcols=picks, intercept=intercept)
         final_cri = eval('final_mdl.'+criterion)
         cur_cri = final_cri
         pvalues = final_mdl.pvalues.to_dict()
+        params = final_mdl.params.to_dict()
     else:
         if criterion in SMALL_BETTER:
             final_cri, cur_cri = np.inf, np.inf
         else:
             final_cri, cur_cri = -np.inf, -np.inf
         pvalues = {}
+        params = {}
     need_imprv = True
     # 存放过程数据
     step_data = [(final_cri, # 评价指标值
                   picks.copy(), # 保留的变量列表
+                  params, # 保留的变量系数
                   pvalues, # 变量P值
                   () if len(picks) == 0 else ('add', picks)) # 变量筛选动作
                  ]
     
+    def _joblib_parl_reg(args_list):
+        if n_jobs == 0:
+            cri_xnew = [_fit_new(*args) for args in args_list]
+        else:
+            cri_xnew = joblib_parl(_fit_new, args_list, n_jobs, backend=jb_backend, **kw_jb)
+        cri_xnew.sort(key=lambda x: x[0])
+        return cri_xnew
+    
     # 逐步准入
     if method in ['forward', 'both']:
         i = 0
         while lefts and need_imprv and i < max_iter:
             args_list = [[df, ycol, picks, new, intercept, criterion, 'add'] for new in lefts]
-            if n_jobs == 0:
-                cri_xnew = [_fit_new(*args) for args in args_list]
-            else:
-                if n_jobs != 1 and jb_backend == 'multiprocessing':
-                    # joblib设置backend为multiprocessing时须将执行函数入参改为_fit_new_这样的形式，否则会卡住没反应
-                    cri_xnew = joblib_parl_(_fit_new_, args_list, n_jobs, backend=jb_backend, **kw_jb)
-                    # cri_xnew = multi_process_concurrent(
-                    #             _fit_new, args_list, multi_line=n_jobs, keep_order=False, logger=False)
-                else:
-                    cri_xnew = joblib_parl(_fit_new, args_list, n_jobs, backend=jb_backend, **kw_jb)
-            cri_xnew.sort(key=lambda x: x[0])
+            cri_xnew = _joblib_parl_reg(args_list)
             if criterion in SMALL_BETTER:
                 cur_cri, xbest, cur_mdl = cri_xnew[0]
             else:
                 cur_cri, xbest, cur_mdl = cri_xnew[-1]
             better = _is_better(final_cri, cur_cri, 'add')
             abs_ok = _abs_ok(cur_cri, 'add')
             if (len(picks) < nx_min) or \
                (len(picks) < nx_max and abs_ok and better):
                 final_cri, final_mdl = cur_cri, cur_mdl
                 picks.append(xbest)
                 lefts.remove(xbest)
                 step_data.append((final_cri, picks.copy(),
-                                  final_mdl.pvalues.to_dict(), ('add', [xbest])))
+                                  final_mdl.params.to_dict(),
+                                  final_mdl.pvalues.to_dict(),
+                                  ('add', [xbest])))
             else:
                 need_imprv = False
                 
             # 准入后剔除不显著变量
             if method == 'both':
                 n_picks = len(picks)
-                n_can_del = max(n_picks-nx_min, 0)
+                n_can_del = n_picks - nx_min
                 if n_can_del > 0:
                     if intercept:
                         may_dels = final_mdl.pvalues.iloc[1:].copy()
                     else:
                         may_dels = final_mdl.pvalues.copy()
                     may_dels = may_dels.sort_values(ascending=False)
                     may_dels = may_dels[may_dels > x_pvalue_out]
                     to_dels = may_dels.index.tolist()[:n_can_del]
                     if len(to_dels) > 0:
                         for xcol in to_dels:
                             picks.remove(xcol)
                         final_mdl = lr_smf_df(df, ycol, xcols=picks, intercept=intercept)
                         final_cri = eval('final_mdl.'+criterion)
                         step_data.append((final_cri, picks.copy(),
-                                          final_mdl.pvalues.to_dict(), ('del', to_dels)))
+                                          final_mdl.params.to_dict(),
+                                          final_mdl.pvalues.to_dict(),
+                                          ('del', to_dels)))
                     
             i += 1
     
     # 逐步准出
     elif method == 'backward':
         i = 0
         while lefts and need_imprv and i < max_iter:
             args_list = [[df, ycol, picks, new, intercept, criterion, 'del'] for new in lefts]
-            if n_jobs == 0:
-                cri_xnew = [_fit_new(*args) for args in args_list]
-            else:
-                if n_jobs != 1 and jb_backend == 'multiprocessing':
-                    cri_xnew = joblib_parl_(_fit_new_, args_list, n_jobs, backend=jb_backend, **kw_jb)
-                    # cri_xnew = multi_process_concurrent(
-                    #             _fit_new, args_list, multi_line=n_jobs, keep_order=False, logger=False)
-                else:
-                    cri_xnew = joblib_parl(_fit_new, args_list, n_jobs, backend=jb_backend, **kw_jb)
-            cri_xnew.sort(key=lambda x: x[0])
+            cri_xnew = _joblib_parl_reg(args_list)
             if criterion in SMALL_BETTER:
                 cur_cri, xworst, cur_mdl = cri_xnew[0]
             else:
                 cur_cri, xworst, cur_mdl = cri_xnew[-1]
             better = _is_better(final_cri, cur_cri, 'del')
             abs_ok = _abs_ok(cur_cri, 'del')
             if (len(picks) > nx_max) or \
                (len(picks) > nx_min and abs_ok and better):
                 final_cri, final_mdl = cur_cri, cur_mdl
                 picks.remove(xworst)
                 lefts.remove(xworst)
                 step_data.append((final_cri, picks.copy(),
-                                  final_mdl.pvalues.to_dict(), ('del', [xworst])))
+                                  final_mdl.params.to_dict(),
+                                  final_mdl.pvalues.to_dict(),
+                                  ('del', [xworst])))
             else:
                 need_imprv = False
             i += 1
     
     step_data = pd.DataFrame(
                     step_data,
-                    columns=[criterion, 'picks', 'pvalue', 'change'])
+                    columns=[criterion, 'picks', 'param', 'pvalue', 'change'])
     
     return picks, final_mdl, step_data
 
 
-def stepreg_mp(args):
-    return stepreg(*args)
-
-
 if __name__ == '__main__':
     import sklearn.datasets as datasets
     from dramkit import TimeRecoder
-    from dramkit.gentools import func_runtime_test
-    tr = TimeRecoder()
+    
     # '''
     data = datasets.load_diabetes()
     xcols, y = data['feature_names'], data['target']
     df = pd.DataFrame(data['data'], columns=xcols)
     df['y'] = y
 
 
     ycol = 'y'
     xcols = None
+    # xcols = [x for x in df.columns if x != ycol]
     xcols_fixed = None
     intercept = True
     criterion = 'bic'
+    # criterion = 'rsquared'
+    # criterion = 'r2'
+    # criterion = 'r2_adj'
+    # criterion = 'rsquared_adj'
     cri_tol_in = 0.0
     cri_tol_out = 0.0
     cri_abs_in = None
     cri_abs_out = None
     x_pvalue_out = 0.05
     nx_min = None
-    nx_min = 5
+    # nx_min = 5
     # nx_min = df.shape[1]-1
     nx_max = None
     # method = 'forward'
     method = 'both'
     # method = 'backward'
     max_iter = None
-    # n_jobs = 5
+    # max_iter = 2
     n_jobs = 0
-    jb_backend: str = 'loky'
-    # jb_backend = 'threading'
+    # n_jobs = 1
+    jb_backend = 'threading'
+    # jb_backend: str = 'loky'
     # jb_backend = 'multiprocessing'
     kw_jb = {}
     kwargs = {}
     # '''
     
+    # # df = df.iloc[:4, :]
+    # df.iloc[:2, :] = np.nan
+    
     args = [df,
             ycol,
             xcols,
             xcols_fixed,
             intercept,
             criterion,
             cri_tol_in,
@@ -390,25 +403,27 @@
             nx_min,
             nx_max,
             method,            
             max_iter,
             n_jobs,
             jb_backend
             ]
-    n = 100
+    n = 10
 
     # '''
+    tr = TimeRecoder()
     final_xcols, final_mdl, step_data = \
           stepreg(*args)
     print(final_xcols)
 
     tr.used()
     # '''
 
     '''
+    from dramkit.gentools import func_runtime_test
     def test():
         t, res = func_runtime_test(
                           stepreg,
                           n=n,
                           return_all=True,
                           df=df,
                           ycol=ycol,
@@ -465,28 +480,19 @@
     pool.join()
     results = [eval('task_%s.get()'%i) for i in range(n)]
     print(results[0][0])
     tr.used()
     # '''
     
     '''
+    from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
     tr = TimeRecoder()
     res = multi_process_concurrent(stepreg,
                                    [args for _ in range(n)],
                                    multi_line=5,
                                    keep_order=False)
     print(res[0][0])
     tr.used()
     # '''
-    
-    '''
-    tr = TimeRecoder()
-    res = multi_process_concurrent(stepreg_mp,
-                                   [args for _ in range(n)],
-                                   multi_line=5,
-                                   keep_order=True)
-    print(res[0][0])
-    tr.used()
-    # '''
```

### Comparing `dramkit-0.5.45/dramkit/datsci/time_series.py` & `dramkit-0.5.46/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/topsis.py` & `dramkit-0.5.46/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.46/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/utils_ml.py` & `dramkit-0.5.46/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/datsci/zigzag.py` & `dramkit-0.5.46/dramkit/datsci/zigzag.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.46/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/gentools.py` & `dramkit-0.5.46/dramkit/gentools.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 import inspect
 import logging
 import operator
 import re
 import string
 import sys
 import time
+import warnings
 import traceback
 import urllib.parse
 from collections import Counter
 from collections.abc import Callable, Iterable
 from functools import reduce, wraps
 from io import StringIO
 from itertools import product
 from random import randint, random, uniform
 from typing import Any, Literal, NewType, Union
 
 import numpy as np
 import pandas as pd
 from beartype import beartype as checkin
-from beartype.typing import List
+from beartype.typing import List, Tuple
 from tqdm import tqdm
 
 from dramkit.logtools.utils_logger import logger_show
 from dramkit.speedup.multi_thread import SingleThread
 
 PYTHON_VERSION = '.'.join([x.zfill(2) for x in sys.version.split(' ')[0].split('.')])
 
@@ -47,15 +48,15 @@
     >>> tr.useds()
     >>> time.sleep(60)
     >>> tr.usedm()
     >>> time.sleep(5)
     >>> tr.used()
     '''
     
-    def __init__(self, monotonic=True, logger=None):
+    def __init__(self, monotonic=False, logger=None):
         self.monotonic = monotonic
         self.strt_tm = self.now()
         self.end_tm = None
         self.logger = logger
         
     def _check_logger(self, logger=None):
         if isnull(logger):
@@ -299,14 +300,20 @@
                     logger_error=logger_error,
                     logger_timeout=logger_timeout,
                     timeout_show_str=timeout_show_str,
                     kill_when_timeout=kill_when_timeout,
                     **kwargs)
         return timeouter
     return transfunc
+
+
+def _chose_logger(logger, kwargs):
+    if isnull(logger) and 'logger' in kwargs:
+        return kwargs['logger']
+    return logger
         
         
 def try_repeat_run(n_max_run=3,
                    logger=None,
                    sleep_seconds=0,
                    force_rep=False):
     '''
@@ -349,106 +356,178 @@
     >>> a = repeat_test('repeat test...')
     >>> print(a)
     '''
     def transfunc(func):
         @wraps(func)
         def repeater(*args, **kwargs):
             '''尝试多次运行func'''
+            logger_ = _chose_logger(logger, kwargs)
             if not force_rep:
                 n_run, ok = 0, False
                 while not ok and n_run < n_max_run:
                     n_run += 1
-                    # if isnull(logger) and 'logger' in kwargs:
-                    #     logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
-                    #                 kwargs['logger'], 'info')
-                    # else:
-                    #     logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
-                    #                 logger, 'info')
+                    # logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
+                    #             logger_, 'info')
                     try:
                         result = func(*args, **kwargs)
                         return result
                     except:
                         if n_run == n_max_run:
-                            if isnull(logger) and 'logger' in kwargs:
-                                logger_show(traceback.format_exc(), kwargs['logger'])
-                                logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
-                                            kwargs['logger'], 'error')
-                            else:
-                                logger_show(traceback.format_exc(), logger)
-                                logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
-                                            logger, 'error')                            
+                            logger_show(traceback.format_exc(), logger_)
+                            logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
+                                        logger_, 'error')                            
                             return
                         else:
                             if sleep_seconds > 0:
                                 time.sleep(sleep_seconds)
                             else:
                                 pass
             else:
                 n_run = 0
                 while n_run < n_max_run:
                     n_run += 1
                     try:
                         result = func(*args, **kwargs)
-                        if isnull(logger) and 'logger' in kwargs:
-                            logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
-                                        kwargs['logger'], 'info')
-                        else:
-                            logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
-                                        logger, 'info')
+                        logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
+                                    logger_, 'info')
                     except:
-                        if isnull(logger) and 'logger' in kwargs:
-                            logger_show(traceback.format_exc(), kwargs['logger'])
-                            logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
-                                        kwargs['logger'], 'error')
-                        else:
-                            logger_show(traceback.format_exc(), logger)
-                            logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
-                                        logger, 'error')
+                        logger_show(traceback.format_exc(), logger_)
+                        logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
+                                    logger_, 'error')
                         result = None
                     if sleep_seconds > 0:
                         time.sleep(sleep_seconds)
                 return result
         return repeater
     return transfunc
 
 
+def catch_warnings(logger=None):
+    '''
+    作为装饰器捕获函数运行警告
+    
+    Parameters
+    ----------
+    logger : None, logging.Logger
+        日志记录器，若为None，则会优先使用被调用函数参数中的logger
+    
+    Examples
+    --------
+    .. code-block:: python
+        :linenos:
+
+        from dramkit import simple_logger
+        logger = simple_logger()
+
+        @catch_warnings(logger)
+        def test_warn():
+            print('test warn...')
+            raise_warn('TestWarn', 'test warn')
+            
+        @catch_warnings()
+        def test_warn1(logger=None):
+            raise_warn('TestWarn1', 'test warn1')
+            
+        @catch_warnings(simple_logger(logname='test'))
+        @capture_print()
+        def test_warn2(logger=None):
+            print('test_warn2...')
+            
+        @catch_warnings(False)
+        def test_warn3(logger=None):
+            print('test_warn3...')
+            raise_warn('TestWarn3', 'test warn3')
+
+    >>> test_warn()
+    >>> test_warn1(logger=simple_logger('./_test/catch_warnings_test.log'))
+    >>> test_warn2(logger=simple_logger('./_test/catch_warnings_test.log'))    
+    >>> test_warn3()    
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def catcher(*args, **kwargs):
+            '''运行func并捕获警告信息'''
+            logger_ = _chose_logger(logger, kwargs)
+            with warnings.catch_warnings(record=True) as warns:
+                res = func(*args, **kwargs)
+                for warn in warns:
+                    wmsg = '%s: %s'%(warn.category.__name__, warn.message)
+                    logger_show(wmsg, logger=logger_, level='warn')
+            return res
+        return catcher
+    return transfunc
+
+
+def raise_warn(name: str,
+               msg: str,
+               code: Union[int, str] = None,
+               **kwargs):
+    '''
+    | 抛出警告
+    | name警告名称、msg警告信息、code警告代码、logger日志记录器
+    
+    Examples
+    --------
+    >>> from dramkit import simple_logger
+    >>> logger = simple_logger('./_test/test_raise_warn.log', 'a')    
+    >>> raise_warn('MyWarn1', 'test mywarn', logger=logger)
+    >>> raise_warn('MyWarn2', 'test mywarn', code=1, logger=logger)
+    >>> raise_warn('MyWarn1', 'test mywarn')
+    '''
+    exec('class {}(Warning): pass'.format(name))
+    if not 'logger' in kwargs:
+        warnings.warn(msg, category=eval(name))
+        return
+    wmsg = '%s: %s'%(name, msg)
+    if not isnull(code):
+        wmsg = 'WarnCode: %s\n%s'%(code, wmsg)
+    with warnings.catch_warnings(record=True) as warns:
+        warnings.warn(wmsg, category=eval(name))
+        for warn in warns:
+            logger_show(warn.message, logger=kwargs['logger'], level='warn')
+
+
 def raise_error(name: str,
                 msg: str,
-                logger: logging.Logger = None,
-                code: Union[int, str] = None):
+                code: Union[int, str] = None,
+                **kwargs):
     '''
     | 抛出异常
     | name异常名称、msg异常信息、code异常代码、logger日志记录器
     
     Examples
     --------
     >>> from dramkit import simple_logger
     >>> logger = simple_logger('./_test/test_raise_error.log', 'a')    
     >>> raise_error('MyError1', 'test myerror', logger=logger)
-    >>> raise_error('MyError2', 'test myerror', logger=logger, code=1)
+    >>> raise_error('MyError2', 'test myerror', code=1, logger=logger)
     '''
     exec('class {}(Exception): pass'.format(name))
-    try:
+    if not 'logger' in kwargs:
         exec('raise {}("{}")'.format(name, msg))
-    except:
-        emsg = traceback.format_exc()
-        if not isnull(code):
-            emsg = 'ErrorCode: %s\n'%code + emsg
-        logger_show(emsg, logger=logger,
-                    level='err', err_exc_info=False)
-        raise
+    else:
+        try:
+            exec('raise {}("{}")'.format(name, msg))
+        except:
+            emsg = traceback.format_exc().rstrip()
+            # emsg = traceback.format_exc()
+            if not isnull(code):
+                emsg = 'ErrorCode: %s\n'%code + emsg
+            logger_show(emsg, logger=kwargs['logger'],
+                        level='err', err_exc_info=False)
+            raise
         
         
 class RaiseError(object):
     
     def __init__(self, logger=None):
         self.logger = logger
         
     def raise_error(self, name, msg, code=None):
-        raise_error(name, msg, logger=self.logger, code=code)
+        raise_error(name, msg, code=code, logger=self.logger)
 
 
 def catch_error(logger=None, raise_error=True):
     '''
     作为装饰器捕获函数运行错误
     
     Parameters
@@ -492,28 +571,26 @@
     def transfunc(func):
         @wraps(func)
         def catcher(*args, **kwargs):
             '''运行func并捕获错误信息'''
             try:
                 return func(*args, **kwargs)
             except:
+                logger_ = _chose_logger(logger, kwargs)
                 err = 'func `%s` error info:\n%s'%(func.__name__, traceback.format_exc())
-                if isnull(logger) and 'logger' in kwargs:
-                    logger_show(err, kwargs['logger'], 'error', err_exc_info=False)
-                else:
-                    logger_show(err, logger, 'error', err_exc_info=False)
+                logger_show(err, logger_, 'error', err_exc_info=False)
                 if raise_error:
                     raise
                 else:
                     return None
         return catcher
     return transfunc
 
 
-def capture_print(logger=None, del_last_blank=True):
+def capture_print(logger=None, del_last_blank=True, ori_print=False):
     '''
     作为装饰器捕获函数中的print内容
     
     Parameters
     ----------
     logger : None, logging.Logger
         日志记录器，若为None，则会优先使用被调用函数参数中的logger
@@ -537,21 +614,26 @@
         @capture_print(simple_logger(logname='test'))
         def test_print2(logger=None):
             print('test_print2...')
             
         @capture_print(False)
         def test_print3(logger=None):
             print('test_print3...')
+            
+        @capture_print()
+        def test_print4(**kwargs):
+            print('test_print4...')
 
     >>> test_print()
     test_print...
         [INFO: 2023-04-29 10:45:41,671]
     >>> test_print1(logger=simple_logger('./_test/capture_print_test.log'))
     >>> test_print2(logger=simple_logger('./_test/capture_print_test.log'))    
     >>> test_print3()
+    >>> test_print4(logger=simple_logger('./_test/capture_print_test.log'))
     '''
     def transfunc(func):
         @wraps(func)
         def capturer(*args, **kwargs):
             '''运行func并捕获print内容'''
             # 替换默认的标准输出流
             output = StringIO()
@@ -561,23 +643,92 @@
             sys.stdout = sys.__stdout__
             strs = output.getvalue()
             if del_last_blank and len(strs) > 0:
                 strs = strs[:-1] if strs[-1] in string.whitespace else strs
             # if del_last_blank:
             #     strs = strs.rstrip()
             if len(strs) > 0:
-                if isnull(logger) and 'logger' in kwargs:
-                    logger_show(strs, kwargs['logger'], 'info')
+                if ori_print:
+                    print(strs)
                 else:
-                    logger_show(strs, logger, 'info')
+                    logger_ = _chose_logger(logger, kwargs)
+                    logger_show(strs, logger_, 'info')
             return result
         return capturer
     return transfunc
 
 
+def record_run_time(logger=None):
+    '''
+    作为装饰器记录函数进入、退出时间以及用时
+    
+    Examples
+    --------
+    .. code-block:: python
+        :linenos:
+
+        from dramkit import simple_logger
+        logger = simple_logger()
+
+        @record_run_time(logger)
+        def wait():
+            print('wait...')
+            time.sleep(3)
+
+        @record_run_time()
+        def wait1(logger=None):
+            print('wait...')
+            time.sleep(3)
+            
+        @record_run_time(simple_logger(logname='test'))
+        def wait2(logger=None):
+            print('wait...')
+            time.sleep(3)
+            
+        @record_run_time(False)
+        def wait3(logger=None):
+            print('wait...')
+            time.sleep(3)
+
+    >>> wait()
+    enter func `wait` at: 2023-07-06 16:45:26.
+        [INFO: 2023-07-06 16:45:26,042]
+    wait...
+    exit func `wait` at: 2023-07-06 16:45:29.
+        [INFO: 2023-07-06 16:45:29,048]
+    func `wait` run time: 3.006651s.
+        [INFO: 2023-07-06 16:45:29,049]
+    >>> wait1(logger=simple_logger('./_test/record_run_time_test.log'))
+    >>> wait1(logger=simple_logger('./_test/record_run_time_test.log', screen_show=False))
+    >>> wait2(logger=simple_logger('./_test/record_run_time_test.log'))    
+    >>> wait3()
+
+    See Also
+    --------
+    :func:`dramkit.gentools.log_used_time`
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def timer(*args, **kwargs):
+            '''运行func并记录用时'''
+            logger_ = _chose_logger(logger, kwargs)
+            t0 = time.time()
+            logger_show('enter func `%s` at: %s.'%(func.__name__, time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(t0))),
+                        logger_, 'info')
+            result = func(*args, **kwargs)
+            t = time.time()
+            # logger_show('exit func `%s` at: %s.'%(func.__name__, time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(t))),
+            #             logger_, 'info')
+            logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
+                        logger_, 'info')
+            return result
+        return timer
+    return transfunc
+
+
 def log_used_time(logger=None):
     '''
     作为装饰器记录函数运行用时
     
     Parameters
     ----------
     logger : None, logging.Logger
@@ -634,20 +785,17 @@
     def transfunc(func):
         @wraps(func)
         def timer(*args, **kwargs):
             '''运行func并记录用时'''
             t0 = time.monotonic()
             result = func(*args, **kwargs)
             t = time.monotonic()
-            if isnull(logger) and 'logger' in kwargs:
-                logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
-                            kwargs['logger'], 'info')
-            else:
-                logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
-                            logger, 'info')
+            logger_ = _chose_logger(logger, kwargs)
+            logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
+                        logger_, 'info')
             return result
         return timer
     return transfunc
 
 
 def print_used_time(func):
     '''
@@ -697,14 +845,49 @@
             logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)), kwargs['logger'])
         else:
             print('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)))
         return result
     return timer
 
 
+def func_params_process_decorator(func_params, *args_p, **kwargs_p):
+    '''
+    | 作为装饰器，在调用函数之前对函数入参进行处理 
+    | func_params接收参数顺序必须为func_params(*args_p, *args, **kwargs_p, **kwargs) 
+    | 其中args_p, kwargs_p为func_params本身参数，args和kwargs为目标函数参数
+
+    Examples
+    --------
+    >>> def params_process(a, *args, b=3, **kwargs):
+    ...    args = list(args)
+    ...    args[0] = args[0] + a
+    ...    if 'z' in kwargs:
+    ...        kwargs['z'] = kwargs['z'] + b
+    ...    return args, kwargs
+    ...
+    ... @func_params_process_decorator(params_process, 2, b=4)
+    ... def a(x, y, z=4):
+    ...     return x+y+z
+    >>> a(2, 3)
+    11
+    >>> a(2, 3, z=5)
+    16
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def processer(*args, **kwargs):
+            '''函数结果处理'''
+            args_, kwargs_ = func_params(
+                             *args_p, *args, **kwargs_p, **kwargs)
+            res = func(*args_, **kwargs_)
+            return res
+        return processer
+    return transfunc
+
+
 def func_res_process_decorator(func_res, *args_res, **kwargs_res):
     '''
     作为装饰器处理函数输出结果
     
     Examples
     --------
     >>> def res_process(res, k, b):
@@ -858,15 +1041,16 @@
     elif func_update == 'replace':
         func_update = lambda arg, arg_old: arg
     arg_new = func_update(arg, arg_old)
         
     return arg_new, kwargs
 
 
-def roulette_base(fitness):
+@checkin
+def roulette_base(fitness: Union[list, tuple, dict]):
     '''
     基本轮盘赌法
     
     Parameters
     ----------
     fitness : list
         所有备选对象的fitness值列表
@@ -877,24 +1061,28 @@
 
     :returns: `int` - 返回被选中对象的索引号
 
     References
     ----------
     https://blog.csdn.net/armwangEric/article/details/50775206
     '''
-    sum_fits = sum(fitness)
+    if isinstance(fitness, dict):
+        sum_fits = sum(list(fitness.values()))
+    else:
+        sum_fits = sum(fitness)
+        fitness = dict(enumerate(fitness))
     rand_point = uniform(0, sum_fits)
     accumulator = 0.0
-    for idx, fitn in enumerate(fitness):
+    for idx, fitn in fitness.items():
         accumulator += fitn
-        if accumulator >= rand_point:
+        if rand_point <= accumulator:
             return idx
 
 
-def roulette_stochastic_accept(fitness):
+def roulette_stochastic_accept(fitness: Union[list, tuple, dict]):
     '''
     轮盘赌法，随机接受法
     
     Parameters
     ----------
     fitness : list
         所有备选对象的fitness值列表
@@ -905,20 +1093,23 @@
 
     :returns: `int` - 返回被选中对象的索引号
 
     References
     ----------
     https://blog.csdn.net/armwangEric/article/details/50775206
     '''
+    if not isinstance(fitness, dict):
+        fitness = dict(enumerate(fitness))
     n = len(fitness)
-    max_fit = max(fitness)
+    max_fit = max(list(fitness.values()))
+    keys = list(fitness.keys())
     while True:
         idx = randint(0, n-1)
-        if random() <= fitness[idx] / max_fit:
-            return idx
+        if random() <= fitness[keys[idx]] / max_fit:
+            return keys[idx]
 
 
 def roulette_count(fitness, n=10000, rand_func=None):
     '''
     轮盘赌法n次模拟，返回每个备选对象在n次模拟中被选中的次数
 
     Parameters
@@ -957,18 +1148,15 @@
     {'a': 988, 'b': 1971, 'c': 3041}
     '''
     
     if rand_func is None:
         rand_func = roulette_stochastic_accept
     
     if isinstance(fitness, dict):
-        keys, vals = [], []
-        for k, v in fitness.items():
-            keys.append(k)
-            vals.append(v)
+        keys, vals = list(fitness.keys()), list(fitness.values())
         randpicks = [rand_func(vals) for _ in range(n)]
         idx_picks = [(x, randpicks.count(x)) for x in range(len(vals))]
         return {keys[x[0]]: x[1] for x in idx_picks}
 
     elif (isinstance(fitness[0], list) or isinstance(fitness[0], tuple)):
         keys, vals = [], []
         for k, v in fitness:
@@ -978,14 +1166,16 @@
         idx_picks = [(x, randpicks.count(x)) for x in range(len(vals))]
         return [(keys[x[0]], x[1]) for x in idx_picks]
 
     elif (isinstance(fitness[0], int) or isinstance(fitness[0], float)):
         randpicks = [rand_func(fitness) for _ in range(n)]
         idx_picks = [(x, randpicks.count(x)) for x in range(len(fitness))]
         return idx_picks
+    
+    raise ValueError('未识别的fitness格式！')
 
 
 def rand_sum(target_sum, n, lowests, highests, isint=True, n_dot=6):
     '''
     在指定最大最小值范围内随机选取若干个随机数，所选取数之和为定值
 
     Parameters
@@ -2260,14 +2450,23 @@
         if same_keep == 'left':
             df_right = df_right.drop(same_cols, axis=1)
         elif same_keep == 'right':
             df_left = df_left.drop(same_cols, axis=1)
         else:
             raise ValueError('same_keep参数只接受`left`或`right`！')
     return pd.merge(df_left, df_right, **kwargs)
+
+
+def merge_dfs(dfs: Union[List[pd.DataFrame],
+                         Tuple[pd.DataFrame]],
+              **kw_updf):
+    res = dfs[0]
+    for k in range(1, len(dfs)):
+        res = update_df(res, dfs[k], **kw_updf)
+    return res
     
     
 def update_df(df_old, df_new, idcols=None,
               del_dup_cols=None, rep_keep='new',
               sort_cols=None, ascendings=True,
               method='merge', logger=None):
     '''
@@ -2901,15 +3100,19 @@
     '''
     if df.shape[0] == 0:
         return df
     idcols = check_list_arg(idcols, allow_none=True)
     if isnull(idcols):
         vcols = check_list_arg(vcols, allow_none=True)
         if isnull(vcols):
-            vcols = [x for x in df.columns if not x != full_col]
+            vcols = [x for x in df.columns if x != full_col]
+        df = df[[full_col]+vcols].copy()
+        if not isnull(val_nan):
+            for c in vcols:
+                df[c] = df[c].fillna(val_nan)
         res = pd.DataFrame({full_col: fulls})
         res = pd.merge(res, df, how='left', on=full_col)
         res = res.sort_values(full_col)
         if fill in ['ffill', 'bfill']:
             res = res.fillna(method=fill)
         elif fill == 'ffillbfill':
             res = res.fillna(method='ffill').fillna(method='bfill')
@@ -3351,23 +3554,68 @@
     #     cols_groupby = [cols_groupby]
     # cols = [cols_val] if isinstance(cols_val, str) else cols_val
     # df = data.reindex(columns=cols_groupby+cols)
     raise NotImplementedError
     
     
 def merge_dicts(dicts):
-    '''将多个字典合并成一个字典'''
+    '''
+    | 将多个字典合并成一个字典
+    | 注意：若字典中key相同，则合并之后前面的值会被后面的值更新覆盖
+    '''
     assert isinstance(dicts, (list, tuple))
     assert all([isinstance(x, dict) for x in dicts])
     res = {}
     for d in dicts:
         res.update(d)
     return res
 
 
+@checkin
+def get_new_literal_type(
+        name: str,
+        l: Union[List[Union[str, int, float]]]):
+    '''按l指定值的范围生成一个新的类型，类型名为name'''
+    allows = ', '.join(["'%s'"%x 
+                        if isinstance(x, str) else "%s"%x
+                        for x in l])
+    allows = 'Literal[{}]'.format(allows)
+    allows = eval(allows)
+    return NewType(name, allows)
+
+
+_DictActType = get_new_literal_type(
+    '_DictActType', ['+', '-', '*', '/', '**'])
+
+@checkin
+def merge_dicts_act(dicts: Union[List[dict]],
+                    act: str):
+    '''
+    按act指定方式进行字典合并，act支持_DictActType中指定的操作类型
+    
+    Examples
+    --------
+    >>> dicts = [{'a': 1, 'b': 2}, {'a': 2, 'b': 3}, {'c': 4}]
+    >>> merge_dicts_act(dicts, '+')
+    {'a': 3, 'b': 5, 'c': 4}
+    >>> merge_dicts_act(dicts, '*')
+    {'a': 2, 'b': 6, 'c': 4}
+    >>> merge_dicts_act(dicts, '**')
+    {'a': 1, 'b': 8, 'c': 4}
+    '''
+    res = {}
+    for d in dicts:
+        for k, v in d.items():
+            if k not in res:
+                res[k] = v
+            else:
+                exec('res[k] %s= v'%act)
+    return res
+
+
 def link_lists(lists):
     '''
     | 将多个列表连接成一个列表
     | 注：lists为列表，其每个元素也为一个列表
     
     Examples
     --------
```

### Comparing `dramkit-0.5.45/dramkit/install_check.py` & `dramkit-0.5.46/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/iotools.py` & `dramkit-0.5.46/dramkit/iotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import subprocess
 import sys
 import time
 import traceback
 import zipfile
 from pathlib import Path
 from urllib.request import urlopen
+from collections.abc import Callable
 
 import pandas as pd
 import requests
 import yaml
 from tqdm import tqdm
 
 from dramkit.datetimetools import timestamp2str
@@ -28,14 +29,15 @@
                               cut_range_to_subs,
                               get_tmp_col,
                               get_update_kwargs,
                               isnull,
                               merge_df,
                               run_func_with_timeout_thread,
                               update_df,
+                              merge_dfs,
                               raise_error,
                               fmt)
 from dramkit.logtools.utils_logger import close_log_file, logger_show
 from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
 
 _WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
@@ -589,51 +591,55 @@
                       **kwargs)
 
 
 def load_dfs_pd(fpaths,
                 kwargs_sort={},
                 kwargs_drop_dup={},
                 mark_file=False,
+                kwargs_updf={},
                 **kwargs_loaddf):
     '''
     读取指定路径列表中所有的dataframe数据文件，整合到一个df里面
 
     Parameters
     ----------
     fpaths : list
         文件夹路径列表
     kwargs_sort : dict
         设置sort_values接受的排序参数
     kwargs_drop_dup : dict
         设置drop_duplicates接受的去重参数
+    kwargs_updf :
+        :func:`dramkit.gentools.update_df` 接受的df合并参数
     **kwargs_loaddf :
         :func:`dramkit.iotools.load_df_pd` 接受的其它参数
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
     data = []
     for fpath in tqdm(fpaths):
         df = load_df_pd(fpath, **kwargs_loaddf)
         if mark_file:
             df[get_tmp_col(df, 'fromfile')] = fpath
         data.append(df)
-    data = pd.concat(data, axis=0)
+    data = merge_dfs(data, **kwargs_updf)
     if len(kwargs_sort) > 0:
         _, kwargs_sort = get_update_kwargs('inplace', True, kwargs_sort)
         data.sort_values(**kwargs_sort, inplace=True)
     if len(kwargs_drop_dup) > 0:
         _, kwargs_drop_dup = get_update_kwargs('inplace', True, kwargs_drop_dup)
         data.drop_duplicates(**kwargs_drop_dup, inplace=True)
     return data
 
 
 def load_csvs(fpaths,
               kwargs_sort={},
               kwargs_drop_dup={},
+              kwargs_updf={},
               **kwargs_loadcsv):
     '''
     读取指定路径列表中所有的csv文件，整合到一个df里面
 
     Parameters
     ----------
     fpaths : list
@@ -647,20 +653,22 @@
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
     return load_dfs_pd(fpaths,
                        kwargs_sort=kwargs_sort,
                        kwargs_drop_dup=kwargs_drop_dup,
+                       kwargs_updf=kwargs_updf,
                        **kwargs_loadcsv)
 
 
 def load_csvs_dir(fdir,
                   kwargs_sort={},
                   kwargs_drop_dup={},
+                  kwargs_updf={},
                   **kwargs_loadcsv):
     '''
     读取指定文件夹中所有的csv文件，整合到一个df里面
 
     Parameters
     ----------
     fdir : str
@@ -674,21 +682,22 @@
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
     files = os.listdir(fdir)
     files = [os.path.join(fdir, x) for x in files if x[-4:] == '.csv']
     data = load_csvs(files, kwargs_sort, kwargs_drop_dup,
-                     **kwargs_loadcsv)
+                     kwargs_updf, **kwargs_loadcsv)
     return data
 
 
 def load_excels(fdirorfpaths,
                 kwargs_sort={},
                 kwargs_drop_dup={},
+                kwargs_updf={},
                 **kwargs_readexcel):
     '''
     读取指定文件夹中所有的excel文件，整合到一个df里面
 
     Parameters
     ----------
     fdirorfpaths : str, list
@@ -708,14 +717,15 @@
         fpaths = os.listdir(fdirorfpaths)
         fpaths = [os.path.join(fdirorfpaths, x) for x in fpaths if x[-4:] == '.xls' or x[-5:] == '.xlsx']
     else:
         fpaths = fdirorfpaths
     return load_dfs_pd(fpaths,
                        kwargs_sort=kwargs_sort,
                        kwargs_drop_dup=kwargs_drop_dup,
+                       kwargs_updf=kwargs_updf,
                        **kwargs_readexcel)
 
 
 def archive_df(df_old, df_new, idcols=None,
                del_dup_cols=None, rep_keep='new',
                sort_cols=None, ascendings=True,
                old_ftype=None, new_ftype=None,
@@ -1584,73 +1594,88 @@
 
 
 def extract_7z():
     '''7z命令解压文件'''
     raise NotImplementedError
 
 
-def cmdrun(cmd_str, logger=None):
-    '''调用cmd执行cmd_str命令'''
+def cmdrun(cmd_str, logger=None, encoding=None):
+    '''
+    调用cmd执行cmd_str命令
+    
+    Examples
+    --------
+    cmdrun('python ./_test/_test_cmdrun.py')
+    '''
+    if isnull(encoding):
+        encoding = 'gbk' if _WINDOWS_SYSTEM else 'utf-8'
     p = subprocess.Popen(cmd_str,
                          shell=True,
                          stdout=subprocess.PIPE,
                          stderr=subprocess.STDOUT,
-                         encoding='gbk'
+                         encoding=encoding
                          )
     res = p.communicate()[0]
     logger_show(res, logger)
     return res
 
 
 def _cmdrun(args):
     return cmdrun(*args)
     
     
 def cmdruns_multi_process(cmd_str_list, logger=None,
-                          multi_line=None, keep_order=True):
-    args_list = [[cmd_str, logger] for cmd_str in cmd_str_list]
+                          multi_line=None, keep_order=True,
+                          encoding=None):
+    args_list = [[cmd_str, logger, encoding] for cmd_str in cmd_str_list]
     if not keep_order:
         res = multi_process_concurrent(cmdrun, args_list,
                                        multi_line=multi_line,
                                        keep_order=False)
     else:
         res = multi_process_concurrent(_cmdrun, args_list,
                                        multi_line=multi_line,
                                        keep_order=True)
     logger_show('\n'.join(res), logger)
     return res
     
     
 def cmd_run_pys_multi_process(py_list, logger=None,
-                              multi_line=None, keep_order=True):
+                              multi_line=None,
+                              keep_order=True,
+                              encoding=None):
     cmd_str_list = ['python %s'%py for py in py_list]
     return cmdruns_multi_process(cmd_str_list, logger=logger,
-                                 multi_line=multi_line, keep_order=keep_order)
+                                 multi_line=multi_line,
+                                 keep_order=keep_order,
+                                 encoding=encoding)
     
     
-def cmd_run_pys(py_list, logger=None):
+def cmd_run_pys(py_list, logger=None, encoding=None):
     '''cmd命令批量运行py脚本，logger捕捉日志'''
     if not isinstance(py_list, (list, tuple)):
         py_list = [py_list]
     for k in range(len(py_list)):
         py = py_list[k]
         logger_show('{}/{} running {} ...'.format(k+1, len(py_list), py),
                     logger)
         if not os.path.exists(py):
             logger_show('%s 不存在！'%py, None, level='warn')
             continue
-        # cmd_str = 'python {}'.format(file)
+        cmd_str = 'python {}'.format(py)
         # os.system(cmd_str)
         # subprocess.call(cmd_str)
-        p = subprocess.Popen(['python', py],
-                              shell=True,
-                              stdout=subprocess.PIPE,
-                              stderr=subprocess.STDOUT,
-                              encoding='gbk'
-                              )
+        if isnull(encoding):
+            encoding = 'gbk' if _WINDOWS_SYSTEM else 'utf-8'
+        p = subprocess.Popen(cmd_str, # ['python', py], # windows下可以这么写，linux下不行
+                             shell=True,
+                             stdout=subprocess.PIPE,
+                             stderr=subprocess.STDOUT,
+                             encoding=encoding
+                             )
         logger_show(p.communicate()[0], logger)
     # close_log_file(logger)
 
 
 def rename_files_in_dir(dir_path, func_rename):
     '''
     对指定文件夹中的文件进行批量重命名
@@ -1673,29 +1698,31 @@
 def find_files_include_str(target_str, fpaths, re_match=False,
                            return_all_find=False, logger=None):
     '''    
     在指定文件路径列表中，查找哪些文件里面包含了目标字符串
 
     Parameters
     ----------
-    target_str : str
-        目标字符串
+    target_str : str, Callable
+        目标字符串，若为函数则调用方式应为target_str(line)
     fpaths : str, list
         文件路径列表
     re_match : bool
         若为True，则目标字符串 ``target_str`` 按正则表达式处理
     return_all_find : bool
         若为True，则返回所有找到的目标字符串，否则只返回第一个
     logger : None, logging.Logger
         日志记录器
 
 
     :returns: `dict` - 返回dict, key为找到的文件路径，value为包含目标字符串的文本内容(仅第一次出现的位置)
     '''
     def _isin(line, tgt):
+        if isinstance(target_str, Callable):
+            return target_str(line)
         if not re_match:
             return tgt in line
         else:
             return not re.search(tgt, line) is None
     fpaths = check_list_arg(fpaths)
     files = []
     for fpath in fpaths:
```

### Comparing `dramkit-0.5.45/dramkit/logtools/logger_general.py` & `dramkit-0.5.46/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.46/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.46/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/logtools/utils_logger.py` & `dramkit-0.5.46/dramkit/logtools/utils_logger.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.46/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/openai/openai_chat.py` & `dramkit-0.5.46/dramkit/openai/openai_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 CON = True # 是否允许连续对话
 N_MAX_CON = 20 # 连续对话信息保留的最大轮数
 MAX_PROMPT_LEN = 1500
 
 
 def load_config():
     cfg = {}
-    cfg_dir = get_parent_path(os.path.dirname(__file__), 2)
-    fcfg = os.path.join(cfg_dir, 'config/openai.yml')
+    cfg_dir = get_parent_path(os.path.dirname(__file__), 1)
+    fcfg = os.path.join(cfg_dir, '_config/openai.yml')
     if os.path.exists(fcfg):
         cfg = load_yml(fcfg)
     if not 'secret_key' in cfg:
         cfg['secret_key'] = 'openaiapikeykey'
     if not 'secret_iv' in cfg:
         cfg['secret_iv'] = 'openaiapikeyiv'
     return cfg
```

### Comparing `dramkit-0.5.45/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.46/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/alo.py` & `dramkit-0.5.46/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.46/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/boa.py` & `dramkit-0.5.46/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/cs.py` & `dramkit-0.5.46/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/ga.py` & `dramkit-0.5.46/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/gwo.py` & `dramkit-0.5.46/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.46/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/hho.py` & `dramkit-0.5.46/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.46/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/pso.py` & `dramkit-0.5.46/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.46/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/optimizer/woa.py` & `dramkit-0.5.46/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/_Git_notes.py` & `dramkit-0.5.46/dramkit/other/_Git_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/_Linux_notes.py` & `dramkit-0.5.46/dramkit/other/_Linux_notes.py`

 * *Files 19% similar despite different names*

```diff
@@ -136,8 +136,44 @@
 npm -v
 
 npm install -g pnpm # npm安装pnpm
 
 # unzip解压覆盖
 unzip -o xxx.zip
 
+# 查看ip信息
+ifconfig
+
+# 查看所有系统变量（环境变量）
+env
+echo $变量名，如echo $PATH、echo $USER
+
+# https://blog.csdn.net/weixin_53610475/article/details/126818148
+# 查看gpu显卡信息
+lspci | grep -i nvidia
+
+# https://blog.csdn.net/u013250861/article/details/130547611
+# ubuntu server开启root用户登录
+# 1. 给root账户设置密码，在当前普通用户界面下输入命令，设置密码:
+sudo passwd root
+# 2. 修改sshd配置
+sudo vim /etc/ssh/sshd_config
+找到#PermitRootLogin prohibit-password，默认是注释掉的。直接在下面添加一行：
+PermitRootLogin yes，保存并退出。
+# 3. 重启sshd服务
+sudo systemctl restart sshd
+
+# ubuntu修改时区
+# 查看时区
+timedatectl
+# 查看可用时区
+timedatectl list-timezones
+# 修改时区
+sudo timedatectl set-timezone Asia/Shanghai
+
+# TODO: 用户授权
+# 文件夹对所有用户授权
+chmod -R a+rwx dir_path
+# 改变文件夹所有者
+chown ‐R root ./abc # 改变abc这个目录及其下面所有的文件和目录的所有者是root
+
 # '''
```

### Comparing `dramkit-0.5.45/dramkit/other/_Python_notes.py` & `dramkit-0.5.46/dramkit/other/_Python_notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # Python笔记
 
 # 参考：
 # pip命令：https://blog.csdn.net/fancunshuai/article/details/124994040
 
 py_notes = \
 r'''
+# spyder启动失败查找原因
+在cmd中运行spyder，会看到报错信息
+
 # conda查看镜像
 conda config --show-sources
 
 # conda设置镜像
 # 首先用命令创建配置文件（或手动创建）.condarc：
 conda config --set show_channel_urls yes # 设置搜索时显示通道地址
 # 在.condarc中添加常用镜像源：
@@ -78,17 +81,33 @@
 
 # conda虚拟环境安装spyder
 conda install spyder
 
 # conda虚拟环境安装notebook
 conda install nb_conda
 
+# conda删除缓存
+conda clean --all
+
+# pip删除缓存
+pip cache purge
+
 # pip安装忽略依赖
 --no-dependencies
  
 # pip强制重新安装所有软件包，即使它们已经是最新的
 --force-reinstall
 
 # pip批量安装文件夹下所有的whl包
 pip install /dirpath/*.whl
 
+# jupyter notebook cell转为markdown快捷键：Esc(命令模式)+m
+
+# linux下安装talib
+tar -xzf ta-lib-0.4.0-src.tar.gz
+cd ta-lib/
+./configure --prefix=/usr
+make
+sudo make install
+pip install TA-Lib
+
 # '''
```

### Comparing `dramkit-0.5.45/dramkit/other/_Vim_notes.py` & `dramkit-0.5.46/dramkit/other/_Vim_notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,49 @@
 " 折叠配置
 set foldenable 
 set foldmethod=manual
 set foldcolumn=1
 " 查看折叠是否设置成功
 :set foldmethod?
 " 常用折叠快捷键
-zf "将选中位置创建折叠区域
-za "反复展开或折叠当前区域
-zR "展开所有折叠区
-zM "合上所有折叠区
+zf " 将选中位置创建折叠区域
+za " 反复展开或折叠当前区域
+zR " 展开所有折叠区
+zM " 合上所有折叠区
+ggdG " 清除全部内容
+ggvG " 全选
+
+# linux查看vim是否支持外部复制粘贴（clipboard前应有加号+）
+vim --version | grep clipboard
+# 若clipboard前无加号+，安装vim-gtk
+sudo apt install vim-gtk
+
+" 全选复制到剪切板
+ggVG+y
+ggvG+y
+" 从前切板粘贴（注意"也是命令的一部分）
+"+p
 # '''
 
 # 默认配置文件.vimrc
 
 # 配置模板1
 r'''
 " 显示行号
 set number
 " 当前行高亮（下划线突出显示当前行）
 set cursorline 
+
+" 解决中文乱码
+set fileencodings=utf-8,ucs-bom,gb18030,gbk,gb2312,cp936
+set termencoding=utf-8
+set encoding=utf-8
+
+" 搜索高亮
+set hlsearch
 '''
 
 # 配置模板2
 # https://blog.csdn.net/tata_2016/article/details/119715508
 r'''
 filetype on
```

### Comparing `dramkit-0.5.45/dramkit/other/debt_cal.py` & `dramkit-0.5.46/dramkit/other/debt_cal.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/langconv.py` & `dramkit-0.5.46/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/othertools.py` & `dramkit-0.5.46/dramkit/other/othertools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/replace_endblank.py` & `dramkit-0.5.46/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/other/zh_wiki.py` & `dramkit-0.5.46/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/plot_barline.py` & `dramkit-0.5.46/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/plot_common.py` & `dramkit-0.5.46/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.46/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.46/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/twinx_align.py` & `dramkit-0.5.46/dramkit/plottools/twinx_align.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/plottools/utils_plot.py` & `dramkit-0.5.46/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.46/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.46/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.46/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sorts/insert_sort.py` & `dramkit-0.5.46/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.46/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sorts/quick_sort.py` & `dramkit-0.5.46/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/speedup/_mp_test1.py` & `dramkit-0.5.46/dramkit/speedup/_mp_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/speedup/_mp_test2.py` & `dramkit-0.5.46/dramkit/speedup/_mp_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/speedup/_mp_test3.py` & `dramkit-0.5.46/dramkit/speedup/_mp_test3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/speedup/iotools_tmp.py` & `dramkit-0.5.46/dramkit/speedup/_tmp_iotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/speedup/multi_process_concurrent.py` & `dramkit-0.5.46/dramkit/speedup/multi_process_concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,45 +70,45 @@
     '''注：若此目标函数定义在__name__ == '__main__'之后，则在windows下会报错'''
     print('task id:', idx)
     time.sleep(sleep_tm)
     print('task id: {}; slept: {}s.'.format(idx, sleep_tm))
     return [idx, sleep_tm]
 
 
-def _func_test_win_new(args):
+def _func_test_win_mp(args):
     return _func_test_win(*args)
 
 #%%
 if __name__ == '__main__':
     from dramkit import TimeRecoder
 
     def func(idx, sleep_tm):
         '''注：若此目标函数定义在__name__ == '__main__'之后，则在windows下会报错'''
         print('task id:', idx)
         time.sleep(sleep_tm)
         print('task id: {}; slept: {}s.'.format(idx, sleep_tm))
         return [idx, sleep_tm]
 
-    def func_new(args):
+    def func_mp(args):
         return func(*args)
 
     args_list = [[1, 2], [3, 4], [4, 5], [2, 3]]
     # args_list = [[1, 20], [3, 40], [4, 50], [2, 30]]
 
 
     '''
     tmprint('multi-process, concurrent...................')
     tr = TimeRecoder()
     if _WINDOWS_SYSTEM:
-        results_Order = multi_process_concurrent(_func_test_win_new, args_list,
+        results_Order = multi_process_concurrent(_func_test_win_mp, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(_func_test_win, args_list,
                                                    keep_order=False)
-        results_Order2 = multi_process_concurrent(_func_test_win_new, args_list,
+        results_Order2 = multi_process_concurrent(_func_test_win_mp, args_list,
                                                   keep_order=True, multi_line=2)
     else:
-        results_Order = multi_process_concurrent(func_new, args_list,
+        results_Order = multi_process_concurrent(func_mp, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(func, args_list,
                                                    keep_order=False)
     tr.used()
     # '''
```

### Comparing `dramkit-0.5.45/dramkit/speedup/multi_thread.py` & `dramkit-0.5.46/dramkit/speedup/multi_thread.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.46/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.46/dramkit/sqltools/_MySQL_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.46/dramkit/sqltools/_Oracle_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.46/dramkit/sqltools/cxoracle.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/py_hive.py` & `dramkit-0.5.46/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.46/dramkit/sqltools/py_mysql.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.46/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit/webtools/utils_html.py` & `dramkit-0.5.46/dramkit/webtools/utils_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,13 +126,13 @@
     open_html(path_html, '360chrome')
 
     bsobj = html_to_soup(path_html, encoding='utf-8')
     path_html_ = './_test/gauge_text_rewright.html'
     soup_to_html(bsobj, path_html_, encoding='utf-8')
     open_html(path_html_, '360chrome')
     insert_src_head_end(path_html_,
-                        '../../../assets/Echarts/echart_js/echarts.js',
+                        '../../_assets/Echarts/echart_js/echarts.js',
                         encoding='utf-8')
     insert_src_head_end(path_html_,
-                        '../../../assets/Echarts/echart_js/echarts.js',
+                        '../../_assets/Echarts/echart_js/echarts.js',
                         encoding='utf-8')
     del_js_head_end(path_html_, encoding='utf-8')
```

### Comparing `dramkit-0.5.45/dramkit/wechat/qywechat.py` & `dramkit-0.5.46/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.45/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.46/dramkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.45
+Version: 0.5.46
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.45/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.46/dramkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 dramkit/_tmp/CRR.py
 dramkit/_tmp/CtrlPreTS.py
 dramkit/_tmp/NPairSum.py
 dramkit/_tmp/PIDtest.py
 dramkit/_tmp/PIDtest2.py
 dramkit/_tmp/VMD.py
 dramkit/_tmp/__init__.py
+dramkit/_tmp/_dijkstra.py
 dramkit/_tmp/cca_test.py
 dramkit/_tmp/dtw_test.py
 dramkit/_tmp/explore.py
 dramkit/_tmp/feature_selection.py
 dramkit/_tmp/gini.py
+dramkit/_tmp/important_sample.py
 dramkit/_tmp/merge_sort.py
 dramkit/_tmp/mouse_move.py
 dramkit/_tmp/mpc_test1.py
 dramkit/_tmp/options_Implied_volatility.py
 dramkit/_tmp/pf_test.py
 dramkit/_tmp/plot_test.py
 dramkit/_tmp/plot_test2.py
 dramkit/_tmp/simple_smooth.py
-dramkit/_tmp/step_reg.py
+dramkit/_tmp/test_Wrapper.py
 dramkit/_tmp/test_async_washs.py
 dramkit/_tmp/test_await_timeout.py
 dramkit/_tmp/test_backtrader.py
 dramkit/_tmp/test_chatgpt_v1.py
 dramkit/_tmp/test_code.py
 dramkit/_tmp/test_find_peaks.py
 dramkit/_tmp/test_get_var_name.py
@@ -67,31 +69,28 @@
 dramkit/chncal/constants_fate.py
 dramkit/chncal/constants_hko.py
 dramkit/chncal/constants_trade_dates.py
 dramkit/chncal/constants_wuxing.py
 dramkit/chncal/constants_zodiac_marry.py
 dramkit/chncal/solar_terms.py
 dramkit/datsci/__init__.py
-dramkit/datsci/_rl_mab.py
-dramkit/datsci/_rl_markov.py
-dramkit/datsci/_rl_mcdp.py
 dramkit/datsci/_utils_ann.py
 dramkit/datsci/activate_funcs.py
 dramkit/datsci/ahp.py
 dramkit/datsci/ahp_sim_ri.py
 dramkit/datsci/apriori.py
 dramkit/datsci/curvature.py
 dramkit/datsci/elm_cls.py
 dramkit/datsci/elm_reg.py
 dramkit/datsci/entropy_weight.py
 dramkit/datsci/find_maxmin.py
 dramkit/datsci/freq_item_set.py
+dramkit/datsci/level_score.py
 dramkit/datsci/lr.py
 dramkit/datsci/preprocess.py
-dramkit/datsci/rl_markov_new.py
 dramkit/datsci/stats.py
 dramkit/datsci/stepreg.py
 dramkit/datsci/time_series.py
 dramkit/datsci/topsis.py
 dramkit/datsci/utils_lgb.py
 dramkit/datsci/utils_ml.py
 dramkit/datsci/zigzag.py
@@ -131,33 +130,50 @@
 dramkit/other/__init__.py
 dramkit/other/debt_cal.py
 dramkit/other/langconv.py
 dramkit/other/othertools.py
 dramkit/other/replace_endblank.py
 dramkit/other/zh_wiki.py
 dramkit/plottools/__init__.py
+dramkit/plottools/_plot_bar.py
+dramkit/plottools/_plot_heatmap.py
 dramkit/plottools/plot_barline.py
 dramkit/plottools/plot_common.py
 dramkit/plottools/plot_histdist.py
 dramkit/plottools/plot_scatter.py
 dramkit/plottools/twinx_align.py
 dramkit/plottools/utils_plot.py
 dramkit/pystyles/__init__.py
 dramkit/pystyles/dramkit_style.py
+dramkit/rl/__init__.py
+dramkit/rl/_approx.py
+dramkit/rl/_mab.py
+dramkit/rl/_markov.py
+dramkit/rl/_markov_new.py
+dramkit/rl/_mc.py
+dramkit/rl/_notes.py
+dramkit/rl/_td.py
+dramkit/rl/_td_dict.py
+dramkit/rl/_tmpMountainCar-v0_tf.py
+dramkit/rl/_tmprl_utils.py
+dramkit/rl/_tmp第7章-DQN算法.py
+dramkit/rl/env_hungrygame.py
+dramkit/rl/gym_best_pi.py
+dramkit/rl/utils_gym.py
 dramkit/sorts/__init__.py
 dramkit/sorts/bubble_sort.py
 dramkit/sorts/bucket_sort.py
 dramkit/sorts/insert_sort.py
 dramkit/sorts/insert_sort_bin.py
 dramkit/sorts/quick_sort.py
 dramkit/speedup/__init__.py
 dramkit/speedup/_mp_test1.py
 dramkit/speedup/_mp_test2.py
 dramkit/speedup/_mp_test3.py
-dramkit/speedup/iotools_tmp.py
+dramkit/speedup/_tmp_iotools.py
 dramkit/speedup/job_lib.py
 dramkit/speedup/multi_process_concurrent.py
 dramkit/speedup/multi_thread.py
 dramkit/sqltools/_Hive_notes.py
 dramkit/sqltools/_MySQL_notes.py
 dramkit/sqltools/_Oracle_notes.py
 dramkit/sqltools/__init__.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dramkit-0.5.45/setup.py` & `dramkit-0.5.46/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,28 +34,29 @@
       platforms='any',
       setup_requires=[],
       install_requires=['pycryptodome',
                         'cryptography',
                         'tqdm',
                         'pymysql',
                         'sqlalchemy',
-                        'openai',
+                        # 'openai',
                         'beartype'],
       packages=['dramkit',
                 'dramkit.backpacks',
                 'dramkit.chncal',
                 'dramkit.datsci',
                 'dramkit.find_addends',                
                 'dramkit.logtools',
                 'dramkit.openai',
                 'dramkit.optimizer',
                 'dramkit.other',
                 'dramkit.plottools',
-                'dramkit.pystyles',                
+                'dramkit.pystyles', 
+                'dramkit.rl',
                 'dramkit.sorts',
                 'dramkit.speedup',
-				'dramkit.sqltools',
+                'dramkit.sqltools',
                 'dramkit.webtools',
                 'dramkit.wechat',
                 'dramkit._tmp'
                 ]
       )
```

