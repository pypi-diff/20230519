# Comparing `tmp/ladybug-grasshopper-1.9.3.tar.gz` & `tmp/ladybug-grasshopper-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-grasshopper-1.9.3.tar", last modified: Wed Jul  8 14:55:46 2020, max compression
+gzip compressed data, was "dist/ladybug-grasshopper-1.9.4.tar", last modified: Fri Jul 10 22:09:45 2020, max compression
```

## Comparing `ladybug-grasshopper-1.9.3.tar` & `ladybug-grasshopper-1.9.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5535 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import STAT.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Apply Analysis Period.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4801 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To IP.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7634 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB PMV Comfort.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7432 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Monthly Chart.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7039 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Export UserObject.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3905 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Data to Legacy.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3959 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Humidity Metrics.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6630 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Spatial Heatmap.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4802 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import Design Day.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3981 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB EPWmap.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     9398 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Wind Rose.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3795 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Data.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import DDY.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3781 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Time Interval Operation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     8905 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB SunPath.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5212 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Solar Body Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4519 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Calculate HOY.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To SI.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Legend Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Header.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4512 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Open Directory.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3788 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Relative Humidity from Dew Point.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5127 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Solar MRT from Solar Components.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5761 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Mass Arithmetic Operation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6970 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB UTCI Comfort.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4840 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Download Weather.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6709 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import EPW.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6170 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Legend Parameters Categorized.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3004 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import Location.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6128 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Arithmetic Operation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5722 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Sync Grasshopper File.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3375 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Location.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4686 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Unit Converter.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6407 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Adaptive Comfort.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4100 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Orient to Camera.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3762 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Convert to Timestep.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4814 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Create Legend.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3564 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Location.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3976 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Data.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Data Type.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Generate Point Grid.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7329 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Versioner.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To Unit.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4726 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Degree Days.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3177 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Apply Conditional Statement.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4057 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Header.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6305 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Hourly Plot.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5431 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Indoor Solar MRT.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4647 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Analysis Period.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5553 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Outdoor Solar MRT.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5486 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Design Day.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3786 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Comfort Statistics.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4967 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Adaptive Comfort Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3784 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Color Range.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB PMV Comfort Parameters.ghuser
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14458 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Wind Rose.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3316 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Design Day.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Degree Days.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB EPWmap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3582 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Time Interval Operation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1968 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Data Type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1606 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1383 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2397 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Generate Point Grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Unit Converter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2816 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2955 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Convert to Timestep.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Sync Grasshopper File.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To SI.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Relative Humidity from Dew Point.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7509 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import EPW.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2326 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Color Range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2854 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Data to Legacy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7417 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Hourly Plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5767 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB UTCI Comfort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4067 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Indoor Solar MRT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Legend Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3370 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Solar MRT from Solar Components.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4983 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Legend Parameters Categorized.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1301 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import STAT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Calculate HOY.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2936 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Solar Body Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Comfort Statistics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import Design Day.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import Location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To IP.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13262 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Versioner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2430 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Apply Conditional Statement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3520 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Spatial Heatmap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Humidity Metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Outdoor Solar MRT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4242 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Adaptive Comfort Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To Unit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3605 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Arithmetic Operation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB PMV Comfort Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8562 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB PMV Comfort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7957 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Monthly Chart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Apply Analysis Period.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Mass Arithmetic Operation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2860 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Create Legend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2948 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Orient to Camera.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import DDY.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Analysis Period.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7084 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Adaptive Comfort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13824 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB SunPath.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1555 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Open Directory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11299 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Export UserObject.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3300 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Download Weather.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      341 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/.github/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/samples/
--rw-rw-r--   0 travis    (2000) travis    (2000)    41307 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/samples/outdoor_comfort.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    21131 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/samples/windrose_plot.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1863 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/pass_tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    35141 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1863 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6544 2020-07-08 14:55:46.000000 ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      862 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-07-08 14:55:00.000000 ladybug-grasshopper-1.9.3/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5535 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import STAT.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Apply Analysis Period.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4801 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To IP.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7634 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB PMV Comfort.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7432 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Monthly Chart.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7039 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Export UserObject.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3905 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Data to Legacy.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3959 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Humidity Metrics.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6630 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Spatial Heatmap.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4802 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import Design Day.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3981 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB EPWmap.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9398 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Wind Rose.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3795 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Data.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import DDY.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3781 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Time Interval Operation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8905 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB SunPath.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5212 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Solar Body Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4519 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Calculate HOY.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To SI.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Legend Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Header.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4512 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Open Directory.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3788 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Relative Humidity from Dew Point.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5127 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Solar MRT from Solar Components.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5761 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Mass Arithmetic Operation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6970 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB UTCI Comfort.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4840 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Download Weather.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6709 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import EPW.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6170 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Legend Parameters Categorized.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3004 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import Location.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6128 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Arithmetic Operation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5722 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Sync Grasshopper File.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3375 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Location.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4686 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Unit Converter.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6407 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Adaptive Comfort.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4100 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Orient to Camera.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3762 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Convert to Timestep.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4814 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Create Legend.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3564 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Location.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3976 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Data.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Data Type.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Generate Point Grid.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7406 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Versioner.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To Unit.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4726 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Degree Days.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3177 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Apply Conditional Statement.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4057 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Header.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6305 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Hourly Plot.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5431 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Indoor Solar MRT.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4647 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Analysis Period.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5553 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Outdoor Solar MRT.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5486 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Design Day.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3786 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Comfort Statistics.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4967 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Adaptive Comfort Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3784 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Color Range.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB PMV Comfort Parameters.ghuser
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14458 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Wind Rose.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Header.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3316 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Design Day.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Degree Days.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB EPWmap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3582 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Time Interval Operation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1968 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Data Type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1606 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1383 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2397 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Generate Point Grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Unit Converter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2816 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Header.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2955 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Convert to Timestep.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Sync Grasshopper File.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To SI.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Relative Humidity from Dew Point.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7509 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import EPW.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2326 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Color Range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2854 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Data to Legacy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7417 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Hourly Plot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5767 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB UTCI Comfort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4067 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Indoor Solar MRT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Legend Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3370 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Solar MRT from Solar Components.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4983 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Legend Parameters Categorized.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1301 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import STAT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Calculate HOY.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2936 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Solar Body Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Comfort Statistics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import Design Day.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import Location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To IP.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13501 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Versioner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2430 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Apply Conditional Statement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3520 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Spatial Heatmap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Humidity Metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Outdoor Solar MRT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4242 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Adaptive Comfort Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To Unit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3605 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Arithmetic Operation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB PMV Comfort Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8562 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB PMV Comfort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7957 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Monthly Chart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Apply Analysis Period.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Mass Arithmetic Operation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2860 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Create Legend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2948 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Orient to Camera.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import DDY.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Analysis Period.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7084 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Adaptive Comfort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13824 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB SunPath.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1555 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Open Directory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11299 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Export UserObject.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3300 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Download Weather.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      341 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/.github/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/samples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41307 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/samples/outdoor_comfort.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21131 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/samples/windrose_plot.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1863 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/pass_tests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35141 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1863 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6544 2020-07-10 22:09:45.000000 ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      862 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-07-10 22:08:58.000000 ladybug-grasshopper-1.9.4/deploy.sh
```

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import STAT.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import STAT.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Apply Analysis Period.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Apply Analysis Period.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To IP.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To IP.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB PMV Comfort.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB PMV Comfort.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Monthly Chart.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Monthly Chart.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Export UserObject.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Export UserObject.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Data to Legacy.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Data to Legacy.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Humidity Metrics.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Humidity Metrics.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Spatial Heatmap.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Spatial Heatmap.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import Design Day.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import Design Day.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB EPWmap.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB EPWmap.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Wind Rose.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Wind Rose.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Data.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Data.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import DDY.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import DDY.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Time Interval Operation.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Time Interval Operation.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB SunPath.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB SunPath.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Solar Body Parameters.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Solar Body Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Calculate HOY.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Calculate HOY.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To SI.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To SI.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Legend Parameters.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Legend Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Header.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Header.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Open Directory.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Open Directory.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Relative Humidity from Dew Point.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Relative Humidity from Dew Point.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Solar MRT from Solar Components.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Solar MRT from Solar Components.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Mass Arithmetic Operation.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Mass Arithmetic Operation.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB UTCI Comfort.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB UTCI Comfort.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Download Weather.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Download Weather.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import EPW.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import EPW.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Legend Parameters Categorized.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Legend Parameters Categorized.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Import Location.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Import Location.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Arithmetic Operation.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Arithmetic Operation.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Sync Grasshopper File.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Sync Grasshopper File.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Location.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Location.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Unit Converter.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Unit Converter.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Adaptive Comfort.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Adaptive Comfort.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Orient to Camera.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Orient to Camera.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Convert to Timestep.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Convert to Timestep.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Create Legend.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Create Legend.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Location.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Location.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Data.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Data.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Construct Data Type.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Construct Data Type.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Generate Point Grid.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Generate Point Grid.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB To Unit.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB To Unit.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Degree Days.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Degree Days.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Apply Conditional Statement.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Apply Conditional Statement.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Header.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Header.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Hourly Plot.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Hourly Plot.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Indoor Solar MRT.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Indoor Solar MRT.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Analysis Period.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Analysis Period.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Outdoor Solar MRT.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Outdoor Solar MRT.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Deconstruct Design Day.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Deconstruct Design Day.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Comfort Statistics.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Comfort Statistics.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Adaptive Comfort Parameters.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Adaptive Comfort Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB Color Range.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB Color Range.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/user_objects/LB PMV Comfort Parameters.ghuser` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/user_objects/LB PMV Comfort Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Wind Rose.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Wind Rose.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Header.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Header.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Design Day.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Design Day.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Degree Days.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Degree Days.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB EPWmap.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB EPWmap.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Time Interval Operation.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Time Interval Operation.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Data Type.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Data Type.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Location.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Location.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Deconstruct Data.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Deconstruct Data.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Generate Point Grid.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Generate Point Grid.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Unit Converter.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Unit Converter.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Header.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Header.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Convert to Timestep.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Convert to Timestep.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Sync Grasshopper File.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Sync Grasshopper File.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To SI.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To SI.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Relative Humidity from Dew Point.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Relative Humidity from Dew Point.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import EPW.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import EPW.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Color Range.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Color Range.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Data to Legacy.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Data to Legacy.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Hourly Plot.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Hourly Plot.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB UTCI Comfort.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB UTCI Comfort.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Indoor Solar MRT.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Indoor Solar MRT.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Legend Parameters.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Legend Parameters.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Location.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Location.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Solar MRT from Solar Components.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Solar MRT from Solar Components.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Legend Parameters Categorized.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Legend Parameters Categorized.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Construct Data.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Construct Data.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import STAT.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import STAT.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Calculate HOY.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Calculate HOY.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Solar Body Parameters.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Solar Body Parameters.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Comfort Statistics.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Comfort Statistics.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import Design Day.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import Design Day.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import Location.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import Location.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To IP.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To IP.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Versioner.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Versioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,27 @@
     
     Returns:
         Vviiiiiz!: !!!
 """
 
 ghenv.Component.Name = 'LB Versioner'
 ghenv.Component.NickName = 'Versioner'
-ghenv.Component.Message = '0.1.0'
+ghenv.Component.Message = '0.1.1'
 ghenv.Component.Category = 'Ladybug'
 ghenv.Component.SubCategory = '5 :: Version'
 ghenv.Component.AdditionalHelpFromDocStrings = '1'
 
 try:
     from ladybug.futil import preparedir, nukedir, copy_file_tree, unzip_file
     from ladybug.config import folders
 except ImportError as e:
     raise ImportError('\nFailed to import ladybug:\n\t{}'.format(e))
 
 try:
+    from ladybug_rhino.pythonpath import iron_python_search_path, create_python_package_dir
     from ladybug_rhino.download import download_file_by_name
     from ladybug_rhino.grasshopper import all_required_inputs, give_warning
 except ImportError as e:
     raise ImportError('\nFailed to import ladybug_rhino:\n\t{}'.format(e))
 
 import os
 import subprocess
@@ -247,14 +248,16 @@
     rh_ver = ver_dict['ladybug-rhino']
     stderr = update_libraries_pip(py_exe, 'ladybug-rhino[cli]', rh_ver)
     if os.path.isdir(os.path.join(py_lib, 'ladybug_rhino-{}.dist-info'.format(rh_ver))):
         print 'Ladybug-rhino Python library successfully installed!\n '
     else:
         give_warning(ghenv.Component, stderr)
         print stderr
+    if os.name != 'nt':  # make sure libraries are copied to the rhino scripts folder
+        iron_python_search_path(create_python_package_dir())
 
     # install the grasshopper components
     print 'Installing Ladybug Tools Grasshopper components.'
     gh_ver = ver_dict['lbt-grasshopper']
     uo_folder = UserObjectFolders[0]
     stderr = update_libraries_pip(py_exe, 'lbt-grasshopper', gh_ver, uo_folder)
     lbgh_ver = ver_dict['ladybug-grasshopper']
```

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Apply Conditional Statement.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Apply Conditional Statement.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Spatial Heatmap.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Spatial Heatmap.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Humidity Metrics.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Humidity Metrics.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Outdoor Solar MRT.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Outdoor Solar MRT.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Adaptive Comfort Parameters.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Adaptive Comfort Parameters.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB To Unit.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB To Unit.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Arithmetic Operation.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Arithmetic Operation.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB PMV Comfort Parameters.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB PMV Comfort Parameters.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB PMV Comfort.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB PMV Comfort.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Monthly Chart.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Monthly Chart.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Apply Analysis Period.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Apply Analysis Period.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Mass Arithmetic Operation.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Mass Arithmetic Operation.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Create Legend.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Create Legend.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Orient to Camera.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Orient to Camera.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Import DDY.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Import DDY.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Analysis Period.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Analysis Period.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Adaptive Comfort.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Adaptive Comfort.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB SunPath.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB SunPath.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Open Directory.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Open Directory.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Export UserObject.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Export UserObject.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper/src/LB Download Weather.py` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper/src/LB Download Weather.py`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/.github/ISSUE_TEMPLATE.md` & `ladybug-grasshopper-1.9.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/samples/outdoor_comfort.gh` & `ladybug-grasshopper-1.9.4/samples/outdoor_comfort.gh`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/samples/windrose_plot.gh` & `ladybug-grasshopper-1.9.4/samples/windrose_plot.gh`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/PKG-INFO` & `ladybug-grasshopper-1.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-grasshopper
-Version: 1.9.3
+Version: 1.9.4
 Summary: Ladybug plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/ladybug-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/ladybug-grasshopper.svg?branch=master)](https://travis-ci.org/ladybug-tools/ladybug-grasshopper)
```

### Comparing `ladybug-grasshopper-1.9.3/README.md` & `ladybug-grasshopper-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/.travis.yml` & `ladybug-grasshopper-1.9.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/LICENSE` & `ladybug-grasshopper-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/PKG-INFO` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-grasshopper
-Version: 1.9.3
+Version: 1.9.4
 Summary: Ladybug plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/ladybug-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/ladybug-grasshopper.svg?branch=master)](https://travis-ci.org/ladybug-tools/ladybug-grasshopper)
```

### Comparing `ladybug-grasshopper-1.9.3/ladybug_grasshopper.egg-info/SOURCES.txt` & `ladybug-grasshopper-1.9.4/ladybug_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-grasshopper-1.9.3/setup.py` & `ladybug-grasshopper-1.9.4/setup.py`

 * *Files identical despite different names*

