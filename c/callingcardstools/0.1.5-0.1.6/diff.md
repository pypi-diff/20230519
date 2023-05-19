# Comparing `tmp/callingcardstools-0.1.5.tar.gz` & `tmp/callingcardstools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.5.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.6.tar", max compression
```

## Comparing `callingcardstools-0.1.5.tar` & `callingcardstools-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.5/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/ReadRecords.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.5/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    17091 2023-05-15 16:54:18.678237 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/combine_qc.py
--rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.5/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.5/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.5/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.5/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/__init__.py
--rw-r--r--   0        0        0     6020 2023-05-16 01:28:13.619621 callingcardstools-0.1.5/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/utils.py
--rw-r--r--   0        0        0     2016 2023-05-16 01:33:28.098799 callingcardstools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.5/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.6/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0    12696 2023-05-19 17:22:15.828857 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/Qbed.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     4285 2023-05-19 16:36:45.137643 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/combine.py
+-rw-r--r--   0        0        0     9405 2023-05-19 16:10:01.287403 callingcardstools-0.1.6/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.6/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.6/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.6/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.1.6/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.1.6/callingcardstools/BarcodeParser/mammals/__init__.py
+-rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/combine_qc.py
+-rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.6/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.6/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.6/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.6/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.1.6/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.6/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.6/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     6020 2023-05-16 01:28:13.619621 callingcardstools-0.1.6/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.6/callingcardstools/utils.py
+-rw-r--r--   0        0        0     2016 2023-05-19 17:32:02.343826 callingcardstools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 callingcardstools-0.1.6/setup.py
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.6/PKG-INFO
```

### Comparing `callingcardstools-0.1.5/LICENSE` & `callingcardstools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/README.md` & `callingcardstools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.6/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.6/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.6/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,242 @@
 # pylint:disable=W1203
 import os
 import argparse
+from typing import Iterator, Generator
 import logging
+from itertools import islice
+import multiprocessing as mp
 import tempfile
 
 import pysam
 
 from callingcardstools.Alignment.AlignmentTagger import AlignmentTagger
-from callingcardstools.QC.StatusFlags import StatusFlags
-from callingcardstools.QC.create_status_coder import create_status_coder # noqa
-from .ReadRecords import ReadRecords
+from callingcardstools.QC.create_status_coder import create_status_coder  # noqa
+from callingcardstools.BarcodeParser.mammals.BarcodeQcCounter import BarcodeQcCounter  # noqa
+from .Qbed import Qbed
 
-__all__ = ['parse_bam']
+__all__ = ['main']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def parse_args(
-    subparser, 
-    script_description, 
-    common_args) -> argparse.ArgumentParser: # noqa
-    """This is intended to be used as a subparser for a parent parser passed 
-    from __main__.py. It adds the arguments required to iterate over mammals 
-    alignments, set tags and create both a summary and the qbed (quantified 
+    subparser,
+    script_description,
+    common_args) -> argparse.ArgumentParser:  # noqa
+    """This is intended to be used as a subparser for a parent parser passed
+    from __main__.py. It adds the arguments required to iterate over mammals
+    alignments, set tags and create both a summary and the qbed (quantified
     hops file)
 
     Args:
-        subparser (argparse.ArgumentParser): See __main__.py -- this is the 
+        subparser (argparse.ArgumentParser): See __main__.py -- this is the
         subparser for the parent parser in __main__.py
-        script_desc (str): Description of this script, which is set in 
-        __main__.py. The description is set in __main__.py so that all of 
-        the script descriptions are together in one spot and it is easier to 
+        script_desc (str): Description of this script, which is set in
+        __main__.py. The description is set in __main__.py so that all of
+        the script descriptions are together in one spot and it is easier to
         write a unified cmd line interface
-        common_args (argparse.ArgumentParser): These are the common arguments 
+        common_args (argparse.ArgumentParser): These are the common arguments
         for all scripts in callingCardsTools, for instance logging level
 
     Returns:
-        argparse.ArgumentParser: The subparser with the this additional 
-        cmd line tool added to it -- intended to be gathered in __main__.py 
+        argparse.ArgumentParser: The subparser with the this additional
+        cmd line tool added to it -- intended to be gathered in __main__.py
         to create a unified cmd line interface for the package
     """
     parser = subparser.add_parser(
         'process_mammals_bam',
         help=script_description,
         prog='process_mammals_bam',
         parents=[common_args]
     )
 
     # set the function to call when this subparser is used
-    parser.set_defaults(func=parse_bam)
+    parser.set_defaults(func=main)
 
-    parser = parser.add_argument_group('input')
-    parser.add_argument(
+    input_group = parser.add_argument_group('input')
+    input_group.add_argument(
         "-i",
         "--input",
-        help="path to bam file. Note that this must be " +
-        "sorted, and that an index .bai file must " +
+        help="path to bam file. Note that this must be "
+        "sorted, and that an index .bai file must "
         "exist in the same directory",
         required=True)
-    parser.add_argument(
+    input_group.add_argument(
         "-b",
         "--barcode_details",
         help="path to the barcode details json",
         required=True)
-    parser.add_argument(
+    input_group.add_argument(
         "-g",
         "--genome",
-        help="path to genome fasta file. " +
-        "Note that a index .fai must exist " +
+        help="path to genome fasta file. "
+        "Note that a index .fai must exist "
         "in the same directory",
         required=True)
-
-    parse_bam_output = parser.add_argument_group('output')
-    parse_bam_output.add_argument(
-        "-o",
-        "--output_prefix",
-        help="path to output directory. if not provided, " +
-        "output to current working directory",
-        default="",
-        required=False)
-    parse_bam_output.add_argument(
-        "-qc",
-        "--record_barcode_qc",
-        help="set to False to avoid recording barcode qc " +
-        "details while processing the bam. Defaults to True, but this " +
-        "can take an enormous amount of memory. Set to false if there " +
-        "is a memory problem.",
-        default=True,
-        type=bool,
-        required=False)
-    parse_bam_output.add_argument(
-        "-t",
-        "--tally",
-        help="tally srt and multi srt sites. this creates two additional " +
-        "qc summaries",
-        default=True,
-        type=bool,
-        required=False)
-
-    parse_bam_settings = parser.add_argument_group('settings')
-    parse_bam_settings.add_argument(
+    input_group.add_argument(
         "-q",
         "--mapq_threshold",
-        help="Reads less than or equal to mapq_threshold " +
+        help="Reads less than or equal to mapq_threshold "
         "will be marked as failed",
         type=int,
         default=10)
 
+    parse_bam_output = parser.add_argument_group('output')
+    parse_bam_output.add_argument(
+        "-s",
+        "--suffix",
+        help="suffix to add to output files. "
+        "Defaults to the input filename minus the extension",
+        default="",
+        required=False)
+    parse_bam_output.add_argument(
+        "-p",
+        "--pickle",
+        help="Set this flag to save the qbed and qc data as pickle files. "
+        "this is useful when processing split files in parallel and then "
+        "combining later. Defaults to False, which saves as qbed/tsv",
+        action="store_true")
+    
     return subparser
 
 
-def parse_bam(args: argparse.Namespace) -> None:
+def process_chunk(bam_in: pysam.AlignmentFile,
+                  barcode_details_path: str,
+                  genome_path: str,
+                  mapq_threshold: int,
+                  annotation_tags: list = ['ST']) -> dict:
     """This function is called when the subparser for this script is used.
     It parses the bam file, sets tags, and creates a summary and qbed file
-    
+
     Args:
