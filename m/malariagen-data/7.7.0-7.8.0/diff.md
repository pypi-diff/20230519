# Comparing `tmp/malariagen_data-7.7.0.tar.gz` & `tmp/malariagen_data-7.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malariagen_data-7.7.0.tar", max compression
+gzip compressed data, was "malariagen_data-7.8.0.tar", max compression
```

## Comparing `malariagen_data-7.7.0.tar` & `malariagen_data-7.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/LICENSE
--rw-r--r--   0        0        0      987 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/__init__.py
--rw-r--r--   0        0        0    10005 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/af1.py
--rw-r--r--   0        0        0    92185 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/ag3.py
--rw-r--r--   0        0        0     9451 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/amin1.py
--rw-r--r--   0        0        0        0 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/__init__.py
--rw-r--r--   0        0        0    21458 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/base.py
--rw-r--r--   0        0        0    15325 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/genome_features.py
--rw-r--r--   0        0        0     3204 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/genome_sequence.py
--rw-r--r--   0        0        0    27811 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/sample_metadata.py
--rw-r--r--   0        0        0    44992 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anoph/snp_data.py
--rw-r--r--   0        0        0   216664 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/anopheles.py
--rw-r--r--   0        0        0    10514 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/mjn.py
--rw-r--r--   0        0        0     1253 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/pf7.py
--rw-r--r--   0        0        0     4442 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/pf7_config.json
--rw-r--r--   0        0        0    11756 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/plasmodium.py
--rw-r--r--   0        0        0    14253 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/plotly_dendrogram.py
--rw-r--r--   0        0        0     1253 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/pv4.py
--rw-r--r--   0        0        0     2060 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/pv4_config.json
--rw-r--r--   0        0        0    26186 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/util.py
--rw-r--r--   0        0        0    17981 2023-05-18 12:40:21.116125 malariagen_data-7.7.0/malariagen_data/veff.py
--rw-r--r--   0        0        0     1923 2023-05-18 12:43:01.923871 malariagen_data-7.7.0/pyproject.toml
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 malariagen_data-7.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/LICENSE
+-rw-r--r--   0        0        0      987 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/__init__.py
+-rw-r--r--   0        0        0    10005 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/af1.py
+-rw-r--r--   0        0        0    92409 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/ag3.py
+-rw-r--r--   0        0        0     9451 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/amin1.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/__init__.py
+-rw-r--r--   0        0        0    21458 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/base.py
+-rw-r--r--   0        0        0    15659 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/genome_features.py
+-rw-r--r--   0        0        0     3204 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/genome_sequence.py
+-rw-r--r--   0        0        0    27811 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/sample_metadata.py
+-rw-r--r--   0        0        0    45071 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/snp_data.py
+-rw-r--r--   0        0        0   219720 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/anopheles.py
+-rw-r--r--   0        0        0    10514 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/mjn.py
+-rw-r--r--   0        0        0     1253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pf7.py
+-rw-r--r--   0        0        0     4442 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pf7_config.json
+-rw-r--r--   0        0        0    11756 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/plasmodium.py
+-rw-r--r--   0        0        0    14253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/plotly_dendrogram.py
+-rw-r--r--   0        0        0     1253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pv4.py
+-rw-r--r--   0        0        0     2060 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pv4_config.json
+-rw-r--r--   0        0        0    26186 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/util.py
+-rw-r--r--   0        0        0    17981 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/veff.py
+-rw-r--r--   0        0        0     2028 2023-05-19 18:54:41.669683 malariagen_data-7.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 malariagen_data-7.8.0/PKG-INFO
```

### Comparing `malariagen_data-7.7.0/LICENSE` & `malariagen_data-7.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/__init__.py` & `malariagen_data-7.8.0/malariagen_data/__init__.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/af1.py` & `malariagen_data-7.8.0/malariagen_data/af1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/ag3.py` & `malariagen_data-7.8.0/malariagen_data/ag3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1863,16 +1863,17 @@
         fig.yaxis.axis_label = "Copy number"
         fig.yaxis.ticker = list(range(y_max + 1))
         self._bokeh_style_genome_xaxis(fig, region_prepped.contig)
         fig.add_layout(fig.legend[0], "right")
 
         if show:
             bkplt.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     def plot_cnv_hmm_coverage(
         self,
         sample,
         region,
         sample_set=None,
         y_max="auto",
@@ -1910,19 +1911,14 @@
         circle_kwargs : dict, optional
             Passed through to bokeh circle() function.
         line_kwargs : dict, optional
             Passed through to bokeh line() function.
         show : bool, optional
             If true, show the plot.
 
-        Returns
-        -------
-        fig : Figure
-            Bokeh figure.
-
         """
         debug = self._log.debug
 
         import bokeh.layouts as bklay
         import bokeh.plotting as bkplt
 
         debug("plot the main track")
@@ -1957,16 +1953,17 @@
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
         if show:
             bkplt.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     def plot_cnv_hmm_heatmap_track(
         self,
         region: base_params.single_region,
         sample_sets=None,
         sample_query=None,
         max_coverage_variance=DEFAULT_MAX_COVERAGE_VARIANCE,
@@ -2109,29 +2106,32 @@
         fig.yaxis.ticker = bkmod.FixedTicker(
             ticks=np.arange(len(sample_id)),
         )
         fig.yaxis.major_label_overrides = {i: s for i, s in enumerate(sample_id)}
         fig.yaxis.major_label_text_font_size = f"{row_height}px"
 
         debug("add color bar")
-        color_bar = bkmod.ColorBar(
+        # For some reason, mypy reports: Module has no attribute "ColorBar"
+        # ...but this works fine, so ignore for now.
+        color_bar = bkmod.ColorBar(  # type: ignore
             title="Copy number",
             color_mapper=color_mapper,
             major_label_overrides={
                 -1: "unknown",
                 4: "4+",
             },
             major_label_policy=bkmod.AllLabels(),
         )
         fig.add_layout(color_bar, "right")
 
         if show:
             bkplt.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     def plot_cnv_hmm_heatmap(
         self,
         region,
         sample_sets=None,
         sample_query=None,
         max_coverage_variance=DEFAULT_MAX_COVERAGE_VARIANCE,
@@ -2167,21 +2167,14 @@
         row_height : int, optional
             Plot height per row (sample) in pixels (px).
         track_height : int, optional
             Absolute plot height for HMM track in pixels (px), overrides
             row_height.
         genes_height : int, optional
             Height of genes track in pixels (px).
-        show : bool, optional
-            If true, show the plot.
-
-        Returns
-        -------
-        fig : Figure
-            Bokeh figure.
 
         """
         debug = self._log.debug
 
         import bokeh.layouts as bklay
         import bokeh.plotting as bkplt
 
@@ -2216,16 +2209,17 @@
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
         if show:
             bkplt.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     def _view_alignments_add_site_filters_tracks(
         self, *, contig, visibility_window, tracks
     ):
         debug = self._log.debug
 
         for site_mask in self.site_mask_ids:
@@ -2345,14 +2339,16 @@
         sample_sets=None,
         sample_query=None,
         sort=True,
         row_height=4,
         colors="T10",
         xgap=0,
         ygap=0.5,
+        show=True,
+        renderer=None,
     ):
         """Plot a heatmap of ancestry-informative marker (AIM) genotypes.
 
         Parameters
         ----------
         aims : {'gamb_vs_colu', 'gambcolu_vs_arab'}
             Which ancestry informative markers to use.
@@ -2543,15 +2539,19 @@
         )
 
         fig.update_layout(
             title=f"AIMs - {aims}",
             height=max(300, row_height * len(samples) + 100),
         )
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
 
 @numba.njit("Tuple((int8, int64))(int8[:], int8)")
 def _cn_mode_1d(a, vmax):
     # setup intermediates
     m = a.shape[0]
     counts = np.zeros(vmax + 1, dtype=numba.int64)
```

### Comparing `malariagen_data-7.7.0/malariagen_data/amin1.py` & `malariagen_data-7.8.0/malariagen_data/amin1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/anoph/base.py` & `malariagen_data-7.8.0/malariagen_data/anoph/base.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/anoph/genome_features.py` & `malariagen_data-7.8.0/malariagen_data/anoph/genome_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     genes_height: TypeAlias = Annotated[
         int,
         "Genes track height in pixels (px).",
     ]
     genes_height_default: genes_height = 120
     show: TypeAlias = Annotated[
         bool,
-        "If true, show the plot.",
+        "If true, show the plot. If False, do not show the plot, but return the figure.",
     ]
     toolbar_location: TypeAlias = Annotated[
         Literal["above", "below", "left", "right"],
         "Location of bokeh toolbar.",
     ]
     toolbar_location_default: toolbar_location = "above"
     x_range: TypeAlias = Annotated[
@@ -75,16 +75,16 @@
         Union[str, bool],
         "Plot title. If True, a title may be automatically generated.",
     ]
     figure: TypeAlias = Annotated[
         # Use quite a broad type here to accommodate both single-panel figures
         # created via bokeh.plotting and multi-panel figures created via
         # bokeh.layouts.
-        bokeh.model.Model,
-        "A bokeh figure.",
+        Optional[bokeh.model.Model],
+        "A bokeh figure (only returned if show=False).",
     ]
 
 
 class AnophelesGenomeFeaturesData(AnophelesGenomeSequenceData):
     def __init__(
         self,
         *,
@@ -230,14 +230,19 @@
         debug("Find the transcript annotation.")
         df_genome_features = self.genome_features().set_index("ID")
         parent = df_genome_features.loc[transcript]
 
         if title is True:
             title = f"{transcript} ({parent.strand})"
 
+        if x_range is None:
+            x_range = bokeh.models.Range1d(
+                parent.start - 2_000, parent.end + 2_000, bounds="auto"
+            )
+
         debug("Define tooltips for hover.")
         tooltips = [
             ("Type", "@type"),
             ("Location", "@contig:@start{,}-@end{,}"),
         ]
 
         debug("Make a figure.")
@@ -251,14 +256,15 @@
             height=height,
             tools=["xpan", "xzoom_in", "xzoom_out", xwheel_zoom, "reset", "hover"],
             toolbar_location=toolbar_location,
             active_scroll=xwheel_zoom,
             active_drag="xpan",
             tooltips=tooltips,
             x_range=x_range,
+            y_range=bokeh.models.Range1d(-0.6, 0.6),
         )
 
         debug("Find child components of the transcript.")
         data = self.genome_feature_children(parent=transcript, attributes=None)
         data["bottom"] = -0.4
         data["top"] = 0.4
 
@@ -329,21 +335,21 @@
             fill_color="blue",
             line_width=0,
             fill_alpha=0.5,
         )
 
         debug("Tidy up the figure.")
         fig.yaxis.ticker = []
-        fig.y_range = bokeh.models.Range1d(-0.6, 0.6)
         self._bokeh_style_genome_xaxis(fig, parent.contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Plot a genes track, using bokeh.",
     )
     def plot_genes(
         self,
@@ -408,14 +414,15 @@
                 "hover",
             ],
             toolbar_location=toolbar_location,
             active_scroll=xwheel_zoom,
             active_drag="xpan",
             tooltips=tooltips,
             x_range=x_range,
+            y_range=bokeh.models.Range1d(-0.4, 2.2),
         )
 
         debug("add functionality to click through to vectorbase")
         url = "https://vectorbase.org/vectorbase/app/record/gene/@ID"
         taptool = fig.select(type=bokeh.models.TapTool)
         taptool.callback = bokeh.models.OpenURL(url=url)
 
@@ -427,26 +434,26 @@
             right="end",
             source=data,
             line_width=0.5,
             fill_alpha=0.5,
         )
 
         debug("tidy up the plot")
-        fig.y_range = bokeh.models.Range1d(-0.4, 2.2)
         fig.ygrid.visible = False
         yticks = [0.4, 1.4]
         yticklabels = ["-", "+"]
         fig.yaxis.ticker = yticks
         fig.yaxis.major_label_overrides = {k: v for k, v in zip(yticks, yticklabels)}
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     def _plot_genes_setup_data(self, *, region):
         attributes = [a for a in self._gff_default_attributes if a != "Parent"]
         df_genome_features = self.genome_features(region=region, attributes=attributes)
         data = df_genome_features.query(f"type == '{self._gff_gene_type}'").copy()
         tooltips = [(a.capitalize(), f"@{a}") for a in attributes]
         tooltips += [("Location", "@contig:@start{,}-@end{,}")]
```

### Comparing `malariagen_data-7.7.0/malariagen_data/anoph/genome_sequence.py` & `malariagen_data-7.8.0/malariagen_data/anoph/genome_sequence.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/anoph/sample_metadata.py` & `malariagen_data-7.8.0/malariagen_data/anoph/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/anoph/snp_data.py` & `malariagen_data-7.8.0/malariagen_data/anoph/snp_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1065,16 +1065,17 @@
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Plot SNPs in a given genome region. SNPs are shown as rectangles,
             with segregating and non-segregating SNPs positioned on different levels,
             and coloured by site filter.
@@ -1194,15 +1195,15 @@
             height=height,
             toolbar_location="above",
             x_range=x_range,
             y_range=(0.5, 2.5),
             tooltips=tooltips,
         )
         hover_tool = fig.select(type=bokeh.models.HoverTool)
-        hover_tool.names = ["snps"]
+        hover_tool.name = "snps"
 
         # Plot gaps in the reference genome.
         df_n_runs = pd.DataFrame(
             {"left": n_starts + 0.6, "right": n_stops + 0.4, "top": 2.5, "bottom": 0.5}
         )
         fig.quad(
             top="top",
@@ -1243,16 +1244,17 @@
         fig.xaxis.axis_label = f"Contig {resolved_region.contig} position (bp)"
         fig.xaxis.ticker = bokeh.models.AdaptiveTicker(min_interval=1)
         fig.xaxis.minor_tick_line_color = None
         fig.xaxis[0].formatter = bokeh.models.NumeralTickFormatter(format="0,0")
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Compute genome accessibility array.",
         returns="An array of boolean values identifying accessible genome sites.",
     )
     def is_accessible(
```

### Comparing `malariagen_data-7.7.0/malariagen_data/anopheles.py` & `malariagen_data-7.8.0/malariagen_data/anopheles.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,22 @@
                 "ygridoff",
                 "gridon",
                 "none",
             ]
         ],
         "The figure template name (must be a key in plotly.io.templates).",
     ]
-    figure: TypeAlias = Annotated[go.Figure, "A plotly figure."]
+    show: TypeAlias = Annotated[
+        bool,
+        "If true, show the plot. If False, do not show the plot, but return the figure.",
+    ]
+    renderer: TypeAlias = Annotated[Optional[str], "The name of the renderer to use."]
+    figure: TypeAlias = Annotated[
+        Optional[go.Figure], "A plotly figure (only returned if show=False)."
+    ]
 
 
 class ihs_params:
     window_size: TypeAlias = Annotated[
         int,
         """
         The size of window in number of SNPs used to summarise iHS over.
