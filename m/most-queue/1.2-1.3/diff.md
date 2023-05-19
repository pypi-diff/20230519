# Comparing `tmp/most_queue-1.2.tar.gz` & `tmp/most_queue-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_queue-1.2.tar", last modified: Wed May 17 17:27:29 2023, max compression
+gzip compressed data, was "most_queue-1.3.tar", last modified: Wed May 17 17:44:11 2023, max compression
```

## Comparing `most_queue-1.2.tar` & `most_queue-1.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.311880 most_queue-1.2/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.2/LICENSE
--rw-rw-rw-   0        0        0     6336 2023-05-17 17:27:29.311880 most_queue-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.101980 most_queue-1.2/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.130440 most_queue-1.2/most_queue/sim/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0    14589 2023-05-17 17:16:20.000000 most_queue-1.2/most_queue/sim/fj_delta_im.py
--rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most_queue-1.2/most_queue/sim/fj_im.py
--rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most_queue-1.2/most_queue/sim/flow_sum_im.py
--rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most_queue-1.2/most_queue/sim/network_im_prty.py
--rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most_queue-1.2/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most_queue-1.2/most_queue/sim/rand_destribution.py
--rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most_queue-1.2/most_queue/sim/smo_batch_sim.py
--rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most_queue-1.2/most_queue/sim/smo_im.py
--rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most_queue-1.2/most_queue/sim/smo_im_prty.py
--rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most_queue-1.2/most_queue/sim/smo_impatient_im.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.193428 most_queue-1.2/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.2/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most_queue-1.2/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.2/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.2/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.2/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.2/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.2/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.2/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.2/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.2/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.2/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/passage_time.py
--rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.2/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.2/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.2/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.297156 most_queue-1.2/most_queue/theory/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.2/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most_queue-1.2/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4719 2023-05-17 17:21:01.000000 most_queue-1.2/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19414 2022-09-16 07:43:39.000000 most_queue-1.2/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10650 2022-09-15 16:54:06.000000 most_queue-1.2/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.2/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     5943 2022-09-15 16:55:04.000000 most_queue-1.2/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most_queue-1.2/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.2/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most_queue-1.2/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    22232 2023-05-17 14:00:37.000000 most_queue-1.2/most_queue/theory/m_h2_h2warm.py
--rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most_queue-1.2/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most_queue-1.2/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most_queue-1.2/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    23133 2023-05-16 19:00:21.000000 most_queue-1.2/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most_queue-1.2/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most_queue-1.2/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most_queue-1.2/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most_queue-1.2/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.2/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most_queue-1.2/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most_queue-1.2/most_queue/theory/prty_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.2/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/sv_sum_calc.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.2/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.299414 most_queue-1.2/most_queue/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.2/most_queue/utils/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.2/most_queue/utils/approx_cdf_make.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.300880 most_queue-1.2/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.2/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.310819 most_queue-1.2/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.2/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.2/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.2/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.105404 most_queue-1.2/most_queue.egg-info/
--rw-rw-rw-   0        0        0     6336 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2475 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.2/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      105 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-05-17 17:21:55.000000 most_queue-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 17:27:29.311880 most_queue-1.2/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-05-17 17:25:23.000000 most_queue-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.336186 most_queue-1.3/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.3/LICENSE
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:44:11.335121 most_queue-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.286991 most_queue-1.3/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.297810 most_queue-1.3/most_queue/sim/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0    14589 2023-05-17 17:16:20.000000 most_queue-1.3/most_queue/sim/fj_delta_im.py
+-rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most_queue-1.3/most_queue/sim/fj_im.py
+-rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most_queue-1.3/most_queue/sim/flow_sum_im.py
+-rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most_queue-1.3/most_queue/sim/network_im_prty.py
+-rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most_queue-1.3/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most_queue-1.3/most_queue/sim/rand_destribution.py
+-rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most_queue-1.3/most_queue/sim/smo_batch_sim.py
+-rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most_queue-1.3/most_queue/sim/smo_im.py
+-rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most_queue-1.3/most_queue/sim/smo_im_prty.py
+-rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most_queue-1.3/most_queue/sim/smo_impatient_im.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.310410 most_queue-1.3/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.3/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most_queue-1.3/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.3/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.3/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.3/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.3/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.3/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.3/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.3/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.3/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.3/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/passage_time.py
+-rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.3/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.3/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.3/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.329668 most_queue-1.3/most_queue/theory/
+-rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.3/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.3/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most_queue-1.3/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4688 2023-05-17 17:43:06.000000 most_queue-1.3/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19284 2023-05-17 17:43:30.000000 most_queue-1.3/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10650 2023-05-17 17:35:09.000000 most_queue-1.3/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.3/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     5877 2023-05-17 17:40:32.000000 most_queue-1.3/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most_queue-1.3/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.3/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most_queue-1.3/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    22232 2023-05-17 14:00:37.000000 most_queue-1.3/most_queue/theory/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most_queue-1.3/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most_queue-1.3/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most_queue-1.3/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    23133 2023-05-16 19:00:21.000000 most_queue-1.3/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most_queue-1.3/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most_queue-1.3/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most_queue-1.3/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most_queue-1.3/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.3/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most_queue-1.3/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most_queue-1.3/most_queue/theory/prty_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.3/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/sv_sum_calc.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.3/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.330442 most_queue-1.3/most_queue/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.3/most_queue/utils/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.3/most_queue/utils/approx_cdf_make.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.331482 most_queue-1.3/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.3/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.333901 most_queue-1.3/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.3/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.3/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.3/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.291816 most_queue-1.3/most_queue.egg-info/
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2475 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.3/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-05-17 17:43:52.000000 most_queue-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:44:11.336866 most_queue-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-05-17 17:43:57.000000 most_queue-1.3/setup.py
```

### Comparing `most_queue-1.2/LICENSE` & `most_queue-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/PKG-INFO` & `most_queue-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most_queue
-Version: 1.2
+Version: 1.3
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.2/README.md` & `most_queue-1.3/README.md`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/fj_delta_im.py` & `most_queue-1.3/most_queue/sim/fj_delta_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/fj_im.py` & `most_queue-1.3/most_queue/sim/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/flow_sum_im.py` & `most_queue-1.3/most_queue/sim/flow_sum_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/network_im_prty.py` & `most_queue-1.3/most_queue/sim/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/queue_finite_source_sim.py` & `most_queue-1.3/most_queue/sim/queue_finite_source_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/rand_destribution.py` & `most_queue-1.3/most_queue/sim/rand_destribution.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/smo_batch_sim.py` & `most_queue-1.3/most_queue/sim/smo_batch_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/smo_im.py` & `most_queue-1.3/most_queue/sim/smo_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/smo_im_prty.py` & `most_queue-1.3/most_queue/sim/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/sim/smo_impatient_im.py` & `most_queue-1.3/most_queue/sim/smo_impatient_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/ek_d_n.py` & `most_queue-1.3/most_queue/tests/ek_d_n.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/fj_calc.py` & `most_queue-1.3/most_queue/tests/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/fj_im.py` & `most_queue-1.3/most_queue/tests/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/flow_sum.py` & `most_queue-1.3/most_queue/tests/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/gi_m_1_calc.py` & `most_queue-1.3/most_queue/tests/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/gi_m_n_calc.py` & `most_queue-1.3/most_queue/tests/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/m_d_n_calc.py` & `most_queue-1.3/most_queue/tests/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/m_ph_n_prty.py` & `most_queue-1.3/most_queue/tests/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/mg1_calc.py` & `most_queue-1.3/most_queue/tests/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/mg1_warm_calc.py` & `most_queue-1.3/most_queue/tests/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/mgn_tt.py` & `most_queue-1.3/most_queue/tests/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/mmn3_pnz_cox_approx.py` & `most_queue-1.3/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/mmn_prty_pnz_approx.py` & `most_queue-1.3/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/network_im_prty.py` & `most_queue-1.3/most_queue/tests/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/passage_time.py` & `most_queue-1.3/most_queue/tests/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/smo_im.py` & `most_queue-1.3/most_queue/tests/smo_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/smo_im_prty.py` & `most_queue-1.3/most_queue/tests/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/tests/weibull.py` & `most_queue-1.3/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/batch_mm1.py` & `most_queue-1.3/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/diff5dots.py` & `most_queue-1.3/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/ek_d_n_calc.py` & `most_queue-1.3/most_queue/theory/ek_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/engset_model.py` & `most_queue-1.3/most_queue/theory/engset_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-import math
 from diff5dots import diff5dots
 import sv_sum_calc
 
 
 class Engset:
     """
     Расчет СМО М\М\1 с конечным числом источников m
```

