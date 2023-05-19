# Comparing `tmp/RecruitPlotEasy-3.1.1.tar.gz` & `tmp/RecruitPlotEasy-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecruitPlotEasy-3.1.1.tar", last modified: Wed Apr 12 17:53:21 2023, max compression
+gzip compressed data, was "RecruitPlotEasy-3.2.0.tar", last modified: Fri May 19 20:02:24 2023, max compression
```

## Comparing `RecruitPlotEasy-3.1.1.tar` & `RecruitPlotEasy-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:53:21.251305 RecruitPlotEasy-3.1.1/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-04-12 17:53:21.251305 RecruitPlotEasy-3.1.1/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.1.1/README.md
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:53:21.141951 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-04-12 17:53:20.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      725 2023-04-12 17:53:21.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/SOURCES.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-04-12 17:53:20.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/dependency_links.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-04-12 17:53:20.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/entry_points.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-04-12 17:53:20.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/requires.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-04-12 17:53:20.000000 RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/top_level.txt
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:53:21.188814 RecruitPlotEasy-3.1.1/rpe2_code/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.1.1/rpe2_code/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.1.1/rpe2_code/recruit_plot_easy_2_database.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    34597 2023-04-12 17:31:40.000000 RecruitPlotEasy-3.1.1/rpe2_code/recruit_plot_easy_2_plot.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      630 2023-04-12 17:53:01.000000 RecruitPlotEasy-3.1.1/rpe2_code/rpe2_main.py
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:53:21.251305 RecruitPlotEasy-3.1.1/rpe2_code/supports/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/agnostic_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/bam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/blast_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/cig_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/fasta_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/file_checker.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/mdz_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/protein_predictor.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.1.1/rpe2_code/supports/sam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-04-12 17:53:21.251305 RecruitPlotEasy-3.1.1/setup.cfg
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-04-12 17:53:05.000000 RecruitPlotEasy-3.1.1/setup.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.443920 RecruitPlotEasy-3.2.0/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:02:24.442922 RecruitPlotEasy-3.2.0/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.2.0/README.md
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.267882 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      767 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/entry_points.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/requires.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/top_level.txt
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.333576 RecruitPlotEasy-3.2.0/rpe2_code/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.2.0/rpe2_code/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_database.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     6982 2023-05-19 19:59:39.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_describe.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    38422 2023-05-19 19:59:26.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_plot.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      889 2023-05-19 20:00:42.000000 RecruitPlotEasy-3.2.0/rpe2_code/rpe2_main.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.440928 RecruitPlotEasy-3.2.0/rpe2_code/supports/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/agnostic_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/bam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/blast_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/cig_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/fasta_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/file_checker.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/mdz_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/protein_predictor.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/sam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-05-19 20:02:24.443920 RecruitPlotEasy-3.2.0/setup.cfg
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-05-19 20:02:12.000000 RecruitPlotEasy-3.2.0/setup.py
```

### Comparing `RecruitPlotEasy-3.1.1/RecruitPlotEasy.egg-info/SOURCES.txt` & `RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 RecruitPlotEasy.egg-info/SOURCES.txt
 RecruitPlotEasy.egg-info/dependency_links.txt
 RecruitPlotEasy.egg-info/entry_points.txt
 RecruitPlotEasy.egg-info/requires.txt
 RecruitPlotEasy.egg-info/top_level.txt
 rpe2_code/__init__.py
 rpe2_code/recruit_plot_easy_2_database.py
+rpe2_code/recruit_plot_easy_2_describe.py
 rpe2_code/recruit_plot_easy_2_plot.py
 rpe2_code/rpe2_main.py
 rpe2_code/supports/__init__.py
 rpe2_code/supports/agnostic_reader.py
 rpe2_code/supports/bam_parser.py
 rpe2_code/supports/blast_parser.py
 rpe2_code/supports/cig_parser.py