-        args (argparse.Namespace): The arguments passed from the cmd line
-        
-        Raises:
-            FileNotFoundError: If the input file does not exist
-            
-        Returns:
-            None
+        bam_in (pysam.AlignmentFile): The bam file to parse
+        contig (str): The contig to parse
+        barcode_details_path (str): The path to the barcode details json
+        genome_path (str): The path to the genome fasta file
+        mapq_threshold (int): Reads less than or equal to mapq_threshold
+        will be marked as failed
+        annotation_tags (list, optional): The tags to use for annotation.
+
+    Returns:
+        dict: A dictionary with the following keys:
+            'passing': A list of passing reads
+            'failing': A list of failing reads
+            'qbed': A Qbed object
+            'barcode_qc': A BarcodeQcCounter object
     """
+    output_dict = {
+        'passing': [],
+        'failing': [],
+        'qbed': Qbed(),
+        'barcode_qc': BarcodeQcCounter()
+    }
+    # create an AlignmentTagger object
+    at = AlignmentTagger(barcode_details_path,
+                         genome_path)  # pylint:disable=C0103
+    status_coder = create_status_coder(at.insert_seq, mapq_threshold)
+
+    # start iterating over the bam_chunk
+    logger.debug("iterating over bam chunk...")
+    for read in bam_in.fetch():
+        # only look at mapped primary alignments
+        if not read.is_secondary and \
+            not read.is_supplementary and \
+                not read.is_unmapped:
+            # parse the barcode, tag the read
+            tagged_read = at.tag_read(read)
+            # eval the read based on quality expectations, get the status
+            status = status_coder(tagged_read)
+            # add the data to the qbed and qc records
+            output_dict['qbed'].update(tagged_read, 
+                                       status, 
+                                       annotation_tags=annotation_tags)
+            if status == 0:
+                # add the read to the passing_read list
+                output_dict['passing'].append(tagged_read['read'])
+            else:
+                # add the read to the failing_read list
+                output_dict['failing'].append(tagged_read['read'])
+            # record barcode QC
+            bc_counter_dict = {k: (v['query'], v['dist'] == 0) for
+                               k, v in (tagged_read['barcode_details']
+                                        ['details'].items())}
+            bc_status = all([v[1] for v in bc_counter_dict.values()])
+            output_dict['barcode_qc'].update(
+                bc_counter_dict['r1_pb'][0],
+                bc_counter_dict['r1_lrt1'][0],
+                bc_counter_dict['r1_lrt2'][0],
+                bc_counter_dict['r1_srt'][0],
+                bc_status)
+
+    return output_dict
+
+
+def main(args: argparse.Namespace) -> None:
+
+    logger.debug(args)
+
     # Check input paths
-    logging.info('checking input...')
+    logger.info('checking input...')
     input_path_list = [args.input,
                        args.barcode_details,
                        args.genome]
-    if args.output_prefix:
-        input_path_list.append(args.output_prefix)
     for input_path in input_path_list:
         if not os.path.exists(input_path):
             error_msg = f"Input file DNE: {input_path}"
-            logging.debug(error_msg)
+            logger.debug(error_msg)
             raise FileNotFoundError(error_msg)
 
-    logging.info(f'beginning to parse {args.input}')
-    output_bampath_dict = \
-        {k: os.path.join(
-            args.output_prefix,
-            os.path.splitext(os.path.basename(args.input))[0]+'_'+k+'.bam')
-            for k in ['passing', 'failing']}
-
-    logging.info(args)
-
-    qbed_output = os.path.join(
-        args.output_prefix,
-        os.path.splitext(os.path.basename(args.input))[0] + '.qbed')
-    qc_output = os.path.join(
-        args.output_prefix,
-        os.path.splitext(os.path.basename(args.input))[0] + '_qc.tsv')
-
-    logging.info(f"qbed output: {qbed_output}")
-    logging.info(f"qc_output: {qc_output}")
+    output_basename = os.path.splitext(os.path.basename(args.input))[0]
 
     # open the bam file
+    logger.info(f'beginning to parse {args.input}')
     bam_in = pysam.AlignmentFile(args.input)  # pylint:disable=E1101
 
-    # open output files for tagged bam reads
-    output_bam_dict = \
-        {k: pysam.AlignmentFile(v, "wb", header=bam_in.header)  
-            for k, v in output_bampath_dict.items()}
-
-    # create an AlignmentTagger object
-    at = AlignmentTagger(args.barcode_details,
-                         args.genome)  # pylint:disable=C0103
-
-    # create a temp directory which will be destroyed when this context block
-    # exits
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        # create tmp files and use them to instantiate the ReadRecords object
-        qbed_tmp_file = os.path.join(tmp_dir, "tmp_qbed.tsv")
-        qc_tmp_file = os.path.join(tmp_dir, "tmp_qc.tsv")
-        # instantiate ReadRecords object to handle creating qbed, qc files
-        read_records = ReadRecords(qbed_tmp_file, qc_tmp_file)
-        # create a status coder object to handle adding status codes
-        # to the reads
-        status_coder = create_status_coder(at.insert_seq, args.mapq_threshold)
-        logging.info("iterating over bam file...")
-        for read in bam_in.fetch():
-            # only look at mapped primary alignments
-            if not read.is_secondary and \
-                not read.is_supplementary and \
-                    not read.is_unmapped:
-                # parse the barcode, tag the read
-                tagged_read = at.tag_read(read)
-                # eval the read based on quality expectations, get the status
-                status = status_coder(tagged_read)
-                # add the data to the qbed and qc records
-                read_records\
-                    .add_read_info(
-                        tagged_read,
-                        status,
-                        insert_offset=at.insert_length,
-                        annotation_tags=at.annotation_tags,
-                        record_barcode_qc=args.record_barcode_qc)
-                # write the read out to the appropriate tagged bamfile
-                if status == 0:
-                    output_bam_dict['passing'].write(tagged_read['read'])
-                else:
-                    output_bam_dict['failing'].write(tagged_read['read'])
-
-        logging.info("writing qBed...")
-        read_records.to_qbed(qbed_output, args.tally)
-        if args.record_barcode_qc:
-            logging.info("writing qc...")
-            read_records.summarize_qc(qc_output)
+    result_dict = process_chunk(bam_in,
+                                args.barcode_details,
+                                args.genome,
+                                args.mapq_threshold)
+
+    # write out
+    logger.info("writing unsorted bam files to a temporary directory...")
+    with tempfile.TemporaryDirectory() as tmpdir:
+        # write the passing reads to a bam file
+        tmp_passing_bam_output = os.path.join(tmpdir, 'passing.bam')
+        with pysam.AlignmentFile(tmp_passing_bam_output,
+                                 'wb',
+                                 header=bam_in.header) as tmp_passing_bam:
+            for read in result_dict['passing']:
+                tmp_passing_bam.write(read)
+
+        # write the failing reads to a bam file
+        tmp_failing_bam_output = os.path.join(tmpdir, 'failing.bam')
+        with pysam.AlignmentFile(tmp_failing_bam_output,
+                                 'wb',
+                                 header=bam_in.header) as tmp_failing_bam:
+            for read in result_dict['failing']:
+                tmp_failing_bam.write(read)
+
+        # sort the passing and failing bam files with pysam
+        logger.info("sorting passing and failing bam files...")
+        try:
+            passing_output_filename = \
+                output_basename + '_' + args.suffix + '_passing.bam' \
+                if args.suffix else output_basename + '_passing.bam'
+            pysam.sort("-o", passing_output_filename,
+                       tmp_passing_bam_output)
+        except pysam.SamtoolsError as exc:
+            raise pysam.SamtoolsError('Error sorting passing bam file') from exc  # noqa
+        try:
+            failing_output_filename = \
+                output_basename + '_' + args.suffix + '_failing.bam' \
+                if args.suffix else output_basename + '_failing.bam'
+            pysam.sort("-o", failing_output_filename,
+                       tmp_failing_bam_output)
+        except pysam.SamtoolsError as exc:
+            raise pysam.SamtoolsError('Error sorting failing bam file') from exc  # noqa
+
+    # write out
+    result_dict['qbed'].write(output_basename, args.suffix, args.pickle)
+    result_dict['barcode_qc'].write(output_basename, args.suffix, args.pickle)
 
-    logging.info(f"file: {args.input} complete!")
+    logger.info(f"file: {args.input} complete!")
```

### Comparing `callingcardstools-0.1.5/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.6/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.6/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.6/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.6/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 logger = logging.getLogger(__name__)
 
 # TODO: use this to re-write the barcodeparser object. reduce the barcode
 # parse to common attr and methods for any organism, and then extend it
 # for mammals/yeast. use this as the yeast basis. Do not align the barcode
 # components more than once in the iteration of the fastq file.
 
+
 class InnerDefaultDict(defaultdict):
     def __init__(self, data_type=int):
         super().__init__(data_type)
 
+
 class MiddleDefaultDict1(defaultdict):
     def __init__(self, data_type=int):
         super().__init__(partial(InnerDefaultDict, data_type))
 
+
 class MiddleDefaultDict2(defaultdict):
     def __init__(self, data_type=int):
         super().__init__(partial(MiddleDefaultDict1, data_type))
 
+
 class OuterDefaultDict(defaultdict):
     def __init__(self, data_type=int):
         super().__init__(partial(MiddleDefaultDict2, data_type))
 
 
 class BarcodeQcCounter:
     """A class for counting and processing barcode quality control data.
