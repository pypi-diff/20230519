# Comparing `tmp/modbedtools-0.1.0.tar.gz` & `tmp/modbedtools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbedtools-0.1.0.tar", last modified: Fri Jan 20 05:28:33 2023, max compression
+gzip compressed data, was "modbedtools-0.1.1.tar", last modified: Fri May 19 14:39:30 2023, max compression
```

## Comparing `modbedtools-0.1.0.tar` & `modbedtools-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-01-20 05:28:33.476890 modbedtools-0.1.0/
--rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.0/LICENSE
--rw-r--r--   0 dli        (501) staff       (20)     4174 2023-01-20 05:28:33.476183 modbedtools-0.1.0/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)     3729 2023-01-19 05:40:14.000000 modbedtools-0.1.0/README.md
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-01-20 05:28:33.470480 modbedtools-0.1.0/modbed/
--rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.0/modbed/__init__.py
--rw-r--r--   0 dli        (501) staff       (20)     5083 2023-01-20 04:59:25.000000 modbedtools-0.1.0/modbed/modbed.py
--rw-r--r--   0 dli        (501) staff       (20)       22 2023-01-18 19:39:24.000000 modbedtools-0.1.0/modbed/version.py
--rwxr-xr-x   0 dli        (501) staff       (20)     2694 2023-01-19 04:42:32.000000 modbedtools-0.1.0/modbedtools
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-01-20 05:28:33.475344 modbedtools-0.1.0/modbedtools.egg-info/
--rw-r--r--   0 dli        (501) staff       (20)     4174 2023-01-20 05:28:33.000000 modbedtools-0.1.0/modbedtools.egg-info/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)      266 2023-01-20 05:28:33.000000 modbedtools-0.1.0/modbedtools.egg-info/SOURCES.txt
--rw-r--r--   0 dli        (501) staff       (20)        1 2023-01-20 05:28:33.000000 modbedtools-0.1.0/modbedtools.egg-info/dependency_links.txt
--rw-r--r--   0 dli        (501) staff       (20)        6 2023-01-20 05:28:33.000000 modbedtools-0.1.0/modbedtools.egg-info/requires.txt
--rw-r--r--   0 dli        (501) staff       (20)        7 2023-01-20 05:28:33.000000 modbedtools-0.1.0/modbedtools.egg-info/top_level.txt
--rw-r--r--   0 dli        (501) staff       (20)       38 2023-01-20 05:28:33.477076 modbedtools-0.1.0/setup.cfg
--rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.0/setup.py
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.805696 modbedtools-0.1.1/
+-rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.1/LICENSE
+-rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:39:30.805079 modbedtools-0.1.1/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)     7644 2023-05-19 14:36:16.000000 modbedtools-0.1.1/README.md
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.799752 modbedtools-0.1.1/modbed/
+-rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.1/modbed/__init__.py
+-rw-r--r--   0 dli        (501) staff       (20)     6620 2023-05-15 19:56:33.000000 modbedtools-0.1.1/modbed/modbed.py
+-rw-r--r--   0 dli        (501) staff       (20)       22 2023-05-15 15:53:10.000000 modbedtools-0.1.1/modbed/version.py
+-rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.1/modbedtools
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.803876 modbedtools-0.1.1/modbedtools.egg-info/
+-rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)      266 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dli        (501) staff       (20)        1 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dli        (501) staff       (20)        6 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/requires.txt
+-rw-r--r--   0 dli        (501) staff       (20)        7 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/top_level.txt
+-rw-r--r--   0 dli        (501) staff       (20)       38 2023-05-19 14:39:30.805897 modbedtools-0.1.1/setup.cfg
+-rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.1/setup.py
```

### Comparing `modbedtools-0.1.0/LICENSE` & `modbedtools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.0/modbed/modbed.py` & `modbedtools-0.1.1/modbed/modbed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,90 @@
 import sys
 import os
 import gzip
 import pysam
 
 