@@ -1178,27 +1185,23 @@
         phet_roh,
         phet_nonroh,
         transition,
         window_size,
         sample_id,
         contig,
     ):
-        # conditional import, pomegranate takes a long time to install on
-        # linux due to lack of prebuilt wheels on PyPI
+        # This implementation is based on scikit-allel, but modified to use
+        # moving window computation of het counts.
         from allel.stats.misc import tabulate_state_blocks
-
-        # this implementation is based on scikit-allel, but modified to use
-        # moving window computation of het counts
         from allel.stats.roh import _hmm_derive_transition_matrix
 
-        # noinspection PyUnresolvedReferences
-        from pomegranate import (  # pyright: ignore
-            HiddenMarkovModel,
-            PoissonDistribution,
-        )
+        # Protopunica is pomegranate frozen at version 0.14.8, wich is compatible
+        # with the code here. Also protopunica has binary wheels available from
+        # PyPI and so installs much faster.
+        from protopunica import HiddenMarkovModel, PoissonDistribution
 
         # het probabilities
         het_px = np.concatenate([(phet_roh,), phet_nonroh])
 
         # start probabilities (all equal)
         start_prob = np.repeat(1 / het_px.size, het_px.size)
 
@@ -1543,23 +1546,24 @@
         summary="""
             Plot explained variance ratios from a principal components analysis
             (PCA) using a plotly bar plot.
         """,
         parameters=dict(
             kwargs="Passed through to px.bar().",
         ),