@@ -66,18 +70,14 @@
         """
         if pickle_path:
             if not os.path.exists(pickle_path):
                 msg = f"Path to pickle file {pickle_path} does not exist"
                 raise FileNotFoundError(msg)
             self.load(pickle_path)
         else:
-            # self._metrics = defaultdict(
-            #     lambda: defaultdict(
-            #         lambda: defaultdict(lambda: defaultdict(int)))
-            # )
             self._metrics = OuterDefaultDict(int)
             self._r1_transposon_seq_dict = defaultdict(set)
 
     @property
     def metrics(self) -> defaultdict:
         """Returns the _metrics attribute.
 
@@ -384,8 +384,8 @@
                 filename + "_r2_transposon_summary" + append_suffix + ".csv"
             r2_transposon_summary_path = os.path.join(
                 output_dirpath, r2_transposon_summary_basename)
             r2_transposon_summary_df = pd.DataFrame(r2_transposon_summary)
             logger.info("writing r2_transposon_summary "
                         "to %s{r2_transposon_summary_path}")
             r2_transposon_summary_df.to_csv(
-                r2_transposon_summary_path, index=False)
+                r2_transposon_summary_path, index=False)
```

### Comparing `callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/combine_qc.py` & `callingcardstools-0.1.6/callingcardstools/BarcodeParser/yeast/combine_qc.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.1.6/callingcardstools/QC/StatusFlags.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.6/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.6/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.6/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.6/callingcardstools/Reads/split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.6/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.6/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.6/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.6/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.6/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.6/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/__main__.py` & `callingcardstools-0.1.6/callingcardstools/__main__.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/callingcardstools/utils.py` & `callingcardstools-0.1.6/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.5/pyproject.toml` & `callingcardstools-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.5"
+version = "0.1.6"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
```

### Comparing `callingcardstools-0.1.5/setup.py` & `callingcardstools-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 packages = \
 ['callingcardstools',
  'callingcardstools.Alignment',
  'callingcardstools.Alignment.mammals',
  'callingcardstools.Alignment.yeast',
  'callingcardstools.BarcodeParser',
+ 'callingcardstools.BarcodeParser.mammals',
  'callingcardstools.BarcodeParser.yeast',
  'callingcardstools.QC',
  'callingcardstools.Reads',
  'callingcardstools.Resources',
  'callingcardstools.Resources.human',
  'callingcardstools.Resources.mouse',
  'callingcardstools.Resources.yeast']
@@ -28,15 +29,15 @@
  'scipy>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.5/PKG-INFO` & `callingcardstools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

