# Comparing `tmp/nemreader-0.8.4.tar.gz` & `tmp/nemreader-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemreader-0.8.4.tar", last modified: Sun Apr 23 00:34:35 2023, max compression
+gzip compressed data, was "nemreader-0.8.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nemreader-0.8.4.tar` & `nemreader-0.8.6.tar`

### file list

```diff
@@ -1,224 +1,225 @@
--rwxr-xr-x   0        0        0      135 2022-11-03 05:28:29.076363 nemreader-0.8.4/.flake8
--rwxr-xr-x   0        0        0     1220 2023-02-14 09:16:32.284457 nemreader-0.8.4/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0     1185 2023-02-14 09:12:50.910658 nemreader-0.8.4/.gitignore
--rw-r--r--   0        0        0     1074 2022-10-22 23:26:41.875203 nemreader-0.8.4/LICENSE
--rw-r--r--   0        0        0       26 2022-10-22 23:26:41.875203 nemreader-0.8.4/MANIFEST.in
--rw-r--r--   0        0        0     1004 2023-02-14 09:16:46.737509 nemreader-0.8.4/README.md
--rw-r--r--   0        0        0   101291 2022-10-22 23:26:41.875203 nemreader-0.8.4/docs/_static/img/nmi-suffixes.jpg
--rw-r--r--   0        0        0    38420 2022-10-22 23:26:41.879203 nemreader-0.8.4/docs/_static/img/nmi-suffixes2.png
--rw-r--r--   0        0        0    10717 2022-10-22 23:26:41.879203 nemreader-0.8.4/docs/_static/img/plot_cal.png
--rw-r--r--   0        0        0    14205 2022-10-22 23:26:41.879203 nemreader-0.8.4/docs/_static/img/plot_profile.png
--rwxr-xr-x   0        0        0     5363 2022-10-22 23:37:45.243073 nemreader-0.8.4/docs/file-format.md
--rwxr-xr-x   0        0        0      658 2023-04-18 15:51:04.038645 nemreader-0.8.4/docs/gen_ref_pages.py
--rwxr-xr-x   0        0        0      469 2022-10-19 19:12:36.373067 nemreader-0.8.4/docs/index.md
--rwxr-xr-x   0        0        0      164 2022-11-03 10:18:21.085359 nemreader-0.8.4/docs/installation.md
--rwxr-xr-x   0        0        0     5141 2023-02-14 09:12:50.918658 nemreader-0.8.4/docs/quickstart.md
--rw-r--r--   0        0        0       60 2022-10-22 23:53:10.163094 nemreader-0.8.4/docs/requirements.txt
--rw-r--r--   0        0        0    29436 2023-02-14 09:12:50.918658 nemreader-0.8.4/examples/Example_NEM12_ManyNMIs.zip
--rw-r--r--   0        0        0      708 2023-04-19 04:17:11.605921 nemreader-0.8.4/examples/Example_different_intervals.zip
--rw-r--r--   0        0        0      288 2023-04-04 20:03:11.422958 nemreader-0.8.4/examples/invalid/Example_NEM12_15min_200_30min_300.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.4/examples/invalid/Example_NEM12_15min_200_30min_400.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.4/examples/invalid/Example_NEM12_30min_200_15min_300.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.4/examples/invalid/Example_NEM12_30min_200_15min_400.csv
--rw-r--r--   0        0        0       37 2023-04-21 21:45:40.913328 nemreader-0.8.4/examples/invalid/Example_NEM12_empty.csv
--rw-r--r--   0        0        0     1147 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/invalid/Example_NEM12_incomplete_interval.csv
--rw-r--r--   0        0        0      759 2022-10-28 17:58:36.467564 nemreader-0.8.4/examples/invalid/Example_NEM12_missing_header.csv
--rw-r--r--   0        0        0     1505 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/invalid/Example_NEM12_powercor.csv
--rw-r--r--   0        0        0      316 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/invalid/Example_NEM12_powercor.csv.zip
--rw-r--r--   0        0        0     1409 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/invalid/Example_NEM12_powercor_missing_fields.csv
--rw-r--r--   0        0        0        0 2022-10-22 23:48:37.878241 nemreader-0.8.4/examples/invalid/Example_empty_file.csv
--rw-r--r--   0        0        0     1424 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     2190 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1016 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      534 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      861 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      836 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      769 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      513 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1325 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      525 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1614 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1272 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1066 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      702 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      893 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      867 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      688 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      650 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      330 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      432 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      358 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      355 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      346 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      349 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      497 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      391 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      331 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      477 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      882 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      751 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1101 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0     1508 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      956 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1635 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      892 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1652 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      552 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      725 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      934 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      862 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      949 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      788 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      901 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      380 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      632 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      796 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      759 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      761 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      361 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      364 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      332 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      336 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1368 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1371 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1315 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1320 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      583 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      586 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      384 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      387 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      705 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      700 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1125 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      500 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      490 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      320 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      388 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      304 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      324 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      307 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      329 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      351 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      305 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      898 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1170 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      951 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     2136 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      883 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1972 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      550 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      553 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1017 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      851 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1488 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      771 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1450 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      352 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      961 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      717 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      693 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1070 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      294 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      366 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      343 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      299 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      400 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      337 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      345 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      334 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      276 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      293 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.879203 nemreader-0.8.4/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      274 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      279 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      313 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      307 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      320 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      323 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      334 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      327 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      330 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      310 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      288 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      276 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      309 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      340 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      294 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_actual_interval.csv
--rw-r--r--   0        0        0     1373 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_different_interval_length.csv
--rw-r--r--   0        0        0     4497 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_multiple_meters.csv
--rw-r--r--   0        0        0      521 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_multiple_quality.csv
--rw-r--r--   0        0        0      337 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_no_scheduled_read.csv
--rw-r--r--   0        0        0      887 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_substituted_interval.csv
--rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM12_upper_case_units.csv
--rw-r--r--   0        0        0      185 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM13_consumption_data.csv
--rw-r--r--   0        0        0      345 2022-10-22 23:26:41.883204 nemreader-0.8.4/examples/unzipped/Example_NEM13_forward_estimate.csv
--rwxr-xr-x   0        0        0      594 2022-10-22 23:45:00.094390 nemreader-0.8.4/mkdocs.yml
--rw-r--r--   0        0        0      764 2023-04-18 16:37:46.193786 nemreader-0.8.4/nemreader/__init__.py
--rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883204 nemreader-0.8.4/nemreader/__main__.py
--rw-r--r--   0        0        0     3754 2023-04-18 16:29:44.284846 nemreader-0.8.4/nemreader/cli.py
--rw-r--r--   0        0        0     3515 2023-04-18 15:51:04.094646 nemreader-0.8.4/nemreader/nem_objects.py
--rw-r--r--   0        0        0    23144 2023-04-21 05:32:50.457619 nemreader-0.8.4/nemreader/nem_reader.py
--rw-r--r--   0        0        0     6000 2023-04-19 10:31:41.476738 nemreader-0.8.4/nemreader/output_db.py
--rw-r--r--   0        0        0     5139 2023-04-18 16:01:53.042738 nemreader-0.8.4/nemreader/outputs.py
--rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.4/nemreader/py.typed
--rw-r--r--   0        0        0     5595 2023-04-18 15:51:04.154647 nemreader-0.8.4/nemreader/split_days.py
--rw-r--r--   0        0        0       22 2023-04-21 05:47:39.678431 nemreader-0.8.4/nemreader/version.py
--rwxr-xr-x   0        0        0     1381 2023-04-18 16:02:12.775158 nemreader-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     1956 2023-02-14 09:12:50.914658 nemreader-0.8.4/requirements.txt
--rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.4/tests/__init__.py
--rw-r--r--   0        0        0     1157 2022-10-25 19:12:53.653131 nemreader-0.8.4/tests/test_actual_interval.py
--rw-r--r--   0        0        0     1572 2023-04-18 16:14:25.860240 nemreader-0.8.4/tests/test_cli.py
--rw-r--r--   0        0        0      469 2023-04-18 15:51:04.058645 nemreader-0.8.4/tests/test_consumption_data.py
--rw-r--r--   0        0        0      850 2023-04-19 04:30:06.541878 nemreader-0.8.4/tests/test_dataframe_pivot.py
--rw-r--r--   0        0        0      814 2023-04-18 15:51:04.062646 nemreader-0.8.4/tests/test_day_split.py
--rw-r--r--   0        0        0     2099 2023-04-19 04:41:11.878462 nemreader-0.8.4/tests/test_file_outputs.py
--rw-r--r--   0        0        0      359 2022-10-28 17:58:36.471564 nemreader-0.8.4/tests/test_header_datestamp.py
--rw-r--r--   0        0        0     2043 2023-04-21 05:28:47.036795 nemreader-0.8.4/tests/test_incomplete_files.py
--rw-r--r--   0        0        0      995 2023-04-18 15:51:04.086646 nemreader-0.8.4/tests/test_invalid_interval_mixing.py
--rw-r--r--   0        0        0      284 2022-11-30 03:41:57.431559 nemreader-0.8.4/tests/test_legacy.py
--rw-r--r--   0        0        0      252 2023-02-14 09:12:50.918658 nemreader-0.8.4/tests/test_many_nmis.py
--rw-r--r--   0        0        0     1034 2022-10-25 19:12:58.393208 nemreader-0.8.4/tests/test_multiple_quality.py
--rw-r--r--   0        0        0     1488 2022-10-25 19:10:30.098582 nemreader-0.8.4/tests/test_open_examples.py
--rw-r--r--   0        0        0      268 2022-10-25 19:10:50.070968 nemreader-0.8.4/tests/test_optional_columns.py
--rw-r--r--   0        0        0      589 2023-04-19 10:29:02.694420 nemreader-0.8.4/tests/test_output_db.py
--rw-r--r--   0        0        0     1307 2023-04-18 15:51:04.102646 nemreader-0.8.4/tests/test_unit_capitalisation.py
--rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 nemreader-0.8.4/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2023-05-19 19:11:38.923611 nemreader-0.8.6/.flake8
+-rw-r--r--   0        0        0      985 2023-05-19 19:11:38.923611 nemreader-0.8.6/.github/workflows/publish.yml
+-rwxr-xr-x   0        0        0     1212 2023-05-19 19:11:38.923611 nemreader-0.8.6/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0     1185 2023-05-19 19:11:38.923611 nemreader-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1074 2023-05-19 19:11:38.923611 nemreader-0.8.6/LICENSE
+-rw-r--r--   0        0        0       26 2023-05-19 19:11:38.923611 nemreader-0.8.6/MANIFEST.in
+-rw-r--r--   0        0        0     1164 2023-05-19 19:11:38.923611 nemreader-0.8.6/README.md
+-rw-r--r--   0        0        0   101291 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/_static/img/nmi-suffixes.jpg
+-rw-r--r--   0        0        0    38420 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/_static/img/nmi-suffixes2.png
+-rw-r--r--   0        0        0    10717 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/_static/img/plot_cal.png
+-rw-r--r--   0        0        0    14205 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/_static/img/plot_profile.png
+-rwxr-xr-x   0        0        0     5363 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/file-format.md
+-rwxr-xr-x   0        0        0      658 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/gen_ref_pages.py
+-rwxr-xr-x   0        0        0      469 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/index.md
+-rwxr-xr-x   0        0        0      164 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/installation.md
+-rwxr-xr-x   0        0        0     5141 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/quickstart.md
+-rw-r--r--   0        0        0       60 2023-05-19 19:11:38.923611 nemreader-0.8.6/docs/requirements.txt
+-rw-r--r--   0        0        0    29436 2023-05-19 19:11:38.923611 nemreader-0.8.6/examples/Example_NEM12_ManyNMIs.zip
+-rw-r--r--   0        0        0      708 2023-05-19 19:11:38.923611 nemreader-0.8.6/examples/Example_different_intervals.zip
+-rw-r--r--   0        0        0      288 2023-05-19 19:11:38.923611 nemreader-0.8.6/examples/invalid/Example_NEM12_15min_200_30min_300.csv
+-rw-r--r--   0        0        0      480 2023-05-19 19:11:38.923611 nemreader-0.8.6/examples/invalid/Example_NEM12_15min_200_30min_400.csv
+-rw-r--r--   0        0        0      480 2023-05-19 19:11:38.923611 nemreader-0.8.6/examples/invalid/Example_NEM12_30min_200_15min_300.csv
+-rw-r--r--   0        0        0      480 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_30min_200_15min_400.csv
+-rw-r--r--   0        0        0       37 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_empty.csv
+-rw-r--r--   0        0        0     1147 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_incomplete_interval.csv
+-rw-r--r--   0        0        0      759 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_missing_header.csv
+-rw-r--r--   0        0        0     1505 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_powercor.csv
+-rw-r--r--   0        0        0      316 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_powercor.csv.zip
+-rw-r--r--   0        0        0     1409 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_NEM12_powercor_missing_fields.csv
+-rw-r--r--   0        0        0        0 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/invalid/Example_empty_file.csv
+-rw-r--r--   0        0        0     1424 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     2190 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1016 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      534 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      861 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      836 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      769 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      513 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1325 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      525 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1614 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1272 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1066 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      702 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      893 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      867 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      688 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      650 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      432 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      358 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      355 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      278 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      346 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      349 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      497 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      391 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      331 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      477 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      882 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      751 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1101 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0     1508 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      956 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1635 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      892 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1652 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      552 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      725 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      934 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      862 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      949 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      788 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      901 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      380 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      632 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      796 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      759 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      761 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      361 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      364 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      332 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      336 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1368 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1371 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1315 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1320 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      583 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      586 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      384 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      387 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      705 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      700 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1125 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      500 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      490 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      388 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      304 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      324 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      329 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      351 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      305 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      898 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1170 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      951 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     2136 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      883 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1972 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      550 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      553 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1017 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      851 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1488 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      771 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1450 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      352 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      961 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      717 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      693 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1070 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      366 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      343 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      299 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      400 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      278 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      337 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      345 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      293 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      274 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      279 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      313 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      323 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      327 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      310 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      288 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      309 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      340 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      791 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/unzipped/Example_NEM12_actual_interval.csv
+-rw-r--r--   0        0        0     1373 2023-05-19 19:11:38.927611 nemreader-0.8.6/examples/unzipped/Example_NEM12_different_interval_length.csv
+-rw-r--r--   0        0        0     4497 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM12_multiple_meters.csv
+-rw-r--r--   0        0        0      521 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM12_multiple_quality.csv
+-rw-r--r--   0        0        0      337 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM12_no_scheduled_read.csv
+-rw-r--r--   0        0        0      887 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM12_substituted_interval.csv
+-rw-r--r--   0        0        0      791 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM12_upper_case_units.csv
+-rw-r--r--   0        0        0      185 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM13_consumption_data.csv
+-rw-r--r--   0        0        0      345 2023-05-19 19:11:38.931611 nemreader-0.8.6/examples/unzipped/Example_NEM13_forward_estimate.csv
+-rwxr-xr-x   0        0        0      594 2023-05-19 19:11:38.931611 nemreader-0.8.6/mkdocs.yml
+-rw-r--r--   0        0        0      764 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/__main__.py
+-rw-r--r--   0        0        0     3754 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/cli.py
+-rw-r--r--   0        0        0     3515 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/nem_objects.py
+-rw-r--r--   0        0        0    23144 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/nem_reader.py
+-rw-r--r--   0        0        0     6000 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/output_db.py
+-rw-r--r--   0        0        0     5139 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/outputs.py
+-rw-r--r--   0        0        0        0 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/py.typed
+-rw-r--r--   0        0        0     5595 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/split_days.py
+-rw-r--r--   0        0        0       22 2023-05-19 19:11:38.931611 nemreader-0.8.6/nemreader/version.py
+-rwxr-xr-x   0        0        0     1381 2023-05-19 19:11:38.931611 nemreader-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1956 2023-05-19 19:11:38.931611 nemreader-0.8.6/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_actual_interval.py
+-rw-r--r--   0        0        0     1572 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_cli.py
+-rw-r--r--   0        0        0      469 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_consumption_data.py
+-rw-r--r--   0        0        0      850 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_dataframe_pivot.py
+-rw-r--r--   0        0        0      814 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_day_split.py
+-rw-r--r--   0        0        0     2099 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_file_outputs.py
+-rw-r--r--   0        0        0      359 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_header_datestamp.py
+-rw-r--r--   0        0        0     2043 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_incomplete_files.py
+-rw-r--r--   0        0        0      943 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_invalid_interval_mixing.py
+-rw-r--r--   0        0        0      284 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_legacy.py
+-rw-r--r--   0        0        0      252 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_many_nmis.py
+-rw-r--r--   0        0        0     1034 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_multiple_quality.py
+-rw-r--r--   0        0        0     1488 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_open_examples.py
+-rw-r--r--   0        0        0      268 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_optional_columns.py
+-rw-r--r--   0        0        0      589 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_output_db.py
+-rw-r--r--   0        0        0     1307 2023-05-19 19:11:38.931611 nemreader-0.8.6/tests/test_unit_capitalisation.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 nemreader-0.8.6/PKG-INFO
```