-        returns="A plotly figure.",
     )
     def plot_pca_variance(
         self,
         evr: pca_params.evr,
         width: plotly_params.width = 900,
         height: plotly_params.height = 400,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
-    ) -> go.Figure:
+    ) -> plotly_params.figure:
         debug = self._log.debug
 
         debug("prepare plotting variables")
         y = evr * 100  # convert to percent
         x = [str(i + 1) for i in range(len(y))]
 
         debug("set up plotting options")
@@ -1574,15 +1578,19 @@
         )
         debug("apply any user overrides")
         plot_kwargs.update(kwargs)
 
         debug("make a bar plot")
         fig = px.bar(x=x, y=y, **plot_kwargs)
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     def _cohort_alt_allele_counts_melt(self, gt, indices, max_allele):
         ac_alt_melt, an = self._cohort_alt_allele_counts_melt_kernel(
             gt, indices, max_allele
         )
         an_melt = np.repeat(an, max_allele, axis=0)
         return ac_alt_melt, an_melt
@@ -1753,20 +1761,23 @@
             width=width,
             height=height,
             circle_kwargs=circle_kwargs,
             show=show,
             x_range=x_range,
         )
 
-        return fig
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Plot windowed heterozygosity for a single sample over a genome region.",
-        returns="Bokeh figure.",
     )
     def plot_heterozygosity(
         self,
         sample: het_params.sample,
         region: base_params.single_region,
         window_size: het_params.window_size = het_params.window_size_default,
         y_max: het_params.y_max = het_params.y_max_default,
@@ -1774,15 +1785,15 @@
         site_mask: base_params.site_mask = DEFAULT,
         sample_set: Optional[base_params.sample_set] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 170,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
         show: gplt_params.show = True,
-    ):
+    ) -> gplt_params.figure:
         debug = self._log.debug
 
         # normalise to support multiple samples
         if isinstance(sample, (list, tuple)):
             samples = sample
         else:
             samples = [sample]
