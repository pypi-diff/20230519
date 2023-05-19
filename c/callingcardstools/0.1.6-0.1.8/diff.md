# Comparing `tmp/callingcardstools-0.1.6.tar.gz` & `tmp/callingcardstools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.6.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.8.tar", max compression
```

## Comparing `callingcardstools-0.1.6.tar` & `callingcardstools-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.6/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0    12696 2023-05-19 17:22:15.828857 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/Qbed.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     4285 2023-05-19 16:36:45.137643 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/combine.py
--rw-r--r--   0        0        0     9405 2023-05-19 16:10:01.287403 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.6/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.1.6/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
--rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.1.6/callingcardstools/BarcodeParser/mammals/__init__.py
--rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/combine_qc.py
--rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.6/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.6/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.6/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.1.6/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.6/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/__init__.py
--rw-r--r--   0        0        0     6020 2023-05-16 01:28:13.619621 callingcardstools-0.1.6/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/utils.py
--rw-r--r--   0        0        0     2016 2023-05-19 17:32:02.343826 callingcardstools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 callingcardstools-0.1.6/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.8/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.8/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.8/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.8/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0    12786 2023-05-19 17:42:53.279362 callingcardstools-0.1.8/callingcardstools/Alignment/mammals/Qbed.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.8/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     4252 2023-05-19 18:02:51.599306 callingcardstools-0.1.8/callingcardstools/Alignment/mammals/combine_qc.py
+-rw-r--r--   0        0        0     9949 2023-05-19 19:49:33.772526 callingcardstools-0.1.8/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.8/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.8/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.8/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.8/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.8/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.8/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.1.8/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.1.8/callingcardstools/BarcodeParser/mammals/__init__.py
+-rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.1.8/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.8/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.8/callingcardstools/BarcodeParser/yeast/combine_qc.py
+-rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.8/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.8/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.8/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.8/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.8/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.8/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.8/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.8/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.1.8/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.8/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.8/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.8/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.8/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     6389 2023-05-19 18:05:32.236311 callingcardstools-0.1.8/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.8/callingcardstools/utils.py
+-rw-r--r--   0        0        0     1941 2023-05-19 19:54:53.510231 callingcardstools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 callingcardstools-0.1.8/setup.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 callingcardstools-0.1.8/PKG-INFO
```

### Comparing `callingcardstools-0.1.6/LICENSE` & `callingcardstools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/README.md` & `callingcardstools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/mammals/Qbed.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/mammals/Qbed.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,18 @@
                 if suffix else filename + '.qbed'
             logger.info("writing qbed to %s", qbed_output_file)
             qbed_df.to_csv(qbed_output_file, sep='\t', index=False)
 
             qc_output_file = filename + '_' + suffix + '_aln_summary.tsv' \
                 if suffix else filename + '_aln_summary.tsv'
             logger.info("writing qc summary to %s", qc_output_file)
-            status_df.to_csv(qc_output_file, sep='\t', index=False, header=False)
+            status_df.to_csv(qc_output_file, 
+                             sep='\t', 
+                             index=False, 
+                             header=False)
 
             srt_output_file = filename + '_' + suffix + '_srt_count.tsv' \
                 if suffix else filename + '_srt_count.tsv'
             logger.info("writing srt summary to %s", srt_output_file)
             self._srt_writer(srt_output_file, 
                              single_srt_counter, 
                              multi_srt_counter)
```

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/mammals/combine.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/mammals/combine_qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # pylint:disable=W1203
 import os
 import argparse
 import logging
-import multiprocessing as mp
 
 from callingcardstools.BarcodeParser.mammals.BarcodeQcCounter import BarcodeQcCounter  # noqa
 from .Qbed import Qbed
 
 __all__ = ['main']
 
 logger = logging.getLogger(__name__)
@@ -33,17 +32,17 @@
 
     Returns:
         argparse.ArgumentParser: The subparser with the this additional
         cmd line tool added to it -- intended to be gathered in __main__.py
         to create a unified cmd line interface for the package
     """
     parser = subparser.add_parser(
-        'combine_mammals_data',
+        'mammals_combine_qc',
         help=script_description,
-        prog='combine_mammals_data',
+        prog='mammals_combine_qc',
         parents=[common_args]
     )
 
     # set the function to call when this subparser is used
     parser.set_defaults(func=main)
 
     input_group = parser.add_argument_group('input')
```

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # pylint:disable=W1203
 import os
 import argparse
-from typing import Iterator, Generator
 import logging