### Comparing `nemreader-0.8.4/.github/workflows/pythonpackage.yml` & `nemreader-0.8.6/.github/workflows/pythonpackage.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Python package
 
-on: ["push", "pull_request"]
+on: ["pull_request"]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
```

### Comparing `nemreader-0.8.4/.gitignore` & `nemreader-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/LICENSE` & `nemreader-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/README.md` & `nemreader-0.8.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # nem-reader
 
-[![PyPI version](https://badge.fury.io/py/nemreader.svg)](https://badge.fury.io/py/nemreader) ![Python package](https://github.com/aguinane/nem-reader/workflows/Python%20package/badge.svg?branch=develop) [![Documentation Status](https://readthedocs.org/projects/nem-reader/badge/?version=latest)](https://nem-reader.readthedocs.io/en/latest/?badge=latest)
+![Python package](https://github.com/aguinane/nem-reader/workflows/Python%20package/badge.svg?branch=master)
+[![PyPI version](https://img.shields.io/pypi/pyversions/nemreader?color=%2344CC11)](https://pypi.org/project/nemreader/)
+[![PyPi downloads](https://img.shields.io/pypi/dw/nemreader?label=downloads@pypi&color=344CC11)](https://pypi.org/project/nemreader/)
+[![Documentation Status](https://readthedocs.org/projects/nem-reader/badge/?version=latest)](https://nem-reader.readthedocs.io/en/latest/?badge=latest)
 
 The Australian Energy Market Operator (AEMO) defines a [Meter Data File Format (MDFF)](https://www.aemo.com.au/Stakeholder-Consultation/Consultations/Meter-Data-File-Format-Specification-NEM12-and-NEM13) for reading energy billing data.
 This library sets out to parse these NEM12 (interval metering data) and NEM13 (accumulated metering data) data files into a useful python object, for use in other projects.
 
 ---
 
 **[Read the documentation on ReadTheDocs!](https://nem-reader.readthedocs.io/en/latest/)**
```

### Comparing `nemreader-0.8.4/docs/_static/img/nmi-suffixes.jpg` & `nemreader-0.8.6/docs/_static/img/nmi-suffixes.jpg`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/_static/img/nmi-suffixes2.png` & `nemreader-0.8.6/docs/_static/img/nmi-suffixes2.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/_static/img/plot_cal.png` & `nemreader-0.8.6/docs/_static/img/plot_cal.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/_static/img/plot_profile.png` & `nemreader-0.8.6/docs/_static/img/plot_profile.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/file-format.md` & `nemreader-0.8.6/docs/file-format.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/gen_ref_pages.py` & `nemreader-0.8.6/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/docs/quickstart.md` & `nemreader-0.8.6/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/Example_NEM12_ManyNMIs.zip` & `nemreader-0.8.6/examples/Example_NEM12_ManyNMIs.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/Example_different_intervals.zip` & `nemreader-0.8.6/examples/Example_different_intervals.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/invalid/Example_NEM12_incomplete_interval.csv` & `nemreader-0.8.6/examples/invalid/Example_NEM12_incomplete_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/invalid/Example_NEM12_missing_header.csv` & `nemreader-0.8.6/examples/invalid/Example_NEM12_missing_header.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/invalid/Example_NEM12_powercor.csv` & `nemreader-0.8.6/examples/invalid/Example_NEM12_powercor.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/invalid/Example_NEM12_powercor_missing_fields.csv` & `nemreader-0.8.6/examples/invalid/Example_NEM12_powercor_missing_fields.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.6/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_actual_interval.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_actual_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_different_interval_length.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_different_interval_length.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_multiple_meters.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_multiple_meters.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_multiple_quality.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_multiple_quality.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_substituted_interval.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_substituted_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/examples/unzipped/Example_NEM12_upper_case_units.csv` & `nemreader-0.8.6/examples/unzipped/Example_NEM12_upper_case_units.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/mkdocs.yml` & `nemreader-0.8.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/__init__.py` & `nemreader-0.8.6/nemreader/__init__.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/cli.py` & `nemreader-0.8.6/nemreader/cli.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/nem_objects.py` & `nemreader-0.8.6/nemreader/nem_objects.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/nem_reader.py` & `nemreader-0.8.6/nemreader/nem_reader.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/output_db.py` & `nemreader-0.8.6/nemreader/output_db.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/outputs.py` & `nemreader-0.8.6/nemreader/outputs.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/nemreader/split_days.py` & `nemreader-0.8.6/nemreader/split_days.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/pyproject.toml` & `nemreader-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/requirements.txt` & `nemreader-0.8.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_actual_interval.py` & `nemreader-0.8.6/tests/test_actual_interval.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_cli.py` & `nemreader-0.8.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_dataframe_pivot.py` & `nemreader-0.8.6/tests/test_dataframe_pivot.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_day_split.py` & `nemreader-0.8.6/tests/test_day_split.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_file_outputs.py` & `nemreader-0.8.6/tests/test_file_outputs.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_incomplete_files.py` & `nemreader-0.8.6/tests/test_incomplete_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     nf = NEMFile("examples/invalid/Example_NEM12_powercor.csv", strict=False)
     assert "VABD000163" in nf.nmis
 
 
 def test_no_records():
     nf = NEMFile("examples/invalid/Example_NEM12_empty.csv", strict=False)
     meter_data = nf.nem_data()
-    assert len(meter_data.nmis) is 0
+    assert len(meter_data.nmis) == 0
 
 
 def test_empty_file():
     nf = NEMFile("examples/invalid/Example_empty_file.csv", strict=False)
     df = nf.get_data_frame()
     assert df is None
```

### Comparing `nemreader-0.8.4/tests/test_invalid_interval_mixing.py` & `nemreader-0.8.6/tests/test_invalid_interval_mixing.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 
 def test_30min_200_15min_300():
     with pytest.raises(ValueError):
         nf = NEMFile(
             "examples/invalid/Example_NEM12_30min_200_15min_300.csv", strict=False
         )
-        meter_data = nf.nem_data()
+        nf.nem_data()
 
 
 def test_15min_200_30min_300():
     with pytest.raises(ValueError):
         nf = NEMFile(
             "examples/invalid/Example_NEM12_15min_200_30min_300.csv", strict=False
         )
-        meter_data = nf.nem_data()
+        nf.nem_data()
 
 
 def test_30min_200_15min_400():
     with pytest.raises(ValueError):
         nf = NEMFile(
             "examples/invalid/Example_NEM12_30min_200_15min_400.csv", strict=False
         )
-        meter_data = nf.nem_data()
+        nf.nem_data()
 
 
 @pytest.mark.skip(reason="need to rearchitect parser to detect this")
 def test_15min_200_30min_400():
     with pytest.raises(ValueError):
         nf = NEMFile(
             "examples/invalid/Example_NEM12_15min_200_30min_400.csv", strict=False
         )
-        meter_data = nf.nem_data()
+        nf.nem_data()
```

### Comparing `nemreader-0.8.4/tests/test_multiple_quality.py` & `nemreader-0.8.6/tests/test_multiple_quality.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_open_examples.py` & `nemreader-0.8.6/tests/test_open_examples.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_output_db.py` & `nemreader-0.8.6/tests/test_output_db.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/tests/test_unit_capitalisation.py` & `nemreader-0.8.6/tests/test_unit_capitalisation.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.4/PKG-INFO` & `nemreader-0.8.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemreader
-Version: 0.8.4
+Version: 0.8.6
 Summary: nemreader
 Keywords: energy,NEM12,NEM13
 Author-email: Alex Guinman <alex@guinman.id.au>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,18 @@
 Project-URL: Documentation, https://nem-reader.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/aguinane/nem-reader/
 Provides-Extra: dev
 Provides-Extra: test
 
 # nem-reader
 
-[![PyPI version](https://badge.fury.io/py/nemreader.svg)](https://badge.fury.io/py/nemreader) ![Python package](https://github.com/aguinane/nem-reader/workflows/Python%20package/badge.svg?branch=develop) [![Documentation Status](https://readthedocs.org/projects/nem-reader/badge/?version=latest)](https://nem-reader.readthedocs.io/en/latest/?badge=latest)
+![Python package](https://github.com/aguinane/nem-reader/workflows/Python%20package/badge.svg?branch=master)
+[![PyPI version](https://img.shields.io/pypi/pyversions/nemreader?color=%2344CC11)](https://pypi.org/project/nemreader/)
+[![PyPi downloads](https://img.shields.io/pypi/dw/nemreader?label=downloads@pypi&color=344CC11)](https://pypi.org/project/nemreader/)
+[![Documentation Status](https://readthedocs.org/projects/nem-reader/badge/?version=latest)](https://nem-reader.readthedocs.io/en/latest/?badge=latest)
 
 The Australian Energy Market Operator (AEMO) defines a [Meter Data File Format (MDFF)](https://www.aemo.com.au/Stakeholder-Consultation/Consultations/Meter-Data-File-Format-Specification-NEM12-and-NEM13) for reading energy billing data.
 This library sets out to parse these NEM12 (interval metering data) and NEM13 (accumulated metering data) data files into a useful python object, for use in other projects.
 
 ---
 
 **[Read the documentation on ReadTheDocs!](https://nem-reader.readthedocs.io/en/latest/)**
```