### Comparing `most_queue-1.2/most_queue/theory/fj_calc.py` & `most_queue-1.3/most_queue/theory/fj_calc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import mmnr_calc
+import mgn_tt
+import mg1_calc
+import sv_sum_calc
+
+import matplotlib.pyplot as plt
 import most_queue.sim.rand_destribution as rd
-from most_queue.theory import sv_sum_calc
-from most_queue.theory import mmnr_calc
 import math
-from most_queue.theory import mgn_tt
 import time
-from most_queue.sim.fj_im import SmoFJ
-from most_queue.theory import mg1_calc
-import matplotlib.pyplot as plt
 
 
 def get_lambda(min, max):
     l = np.random.randn()
     while l < min or l > max: \
             l = np.random.randn()
     return l
```

### Comparing `most_queue-1.2/most_queue/theory/flow_sum.py` & `most_queue-1.3/most_queue/theory/flow_sum.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import most_queue.sim.rand_destribution as rd
-import math
 from most_queue.sim import flow_sum_im
+
 import copy
 import matplotlib.pyplot as plt
-
+import most_queue.sim.rand_destribution as rd
+import math
 
 class SummatorNumeric:
 
     def __init__(self, a, verbose=False, is_semi=False):
         self.n = len(a)
         self.a = a
         self.num_of_moments = len(a[0])