-from itertools import islice
-import multiprocessing as mp
 import tempfile
 
 import pysam
 
 from callingcardstools.Alignment.AlignmentTagger import AlignmentTagger
 from callingcardstools.QC.create_status_coder import create_status_coder  # noqa
 from callingcardstools.BarcodeParser.mammals.BarcodeQcCounter import BarcodeQcCounter  # noqa
@@ -79,36 +76,43 @@
         help="Reads less than or equal to mapq_threshold "
         "will be marked as failed",
         type=int,
         default=10)
 
     parse_bam_output = parser.add_argument_group('output')
     parse_bam_output.add_argument(
+        "-f",
+        "--filename",
+        help="Filename minus optional suffix "
+        " and extension. Default is the input file basename "
+        "minus the extension",
+        default="",
+        required=False)
+    parse_bam_output.add_argument(
         "-s",
         "--suffix",
-        help="suffix to add to output files. "
-        "Defaults to the input filename minus the extension",
+        help="suffix to add to output files.",
         default="",
         required=False)
     parse_bam_output.add_argument(
         "-p",
         "--pickle",
         help="Set this flag to save the qbed and qc data as pickle files. "
         "this is useful when processing split files in parallel and then "
         "combining later. Defaults to False, which saves as qbed/tsv",
         action="store_true")