@@ -1841,16 +1852,17 @@
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
         if show:
             bokeh.plotting.show(fig_all)
-
-        return fig_all
+            return None
+        else:
+            return fig_all
 
     def _sample_count_het(
         self,
         sample: het_params.single_sample,
         region: Region,
         site_mask: base_params.site_mask,
         window_size: het_params.window_size,
@@ -1996,37 +2008,38 @@
                 "reset",
                 "tap",
                 "hover",
             ],
             active_scroll=xwheel_zoom,
             active_drag="xpan",
             x_range=x_range,
+            y_range=bokeh.models.Range1d(0, 1),
         )
 
         debug("now plot the ROH as rectangles")
         fig.quad(
             bottom="bottom",
             top="top",
             left="roh_start",
             right="roh_stop",
             source=data,
             line_width=0.5,
             fill_alpha=0.5,
         )
 
         debug("tidy up the plot")
-        fig.y_range = bokeh.models.Range1d(0, 1)
         fig.ygrid.visible = False
         fig.yaxis.ticker = []
         self._bokeh_style_genome_xaxis(fig, resolved_region.contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Plot windowed heterozygosity and inferred runs of homozygosity for a
             single sample over a genome region.
         """,
@@ -2126,16 +2139,17 @@
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
         if show:
             bokeh.plotting.show(fig_all)
-
-        return fig_all
+            return None
+        else:
+            return fig_all
 
     @check_types
     @doc(
         summary="""
             Run a principal components analysis (PCA) using biallelic SNPs from
             the selected genome region and samples.
         """,
@@ -3053,14 +3067,16 @@
         colorbar: plotly_params.colorbar = True,
         width: plotly_params.width = None,
         height: plotly_params.height = None,
         text_auto: plotly_params.text_auto = ".0%",
         aspect: plotly_params.aspect = "auto",
         color_continuous_scale: plotly_params.color_continuous_scale = "Reds",
         title: plotly_params.title = True,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
     ) -> plotly_params.figure:
         debug = self._log.debug
 
         debug("check len of input")
         if max_len and len(df) > max_len:
             raise ValueError(f"Input DataFrame is longer than {max_len}")
@@ -3138,15 +3154,19 @@
                 tickvals=[0, 0.2, 0.4, 0.6, 0.8, 1.0],
                 ticktext=["0%", "20%", "40%", "60%", "80%", "100%"],
             )
         )
         if not colorbar:
             fig.update(layout_coloraxis_showscale=False)
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Create a time series plot of variant frequencies using plotly.",
         parameters=dict(
             ds="""
                 A dataset of variant frequencies, such as returned by
@@ -3165,14 +3185,16 @@
     )
     def plot_frequencies_time_series(
         self,
         ds: xr.Dataset,
         height: plotly_params.height = None,
         width: plotly_params.width = None,
         title: plotly_params.title = True,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
     ) -> plotly_params.figure:
         debug = self._log.debug
 
         debug("handle title")
         if title is True:
             title = ds.attrs.get("title", None)