```

### Comparing `most_queue-1.2/most_queue/theory/generate_pareto_noise.py` & `most_queue-1.3/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/gi_m_1_calc.py` & `most_queue-1.3/most_queue/theory/gi_m_1_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import numpy as np
 import math
 from most_queue.sim import rand_destribution as rd
-from most_queue.theory import q_poisson_arrival_calc
-from most_queue.theory import sv_sum_calc
+import q_poisson_arrival_calc
+import sv_sum_calc
 
 
 def get_pi(a, mu, num=100, e=1e-10, approx_distr="Gamma"):
     """
     Вычисление вероятностей состояний СМО
     a - список начальных моментов распределения интервало рекуррентного вх потока заявок
     mu - интенсивность обслуживания
```

### Comparing `most_queue-1.2/most_queue/theory/gi_m_n_calc.py` & `most_queue-1.3/most_queue/theory/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/impatience_calc.py` & `most_queue-1.3/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/m_d_n_calc.py` & `most_queue-1.3/most_queue/theory/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/m_h2_h2warm.py` & `most_queue-1.3/most_queue/theory/m_h2_h2warm.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/m_ph_n_prty.py` & `most_queue-1.3/most_queue/theory/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mg1_calc.py` & `most_queue-1.3/most_queue/theory/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mg1_warm_calc.py` & `most_queue-1.3/most_queue/theory/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mgn_tt.py` & `most_queue-1.3/most_queue/theory/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mmn3_pnz_cox_approx.py` & `most_queue-1.3/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mmn_prty_pnz_approx.py` & `most_queue-1.3/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/mmnr_calc.py` & `most_queue-1.3/most_queue/theory/mmnr_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/network_calc.py` & `most_queue-1.3/most_queue/theory/network_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/network_viewer.py` & `most_queue-1.3/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/passage_time.py` & `most_queue-1.3/most_queue/theory/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/prty_calc.py` & `most_queue-1.3/most_queue/theory/prty_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/q_poisson_arrival_calc.py` & `most_queue-1.3/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/student_stat.py` & `most_queue-1.3/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/sv_sum_calc.py` & `most_queue-1.3/most_queue/theory/sv_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/theory/weibull.py` & `most_queue-1.3/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/utils/approx_cdf_make.py` & `most_queue-1.3/most_queue/utils/approx_cdf_make.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/visualisation/smo_im_vis.py` & `most_queue-1.3/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/visualisation/utils/result_table.py` & `most_queue-1.3/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/visualisation/utils/settings_window.py` & `most_queue-1.3/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue/visualisation/utils/splash_screen.py` & `most_queue-1.3/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/most_queue.egg-info/PKG-INFO` & `most_queue-1.3/most_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most-queue
-Version: 1.2
+Version: 1.3
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.2/most_queue.egg-info/SOURCES.txt` & `most_queue-1.3/most_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `most_queue-1.2/setup.py` & `most_queue-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.02',
+      version='1.03',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