-    
+
     return subparser
 
 
 def process_chunk(bam_in: pysam.AlignmentFile,
                   barcode_details_path: str,
                   genome_path: str,
                   mapq_threshold: int,
-                  annotation_tags: list = ['ST']) -> dict:
+                  annotation_tags: set = {'ST'}) -> dict:
     """This function is called when the subparser for this script is used.
     It parses the bam file, sets tags, and creates a summary and qbed file
 
     Args:
         bam_in (pysam.AlignmentFile): The bam file to parse
         contig (str): The contig to parse
         barcode_details_path (str): The path to the barcode details json
@@ -143,16 +147,16 @@
             not read.is_supplementary and \
                 not read.is_unmapped:
             # parse the barcode, tag the read
             tagged_read = at.tag_read(read)
             # eval the read based on quality expectations, get the status
             status = status_coder(tagged_read)
             # add the data to the qbed and qc records
-            output_dict['qbed'].update(tagged_read, 
-                                       status, 
+            output_dict['qbed'].update(tagged_read,
+                                       status,
                                        annotation_tags=annotation_tags)
             if status == 0:
                 # add the read to the passing_read list
                 output_dict['passing'].append(tagged_read['read'])
             else:
                 # add the read to the failing_read list
                 output_dict['failing'].append(tagged_read['read'])
@@ -182,61 +186,72 @@
                        args.genome]
     for input_path in input_path_list:
         if not os.path.exists(input_path):
             error_msg = f"Input file DNE: {input_path}"
             logger.debug(error_msg)
             raise FileNotFoundError(error_msg)
 
-    output_basename = os.path.splitext(os.path.basename(args.input))[0]
+    output_basename = args.filename if args.filename \
+        else os.path.splitext(os.path.basename(args.input))[0]
 
     # open the bam file
     logger.info(f'beginning to parse {args.input}')
     bam_in = pysam.AlignmentFile(args.input)  # pylint:disable=E1101
 
     result_dict = process_chunk(bam_in,
                                 args.barcode_details,
                                 args.genome,
                                 args.mapq_threshold)
 
     # write out
-    logger.info("writing unsorted bam files to a temporary directory...")
     with tempfile.TemporaryDirectory() as tmpdir:
-        # write the passing reads to a bam file
-        tmp_passing_bam_output = os.path.join(tmpdir, 'passing.bam')
-        with pysam.AlignmentFile(tmp_passing_bam_output,
-                                 'wb',
-                                 header=bam_in.header) as tmp_passing_bam:
-            for read in result_dict['passing']:
-                tmp_passing_bam.write(read)
-
-        # write the failing reads to a bam file
-        tmp_failing_bam_output = os.path.join(tmpdir, 'failing.bam')
-        with pysam.AlignmentFile(tmp_failing_bam_output,
-                                 'wb',
-                                 header=bam_in.header) as tmp_failing_bam:
-            for read in result_dict['failing']:
-                tmp_failing_bam.write(read)
-
-        # sort the passing and failing bam files with pysam
-        logger.info("sorting passing and failing bam files...")
-        try:
-            passing_output_filename = \
-                output_basename + '_' + args.suffix + '_passing.bam' \
-                if args.suffix else output_basename + '_passing.bam'
-            pysam.sort("-o", passing_output_filename,
-                       tmp_passing_bam_output)
-        except pysam.SamtoolsError as exc:
-            raise pysam.SamtoolsError('Error sorting passing bam file') from exc  # noqa
-        try:
-            failing_output_filename = \
-                output_basename + '_' + args.suffix + '_failing.bam' \
-                if args.suffix else output_basename + '_failing.bam'
-            pysam.sort("-o", failing_output_filename,
-                       tmp_failing_bam_output)
-        except pysam.SamtoolsError as exc:
-            raise pysam.SamtoolsError('Error sorting failing bam file') from exc  # noqa
+        if len(result_dict['passing']) > 0:
+            logger.info("writing unsorted passing bam...")
+            # write the passing reads to a bam file
+            tmp_passing_bam_output = os.path.join(tmpdir, 'passing.bam')
+            with pysam.AlignmentFile(tmp_passing_bam_output,
+                                     'wb',
+                                     header=bam_in.header) as tmp_passing_bam:
+                for read in result_dict['passing']:
+                    tmp_passing_bam.write(read)
+            # sort the passing and failing bam files with pysam
+            logger.info("sorting passing bam...")
+
+            try:
+                passing_output_filename = \
+                    output_basename + '_' + args.suffix + '_passing.bam' \
+                    if args.suffix else output_basename + '_passing.bam'
+                pysam.sort("-o", passing_output_filename,
+                           tmp_passing_bam_output)
+            except pysam.SamtoolsError as exc:
+                raise pysam.SamtoolsError('Error sorting passing bam file') from exc  # noqa
+
+        else:
+            logger.info(f"No passing reads found in {args.input}")
+
+        if len(result_dict['failing']) > 0:
+
+            logger.info("writing unsorted failing bam...")
+            tmp_failing_bam_output = os.path.join(tmpdir, 'failing.bam')
+            with pysam.AlignmentFile(tmp_failing_bam_output,
+                                     'wb',
+                                     header=bam_in.header) as tmp_failing_bam:
+                for read in result_dict['failing']:
+                    tmp_failing_bam.write(read)
+
+            try:
+                failing_output_filename = \
+                    output_basename + '_' + args.suffix + '_failing.bam' \
+                    if args.suffix else output_basename + '_failing.bam'
+                logger.info("sorting failing bam...")
+                pysam.sort("-o", failing_output_filename,
+                           tmp_failing_bam_output)
+            except pysam.SamtoolsError as exc:
+                raise pysam.SamtoolsError('Error sorting failing bam file') from exc  # noqa
+        else:
+            logger.info(f"No failing reads found in {args.input}")
 
     # write out
     result_dict['qbed'].write(output_basename, args.suffix, args.pickle)
     result_dict['barcode_qc'].write(output_basename, args.suffix, args.pickle)
 
     logger.info(f"file: {args.input} complete!")
```

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.8/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.8/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.8/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py` & `callingcardstools-0.1.8/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.8/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/combine_qc.py` & `callingcardstools-0.1.8/callingcardstools/BarcodeParser/yeast/combine_qc.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.1.8/callingcardstools/QC/StatusFlags.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.8/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.8/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.8/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.8/callingcardstools/Reads/split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.8/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.1.8/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.8/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.8/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.8/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.8/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.8/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/callingcardstools/__main__.py` & `callingcardstools-0.1.8/callingcardstools/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from logging.config import dictConfig
 from importlib.metadata import version
 
 from .BarcodeParser import barcode_table_to_json
 from .BarcodeParser.yeast import combine_qc as yeast_combine_qc
 from .Reads import legacy_split_fastq, split_fastq
 from .Alignment.yeast import legacy_makeccf
-from .Alignment.mammals import process_alignments as process_mammals_bam
 from .Alignment.yeast import process_alignments as process_yeast_bam
+from .Alignment.mammals import process_alignments as process_mammals_bam
+from .Alignment.mammals import combine_qc as mammals_combine_qc
 
 
 def parse_args() -> Callable[[list], argparse.Namespace]:
     """Create a cmd line argument parser for callingcardstools
 
     Returns:
             Callable[[list],Namespace]: This function returns the main
@@ -46,14 +47,17 @@
         'qBed format file of the passing reads, and a qc file which '
         'allows finer exploration of the barcode and alignment metrics',
 
         'process_mammals_bam': 'Iterate over the reads in an alignment file (bam) and '
         'separate reads into passing.bam and failing.bam, a '
         'qBed format file of the passing reads, and a qc file which '
         'allows finer exploration of the barcode and alignment metrics',