@@ -3254,15 +3276,19 @@
             },
             **kwargs,
         )
 
         debug("tidy plot")
         fig.update_layout(yaxis_range=[-0.05, 1.05])
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Plot markers on a map showing variant frequencies for cohorts grouped
             by area (space), period (time) and taxon.
         """,
@@ -3442,14 +3468,16 @@
         color: plotly_params.color = None,
         symbol: plotly_params.symbol = None,
         jitter_frac: plotly_params.jitter_frac = 0.02,
         random_seed: base_params.random_seed = 42,
         width: plotly_params.width = 900,
         height: plotly_params.height = 600,
         marker_size: plotly_params.marker_size = 10,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
     ) -> plotly_params.figure:
         debug = self._log.debug
 
         debug(
             "set up data - copy and shuffle so that we don't get systematic over-plotting"
         )
@@ -3506,15 +3534,19 @@
 
         debug("tidy up")
         fig.update_layout(
             legend=dict(itemsizing="constant"),
         )
         fig.update_traces(marker={"size": marker_size})
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Plot sample coordinates from a principal components analysis (PCA)
             as a plotly 3D scatter plot.
         """,
@@ -3531,14 +3563,16 @@
         color: plotly_params.color = None,
         symbol: plotly_params.symbol = None,
         jitter_frac: plotly_params.jitter_frac = 0.02,
         random_seed: base_params.random_seed = 42,
         width: plotly_params.width = 900,
         height: plotly_params.height = 600,
         marker_size: plotly_params.marker_size = 5,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
     ) -> plotly_params.figure:
         debug = self._log.debug
 
         debug(
             "set up data - copy and shuffle so that we don't get systematic over-plotting"
         )