-def process_read(read, cutoff):
+def process_read(read, cutoff, base, cpg):
     '''
-    convert bam file with Ml/Mm tags to bed file with methylation information in format: chr, start, end, methylated position array, unmethylated position array.
+    convert bam file with Ml/Mm tags to bed file with methylation information in format: chr, start, end, name, score, strand, methylated position array, unmethylated position array.
     One line per read.
+    if cpg mode is on: for pacbio bam, it assumes C in both strands of an CpG has same methylation level, both C will show at bp level vis
     '''
     if not (read.is_supplementary or read.is_secondary or read.is_unmapped):
         line = []
         chrom = read.reference_name
         start = read.reference_start
         end = read.reference_end
+        name = read.query_name
         align = read.get_aligned_pairs(matches_only=True)
         alignd = {}
         for x in align:
             # aligned dict, key: query pos in read, value: ref pos
             alignd[x[0]] = x[1]
         modbase_key = ('C', 1, 'm') if read.is_reverse else ('C', 0, 'm')
+        if base == 'A':
+            modbase_key = ('T', 1, 'a') if read.is_reverse else ('A', 0, 'a')
         if modbase_key not in read.modified_bases:
             return []
         modbase_list = read.modified_bases[modbase_key]
-        modbase_methy_string = ''
-        modbase_unmet_string = ''
+        modbase_methy_string = '.'
+        modbase_unmet_string = '.'
         modbase_methy_list = []
         modbase_unmet_list = []
+        strand = '-' if read.is_reverse else '+'
         for j in modbase_list:
             if j[0] in alignd:
                 if j[1]/255. >= cutoff:  # methylated base
                     if read.is_reverse:
+                        if base == 'C' and cpg:
+                            modbase_methy_list.append(
+                                str(alignd[j[0]] - start - 1))
                         modbase_methy_list.append(str(start - alignd[j[0]]))
                     else:
                         modbase_methy_list.append(str(alignd[j[0]] - start))
+                        if base == 'C' and cpg:
+                            modbase_methy_list.append(
+                                str(-(alignd[j[0]] - start+1)))
                 else:
                     if read.is_reverse:
+                        if base == 'C' and cpg:
+                            modbase_unmet_list.append(
+                                str(alignd[j[0]] - start - 1))
                         modbase_unmet_list.append(str(start - alignd[j[0]]))
                     else:
                         modbase_unmet_list.append(str(alignd[j[0]] - start))
+                        if base == 'C' and cpg:
+                            modbase_unmet_list.append(
+                                str(-(alignd[j[0]] - start+1)))
         if len(modbase_methy_list):
             modbase_methy_string = ','.join(modbase_methy_list)
         if len(modbase_unmet_list):
             modbase_unmet_string = ','.join(modbase_unmet_list)