+        
+        'mammals_combine_qc': 'Combine qbed and barcodeQC objects which may '
+        'result from splitting the fastq and processing chunks in parallel',
     }
 
     # common options -- these can be applied to all scripts via the 'parent'---
     # argument -- see subparsers.add_parser for parse_bam below ---------------
     common_args = argparse.ArgumentParser(
         prog="callingcardstools", add_help=False)
     common_args_group = common_args.add_argument_group('General')
@@ -112,14 +116,19 @@
 
     subparsers = process_mammals_bam.parse_args(
         subparsers,
         script_descriptions['process_mammals_bam'],
         common_args
     )
 
+    subparsers = mammals_combine_qc.parse_args(
+        subparsers,
+        script_descriptions['mammals_combine_qc'],
+        common_args)
+
     # return the top level parser to be used in the main method below
     return parser
 
 
 def main(args=None) -> None:
     """Entry point to callingcardstools"""
```

### Comparing `callingcardstools-0.1.6/callingcardstools/utils.py` & `callingcardstools-0.1.8/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.6/pyproject.toml` & `callingcardstools-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.6"
+version = "0.1.8"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
 exclude = ['Dockerfile', '*temp_*','docs', 'site', 'tests', '.git','.venv','.github', 'Resources/yeast/README.md']
 include = ["callingcardstools/Resources"]
 
 [tool.poetry.dependencies]
-# note: this is required for scipy
-python = ">=3.8,<3.11"
-pandas = "^1.4.3"
-numpy = "^1.23.1"
+python = ">=3.8"
+pandas = "^1.5.3"
+numpy = "^1.24.3"
 pysam = "^0.19.1"
-Cython = "^0.29.30"
-biopython = "^1.79"
-scipy = "^1.8.1"
 edlib = "^1.3.9"
+biopython = "^1.81"
 
 [tool.poetry.group.dev.dependencies]
-ipykernel = "^6.15.1"
+ipykernel = "^6.23.1"
 docutils = "^0.19"
-mkdocs = "^1.3.1"
-mkdocs-material = "^8.3.9"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocs = "^1.4.3"
+mkdocs-material = "^8.5.11"
+mkdocstrings = {extras = ["python"], version = "^0.19.1"}
 handler = "^1.3.0"
 pytest-cov = "^3.0.0"
-pipenv = "^2022.9.4"
-pyright = "^1.1.269"
-pytest = "^7.1.3"
+pipenv = "^2022.12.19"
+pyright = "^1.1.309"
+pytest = "^7.3.1"
 memory-profiler = "^0.60.0"
-mkdocs-section-index = "^0.3.4"
+mkdocs-section-index = "^0.3.5"
 autopep8 = "^2.0.2"
 
 [tool.pyright]
 include = ["callingcardstools"]
 exclude = ["**/node_modules",
     "**/__pycache__",
     "src/experimental",
```

### Comparing `callingcardstools-0.1.6/setup.py` & `callingcardstools-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,37 +16,35 @@
  'callingcardstools.Resources.mouse',
  'callingcardstools.Resources.yeast']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Cython>=0.29.30,<0.30.0',
- 'biopython>=1.79,<2.0',
+['biopython>=1.81,<2.0',
  'edlib>=1.3.9,<2.0.0',
- 'numpy>=1.23.1,<2.0.0',
- 'pandas>=1.4.3,<2.0.0',
- 'pysam>=0.19.1,<0.20.0',
- 'scipy>=1.8.1,<2.0.0']
+ 'numpy>=1.24.3,<2.0.0',
+ 'pandas>=1.5.3,<2.0.0',
+ 'pysam>=0.19.1,<0.20.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.6',
+    'version': '0.1.8',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `callingcardstools-0.1.6/PKG-INFO` & `callingcardstools-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.6
+Version: 0.1.8
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Cython (>=0.29.30,<0.30.0)
-Requires-Dist: biopython (>=1.79,<2.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: edlib (>=1.3.9,<2.0.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pysam (>=0.19.1,<0.20.0)
-Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Project-URL: Documentation, https://cmatkhan.github.io/callingCardsTools/
 Project-URL: Repository, https://github.com/cmatKhan/callingCardsTools
 Description-Content-Type: text/markdown
 
 # Installation 
 
 ```
```