@@ -3594,15 +3628,19 @@
         debug("tidy up")
         fig.update_layout(
             scene=dict(aspectmode="cube"),
             legend=dict(itemsizing="constant"),
         )
         fig.update_traces(marker={"size": marker_size})
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Plot diversity summary statistics for multiple cohorts.",
         parameters=dict(
             df_stats="Output from `diversity_stats()`.",
             bar_plot_height="Height of bar plots in pixels (px).",
@@ -3618,15 +3656,17 @@
         color: plotly_params.color = None,
         bar_plot_height: int = 450,
         bar_width: int = 30,
         scatter_plot_height: int = 500,
         scatter_plot_width: int = 500,
         template: plotly_params.template = "plotly_white",
         plot_kwargs: Optional[Mapping] = None,
-    ):
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
+    ) -> Optional[Tuple[go.Figure, ...]]:
         debug = self._log.debug
 
         debug("set up common plotting parameters")
         if plot_kwargs is None:
             plot_kwargs = dict()
         default_plot_kwargs = dict(
             hover_name="cohort",
@@ -3653,73 +3693,78 @@
         if color == "taxon":
             self._setup_taxon_colors(plot_kwargs=default_plot_kwargs)
         default_plot_kwargs.update(plot_kwargs)
         plot_kwargs = default_plot_kwargs
         bar_plot_width = 300 + bar_width * len(df_stats)
 
         debug("nucleotide diversity bar plot")
-        fig = px.bar(
+        fig1 = px.bar(
             data_frame=df_stats,
             x="cohort",
             y="theta_pi_estimate",
             error_y="theta_pi_ci_err",
             title="Nucleotide diversity",
             color=color,
             height=bar_plot_height,
             width=bar_plot_width,
             template=template,
             **plot_kwargs,
         )
-        fig.show()
 
         debug("Watterson's estimator bar plot")
-        fig = px.bar(
+        fig2 = px.bar(
             data_frame=df_stats,
             x="cohort",
             y="theta_w_estimate",
             error_y="theta_w_ci_err",
             title="Watterson's estimator",
             color=color,
             height=bar_plot_height,
             width=bar_plot_width,
             template=template,
             **plot_kwargs,
         )
-        fig.show()
 
         debug("Tajima's D bar plot")
-        fig = px.bar(
+        fig3 = px.bar(
             data_frame=df_stats,
             x="cohort",
             y="tajima_d_estimate",
             error_y="tajima_d_ci_err",
             title="Tajima's D",
             color=color,
             height=bar_plot_height,
             width=bar_plot_width,
             template=template,
             **plot_kwargs,
         )
-        fig.show()
 
         debug("scatter plot comparing diversity estimators")
-        fig = px.scatter(
+        fig4 = px.scatter(
             data_frame=df_stats,
             x="theta_pi_estimate",
             y="theta_w_estimate",
             error_x="theta_pi_ci_err",
             error_y="theta_w_ci_err",
             title="Diversity estimators",
             color=color,
             width=scatter_plot_width,
             height=scatter_plot_height,
             template=template,
             **plot_kwargs,
         )
-        fig.show()
+
+        if show:
+            fig1.show(renderer=renderer)
+            fig2.show(renderer=renderer)
+            fig3.show(renderer=renderer)
+            fig4.show(renderer=renderer)
+            return None
+        else:
+            return (fig1, fig2, fig3, fig4)
 
     @check_types
     @doc(
         summary="""
             Run and plot a Fst genome-wide scan to investigate genetic
             differentiation between two cohorts.
         """,
@@ -3799,16 +3844,17 @@
         # tidy up the plot
         fig.yaxis.axis_label = "Fst"
         fig.yaxis.ticker = [0, 1]
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Run and plot a Fst genome-wide scan to investigate genetic
             differentiation between two cohorts.
         """,
@@ -3830,15 +3876,16 @@
         ] = fst_params.max_cohort_size_default,
         random_seed: base_params.random_seed = 42,
         title: Optional[gplt_params.title] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 190,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
-    ) -> None:
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # gwss track
         fig1 = self.plot_fst_gwss_track(
             contig=contig,
             window_size=window_size,
             cohort1_query=cohort1_query,
             cohort2_query=cohort2_query,
             sample_sets=sample_sets,
@@ -3871,15 +3918,19 @@
             [fig1, fig2],
             ncols=1,
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
-        bokeh.plotting.show(fig)
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Open haplotypes zarr.",
         returns="Zarr hierarchy.",
     )
     def open_haplotypes(
@@ -4237,15 +4288,23 @@
             np.percentile(calibration_runs[str(window)], 5) for window in window_sizes
         ]
         q95 = [
             np.percentile(calibration_runs[str(window)], 95) for window in window_sizes
         ]
 
         # make plot
-        fig = bokeh.plotting.figure(width=700, height=400, x_axis_type="log")
+        if title is None:
+            title = sample_query
+        fig = bokeh.plotting.figure(
+            title=title,
+            width=700,
+            height=400,
+            x_axis_type="log",
+            x_range=bokeh.models.Range1d(window_sizes[0], window_sizes[-1]),
+        )
         fig.patch(
             window_sizes + window_sizes[::-1],
             q75 + q25[::-1],
             alpha=0.75,
             line_width=2,
             legend_label="25-75%",
         )
@@ -4258,21 +4317,19 @@
         )
         fig.line(
             window_sizes, q50, line_color="black", line_width=4, legend_label="median"
         )
         fig.circle(window_sizes, q50, color="black", fill_color="black", size=8)
 
         fig.xaxis.ticker = window_sizes
-        fig.x_range = bokeh.models.Range1d(window_sizes[0], window_sizes[-1])
-        if title is None:
-            title = sample_query
-        fig.title = title
         if show:
             bokeh.plotting.show(fig)
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Run h12 genome-wide selection scan.",
         returns=dict(
             x="An array containing the window centre point genomic positions.",
             h12="An array with h12 statistic values for each window.",
@@ -4438,16 +4495,17 @@
         # tidy up the plot
         fig.yaxis.axis_label = "H12"
         fig.yaxis.ticker = [0, 1]
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Plot h12 GWSS data.",
     )
     def plot_h12_gwss(
         self,
@@ -4465,15 +4523,16 @@
         ] = h12_params.max_cohort_size_default,
         random_seed: base_params.random_seed = 42,
         title: Optional[gplt_params.title] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 170,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
-    ) -> None:
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # gwss track
         fig1 = self.plot_h12_gwss_track(
             contig=contig,
             analysis=analysis,
             window_size=window_size,
             sample_sets=sample_sets,
             sample_query=sample_query,
@@ -4505,15 +4564,19 @@
             [fig1, fig2],
             ncols=1,
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
-        bokeh.plotting.show(fig)
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Run a H1X genome-wide scan to detect genome regions with
             shared selective sweeps between two cohorts.
         """,
@@ -4707,16 +4770,17 @@
         # tidy up the plot
         fig.yaxis.axis_label = "H1X"
         fig.yaxis.ticker = [0, 1]
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Run and plot a H1X genome-wide scan to detect genome regions
             with shared selective sweeps between two cohorts.
         """
@@ -4738,15 +4802,16 @@
         ] = h12_params.max_cohort_size_default,
         random_seed: base_params.random_seed = 42,
         title: Optional[gplt_params.title] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 190,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
-    ) -> None:
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # gwss track
         fig1 = self.plot_h1x_gwss_track(
             contig=contig,
             analysis=analysis,
             window_size=window_size,
             cohort1_query=cohort1_query,
             cohort2_query=cohort2_query,
@@ -4779,15 +4844,19 @@
             [fig1, fig2],
             ncols=1,
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
-        bokeh.plotting.show(fig)
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Run iHS GWSS.",
         returns=dict(
             x="An array containing the window centre point genomic positions.",
             ihs="An array with iHS statistic values for each window.",
@@ -5065,16 +5134,17 @@
 
         # tidy up the plot
         fig.yaxis.axis_label = "ihs"
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Run and plot iHS GWSS data.",
     )
     def plot_ihs_gwss(
         self,
@@ -5104,15 +5174,16 @@
         random_seed: base_params.random_seed = 42,
         palette: ihs_params.palette = ihs_params.palette_default,
         title: Optional[gplt_params.title] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 170,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
-    ) -> None:
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # gwss track
         fig1 = self.plot_ihs_gwss_track(
             contig=contig,
             analysis=analysis,
             sample_sets=sample_sets,
             sample_query=sample_query,
             window_size=window_size,
@@ -5156,15 +5227,19 @@
             [fig1, fig2],
             ncols=1,
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
-        bokeh.plotting.show(fig)
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     def _garud_g123(self, gt):
         """Compute Garud's G123."""
 
         # compute diplotype frequencies
         frq_counter = _diplotype_frequencies(gt)
 
@@ -5360,16 +5435,17 @@
         # tidy up the plot
         fig.yaxis.axis_label = "G123"
         fig.yaxis.ticker = [0, 1]
         self._bokeh_style_genome_xaxis(fig, contig)
 
         if show:
             bokeh.plotting.show(fig)
-
-        return fig
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="Plot G123 GWSS data.",
     )
     def plot_g123_gwss(
         self,
@@ -5387,15 +5463,16 @@
         ] = g123_params.max_cohort_size_default,
         random_seed: base_params.random_seed = 42,
         title: Optional[gplt_params.title] = None,
         sizing_mode: gplt_params.sizing_mode = gplt_params.sizing_mode_default,
         width: gplt_params.width = gplt_params.width_default,
         track_height: gplt_params.track_height = 170,
         genes_height: gplt_params.genes_height = gplt_params.genes_height_default,
-    ):
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # gwss track
         fig1 = self.plot_g123_gwss_track(
             contig=contig,
             sites=sites,
             site_mask=site_mask,
             window_size=window_size,
             sample_sets=sample_sets,
@@ -5427,15 +5504,19 @@
             [fig1, fig2],
             ncols=1,
             toolbar_location="above",
             merge_tools=True,
             sizing_mode=sizing_mode,
         )
 
-        bokeh.plotting.show(fig)
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     def _load_data_for_g123(
         self,
         *,
         contig,
         sites,
         site_mask,
@@ -5587,15 +5668,16 @@
         ] = g123_params.min_cohort_size_default,
         max_cohort_size: Optional[
             base_params.max_cohort_size
         ] = g123_params.max_cohort_size_default,
         window_sizes: g123_params.window_sizes = g123_params.window_sizes_default,
         random_seed: base_params.random_seed = 42,
         title: Optional[gplt_params.title] = None,
-    ):
+        show: gplt_params.show = True,
+    ) -> gplt_params.figure:
         # get g123 values
         calibration_runs = self.g123_calibration(
             contig=contig,
             sites=sites,
             site_mask=site_mask,
             sample_query=sample_query,
             sample_sets=sample_sets,
@@ -5617,15 +5699,23 @@
             np.percentile(calibration_runs[str(window)], 5) for window in window_sizes
         ]
         q95 = [
             np.percentile(calibration_runs[str(window)], 95) for window in window_sizes
         ]
 
         # make plot
-        fig = bokeh.plotting.figure(width=700, height=400, x_axis_type="log")
+        if title is None:
+            title = sample_query
+        fig = bokeh.plotting.figure(
+            title=title,
+            width=700,
+            height=400,
+            x_axis_type="log",
+            x_range=bokeh.models.Range1d(window_sizes[0], window_sizes[-1]),
+        )
         fig.patch(
             window_sizes + window_sizes[::-1],
             q75 + q25[::-1],
             alpha=0.75,
             line_width=2,
             legend_label="25-75%",
         )
@@ -5638,19 +5728,20 @@
         )
         fig.line(
             window_sizes, q50, line_color="black", line_width=4, legend_label="median"
         )
         fig.circle(window_sizes, q50, color="black", fill_color="black", size=8)
 
         fig.xaxis.ticker = window_sizes
-        fig.x_range = bokeh.models.Range1d(window_sizes[0], window_sizes[-1])
-        if title is None:
-            title = sample_query
-        fig.title = title
-        bokeh.plotting.show(fig)
+
+        if show:
+            bokeh.plotting.show(fig)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Hierarchically cluster haplotypes in region and produce an interactive plot.
         """,
         parameters=dict(
@@ -5668,14 +5759,16 @@
         linkage_method: hapclust_params.linkage_method = hapclust_params.linkage_method_default,
         count_sort: hapclust_params.count_sort = True,
         distance_sort: hapclust_params.distance_sort = False,
         cohort_size: Optional[base_params.cohort_size] = None,
         random_seed: base_params.random_seed = 42,
         width: plotly_params.width = 1000,
         height: plotly_params.height = 500,
+        show: plotly_params.show = True,
+        renderer: plotly_params.renderer = None,
         **kwargs,
     ) -> plotly_params.figure:
         from scipy.cluster.hierarchy import linkage
 
         from .plotly_dendrogram import create_dendrogram
 
         debug = self._log.debug
@@ -5805,15 +5898,19 @@
                     color=color,
                     symbol=symbol,
                     **plot_kwargs,
                 ).select_traces()
             )
         )
 
-        return fig
+        if show:
+            fig.show(renderer=renderer)
+            return None
+        else:
+            return fig
 
     @check_types
     @doc(
         summary="""
             Construct a median-joining haplotype network and display it using
             Cytoscape.
         """,
```

### Comparing `malariagen_data-7.7.0/malariagen_data/mjn.py` & `malariagen_data-7.8.0/malariagen_data/mjn.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/pf7.py` & `malariagen_data-7.8.0/malariagen_data/pf7.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/pf7_config.json` & `malariagen_data-7.8.0/malariagen_data/pf7_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/plasmodium.py` & `malariagen_data-7.8.0/malariagen_data/plasmodium.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/plotly_dendrogram.py` & `malariagen_data-7.8.0/malariagen_data/plotly_dendrogram.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/pv4.py` & `malariagen_data-7.8.0/malariagen_data/pv4.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/pv4_config.json` & `malariagen_data-7.8.0/malariagen_data/pv4_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/util.py` & `malariagen_data-7.8.0/malariagen_data/util.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/malariagen_data/veff.py` & `malariagen_data-7.8.0/malariagen_data/veff.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.7.0/pyproject.toml` & `malariagen_data-7.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "malariagen_data"
-version = "7.7.0"
+version = "7.8.0"
 description = "A package for accessing and analysing MalariaGEN data."
 authors = [
     "Alistair Miles <alistair.miles@sanger.ac.uk>",
     "Chris Clarkson <cc28@sanger.ac.uk>",
     "Lee Hart <lee.hart@sanger.ac.uk>",
     "Kathryn Murie <km22@sanger.ac.uk>",
     "Nace Kranjc <n.kranjc@imperial.ac.uk>",
     "Kelly Bennett <kb25@sanger.ac.uk>",
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-# numba cannot yet support python 3.11
-python = ">=3.8,<3.11"
-# numba cannot yet support numpy 1.24
-numpy = "<1.24"
+# numba cannot yet support python 3.12
+python = ">=3.8,<3.12"
+# numba cannot yet support numpy 1.25
+numpy = "<1.25"
 numba = "*"
 # force llvmlite above broken version
 llvmlite = ">0.34"
 scipy = "*"
 pandas = "*"
 zarr = "*"
 dask = {version="*", extras=["array"]}
@@ -29,15 +29,15 @@
 gcsfs = "*"
 BioPython = "*"
 scikit-allel = "*"
 xarray = "*"
 plotly = "*"
 # https://github.com/bokeh/bokeh/issues/12614
 # bokeh 3.0 has a problem with stretch sizing modes
-bokeh = "<3.0"
+bokeh = ">=3.1.0"
 statsmodels = "*"
 # 0.17.0 appears to be broken on colab
 ipyleaflet = ">0.17.0"
 ipywidgets = "*"
 # https://stackoverflow.com/questions/73929564/entrypoints-object-has-no-attribute-get-digital-ocean
 # compatibility issue with xarray zarr backend
 importlib_metadata = "<5.0"
@@ -48,14 +48,17 @@
 tqdm = "*"
 dash = "*"
 dash-cytoscape = "*"
 jupyter-dash = "*"
 numpydoc_decorator = ">=2.0.0"
 typing_extensions = "*"
 typeguard = ">=4.0.0"
+protopunica = "*"
+# accelerate plotly - https://plotly.com/python/renderers/#performance
+orjson = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-xdist = "*"
 pytest-cases = "*"
 pytest-cov = "*"
 notebook = "*"
```

### Comparing `malariagen_data-7.7.0/PKG-INFO` & `malariagen_data-7.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: malariagen-data
-Version: 7.7.0
+Version: 7.8.0
 Summary: A package for accessing and analysing MalariaGEN data.
 License: MIT
 Author: Alistair Miles
 Author-email: alistair.miles@sanger.ac.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: BioPython
-Requires-Dist: bokeh (<3.0)
+Requires-Dist: bokeh (>=3.1.0)
 Requires-Dist: dash
 Requires-Dist: dash-cytoscape
 Requires-Dist: dask[array]
 Requires-Dist: fsspec
 Requires-Dist: gcsfs
 Requires-Dist: igv-notebook (>=0.2.3)
 Requires-Dist: importlib_metadata (<5.0)
 Requires-Dist: ipinfo (!=4.4.1)
 Requires-Dist: ipyleaflet (>0.17.0)
 Requires-Dist: ipywidgets
 Requires-Dist: jupyter-dash
 Requires-Dist: llvmlite (>0.34)
 Requires-Dist: numba
-Requires-Dist: numpy (<1.24)
+Requires-Dist: numpy (<1.25)
 Requires-Dist: numpydoc_decorator (>=2.0.0)
+Requires-Dist: orjson
 Requires-Dist: pandas
 Requires-Dist: plotly
+Requires-Dist: protopunica
 Requires-Dist: scikit-allel
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
 Requires-Dist: typeguard (>=4.0.0)
 Requires-Dist: typing_extensions
 Requires-Dist: xarray
```