```

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/recruit_plot_easy_2_database.py` & `RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_database.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/recruit_plot_easy_2_plot.py` & `RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import numpy as np
 
 import sqlite3 as sq
 
 import argparse
 
-import multiprocessing
+#import multiprocessing
 
 class rpdb:
 	def __init__(self, db, id_cut = 95, id_step = 0.5, gen_step = 1000,
 				criteria = "local", id_measure = "local", do_prot = False,
 				output_base = "recruitment_plots"):
 		
 		self.db = db
@@ -317,15 +317,18 @@
 		self.recplot.build()
 	
 class recplot:
 	def __init__(self, data, y, 
 				#cut, 
 				id_step, genome_step, contig_sizes, protein_info, 
 				contig_name_dict, tad = 80, mag_name = None, sample = None,
-				outdir = "recruitment_plots"):
+				outdir = "recruitment_plots", selected_mags = None,
+				font_size = 18, in_group_col = '#ff7f0e', 
+				out_group_col = '#1f77b4', overlay_alpha = 0.25,
+				scroll_zoom = False, save_static_img_as = "svg"):
 		
 		self.raw_data = data
 		self.contig_sizes = contig_sizes
 		self.gen_step = genome_step
 		#Flip k-v
 		self.ct_dict = dict([value, key] for key, value in contig_name_dict.items())
 		self.ct_names = None
@@ -375,19 +378,49 @@
 		
 		self.lower_right_data = None
 		
 		self.output_base = outdir
 
 		self.sample = sample
 		self.mag = mag_name
+		
 		if self.do_prot:
 			self.plot_name = os.path.normpath(self.output_base + "/" +self.sample + "/" + mag_name + "_proteins_recruitment_plot.html")
 		else:
 			self.plot_name = os.path.normpath(self.output_base + "/" +self.sample + "/" + mag_name + "_recruitment_plot.html")
-	
+		
+
+		self.save_img_fmt = save_static_img_as
+		self.scrollable = scroll_zoom
+		
+		self.html_config = {
+			'scrollZoom': self.scrollable,
+				'toImageButtonOptions': {
+				'format': self.save_img_fmt, # one of png, svg, jpeg, webp
+				'filename': self.plot_name,
+				'height': 1080,
+				'width': 1920,
+				'scale': 1 # Multiply title/legend/axis/canvas sizes by this factor
+		  }
+		}
+		
+		self.bot_right_line_col = 'rgb(66,146,198)'
+		self.main_plot_fill_colorscale = ['rgb(247,251,255)', 'rgb(222,235,247)', 'rgb(198,219,239)', 'rgb(158,202,225)', 'rgb(107,174,214)', 'rgb(66,146,198)', 'rgb(33,113,181)', 'rgb(8,81,156)', 'rgb(8,48,107)']
+		
+		self.main_plot_highlight_col = in_group_col
+		
+		self.main_plot_highlight_alpha = overlay_alpha
+		
+		#'#1f77b4' is a medium blue
+		#'#ff7f0e' is a burnt orange
+		self.in_group_depth_col = in_group_col
+		self.out_group_depth_col = out_group_col
+		
+		self.axis_font_size = font_size
+		
 	#Data comes in as a per-base count 
 	def bin_raw(self):
 		print("Processing", self.mag)
 		self.data = {}
 		self.bin_left = {}
 		self.bin_right = {}
 		
@@ -702,15 +735,15 @@
 		
 	def make_plots(self):
 		print("Plotting", self.mag)
 		max_bin_count = self.data.max()
 		if max_bin_count < 1: #i.e. max bin == 0, guarantee this with floats by using 1 as the inequality
 			#min_bin_count = 1
 			print("No best-hit reads were found for", self.mag)
-			print("There is no information to plot for this genome under your current settings. This genome will be skipped.")
+			print("There is no information to plot for this genome under your current read filtering settings. This genome will be skipped.")
 			
 		else:
 			min_bin_count = self.data[np.nonzero(self.data)].min()
 
 			#order of magnitude
 			#smallest oom is this
 			current_oom = -len(str(int(1/min_bin_count))) + 1
@@ -723,18 +756,14 @@
 				min_bin_count *= 10
 				current_oom += 1
 
 			tick_labels = []
 			for oom in tick_positions:
 				tick_labels.append("10e"+str(oom))
 			
-			#'#1f77b4' is a medium blue
-			#'#ff7f0e' is a burnt orange
-			#These are colorblind friendly contrasts.
-			
 			overall_plot =  make_subplots(rows=3, cols=2, 
 										column_widths=[0.66, 0.34], 
 										row_heights = [0.30, 0.10, 0.60],
 
 										shared_xaxes=True,
 										shared_yaxes=True,
 										horizontal_spacing = 0.025,
@@ -786,26 +815,27 @@
 			#Needs to have labels added.
 			overall_plot.add_trace(go.Heatmap(z=np.log10(self.data), 
 									x = self.bin_mids,
 									y = self.y,
 									colorbar = dict(
 										x = -0.1,
 										tickvals = tick_positions,
-										ticktext = tick_labels
+										ticktext = tick_labels,
+										tickfont = {"size": self.axis_font_size}
 										),
-									colorscale="blues",
+									colorscale=self.main_plot_fill_colorscale,
 									hovertemplate = bot_left_hov
 									),
 									row = 3, col = 1)
 			
 			#bot right - only one of these
 			overall_plot.add_trace(go.Bar(x = self.lower_right_data, 
 									y = self.y,
 									orientation='h',
-									marker = dict(color = '#1f77b4'),
+									marker = dict(color = self.bot_right_line_col),
 									hovertemplate = bot_right_hov
 									),
 									row = 3, col = 2)
 			
 			#text_rec = []
 			
 			#We just use the protein labels as a repo - normally it would be filled out
@@ -816,33 +846,33 @@
 											"Genome Region: " + str(s) + "-" + str(e)
 											])
 					self.protein_labels.append(next_label)
 			
 			overall_plot.add_trace(go.Scatter(x = self.bin_mids,
 									y = [1] * len(self.bin_mids),
 									text = self.protein_labels,
-									marker = dict(color = '#1f77b4'),
+									marker = dict(color = self.in_group_depth_col),
 									hoverinfo = "text"
 									),
 									row = 2, col = 1)
 									
 			which_viz = None
 			which_id = None
 			has_default = False
 			group = 0
 			
 			starting_step = len(overall_plot.data)
 			
 			step_groups = {}
 			id_grp = {}
 			
-			
 			tad_ticks = np.linspace(0, self.tad_max, num = 5, dtype = int).tolist()
 			#tad_labels = 
-			tad_colorbar = dict(tickvals = tad_ticks)
+			tad_colorbar = dict(tickvals = tad_ticks, 
+								tickfont = {"size" : self.axis_font_size})
 			
 			#Here, we iterate over the in-groups to add traces for each pct id in-group.
 			for pct_id_cutoff in self.y:
 				self.cutoff = pct_id_cutoff
 				#recalculate data
 				self.top_half()
 				
@@ -865,30 +895,32 @@
 					which_id = pct_id_cutoff
 					has_default = True
 				else:
 					group += 1
 				
 				line_height = self.cutoff-(self.id_step/2)
 				
-				#top left in group
-				overall_plot.add_trace(go.Scatter(x = self.bin_mids, 
-												y = self.upper_left_in,
-												marker = dict(color = '#1f77b4'),
-												visible = False,
-												hovertemplate = in_dep_hov
-												),
-												row = 1, col = 1)
+
 				#top left out group							
 				overall_plot.add_trace(go.Scatter(x = self.bin_mids,
 												y = self.upper_left_out, 
-												marker = dict(color = '#ff7f0e'),
+												marker = dict(color = self.out_group_depth_col),
 												visible = False,
 												hovertemplate = out_dep_hov	
 												), 
 												row = 1, col = 1)
+												
+				#top left in group - this goes second so that it's plotted on top in the layers
+				overall_plot.add_trace(go.Scatter(x = self.bin_mids, 
+												y = self.upper_left_in,
+												marker = dict(color = self.in_group_depth_col),
+												visible = False,
+												hovertemplate = in_dep_hov
+												),
+												row = 1, col = 1)
 
 				#mid right tad
 				#Update fixed colorbar, add the coverage values and this is done.
 				overall_plot.add_trace(go.Heatmap(z = self.tad_in,
 												x = self.tad_contigs,
 												y = self.tad_names,
 												visible = False,
@@ -899,57 +931,63 @@
 												),
 												row = 2, col = 2)
 				
 				#Prevent 0-depth outgroups from running away with the scale
 				#max_in_grp = self.upper_right_in.max() + 1
 				#self.upper_right_out[self.upper_right_out > max_in_grp] = max_in_grp
 				
-				#top right in group default
-				overall_plot.add_trace(go.Scatter(x = self.upper_right_in, 
+
+				#top right out group default
+				overall_plot.add_trace(go.Scatter(x = self.upper_right_out, 
 				y = self.depth_hist_breaks, 
-				marker = dict(color = '#1f77b4'),
+				marker = dict(color = self.out_group_depth_col),
 				visible = False,
-				hovertemplate = top_right_hov_in
+				hovertemplate = top_right_hov_out
 				), 
 				row = 1, col = 2)
-				#top right out group default
-				overall_plot.add_trace(go.Scatter(x = self.upper_right_out, 
+				
+				#top right in group default - same ordering issue as above.
+				overall_plot.add_trace(go.Scatter(x = self.upper_right_in, 
 				y = self.depth_hist_breaks, 
-				marker = dict(color = '#ff7f0e'),
+				marker = dict(color = self.in_group_depth_col),
 				visible = False,
-				hovertemplate = top_right_hov_out
+				hovertemplate = top_right_hov_in
 				), 
 				row = 1, col = 2)
 				
 			#Set default lines as nearest to 90
 			for i in step_groups[which_id]:
 				overall_plot.data[i].visible = True
 				
 			#in-group highlight
 			overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
 									y1 = 100+(self.id_step/2),
 									row = 3, col = 1,
 									line_width=0,
-									fillcolor="red",
-									opacity=0.13)
+									#line_width=5,
+									fillcolor=self.main_plot_highlight_col,
+									#line_color=self.main_plot_highlight_col,
+									#line_dash="dash")
+									opacity=self.main_plot_highlight_alpha)
 									#,layer="below")
 									
 			overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
 									y1 = 100+(self.id_step/2),
 									row = 3, col = 2,
 									line_width=0,
-									fillcolor="red",
-									opacity=0.13)
+									#line_width=5,
+									fillcolor=self.main_plot_highlight_col,
+									#line_color=self.main_plot_highlight_col,
+									#line_dash="dash")
+									opacity=self.main_plot_highlight_alpha)
 									#,layer="below")
+									
+			#print(overall_plot.layout['shapes'])
 				
 			
-				
-			#overall_plot.add_hrect(y0 = 0, y1 = max_tad,
-			#						row = 2, col = 2)
-			
 			left_box = {'type': 'rect', 
 						'x0': 0, 
 						'x1': 1, 
 						'xref': 
 						'x3 domain', 
 						'y0': 0, 
 						'y1': 1, 
@@ -960,41 +998,43 @@
 						'x1': 1, 
 						'xref': 
 						'x4 domain', 
 						'y0': 0, 
 						'y1': 1, 
 						'yref': 'y4 domain'}
 						
+						
+						
 			initial_shapes = list(overall_plot.layout["shapes"])
 			initial_shapes.append(left_box)
 			initial_shapes.append(right_box)
 			overall_plot.layout["shapes"] = tuple(initial_shapes)
 			
 			steps = []
 			for group in step_groups:
 				step = dict(
 						method="update",
 						args=[{"visible": [False] * len(overall_plot.data)},
-							{"shapes": [{'fillcolor': 'red',
+							{"shapes": [{'line': {'width': 0, 'color' : self.main_plot_highlight_col, 'dash' : 'dash'},
+										'fillcolor': self.main_plot_highlight_col,
 										#'layer': 'below',
-										'line': {'width': 0},
-										'opacity': 0.13,
+										'opacity': self.main_plot_highlight_alpha,
 										'type': 'rect',
 										'x0': 0,
 										'x1': 1,
 										'xref': 'x5 domain',
 										'y0': group-(self.id_step/2),
 										'y1': 100+(self.id_step/2),
 										'yref': 'y5'},
 										
 										#lower right highlight
-										{'fillcolor': 'red',
+										{'line': {'width': 0, 'color' : self.main_plot_highlight_col, 'dash' : 'dash'},
+										'fillcolor': self.main_plot_highlight_col,
 										#'layer': 'below',
-										'line': {'width': 0},
-										'opacity': 0.13,
+										'opacity': self.main_plot_highlight_alpha,
 										'type': 'rect',
 										'x0': 0,
 										'x1': 1,
 										'xref': 'x6 domain',
 										'y0': group-(self.id_step/2),
 										'y1': 100+(self.id_step/2),
 										'yref': 'y6'},
@@ -1007,29 +1047,31 @@
 										
 										]
 							}],
 						
 						label = str(round(group, 2))
 				)
 				#lower left and lower right data
-				step["args"][0]["visible"][0] = True
-				step["args"][0]["visible"][1] = True
-				step["args"][0]["visible"][2] = True
+				step["args"][0]["visible"][0] = True #lower left
+				step["args"][0]["visible"][1] = True #lower right
+				step["args"][0]["visible"][2] = True #annotation mid left
 				for i in step_groups[group]:
 					step["args"][0]["visible"][i] = True
 					
 				steps.append(step)
 				
 			id_slider = [dict(
 				#match default viz
 				active=which_viz,
 				currentvalue={"prefix": "Percent ID cutoff: ", "suffix": "%"},
 				pad={"t": 50},
-				bgcolor = '#1f77b4',
-				steps=steps
+				bgcolor = self.in_group_depth_col,
+				steps=steps,
+				#tickfont = {"size" : self.axis_font_size},
+				font = {"size" : self.axis_font_size}
 			)]
 				
 				
 			overall_plot['layout']['xaxis2'].pop('matches')
 
 			overall_plot['layout']['xaxis2']['showticklabels'] = True
 			
@@ -1044,24 +1086,38 @@
 			#print(overall_plot['layout'])
 			
 			overall_plot.update_layout(showlegend = False)
 			overall_plot.update_layout(margin = dict(t=25))
 			overall_plot.update_xaxes(showgrid=False)
 			overall_plot.update_yaxes(showgrid=False)
 			
+			overall_plot.update_xaxes(tickfont = {"size" : self.axis_font_size})
+			overall_plot.update_yaxes(tickfont = {"size" : self.axis_font_size})
+			
 			#overall_plot.update_layout(hovermode="x unified")
 			
 			overall_plot.update_layout(
-				sliders=id_slider
+				sliders=id_slider,
+				plot_bgcolor='#f2f2f2'
 			)
 			
-			#print(overall_plot)
-			#print(overall_plot['layout'])
 			
-			overall_plot.write_html(self.plot_name)
+			#print(overall_plot.data[0])
+			
+			#relayer = list(overall_plot.data)[2:]
+			#relayer.append(overall_plot.data[0])
+			#relayer.append(overall_plot.data[1])
+			#relayer = tuple(relayer)
+			#overall_plot.data = relayer
+			#relayer = None
+			
+			#print(overall_plot.data[0])
+			#print(overall_plot.data[-2])
+			
+			overall_plot.write_html(self.plot_name, config = self.html_config)
 		
 		
 	def build(self):
 		self.bin_raw()
 		self.concatenate()
 		self.make_plots()
 		
@@ -1081,14 +1137,20 @@
 	
 	parser.add_argument('-i', '--id_step',  dest = 'height', type=float, default = 0.5, 
 	help =  'Pct. ID bin height. Reads will be binned every [height] pct. ID. Default 0.5.')
 	
 	parser.add_argument('-o', '--output',  dest = 'outdir', default = "recruitment_plots", 
 	help =  'Base directory for outputs. Defaults to creating "recruitment_plots/" in the CWD.')
 	
+	parser.add_argument('-m', '--mag',  dest = 'mag', default = None, 
+	help =  'Plot only this MAG and exit.')
+	
+	parser.add_argument('--mag_file',  dest = 'mf', default = None, 
+	help =  'A file containing the names of MAGs to plot, one per line. Only these MAGs will be plotted.')
+	
 	args, unknown = parser.parse_known_args()
 	
 	return parser, args
 		
 def run_plot():
 	parser, opts = plot_opts()
 	db = opts.db
@@ -1100,18 +1162,55 @@
 	do_proteins = opts.prot
 	
 	width = opts.width
 	height = opts.height
 	
 	out = opts.outdir
 	
+	#Mag files
+	mag = opts.mag
+	mf = opts.mf
+	
 	mn = rpdb(db, gen_step = width, id_step = height, do_prot = do_proteins, output_base = out)
 	mn.open()
 	mn.parse_db()
 	
+	try:
+		mags_to_plot = list(mn.genomes.keys())
+	except:
+		mags_to_plot = None
+	
+	if mag is not None:
+		#check if the MAG is in the db.
+		if mag in mn.genomes:
+			print("MAG", mag, "detected. Plotting...")
+			mags_to_plot = [mag]
+		else:
+			mags_to_plot = None
+			print("Requested MAG:", mag, "was not found in the database. It cannot be plotted.")
+			print("Consider RecruitPlotEasy's describe module to take a look at your databases' contents.")
+			
+	if mf is not None:
+		mags_to_plot = []
+		with open(mf) as fh:
+			for line in fh:
+				mag = line.strip()
+				mags_to_plot.append(mag)
+	
+	if mags_to_plot is not None:
+		if len(mags_to_plot) == 0:
+			mags_to_plot = None
+		else:
+			mags_to_plot = ['"'+m+'"' for m in mags_to_plot]
+			mags_to_plot = set(mags_to_plot)
+	
+	if mags_to_plot is None:
+		print("No valid MAGs or genomes were detected for plotting.\nRecruitPlotEasy needs at least one to proceed.\n\nQuitting.")
+		sys.exit()
+	
 	if do_proteins:
 		if mn.proteins is None:
 			print("No proteins have been added to this database. Quitting.")
 			mn.close()
 			sys.exit()
 			
 	if do_proteins:
@@ -1119,17 +1218,18 @@
 	else:
 		print("Plotting genome with bin width ", width, 'bases and pct ID height ', height)
 	
 	
 	for sample in mn.samples:
 		mn.set_sample(sample)
 		for mag in mn.mags_in_sample:
-			mn.set_mag(mag)
-			mn.craft_query()
-			mn.load_sample()
+			if mag in mags_to_plot:
+				mn.set_mag(mag)
+				mn.craft_query()
+				mn.load_sample()
 		
 	mn.close()
```

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/agnostic_reader.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/agnostic_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/bam_parser.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/bam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/blast_parser.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/blast_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/cig_parser.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/cig_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/fasta_reader.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/file_checker.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/file_checker.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/protein_predictor.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/protein_predictor.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/rpe2_code/supports/sam_parser.py` & `RecruitPlotEasy-3.2.0/rpe2_code/supports/sam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.1.1/setup.py` & `RecruitPlotEasy-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="RecruitPlotEasy",
-	version="3.1.1",
+	version="3.2.0",
 	author="Kenji Gerhardt",
 	author_email="kenji.gerhardt@gmail.com",
 	description="A tool for visualizing short read mapping efforts",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	include_package_data=True,
```