-        line = [chrom, str(start), str(end), modbase_methy_string,
+        line = [chrom, str(start), str(end), name, '0', strand, modbase_methy_string,
                 modbase_unmet_string]
         return line
     else:
         return []
 
 
-def bam2mod(bamfile, outfile, cutoff=0.5):
+def bam2mod(bamfile, outfile, cutoff=0.5, base='C', cpg=False):
     bam = pysam.AlignmentFile(bamfile, 'rb', check_sq=False)
     if os.path.exists(bamfile+'.bai'):
         num_reads = bam.count()  # this needs index
         print(f'[info] total reads: {num_reads}', file=sys.stderr)
-    outf = '{}.modbed'.format(outfile)
+    cpgtag = '.cpg' if cpg else ''
+    outf = f'{outfile}{cpgtag}.modbed'
     print(f'[info] writing file {outf}', file=sys.stderr)
     with open(outf, "w") as out:
         for read in bam.fetch(until_eof=True):  # this makes bam index optional
-            items = process_read(read, cutoff)
+            items = process_read(read, cutoff, base, cpg)
             if len(items):
-                if items[3] or items[4]:  # for output, need either has modified base or unmodified base
+                # for output, need either has modified base or unmodified base
+                if items[3] != '.' or items[4] != '.':
                     line = '\t'.join(items)
                     out.write(line+'\n')
 
 
 rct = {
     'A': 'T',
     'C': 'G',
@@ -99,51 +118,63 @@
             else:
                 s += line.strip()
         d[k] = s
     return d
 
 
 def addbg(bedfile, fasta_file, output, base):
+    sbase = base.lower()
+    rc_base = rct[base]
+    rc_sbase = rct[base].lower()
     fa = read_fa(fasta_file)
     outf = '{}.modbed'.format(output)
     print(f'[info] writing file {outf}', file=sys.stderr)
     with xopen(bedfile) as fin, open(outf, 'w') as out:
         for line in fin:
             t = line.strip().split('\t')
+            # the fiber-seq data should not count first and last one as told
+            bs = t[-1].split(',')[1:-1]
+            if not len(bs):
+                continue
             chrom = t[0]
             start = int(t[1])
             end = int(t[2])
-            # the fiber-seq data should not count first and last one as told
-            bs = t[-1].split(',')[1:-1]
             # bs = t[-1].split(',')
             bs2 = [int(x) for x in bs]
             # contains start position in genome for each methylated base
             bs3 = [start+x for x in bs2]
             s = fa[chrom]  # the sequence
             c1 = []
             c2 = []
+            c1str = '.'
+            c2str = '.'
             for x in range(start, end+1):
                 if x in bs3:
                     # a methylated base
-                    if s[x].upper() == base:
+                    if s[x] == base or s[x] == sbase:
                         # + strand
                         c1.append(str(x-start))
-                    elif s[x].upper() == rct[base]:
+                    elif s[x] == rc_base or s[x] == rc_sbase:
                         # - strand
                         c1.append(str(start-x))
                 else:
                     # an unmethylated base but need check seq base
-                    if s[x].upper() == base:
+                    if s[x] == base or s[x] == sbase:
                         # + strand
                         c2.append(str(x-start))
-                    elif s[x].upper() == rct[base]:
+                    elif s[x] == rc_base or s[x] == rc_sbase:
                         # - strand
                         c2.append(str(start-x))
-            out.write(
-                f"{chrom}\t{start}\t{end}\t{','.join(c1)}\t{','.join(c2)}\n")
+            if len(c1):
+                c1str = ','.join(c1)
+            if len(c2):
+                c2str = ','.join(c2)
+            if c1str != '.' or c2str != '.':
+                out.write(
+                    f"{chrom}\t{start}\t{end}\t{t[3]}\t{t[4]}\t+\t{c1str}\t{c2str}\n")
 
 
 def main():
     pass
 
 
 if __name__ == "__main__":
```

### Comparing `modbedtools-0.1.0/modbedtools` & `modbedtools-0.1.1/modbedtools`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import argparse
 from modbed import version
 from modbed import modbed
 
 
 def bam2mod_wrap(args):
-    modbed.bam2mod(args.bamfile, args.output, args.cutoff)
+    modbed.bam2mod(args.bamfile, args.output, args.cutoff, args.base, args.cpg)
 
 
 def addbg_wrap(args):
     modbed.addbg(args.bedfile, args.fasta_file, args.output, args.base)
 
 
 if __name__ == '__main__':
@@ -29,14 +29,21 @@
                                        help='additional help')
 
     # bam2mod
     parser_bam2mod = subparsers.add_parser(
         'bam2mod', help='convert bam to modbed')
     parser_bam2mod.add_argument(
         'bamfile', help='bam file with MM/ML tags')
+    parser_bam2mod.add_argument('-b', '--base', choices=['C', 'A', 'c', 'a'], default='C',
+                                const='C',
+                                nargs='?',
+                                type=str.upper,
+                                help='modification base, case in-sensitive, C/c are same. (default: %(default)s)')
+    parser_bam2mod.add_argument("-g", "--cpg", help="output for both C/G bases in CpG, only applys when base is C",
+                                action="store_true")
     parser_bam2mod.add_argument('-c', '--cutoff', type=float,
                                 help='methylation cutoff, >= cutoff as methylated. default: 0.5', default=0.5)
     parser_bam2mod.add_argument(
         '-o', '--output', help='output file name, a suffix .modbed will be added. default: output', default='output')
     parser_bam2mod.set_defaults(func=bam2mod_wrap)
 
     # addbg
```

### Comparing `modbedtools-0.1.0/setup.py` & `modbedtools-0.1.1/setup.py`

 * *Files identical despite different names*

